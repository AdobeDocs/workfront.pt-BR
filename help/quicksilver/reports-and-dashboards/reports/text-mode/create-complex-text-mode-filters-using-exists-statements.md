---
product-area: reporting
navigation-topic: text-mode-reporting
title: Criar filtros complexos do Modo de Texto usando instruções EXISTS
description: Você pode criar filtros complexos do Modo de texto usando instruções EXISTS. Este artigo requer uma compreensão completa da API do Adobe Workfront e da interface de relatório do modo de texto.
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 09492b2657aaf599bb31a19329d5de23791b66ec
workflow-type: tm+mt
source-wordcount: '2649'
ht-degree: 0%

---

# Criar filtros complexos do Modo de Texto usando instruções EXISTS

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Este artigo requer uma compreensão completa da API do Adobe Workfront e da interface de relatório do modo de texto. Para obter informações sobre a API do Workfront, consulte [Noções básicas sobre API](../../../wf-api/general/api-basics.md).\
>Para obter informações sobre como usar o modo de texto, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Visão geral dos relacionamentos entre objetos no Workfront

Todos os objetos são vinculados a outros objetos no banco de dados do Workfront.

Compreender a hierarquia e a interdependência de objetos ajuda a descobrir quais objetos podem ser referenciados nos relatórios.

Para obter informações sobre quais objetos estão no Workfront e sobre sua hierarquia e interdependência, consulte [Visão geral dos objetos do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Ao criar filtros, você pode fazer referência a outros objetos que estão conectados ao objeto do filtro em até dois níveis de relacionamento usando a interface de relatórios padrão.

Por exemplo, você pode fazer referência à ID de Portfolio em um filtro de problema para exibir somente problemas em projetos associados a um determinado portfólio usando a interface padrão. Nesse caso, o portfólio está a dois níveis de problemas.

No entanto, não é possível fazer referência ao Proprietário do Portfolio em um filtro de problema usando a interface padrão para exibir somente problemas de projetos associados a portfólios em que o proprietário é um usuário específico. Você deve usar o modo de texto para acessar o campo Nome do proprietário do Portfolio, que está a três níveis de problemas.

![Ícones de Emissão para o proprietário do portfólio](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Para obter uma lista completa dos objetos no Workfront, consulte [API Explorer](../../../wf-api/general/api-explorer.md).

Para obter informações sobre como navegar no API Explorer e localizar objetos, consulte [Utilização do API Explorer](../../../wf-api/general/using-api-explorer.md).

Ao criar filtros, você deve criar instruções complexas na interface do modo de texto para fazer referência a esses tipos de objetos.

Para obter informações sobre a criação de filtros complexos, consulte [Visão geral de filtros de modo de texto complexos que usam instruções EXISTS](#overview-of-complex-text-mode-filters-that-use-exists-statements) seção deste artigo.

## Visão geral de filtros de modo de texto complexos que usam instruções EXISTS {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Considere o seguinte ao criar filtros que abrangem vários níveis na hierarquia de objetos ou filtrar por objetos ausentes:

* Você deve criar filtros complexos quando quiser fazer referência a objetos não conectados diretamente ao objeto de filtro.
* Você deve usar uma instrução EXISTS para fazer o seguinte:

   * Crie filtros que abrangem vários níveis.
   * Crie filtros que procuram objetos ausentes.\
     Por exemplo, ao criar um relatório de usuário, você pode filtrar por usuários que não registraram tempo por um determinado período.

Considere as seguintes regras ao usar instruções EXISTS em um filtro:

* Há três objetos que você pode referenciar em um filtro EXISTE:

   * O objeto do filtro (Objeto Original).
   * O objeto cujo campo você deseja referenciar (Objeto de Destino).
   * O objeto que conecta os objetos Original e Destino, caso não estejam conectados diretamente um ao outro (Objeto de vinculação).

* Os filtros que usam EXISTS contêm duas instruções separadas vinculadas por um sinal de igual:

   * A declaração antes do sinal de igual se refere ao objeto ao qual você está se referindo (o objeto de vinculação ou de destino).
   * A declaração depois do sinal de igual refere-se ao objeto que você está referenciando (o Objeto original).

* Você deve usar o código de objeto do Objeto de vinculação para conectar suas instruções.\
  Você pode encontrar o código de objeto de todos os objetos no API Explorer.\
  Para obter informações sobre o API Explorer, consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

* Quando um objeto de vinculação está ausente porque os objetos original e de destino estão conectados diretamente uns aos outros, você pode usar o código do objeto de destino em vez do objeto de vinculação.
* Você pode fazer referência a vários campos (Campos de destino) no mesmo objeto (Objeto de destino); nesse caso, você deve conectar as linhas que fazem referência aos campos por AND.\
  Para obter um exemplo de filtragem para mais de um campo que pertence ao Objeto de destino, consulte o [Exemplo 4: filtrar por vários campos: tarefas por Nome do proprietário do Portfolio e ID do Scorecard do alinhamento de Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) neste artigo.

* O único modificador suportado para uma instrução EXISTS é NOTEXISTS.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para editar filtros em um relatório</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar filtros em um relatório</p> <p>Gerenciar permissões de um filtro para editá-lo</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Criar filtros de modo de texto complexos que abrangem vários níveis na hierarquia de objetos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

Você pode criar um filtro que faça referência a objetos em vários níveis da hierarquia de objetos na qual o objeto de filtro existe. Por exemplo, você pode criar um filtro de problemas para problemas que estão em projetos não associados a um determinado Proprietário de Portfolio.

Você sempre deve usar uma instrução EXISTS e a interface de modo de texto para criar esse filtro.

Para obter exemplos de filtros, consulte [Exemplo 1: filtrar problemas por Nome do proprietário do Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) neste artigo.

Para criar um filtro que abrange vários níveis na hierarquia de objetos:

1. Identifique o objeto do filtro. Nós nos referimos a esse objeto como o objeto original.\
   Por exemplo, Problema.

1. Identifique o campo pelo qual deseja filtrar. Nos referimos a esse objeto como o Campo de destino que pertence a um Objeto de destino.\
   Por exemplo, o campo ownerID (Campo alvo), que pertence a Portfolio (Objeto alvo).

1. (Condicional) Se o Objeto original (Ocorrência) e o Campo de destino (ownerID) não estiverem diretamente conectados entre si, você deverá localizar um terceiro objeto, um Objeto de vinculação (Projeto) que os conecte. O objeto de vinculação deve ter pelo menos um campo referenciado das guias Campos ou Referências do objeto original (campo de vinculação exibido no objeto original) e também deve ter um campo vinculado ao objeto de destino exibido nas guias Campos ou Referências do objeto de vinculação. O Campo de vinculação ao Objeto de destino que é exibido no Objeto de vinculação (ou o Campo de vinculação exibido no Objeto de vinculação) deve corresponder ao Campo de destino.

   Por exemplo, a ID (Projeto) (Campo de vinculação exibido no Objeto original) é referenciada a partir de Ocorrências (Objeto original). A ID do proprietário do (Portfolio) (Campo de vinculação ao Objeto de destino) é exibida na guia Campos do Projeto (Objeto de vinculação). Portfolio ownerID também é um campo no Target Object (Portfolio). O campo Vinculação no Objeto de vinculação corresponde ao campo de Direcionamento.\
   ![portfolio_id_in_the_project_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Usando a API Explorer, identifique a variável **Código do objeto** do objeto de vinculação (projeto).\
   Por exemplo, o Código de objeto do projeto é PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Crie um filtro para o Objeto Original.\
   Por exemplo, criar um filtro de Ocorrência.\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para modo de texto**.
1. Cole o seguinte exemplo de fórmula na interface do modo de texto do novo filtro e substitua o texto de exemplo pelos objetos e campos corretos:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>`

   `EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>`

   Para obter um exemplo usando os campos identificados acima, consulte [Exemplo 1: filtrar problemas por Nome do proprietário do Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) neste artigo.

1. Clique em **Salvar Filtro**.

## Criar filtros de modo de texto complexo para objetos ausentes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

Você pode criar um filtro que faça referência a objetos ausentes. Por exemplo, você pode criar um filtro de usuário que mostra quais usuários não registraram horas no Workfront.

Você sempre deve usar um *EXISTE* e a interface do modo de texto para criar esse filtro.

Para obter exemplos de filtros para objetos ausentes, consulte as seguintes seções neste artigo:

* [Exemplo 2: filtro para objetos ausentes: campos personalizados que não aparecem em nenhum formulário personalizado](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Exemplo 3: filtro para objetos ausentes: usuários que não registraram tempo por um determinado período](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

Para criar um filtro que faça referência a objetos ausentes:

1. Identifique o objeto do filtro. Nós nos referimos a esse objeto como o objeto original.\
   Por exemplo, Parâmetro ou Campo personalizado.

1. Identifique o campo pelo qual deseja filtrar. Nos referimos a esse objeto como o Campo de destino que pertence a um Objeto de destino.\
   Por exemplo, o campo categoryID (Campo de público alvo), que pertence à Categoria (Objeto de público alvo).

1. Como o Objeto original (parâmetro) e o Campo de destino (categoryID) não estão diretamente conectados uns aos outros, você deve encontrar um terceiro objeto, um Objeto de vinculação (um Parâmetro de categoria) que os conecta. O objeto de vinculação deve ter pelo menos um campo referenciado das guias Campos ou Referências do objeto original (campo de vinculação exibido no objeto original) e também deve ter um campo vinculado ao objeto de destino exibido nas guias Campos ou Referências do objeto de vinculação. O Campo de vinculação ao Objeto de destino que é exibido no Objeto de vinculação (ou o Campo de vinculação exibido no Objeto de vinculação) deve corresponder ao Campo de destino.

   Por exemplo, a ID do Parâmetro da categoria (Campo de vinculação exibido no Objeto original) é referenciada a partir de Parâmetro (Objeto original). parameterID (Campo de vinculação ao Objeto de destino) é exibido na guia Campos do Parâmetro de categoria (Objeto de vinculação). O Campo de vinculação ao Objeto de destino que é exibido no Objeto de vinculação corresponde ao Campo de destino.

1. Usando a API Explorer, identifique a variável **Código do objeto** do Objeto de vinculação (Parâmetro de categoria).\
   Por exemplo, o Código de Objeto para o Parâmetro da Categoria é CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Crie um filtro para o Objeto Original.\
   Por exemplo, crie um filtro Parâmetro.\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para modo de texto**.
1. (Condicional) Se estiver filtrando por objetos que estão ausentes, cole o seguinte exemplo de fórmula na interface do modo texto do novo filtro e substitua o texto de exemplo pelos objetos e campos corretos:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   Para obter um exemplo de relatórios sobre Campos personalizados não associados ao Forms personalizado, consulte [Exemplo 2: filtro para objetos ausentes: campos personalizados que não aparecem em nenhum formulário personalizado](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) neste artigo.

1. Clique em **Salvar Filtro**.

## Exemplos de filtros do modo de texto que abrangem vários níveis na hierarquia do objeto

Use esses exemplos para criar filtros de modo de texto com instruções EXISTS.

### Exemplo 1: filtrar problemas por Nome do proprietário do Portfolio {#example-1-filter-for-issues-by-portfolio-owner-name}

Usando a interface de modo de texto, é possível criar um filtro para uma lista de problemas para exibir somente problemas que estão em projetos associados a um portfólio cujo proprietário é um usuário específico.

Para filtrar problemas pelo Nome do Proprietário do Portfolio:

1. Criar um filtro de Problema.\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para modo de texto**.
1. Consulte o seguinte código genérico:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>`

1. Cole o código a seguir no **Definir regras de filtro para seu relatório** para substituir o código genérico acima:

   `EXISTS:A:$$OBJCODE=PROJ`

   `EXISTS:A:ID=FIELD:projectID`

   `EXISTS:A:portfolio:ownerID=4d94d7da001699b19edf50de15682221`

   >[!NOTE]
   >
   >* O objeto original é o objeto do relatório: Problema
   >* O objeto de destino é Portfolio.
   >* O objeto de vinculação é projeto.
   >* O campo Target e o campo Linking ao objeto Target referenciado do objeto Linking são ownerID.
   >* O código do Objeto de vinculação aqui é PROJ.
   >* O Campo de vinculação exibido no Objeto original é projectID e o Campo de vinculação é ID.

1. Substitua o valor do Campo de público alvo (ownerID) na última instrução por uma ID de usuário do seu ambiente.
1. Clique em **Salvar Filtro**.

### Exemplo 2: filtro para objetos ausentes: campos personalizados que não aparecem em nenhum formulário personalizado {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Usando a interface do modo de texto, você pode criar um filtro para exibir Campos personalizados (Parâmetros) que não estão associados ao Forms personalizado (Categorias). Esse filtro vincula Parâmetros a Categorias, que são conectadas por meio de outro objeto, Parâmetro de categoria. Como os dois campos não estão diretamente conectados uns aos outros e como você está filtrando informações ausentes, é necessário usar uma instrução EXISTS.

>[!IMPORTANT]
>
>Um Parâmetro é um campo existente na Biblioteca de campos referenciada em um Formulário personalizado. Um Parâmetro de Categoria é a versão de um campo que aparece em um formulário específico. Por exemplo, se o mesmo campo aparecer em 5 formulários, haverá 1 Parâmetro e 5 Parâmetros de categoria no banco de dados do Workfront.

Para filtrar Campos Personalizados que não estão associados a um Formulário Personalizado:

1. Crie um Parâmetro ou um filtro de Campo personalizado.\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para modo de texto**.
1. Consulte o seguinte código genérico:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

1. Cole o código a seguir no **Definir regras de filtro para seu relatório** para substituir o código genérico acima:

   `EXISTS:A:$$OBJCODE=CTGYPA`

   `EXISTS:A:parameterID=FIELD:ID`

   `EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   >[!NOTE]
   >
   >* O Objeto original é o objeto do relatório: Parâmetro.
   >* O Objeto de Destino é Categoria.
   >* O objeto de vinculação é parâmetro de categoria.
   >* O código de objeto do objeto de vinculação é CTGYPA.
   >* O Campo de Vinculação ao Objeto de Destino é parameterID, pois parameterID existe na Tabela de Objetos de Vinculação e na Tabela de Objetos de Destino.
   >* O Campo de vinculação exibido no Objeto original é a ID (do Parâmetro da categoria).

1. Clique em **Salvar Filtro**.

### Exemplo 3: filtro para objetos ausentes: usuários que não registraram tempo por um determinado período {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Usando a interface do modo de texto, é possível criar um filtro para exibir os usuários que não registraram horas por um determinado período. Esse filtro vincula os usuários às horas, que são conectadas uns aos outros diretamente. No entanto, você deve usar uma instrução EXISTS e a interface de modo de texto para poder filtrar por informações ausentes.

Para filtrar usuários que não registraram horas durante a semana passada:

1. Criar um filtro de Usuário.\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para modo de texto**.
1. Consulte o seguinte código genérico:

   `EXISTS:A:$$OBJCODE=<Object code of the Linking Object>`

   `EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

1. Cole o código a seguir no **Definir regras de filtro para seu relatório** para substituir o código genérico acima:

   `EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS`

   >[!NOTE]
   >
   >* O Objeto original é o objeto do relatório: Usuário.
   >* O objeto de destino é a hora.
   >* Você não precisa de um Objeto de vinculação neste exemplo porque Usuários e Horas estão conectados diretamente no banco de dados do Workfront.
   >* Como não há Objeto de Vinculação, você deve usar o Código do Objeto do Objeto de Destino: HORA.
   >* O Campo de vinculação ao Objeto de destino é ownerID (que é exibido no Objeto original; o Objeto de vinculação está ausente).
   >* O Campo de vinculação exibido no Objeto original é a ID (da hora) (exibida no Objeto de destino; o Objeto de vinculação está ausente).
   >* O EXISTE:A:A instrução entryDate se refere aos campos que definem o Objeto do Target (Hora) e usa a mesma sintaxe que em uma instrução de filtro regular. Isso garante que você exiba apenas os usuários que não registraram horas por um período específico, neste caso, a semana anterior.
   >* O modificador NOTEXISTS indica que estamos procurando itens (Horas) que não existem para o objeto do relatório (Usuários).

1. Clique em **Salvar Filtro**.

### Exemplo 4: filtrar por vários campos: tarefas por Nome do proprietário do Portfolio e ID do Scorecard do alinhamento de Portfolio {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Usando a interface de modo de texto, você pode criar um filtro que se refere a mais de um campo no Objeto de destino. Nesse caso, as instruções de filtro que se referem aos Campos de destino devem ser conectadas por AND.

Por exemplo, você pode filtrar uma lista de tarefas para exibir somente as tarefas que atendem aos seguintes critérios:

* Eles estão em um projeto associado a um portfólio cujo proprietário é um usuário específico.
* Eles estão em um projeto associado a um portfólio cujos projetos não estão associados a um scorecard de alinhamento específico.

Para filtrar tarefas pelo Nome do Proprietário do Portfolio e ID do Scorecard do Alinhamento Portfolio:

1. Criar um filtro de Tarefa.\
   Para obter informações sobre como criar filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Alternar para modo de texto**.
1. Cole o código a seguir no **Definir regras de filtro para seu relatório** área:

   `EXISTS:A:$$OBJCODE=PROJ`
   `EXISTS:A:ID=FIELD:projectID`
   `EXISTS:A:portfolio:ownerID=4d80ce5200000528787d57807732a33f`
   `AND:A:EXISTS:A:$$EXISTSMOD=NOTEXISTS`
   `AND:A:EXISTS:A:$$OBJCODE=PROJ`
   `AND:A:EXISTS:A:ID=FIELD:projectID`
   `AND:A:EXISTS:A:portfolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad`

   >[!NOTE]
   >
   >* O Objeto original é o objeto do filtro: Tarefa.
   >* O objeto de destino é Portfolio.
   >* O primeiro Campo de destino é ownerID.
   >* O segundo campo do Target é ID do Scorecard de Alinhamento.
   >* O objeto de vinculação é projeto.
   >* O código do objeto de vinculação é PROJ.
   >* O campo Vinculação ao Objeto de Destino é a ID (do Portfolio).
   >* O Campo de vinculação exibido no Objeto original é projectID.
   >* Substitua a ID do proprietário por uma ID de usuário do seu ambiente.

1. Clique em **Salvar Filtro**.
