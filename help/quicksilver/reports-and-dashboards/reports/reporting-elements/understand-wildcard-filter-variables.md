---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variáveis de filtro curinga
description: Ao usar curingas em filtros, é possível fazer referência a um usuário ou data genérica em vez de um usuário ou data específica. Dessa forma, os elementos criados são dinâmicos e os resultados mudam de acordo com o contexto em que são usados.
author: Lisa
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 2%

---

# Variáveis de filtro curinga

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

O Adobe Workfront suporta variáveis de filtro ou curingas ao criar os seguintes elementos:

* Filtros em listas, relatórios e o Planejador de recursos

   Para obter informações sobre filtros Workfront, consulte o artigo [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Pesquisas avançadas

   Para obter informações sobre pesquisas avançadas, consulte a seção [Usar pesquisa avançada](../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search) no artigo [Pesquisar Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

* Colunas calculadas em visualizações
* Formatação condicional em exibições

   Para obter informações sobre formatação condicional, consulte o artigo [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

* Campos personalizados calculados

   >[!NOTE]
   >
   >As variáveis de filtro curinga não são compatíveis ao referenciar coleções aninhadas em uma coluna calculada.

   Para obter informações sobre campos e colunas personalizados calculados, consulte o artigo [Campos personalizados calculados vs. colunas calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

Ao usar curingas, você pode fazer referência a um usuário ou data genérica em vez de um usuário ou data específica. Dessa forma, os elementos criados são dinâmicos e os resultados mudam de acordo com o contexto em que são usados.

Por exemplo, filtrar $$USER.homeGroupID em um relatório de projeto recupera apenas projetos associados ao Grupo Doméstico do usuário que está conectado.

Você pode usar variáveis de filtro com base em data ou com base no usuário no Workfront.

## Variáveis de filtro curinga com base em data

As opções de curinga com base em data do Workfront podem ser usadas em combinação com qualquer atributo de filtro de data.

Para obter informações sobre como adicionar um curinga com base em data a um relatório, consulte o artigo [Usar curingas com base em data para generalizar relatórios](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Se você criar um cálculo de data e hora que não inclua uma parte de hora ou que use os curingas de data $$TODAY ou $$NOW, o sistema usará a data de acordo com a zona de Horário Universal Coordenado (UTC), não de acordo com seu fuso horário local. Isso pode causar um resultado de data inesperado.

Escolha entre os seguintes curingas com base em data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>Recomendamos que você crie filtros sensíveis a data usando esse curinga para evitar a criação do filtro novamente amanhã, semana que vem ou mês que vem.</p> <p>Por exemplo, se você quiser exibir todas as tarefas vencidas antes de hoje, poderá usar a seguinte regra em um filtro de tarefa: <em>Data Inicial Planejada Inferior A $$TODAY</em>.</p> <p>$$TODAY é sempre igual a meia-noite para o dia atual.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>É semelhante ao curinga $$TODAY, mas inclui a data e a hora atuais. $$NOW é igual à data e hora atuais.</p> <p>Por exemplo, se você quiser exibir todas as entradas de hora fornecidas até o horário atual, é possível fazer isso usando a seguinte regra em um filtro de hora: <em>Data Inicial Planejada Inferior A $$NOW</em>.</p> <p>Observação: Este curinga não é suportado no Planejador de Recursos.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para indicar vários períodos de tempo e vários pontos no tempo (futuro ou passado), é possível combinar curingas com o seguinte:

| Atributos |   |
|---|---|
| **q** | trimestre |
| **h** | hora |
| **d** | dia |
| **w** | semana |
| **m** | mês |
| **y** | ano |

{style=&quot;table-layout:auto&quot;}

| **Qualificadores** |  |
|---|---|
| **b** | início da semana (domingo) |
| **e** | fim da semana (sábado) |

{style=&quot;table-layout:auto&quot;}

| **Operadores** |  |
|---|---|
| **+** | adicionar valor ao valor curinga |
| **-** | subtrair valor do valor curinga |

{style=&quot;table-layout:auto&quot;}

Por exemplo, o curinga `$$TODAYb+2w` refere-se a &quot;2 semanas desde o início desta semana&quot;. O curinga *`$$NOW+2h` refere-se a &quot;daqui a 2 horas&quot;.

## Variáveis de filtro curinga com base no usuário

>[!IMPORTANT]
>
>Se um filtro ou relatório contiver uma variável de filtro curinga baseada no usuário, os resultados sempre mostrarão informações filtradas pelo usuário que está conectado no momento. Quando você compartilha esse filtro ou relatório com outro usuário, o curinga recupera informações para o usuário que está visualizando o relatório. Os dois usuários veem resultados diferentes.

Para obter informações sobre como adicionar um curinga com base no usuário a um relatório, consulte o artigo [Usar curingas baseadas em usuário para generalizar relatórios](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

O Workfront fornece as seguintes variáveis baseadas no usuário:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>A variável mais comum baseada no usuário é $$USER.ID. Isso sempre retorna a ID do usuário conectado. Essa é a ID usada para identificar qual usuário criou cada objeto e suas atribuições de trabalho.</p> <p>Quando usado em relatórios, esse curinga diminui o número de relatórios que você precisa criar no sistema. Você pode criar um relatório e compartilhá-lo com vários usuários, e os resultados são alterados com base no usuário que está conectado e está olhando para o relatório.</p> <p>Por exemplo, para criar um relatório para todos os problemas atribuídos ao usuário que está conectado, você pode usar a seguinte regra em um filtro de problemas: <em>Atribuído à ID igual a $$USER.ID</em>.</p> <p>O Workfront usa essa variável nos seguintes filtros incorporados:</p> 
    <ul> 
     <li>Meus Relatórios</li> 
     <li>Meus projetos</li> 
     <li>Minhas tarefas</li> 
     <li>Meus problemas</li> 
     <li>Minhas horas</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>A variável $$USER.categoryID refere-se a um formulário personalizado específico associado ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>A variável $$USER.accessLevelID refere-se à ID do nível de acesso associado ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>A variável $$USER.accessLevelRank refere-se à classificação do nível de acesso associada ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>A variável $$USER.companyID refere-se à empresa associada ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>A variável $$USER.customerID refere-se à ID da conta do cliente associada ao seu ambiente. Para seu ambiente, há apenas um valor possível para essa variável e ela geralmente é usada apenas ao criar integrações por meio da API.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>A variável $$USER.firstName se refere ao nome do usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>A variável $$USER.lastName se refere ao sobrenome do usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>A variável $$USER.name se refere ao nome completo do usuário conectado.</p> <p>Nota:   <p>Essa variável curinga funciona somente ao modificar um filtro no modo de texto. Não é possível usar esse curinga em filtros que não suportam o modo de texto. Por exemplo, você não pode usar esse curinga nos filtros nas seguintes áreas:</p> 
     <ul> 
      <li> <p>Planejamento de recursos</p> </li> 
      <li> <p>Balanceador de carga de trabalho</p> </li> 
      <li> <p>Análise</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>A variável $$USER.homeGroupID refere-se à ID do Grupo Doméstico do usuário conectado. Como Administrador de grupo, você pode usar essa variável para filtrar apenas itens que pertencem aos usuários do seu Grupo doméstico.</p> <p>Por exemplo, para ver todas as tarefas incompletas em projetos no grupo de finanças, use as seguintes regras de filtro em um filtro de tarefa:<br><em>Projeto: ID de Grupo Igual a $$USER.homeGroupID </em><br><em>Porcentagem Concluída Menor Que 100</em></p> <p>Para ver todas as tarefas incompletas atribuídas a indivíduos em um grupo específico que é o Grupo Doméstico do usuário conectado, use as seguintes regras de filtro em um filtro de tarefa:</p> <p><em>Atribuído a: ID de Grupo Igual a $$USER.homeGroupID<br>Porcentagem Concluída Menor Que 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>A variável $$USER.otherGroupIDs se refere a todos os grupos (incluindo o Grupo Doméstico) associados ao perfil do usuário conectado.</p> <p>A funcionalidade dessa variável é semelhante à da variável $$USER.homeGroupID , exceto que os resultados exibem informações sobre os usuários que pertencem a qualquer um dos grupos associados ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>A variável $$USER.homeTeamID refere-se à ID da Home Team do usuário conectado. Como gerente de equipe, você pode usar essa variável para filtrar apenas itens que pertencem aos usuários em sua Equipe inicial.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.TeamIDs</strong> </p> </td> 
   <td> <p>A variável $$USER.TeamIDs retorna uma lista de todas as equipes associadas ao usuário conectado.</p> <p>A funcionalidade dessa variável é semelhante à da variável $$USER.homeTeamID , exceto que os resultados exibem informações sobre o usuário que pertence a qualquer uma das equipes identificadas no filtro.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>A variável $$USER.roleID refere-se à Função primária do usuário conectado. Usando essa variável, você pode gerar relatórios sobre tarefas ou problemas atribuídos a uma função de trabalho específica.</p> <p>Por exemplo, para ver todas as tarefas atribuídas à Função primária do usuário conectado, você pode usar a seguinte regra de filtro em um filtro de tarefa:</p> <p><em>Tarefa: A ID da função é igual a $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$$USER.roleIDs</td> 
   <td> <p>A variável $$USER.roleIDs se refere a todas as funções de trabalho associadas ao usuário conectado. Usando essa variável, você pode criar relatórios sobre tarefas ou problemas atribuídos a qualquer uma das funções de trabalho associadas ao usuário conectado. </p> <p>Por exemplo, para ver todas as tarefas atribuídas a qualquer uma das funções associadas ao usuário conectado, você pode usar a seguinte regra de filtro em um filtro de tarefa:</p> <p><i>Tarefa: ID de função igual a $$USERID.roleIDs<br></i> </p> <p>Dica: O <i>Tarefa: ID de função igual a $$USERID.roleIDs</i> existe uma regra de filtro nos filtros incorporados Tarefas não atribuídas em minha função e Problemas não atribuídos em minha função. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variáveis de filtro curinga com base em objeto

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>A variável $$OBJCODE refere-se ao tipo de um objeto. </p> 
     <p>Em um formulário personalizado, quando os tipos de objeto selecionados do formulário são incompatíveis com um campo referenciado em um campo personalizado calculado, é possível usar esse curinga para evitar a solução alternativa de criar formulários duplicados para esses tipos de objeto.</p> 
     <p>No campo personalizado calculado, faça isso incluindo o curinga em uma expressão IF para que o cálculo possa produzir valores diferentes para cada um dos tipos de objeto do formulário. </p> 
     <p>Para obter mais informações e um exemplo, consulte a seção <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">Campos personalizados calculados em formulários personalizados com vários objetos</a> no artigo <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Adicionar dados calculados a um formulário personalizado</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
