---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variáveis de filtro de curinga
description: Ao usar curingas em filtros, você pode fazer referência a um usuário ou data genéricos em vez de um usuário ou data específicos. Dessa forma, os elementos criados são dinâmicos e os resultados mudam de acordo com o contexto em que são usados.
author: Courtney
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1439'
ht-degree: 100%

---

# Visão geral das variáveis de filtro de curinga

<!-- Audited: 11/2024 -->

<!--
(NOTE: This article is linked to the training self-serve promoted articles for user-based and date-based wildcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.)
(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.
This was included but it is not supported???:
The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.
For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:
AssignedToID Equals $$USER.roleIDs.)
-->

Usando curingas, você pode fazer referência a um usuário ou data genéricos em vez de um usuário ou data específicos. Dessa forma, os elementos criados são dinâmicos: os resultados mudam dependendo do contexto em que são usados.

Por exemplo, filtrar por $$USER.homeGroupID em um relatório de projeto recupera apenas os projetos associados ao grupo inicial do usuário que está conectado.

Você pode usar variáveis de filtro, também conhecidas como curingas, ao criar os seguintes elementos:

<table>
    <tr>
        <td>Filtros em listas, relatórios e no planejador de recursos</td>
        <td>Para obter informações sobre filtros do Workfront, consulte o artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">Visão geral de filtros</a>.
</td>
    </tr>
    <tr>
        <td>Pesquisas avançadas</td>
        <td>Para obter informações sobre pesquisas avançadas, consulte a seção <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">Usar pesquisa avançada</a> no artigo <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Pesquisa no Adobe Workfront</a>.
    </tr>
    <tr>
        <td>Colunas calculadas em visualizações</td>
        <td></td>
    </tr>
    <tr>
        <td>Formatação condicional em visualizações</td>
        <td>Para obter informações sobre a formatação condicional, consulte o artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">Usar formatação condicional em visualizações</a>.
    </tr>
    <tr>
        <td>Campos personalizados calculados</td>
        <td>As variáveis de filtro curinga não são compátíveis ao referenciar coleções aninhadas em uma coluna calculada.

Para obter informações sobre campos personalizados calculados e colunas calculadas, consulte o artigo <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">Comparação entre campos personalizados calculados e colunas calculadas</a>.
</td>
    </tr>
</table>

## Variáveis de filtro de curinga baseado em data

As opções de curinga baseado em data podem ser usadas em combinação com qualquer atributo de filtro de data. Para obter informações sobre como adicionar um curinga baseado em data a um relatório, consulte o artigo [Usar curingas baseados em data para generalizar relatórios](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Se você criar um cálculo de data e hora que não inclua uma parte de hora ou que use os curingas de data $$TODAY ou $$NOW, o sistema usará a data de acordo com o fuso horário do Tempo Universal Coordenado (UTC), e não de acordo com o seu fuso horário local. Isso pode causar um resultado inesperado na data.

Você pode escolher entre os seguintes curingas baseados em data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>Recomendamos que você crie filtros sensíveis à data usando esse curinga para evitar ter que criar o filtro novamente amanhã, na próxima semana ou no próximo mês.</p> <p>Por exemplo, se você quiser exibir todas as tarefas que vencem antes de hoje, use a seguinte regra em um filtro de tarefas: <em>Data de início planejada anterior a $$TODAY</em>.</p> <p>$$TODAY é sempre igual à meia-noite do dia atual.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Semelhante ao curinga $$TODAY, mas inclui a data e a hora atuais. $$NOW é igual à data e hora atuais.</p> <p>Por exemplo, se você quiser exibir todas as entradas de horas fornecidas até a hora atual, pode fazer isso usando a seguinte regra em um filtro de horas: <em>Data de início planejada anterior a $$NOW</em>.</p> <p>Nota: esse curinga não é compatível com o planejador de recursos.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para indicar vários períodos e vários pontos no tempo (futuros ou passados), você pode combinar os curingas acima com o seguinte:

| Atributos |   |
|---|---|
| **q** | trimestre do calendário |
| **h** | hora |
| **d** | dia |
| **w** | semana |
| **m** | mês |
| **y** | ano |

{style="table-layout:auto"}

| **Qualificadores** | |
|---|---|
| **b** | início do período (sem um atributo especificado, o padrão é início da semana: domingo) |
| **e** | fim do período (sem um atributo especificado, o padrão é fim da semana: sábado) |

{style="table-layout:auto"}

| **Operadores** | |
|---|---|
| **+** | adicionar valor ao curinga |
| **-** | subtrair valor do curinga |

{style="table-layout:auto"}

Por exemplo, o curinga `$$TODAYb+2w` se refere a “2 semanas a partir do início desta semana”. O curinga *`$$NOW+2h` se refere a “daqui a 2 horas”.

## Variáveis de filtro curinga baseado no usuário

>[!IMPORTANT]
>
>Se um filtro ou relatório contiver uma variável de filtro de curinga baseada no usuário, os resultados sempre mostrarão informações filtradas pelo usuário que está conectado no momento. Quando você compartilha esse filtro ou relatório com outro usuário, o curinga recupera informações para o usuário que está vendo o relatório. Os dois usuários veem resultados diferentes.
>
>Para obter informações sobre como adicionar um curinga baseado no usuário a um relatório, consulte o artigo [Usar curingas baseados no usuário para generalizar relatórios](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Você pode escolher entre as seguintes variáveis baseadas no usuário:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td>
   <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    -->
    <p>A variável baseada em usuário mais comum é $$USER.ID. Isso sempre retorna a ID do usuário conectado. Essa é a ID usada para identificar qual usuário criou cada objeto e as respectivas atribuições de trabalho.</p> <p>Quando usado em relatórios, esse curinga diminui o número de relatórios que precisam ser criados no sistema. É possível criar um relatório e compartilhá-lo com vários usuários, e os resultados são alterados com base no usuário que está conectado e vendo o relatório.</p> <p>Por exemplo, para criar um relatório para todos os problemas atribuídos ao usuário que está conectado, você pode usar a seguinte regra em um filtro de problemas: <em>Atribuído à ID igual a $$USER.ID</em>.</p> <p>O Workfront usa essa variável nos seguintes filtros incorporados:</p>
    <ul> 
     <li>Meus relatórios</li> 
     <li>Meus projetos</li> 
     <li>Minhas tarefas</li> 
     <li>Meus problemas</li> 
     <li>Minhas horas</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>A variável $$USER.categoryID se refere a um formulário personalizado específico associado ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>A variável $$USER.accessLevelID se refere à ID do nível de acesso associado ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>A variável $$USER.accessLevelRank refere-se à classificação de nível de acesso associada ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>A variável $$USER.companyID refere-se à empresa associada ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>A variável $$USER.customerID refere-se à ID da conta do cliente associada ao seu ambiente. Para o seu ambiente, há apenas um valor possível para essa variável, o qual normalmente é usado somente ao criar integrações por meio da API.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>A variável $$USER.firstName refere-se ao nome do usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>A variável $$USER.lastName refere-se ao sobrenome do usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>A variável $$USER.name se refere ao nome completo do usuário conectado.</p> <p>Observação:   <p>Essa variável de curinga funciona somente ao modificar um filtro no modo de texto. Não é possível usar esse curinga em filtros que não são compatíveis com o modo de texto. Por exemplo, não é possível usar esse curinga nos filtros nas seguintes áreas:</p> 
     <ul> 
      <li> <p>Planejador de recursos</p> </li> 
      <li> <p>Balanceador de carga de trabalho</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>A variável $$USER.homeGroupID se refere à ID do grupo inicial do usuário conectado. Admins de grupo podem usar essa variável para filtrar somente os itens que pertençam aos usuários no seu grupo inicial.</p> <p>Por exemplo, para ver todas as tarefas incompletas nos projetos do grupo financeiro, use as seguintes regras de filtro em um filtro de tarefa: <br><em>Projeto: ID de grupo igual a $$USER.homeGroupID </em><br><em>Percentual de conclusão menor que 100</em></p> <p>Para ver todas as tarefas incompletas atribuídas a indivíduos em um grupo específico que seja o grupo inicial do usuário conectado, use as seguintes regras de filtro em um filtro de tarefa:</p> <p><em>Atribuído a: ID de grupo igual a $$USER.homeGroupID<br>Percentual de conclusão menor que 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>A variável $$USER.otherGroupIDs refere-se a todos os grupos (incluindo o inicial) associados ao perfil do usuário conectado.</p> <p>A funcionalidade dessa variável é semelhante à de $$USER.homeGroupID, exceto que os resultados exibem informações sobre os usuários que pertencem a qualquer um dos grupos associados ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>A variável $$USER.homeTeamID se refere à ID da equipe inicial do usuário conectado. Gerentes de equipe podem usar essa variável para filtrar apenas os itens que pertencem aos usuários da equipe inicial.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>A variável $$USER.teamIDs retorna uma lista de todas as equipes associadas ao usuário conectado.</p> <p>A funcionalidade dessa variável é semelhante à da variável $$USER.homeTeamID, exceto que os resultados exibem informações sobre o usuário que pertence a qualquer uma das equipes identificadas no filtro.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>A variável $$USER.roleID refere-se à função principal do usuário conectado. Usando essa variável, você pode relatar tarefas ou problemas atribuídos a uma função de trabalho específica.</p> <p>Por exemplo, para ver todas as tarefas atribuídas à função principal do usuário conectado, é possível usar a seguinte regra em um filtro de tarefa:</p> <p><em>Tarefa: ID da função igual a $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>A variável $$USER.roleIDs refere-se a todas as funções de trabalho associadas ao usuário conectado. Usando essa variável, você pode relatar tarefas ou problemas atribuídos a qualquer uma das funções de trabalho associadas ao usuário conectado. </p> <p>Por exemplo, para ver todas as tarefas atribuídas a qualquer uma das funções associadas ao usuário conectado, é possível usar a seguinte regra de filtro em um filtro de tarefa:</p> <p><i>Tarefa: ID da função igual a $$USERID.roleIDs<br></i> </p> <p>Dica: a regra de filtro <i>Tarefa: ID da função igual a $$USERID.roleIDs</i> existe nos filtros internos “Tarefas não atribuídas em minha função” e “Problemas não atribuídos na minha função”. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variáveis de filtro de curinga baseado no objeto

Você pode escolher entre os seguintes curingas baseados em objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>A variável $$OBJCODE refere-se ao tipo de um objeto. </p> 
     <p>Em um formulário personalizado, quando os tipos de objeto selecionados do formulário são incompatíveis com um campo referenciado em um campo personalizado calculado, você pode usar esse caractere curinga para evitar a solução alternativa de criar formulários duplicados para esses tipos de objeto.</p> 
     <p>No campo personalizado calculado, você faz isso incluindo o caractere curinga em uma expressão IF para que o cálculo possa gerar valores diferentes para cada um dos tipos de objeto do formulário. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
