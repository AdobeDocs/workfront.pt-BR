---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exemplos de consulta de Data Connect
description: Exemplos de consultas que você pode usar para se familiarizar com a sintaxe e a estrutura de tipos específicos de consultas.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 1%

---

# Exemplos de consulta da conexão de dados do Workfront

Para ajudá-lo a utilizar melhor os dados do Workfront Data Connect, esta página contém exemplos básicos de consultas que você pode usar para se familiarizar com a sintaxe e a estrutura de tipos específicos de consultas.

## Consulta de dados personalizada

Este exemplo demonstra como você pode compor uma consulta para retornar seus dados personalizados no Workfront, como formulários personalizados e campos personalizados.

### Cenário

Sua organização utiliza um formulário personalizado chamado Integração de finanças. O formulário é anexado a cada projeto e contém os seguintes campos:

* **Unidade de Negócios**: um campo personalizado que contém uma cadeia de caracteres.
* **ProjectID**: um campo personalizado que contém uma cadeia de caracteres numérica.
* **Nome do Projeto Expandido**: um campo de dados personalizado calculado que concatena os valores de Unidade de Negócios, ProjectID e o nome do projeto nativo do Workfront em uma única cadeia de caracteres.

Você precisa incluir essas informações na resposta para uma consulta no Data Connect. Os valores de dados personalizados para um registro no data lake estão contidos em uma coluna intitulada `parametervalues`. Essa coluna é armazenada como um objeto JSON.

### Consulta

```
SELECT
    projectid,
    parametervalues,
    name,
    parametervalues:"DE:Business Unit"::int as BusinessUnit,
    parametervalues:"DE:Project ID"::int as ProjectID,
    parametervalues:"DE:Expanded Project Name"::text as ExpandedProjectName
FROM PROJECTS_CURRENT
WHERE ExpandedProjectName is not null
```

### Resposta

A consulta acima retorna os seguintes dados:

* `projectid`: a ID nativa do projeto do Workfront.
* `parametervalues`: uma coluna armazenando um objeto JSON.
* `name`: o nome nativo do projeto do Workfront.
* `Business Unit`: Um valor de dados personalizado que está incluído no objeto `parametervalues`.
* `Project ID`: Um valor de dados personalizado que está incluído no objeto `parametervalues`.
* `Expanded Project Name`: Um valor de dados personalizado que está incluído no objeto `parametervalues`.

### Explicação

Ao consultar o objeto JSON `parametervalues`, cada campo de dados personalizado pode ser acessado como uma coluna usando o seguinte:

`<field_name>:"<parameter_name>"::<data_type> as <column_name>`

* `<field_name>` é o nome do objeto JSON na tabela que está sendo consultada. No caso de dados personalizados, sempre será `parametervalues`.
* `<parameter_name>` é a cadeia de caracteres `parametername` encontrada na ferramenta de configuração de formulário, embora nem sempre corresponda a esse valor.

>[!NOTE]
>
>Se o nome do parâmetro for alterado na ferramenta de configuração de formulário do Workfront, ele será representado como uma nova coluna no objeto JSON. Dessa forma, recomendamos não alterar o nome de uma coluna depois de criá-la na ferramenta de configuração de formulário. No entanto, o rótulo pode ser alterado sem afetar o objeto JSON.
>
>Se a string de texto para o nome do parâmetro estiver incorreta, a coluna retornará um valor NULL, em vez de um erro.

* `<data_type>` converte o valor sendo retornado do objeto JSON em um tipo de dados apropriado para o campo. Escolher um tipo de dados incompatível para o valor que está sendo retornado resultará em um erro de incompatibilidade de tipo de dados. Os possíveis tipos de dados incluem:

   * `text`
   * `varchar`
   * `int`
   * `float`
   * `number(len,precision)` (por exemplo, `Number(32,4)` retornaria 1234.0987)
   * `date`
   * `timestamp`

* `<column_name>` é o rótulo que você cria para cada coluna de dados personalizada.

>[!NOTE]
>
>Somente os parâmetros com valores atribuídos a eles no formulário serão incluídos no objeto JSON. Se um campo de dados personalizado estiver vazio no formulário, ele não será exibido.

## Tempo em consulta de status

Este exemplo demonstra como medir o tempo que um projeto gastou nos status atribuídos anteriormente. Ele pode ser facilmente adaptado para medir o tempo de tarefas ou problemas em um status, ou pode ser adaptado para medir quanto tempo um objeto teve qualquer outro atributo (incluindo valores de dados personalizados) aplicado a ele.

### Cenário

A liderança de sua organização acredita que você está gastando muito tempo em cada estágio do ciclo de vida do trabalho. Antes de fazer recomendações para melhorar o processo, você deseja criar uma medida de linha de base da frequência com que o status de um projeto muda ao longo do tempo e quantos dias um projeto permanece em determinado status.

Você usará a visualização de dados PROJECTS_EVENT para obter uma lista de cada alteração de status em relação ao objeto do projeto. Você comparará o novo status com o status anterior, capturará o intervalo de tempo efetivo para o status atribuído anteriormente e calculará os dias gastos nesse status.

Usando essa saída bruta de tempo gasto em cada status por projeto, você pode começar a criar visualizações ou agregar mais os dados para criar médias de duração de status por status, tipo de projeto ou hora do ano. Essa linha de base é então usada para definir um referencial que você possa avaliar para atender às expectativas de sua liderança.

A consulta a seguir usa a visualização de dados Conexão de Dados PROJECTS_EVENTS para comparar cada evento de alteração de status do projeto e exibir o tempo em status.

### Consulta

```
-- Calculate the begin/end effective timestamp and duration in days 

SELECT 

    projectid, 
    name as project_name, 
    prev_status as previous_status, 
    status, 
    status_change_date as status_begin_effective_timestamp, 
    case 
        when status_change_date is null then NULL
        else
            nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp) 
    end as status_end_effective_timestamp, 
    datediff('DAYS',status_change_date, nvl(lead(status_change_date) ignore nulls over (partition by projectid order by status_change_date), current_timestamp)) as status_duration_days 

FROM 
    ( -- Filter to just the records that have changed 
     SELECT projectid, 
        name, 
        prev_status, 
        status, 
        begin_effective_timestamp as status_change_date    
     FROM 
        (  -- Calculate records where previous status is different 
          SELECT DISTINCT  
           pe.projectid, 
           pe.name AS name, 
           pe.STATUS, 
           nvl(lag(pe.STATUS) over (partition by pe.projectid order by pe.BEGIN_EFFECTIVE_TIMESTAMP), status) prev_status, 
           begin_effective_timestamp 

          FROM projects_event pe 
         -- Set any WHERE conditions to limit the results as needed 
         --WHERE 
            -- pe.PROJECTID = '5ebe…c1e1' 
        ) 
        WHERE prev_status != status 
    ) 
    order by status_change_date; 
```

### Resposta

A consulta acima retorna os seguintes dados:

* `PROJECTID`: a ID do projeto do Workfront associada ao evento de alteração de status.
* `PROJECT_NAME`: O nome do projeto do Workfront.
* `PREVIOUS_STATUS`: O status do projeto imediatamente antes da alteração.
* `STATUS`: O status do projeto após a alteração.
* `STATUS_BEGIN_EFFECTIVE_TIMESTAMP`: O carimbo de data/hora do evento de alteração quando o status anterior foi definido.
* `STATUS_END_EFFECTIVE_TIMESTAMP`: O carimbo de data/hora do evento de alteração quando o valor de status atualizado foi definido.
* `STATUS_DURATION_DAYS`: a diferença (em dias) entre o carimbo de data/hora efetivo final e o carimbo de data/hora efetivo inicial.

### Explicação

A consulta usa os recursos de rastreamento de eventos de alteração do Data Connect.  Ela determina a data em que um evento que tinha um novo valor de status diferente do evento anterior foi acionado. 

Examinando a consulta de dentro para fora: 

1. Calcular registros em que o status anterior é diferente: 
   * Para cada evento de alteração, use a função lag() para identificar o valor anterior do status. 

2. Filtrar apenas os registros que foram alterados: 

   * Selecione registros do cálculo na etapa 1, onde o status anterior!= status atual. 

3. Calcule o carimbo de data e hora efetivo de início/término e a duração em dias: 

   * `<status_begin_effective_timestamp>`: Calculado na etapa 2. 

   * `<status_end_effective_timestamp>`: Calculado com base no próximo (lead()). `<status_begin_effective_timestamp>`: exibir o status somente se `<status_begin_effective_timestamp>` NÃO for NULL. 
   * `<status_duration_days>`: Diferença de dados entre `<status_begin_effective_timestamp>` e `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>É recomendável usar essa consulta como sua própria &quot;Exibição&quot; no Power BI ou Tableau.  Se quiser trazer outros campos de `<object>_event view`, junte a saída desta consulta de volta ao `<object>_event view`.  Os campos de junção seriam os seguintes: <br>
>Para projects_event: 
>`From projects_event p`
>`Join <above query> c on c.projectid = p.projectid  `
>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`



<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
