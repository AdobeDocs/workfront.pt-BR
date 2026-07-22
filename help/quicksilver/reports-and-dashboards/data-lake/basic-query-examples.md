---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exemplos de consulta de Data Connect
description: Exemplos de consultas que você pode usar para se familiarizar com a sintaxe e a estrutura de tipos específicos de consultas.
author: Courtney
feature: Reports and Dashboards
exl-id: f2da081c-bdce-4012-9797-75be317079ef
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/flDonZVaLR3bTF2aZcY9iy2ZnWbfrdhctL7J8esvxng
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: edee967a5c19d86fd471c4571a0b458f72bf370e
workflow-type: tm+mt
source-wordcount: 2201
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

A consulta usa os recursos de rastreamento de eventos de alteração do Data Connect. Ela determina a data em que um evento que teve um novo valor de status diferente do evento anterior foi acionado. 

Examinando a consulta de dentro para fora: 

1. Calcular registros em que o status anterior é diferente: 
   * Para cada evento de alteração, use a função lag() para identificar o valor anterior do status. 

2. Filtrar apenas os registros que foram alterados: 

   * Selecione registros do cálculo na etapa 1, onde status anterior != status atual. 

3. Calcule o carimbo de data e hora efetivo de início/término e a duração em dias: 

   * `<status_begin_effective_timestamp>`: Calculado na etapa 2. 

   * `<status_end_effective_timestamp>`: Calculado com base no próximo (lead()). `<status_begin_effective_timestamp>`: exibir o status somente se `<status_begin_effective_timestamp>` NÃO for NULL. 
   * `<status_duration_days>`: Diferença de dados entre `<status_begin_effective_timestamp>` e `<status_end_effective_timestamp>`. 

>[!NOTE]
>
>É recomendável usar essa consulta como sua própria &quot;Exibição&quot; no Power BI ou Tableau. Se você quiser trazer outros campos do `<object>_event view`, junte a saída dessa consulta de volta ao `<object>_event view`. Os campos de junção seriam os seguintes: <br>
>Para projects_event: 
>`From projects_event p`>`Join <above query> c on c.projectid = p.projectid  `>`and c. status_begin_effective_timestamp = p begin_effective_timestamp`

## Planning: consulta de tipo de registro único

Este exemplo demonstra como consultar dados do Workfront Planning para obter um único tipo de registro armazenado no data lake da Data Connect.

### Cenário

Sua organização usa o Workfront Planning para rastrear campanhas. Cada registro de campanha inclui um nome, status, data inicial, data final e proprietário. Você deseja obter uma lista de todas as campanhas ativas e seus principais detalhes para usar em um painel.

* Os dados do tipo de registro de planejamento são armazenados na exibição PLANNINGRECORD_CURRENT.
* Cada linha representa um único registro e todos os valores de campo são armazenados em uma coluna JSON chamada FIELD_VALUES.
* O tipo de registro é identificado pela coluna RECORDTYPEID.
* O espaço de trabalho do registro é identificado pela coluna WORKSPACEID (ou pela coluna WORKSPACENAME de um filtro legível).

### Consulta

```sql
SELECT
  recordid,
  FIELD_VALUES:"Name"::text AS campaign_name,
  FIELD_VALUES:"Status"::text AS campaign_status,
  FIELD_VALUES:"Start Date"::date AS start_date,
  FIELD_VALUES:"End Date"::date AS end_date,
  FIELD_VALUES:"Owner"::text AS owner
FROM PLANNINGRECORD_CURRENT
WHERE WORKSPACEID = '<your_campaign_workspace_id>'
AND RECORDTYPEID = '<your_campaign_record_type_id>'
AND FIELD_VALUES:"Status"::text = 'Active'
ORDER BY start_date ASC
```

### Resposta

A consulta acima retorna os seguintes dados:

* **recordid**: a ID de registro exclusiva do Planning para a campanha.
* **campaign_name**: o nome da campanha, extraído do objeto JSON FIELD_VALUES.
* **campaign_status**: o status atual da campanha.
* **start_date**: a data de início da campanha, convertida em um tipo de dados de data.
* **end_date**: a data final da campanha, convertida em um tipo de dados de data.
* **proprietário**: o nome do usuário ou da equipe atribuída como proprietário da campanha.

### Explicação

Os registros do Planning no Data Connect compartilham uma única estrutura de tabela, independentemente do tipo de registro. A coluna RECORDTYPEID é usada para definir o escopo da consulta para um tipo de registro específico — neste caso, Campanhas. Substitua `<your_campaign_record_type_id>` pela ID do tipo de registro que deseja consultar, que pode ser encontrada nas configurações de tipo de registro do Workfront Planning ou consultando RECORDTYPE_CURRENT.

Os valores de campo são armazenados como um objeto JSON na coluna FIELD_VALUES e são acessados usando a mesma sintaxe de notação de dois pontos usada para dados de formulário personalizado:

```
<field_column>:"<field_name>"::<data_type> AS <alias>
```

As referências de nome de campo devem corresponder exatamente ao nome de campo definido na configuração de campo do tipo de registro do Planning, incluindo maiúsculas e minúsculas, espaçamento e emoji.

>[!NOTE]
>
>As IDs de tipo de registro do Planning podem ser encontradas no URL ao exibir um tipo de registro no Workfront Planning. É o caminho do URL que começa com &quot;Rt...&quot;. Os tipos de registro também podem ser encontrados com a seguinte chamada SQL no Data Connect:
>
>
>```sql
>SELECT
>ID AS recordtypeid,
>DISPLAYNAME AS record_type_name,
>WORKSPACEID
>FROM RECORDTYPE_CURRENT
>ORDER BY record_type_name ASC
>```

## Planning: consulta de tipos de registros conectados

Este exemplo demonstra como consultar dados em dois tipos de registro conectados do Planning — um tipo de registro pai e um tipo de registro ao qual está conectado.

### Cenário

Sua organização conecta registros de Campanha a registros Táticos no Workfront Planning. Você deseja produzir um relatório que mostre cada campanha ao lado dos principais detalhes de suas táticas associadas. Eles desejam especificamente mostrar o nome da tática, a prioridade estratégica e a alocação de orçamento para que a liderança possa analisar a atividade da campanha organizada por tática.

Na Conexão de Dados, as conexões entre tipos de registro nativos do Planning são armazenadas diretamente na coluna FIELD_VALUES_RAW de PLANNINGRECORD_CURRENT. Para um campo de referência chamado &quot;Táticas&quot;, o valor é uma matriz JSON de objetos de registro conectados, cada um contendo uma propriedade id com o RECORDID do registro conectado. Use LATERAL FLATTEN da Snowflake para expandir essa matriz em linhas e unir ao tipo de registro conectado.

### Consulta

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  t.FIELD_VALUES:"Name"::text AS tactic_name,
  t.FIELD_VALUES:"Strategic Priority"::text AS strategic_priority,
  t.FIELD_VALUES:"Budget Allocation"::float AS budget_allocation
FROM PLANNINGRECORD_CURRENT c,
INNER JOIN REFERENCE_CURRENT R 
ON r.FROM_REFERENCEID = c.REFERENCE_IDS:"Tactics"::text
INNER JOIN PLANNINGRECORD_CURRENT t
-- Join to the Tactic record using the connected record ID from the array
ON t.RECORDID = r.TO_RECORDID
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
ORDER BY tactic_name, campaign_name
```

### Resposta

A consulta acima retorna os seguintes dados:

* **campaign_id**: a ID de registro exclusiva do Planning para a campanha.
* **campaign_name**: o nome do registro da campanha.
* **campaign_status**: o status atual da campanha.
* **tactic_name**: O nome do registro tático conectado.
* **strategic_priority**: o valor do campo Prioridade Estratégica do registro Tático conectado.
* **budget_allocation**: o valor do campo Alocação de Orçamento do registro Tático conectado, convertido como um flutuante.

### Explicação - KP modificado

As conexões entre tipos de registro nativos do Planning são armazenadas em uma tabela de junção REFERENCE_CURRENT.  A tabela de associação REFERENCE_CURRENT é usada para associações entre RecordType.   Ao unir entre RecordType, o campo TO_RECORDID deve ser usado.

A coluna REFERENCE_ID na view PLANNINGRECORD contém uma lista de todos os campos REFERENCEID aplicáveis a esse registro de planejamento. Você pode acessar a id utilizando a mesma notação JSON como um campo_valor.

```
<reference_ids>:"<reference_name>"::text
```

A exibição REFERENCE_CURRENT contém um ou mais registros em que TO_RECORDID aponta para outros campos `recordId` de planejamento nas exibições PLANNINGRECORD_*.

Para unir outro campo REFERÊNCIA a registros de planejamento adicionais, o mesmo padrão de associação às exibições REFERENCE_CURRENT e PLANNINGRECORD_* seria adicionado à consulta acima.


## Planning: tipo de registro associado à consulta de dados do Workfront Workflow

Este exemplo demonstra como unir um tipo de registro do Workfront Planning a um objeto nativo do Workfront Workflow — neste caso, um Projeto — usando o recurso de conexão nativa do Planning, que armazena referências a objetos externos na exibição REFERENCE_CURRENT.

### Cenário

Sua organização conecta registros do Campaign no Workfront Planning ao Workfront Projects usando o recurso de conexão nativo do Planning. Você deseja produzir um relatório combinado mostrando os detalhes da campanha juntamente com os dados de execução em tempo real do projeto vinculado — especificamente o Percentual concluído atual do projeto, a Data de conclusão planejada e o Proprietário do projeto atribuído — para que os gerentes de campanha possam rastrear o progresso do delivery sem sair do contexto do espaço de trabalho do Planning.

### Consulta

```sql
SELECT
  c.RECORDID AS campaign_id,
  c.FIELD_VALUES:"Name"::text AS campaign_name,
  c.FIELD_VALUES:"Status"::text AS campaign_status,
  conn.TO_EXTERNALID AS linked_project_id,
  p.name AS project_name,
  p.percentcomplete AS project_percent_complete,
  p.plannedcompletiondate AS project_planned_completion,
  p.ownerid AS project_owner_id,
  u.name AS project_owner_name
FROM WORKFRONT.PLANNING.PLANNINGRECORD_CURRENT c
-- Join to the references table to find Workfront Project connections
INNER JOIN WORKFRONT.PLANNING.REFERENCE_CURRENT conn
ON conn.REFERENCE_ID = c.REFERENCE_IDS:"ProjectId"::text
-- Join to the Workfront Projects table on the external ID
INNER JOIN WORKFRONT.WF.PROJECTS_CURRENT p
ON p.projectid = conn.TO_EXTERNALID
-- Join to Users to resolve the project owner name
LEFT JOIN WORKFRONT.WF.USERS_CURRENT u
ON u.userid = p.ownerid
WHERE c.RECORDTYPEID = '<your_campaign_record_type_id>'
AND p.completiontype != 'CPL' -- Exclude completed projects
ORDER BY campaign_name
```

### Resposta

A consulta acima retorna os seguintes dados:

* **campaign_id**: a ID de registro exclusiva do Planning para a campanha.
* **campaign_name**: o nome do registro da campanha.
* **campaign_status**: o status atual da campanha, no Planning.
* **linked_project_id**: a ID de projeto do Workfront de REFERENCE_CURRENT.TO_EXTERNALID, identificando o projeto do Workfront conectado.
* **nome_do_projeto**: o nome de projeto nativo do Workfront de PROJECTS_CURRENT.
* **porcentagem_concluída_do_projeto**: o valor da porcentagem concluída atual do projeto.
* **project_planned_completion**: a data de conclusão planejada do projeto vinculado do Workfront.
* **project_owner_id**: a ID de usuário do Workfront do proprietário do projeto.
* **nome_proprietário_do_projeto**: o nome para exibição do proprietário do projeto, resolvido ingressando em USERS_CURRENT.

### Explicação

As conexões de um tipo de registro do Planning para um objeto nativo do Workfront Workflow são armazenadas em REFERENCE_CURRENT. Cada linha dessa exibição representa um link direcional: TO_EXTERNALID contém a ID do objeto Workfront conectado. As linhas que representam conexões do Workfront são identificadas por `TO_EXTERNALCONNECTIONNAME = 'workfront'` e um valor TO_EXTERNALOBJECTNAME que corresponde ao código da API do tipo de objeto do Workfront — por exemplo, PROJ para Projetos.

A coluna REFERENCE_ID nas tabelas PLANNINGRECORD contém uma lista de todos os campos REFERENCEID aplicáveis a esse registro.  Você pode acessar a id utilizando a mesma notação JSON como um campo_valor.\
Uma única REFERENCE_ID no PLANNINGRECORD_CURRENT pode conter um ou mais links de referência na tabela REFERENCE_CURRENT que se vinculam a objetos de um tipo de objeto específico na tabela Workfront.

```
<reference_ids>:"<reference_name>"::text
```

Observe que as views do Planning (PLANNINGRECORD_CURRENT, REFERENCE_CURRENT) residem no esquema WORKFRONT.PLANNING, enquanto as views nativas do Workfront Workflow (PROJECTS_CURRENT, USERS_CURRENT etc.) residir no esquema WORKFRONT.WF. Junções entre esquemas exigem nomes de tabela totalmente qualificados.

A consulta executa três junções:

1. **Registros de planejamento para a tabela de referências:** REFERENCE_CURRENT unidos em `TO_RECORDID = c.RECORDID` para localizar todas as conexões originadas de cada registro de Campanha. Os filtros em `TO_EXTERNALCONNECTIONNAME = 'workfront'` e `TO_EXTERNALOBJECTNAME = 'PROJ'` restringem os resultados a linhas que representam especificamente conexões com Projetos Workfront.
1. **Tabela de referências para Projetos Workfront:** TO_EXTERNALID contém a ID de projeto nativa do Workfront para o Projeto conectado. Isto foi ingressado diretamente em `PROJECTS_CURRENT.projectid` para recuperar dados do projeto em tempo real.
1. **Projetos para Usuários:** UM LEFT JOIN para USERS_CURRENT resolve a chave estrangeira ownerid no projeto para um nome legível. Uma JUNÇÃO À ESQUERDA é usada aqui para que projetos sem proprietário atribuído ainda sejam incluídos nos resultados.

>[!NOTE]
>
>Ao unir tabelas externas ao Planning, NÃO use o campo TO_RECORDID na consulta.  Não é necessário ao unir a tabelas externas.
>
>Esse padrão pode ser aplicado a qualquer objeto do Workfront Workflow ao qual o Planning oferece suporte para conexão — como Projetos, Portfólios ou Programas — alterando o filtro TO_EXTERNALOBJECTNAME para o código de API do objeto apropriado (por exemplo, PORT para Portfólios ou PRGM para Programas) e unindo-se à tabela WORKFRONT.WF correspondente. Consulte o dicionário de dados da Workfront Data Connect para obter os nomes de colunas da tabela e ID corretos para cada tipo de objeto.

Para unir outro campo REFERENCE a registros externos adicionais, o mesmo padrão de associação a REFERENCE_CURRENT e as exibições do Workfront Workflow seriam adicionadas à consulta acima.

Os valores de registro externo e de Planejamento podem ser unidos na mesma consulta, unindo-se várias vezes à tabela REFERENCE_CURRENT e usando o padrão de junção apropriado.


<!--
## Task query 

Join the project and (assignedTo) users tables into a simple task list.



## Hours query

Join owner (users), hour type, and portfolio tables to provide a sum of hours by user and portfolio for the current year.



## Document approvals query

Measure the cycle time and average number of review cycles per asset.
-->
