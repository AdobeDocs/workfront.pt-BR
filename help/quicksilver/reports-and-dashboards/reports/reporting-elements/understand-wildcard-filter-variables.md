---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Variáveis de filtro curinga
description: Ao usar curingas em filtros, você pode fazer referência a um usuário ou data genérica em vez de a um usuário ou data específica. Dessa forma, os elementos criados são dinâmicos e os resultados mudam de acordo com o contexto em que são usados.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 577761ff5d1fb59db104df5995af953a0b5e6c0c
workflow-type: tm+mt
source-wordcount: '1439'
ht-degree: 1%

---

# Visão geral das variáveis de filtro curinga

<!-- Audited: 11/2024 -->

<!--(NOTE: This article is linked to the training self-serve promoted articles for user-based and date-based wildcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.)
(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.
This was included but it is not supported???:
The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.
For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:
AssignedToID Equals $$USER.roleIDs.)-->

Usando curingas, você pode fazer referência a um usuário ou data genérica em vez de a um usuário ou data específica. Dessa forma, os elementos criados são dinâmicos; os resultados mudam dependendo do contexto em que são usados.

Por exemplo, a filtragem de $$USER.homeGroupID em um relatório de projeto recupera apenas projetos associados ao Grupo inicial do usuário que está conectado.

Você pode usar variáveis de filtro, também conhecidas como curingas, ao criar os seguintes elementos:

<table>
    <tr>
        <td>Filtros em listas, relatórios e no Planejador de recursos</td>
        <td>Para obter informações sobre filtros Workfront, consulte o artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">Visão geral dos filtros</a>.
</td>
    </tr>
    <tr>
        <td>Pesquisas avançadas</td>
        <td>Para obter informações sobre pesquisas avançadas, consulte a seção <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">Usar Pesquisa Avançada</a> no artigo <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Pesquisar Adobe Workfront</a>.
    </tr>
    <tr>
        <td>Colunas calculadas em visualizações</td>
        <td></td>
    </tr>
    <tr>
        <td>Formatação condicional em exibições</td>
        <td>Para obter informações sobre formatação condicional, consulte o artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">Usar formatação condicional nas exibições</a>.
    </tr>
    <tr>
        <td>Campos personalizados calculados</td>
        <td>Não há suporte para variáveis de filtro curinga ao fazer referência a coleções aninhadas em uma coluna calculada.

Para obter informações sobre campos e colunas personalizados calculados, consulte o artigo <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">Campos personalizados calculados vs. colunas calculadas</a>.
</td>
    </tr>
</table>

## Variáveis de filtro curinga com base em data

As opções de curinga com base em data podem ser usadas em combinação com qualquer atributo de filtro de data. Para obter informações sobre como adicionar um curinga baseado em data a um relatório, consulte o artigo [Usar curingas baseados em data para generalizar relatórios](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Se você criar um cálculo de data e hora que não inclua uma parte do tempo ou que use os curingas de data $$TODAY ou $$NOW, o sistema usará a data de acordo com o fuso horário Coordenado Universal Time (UTC), não de acordo com o fuso horário local. Isso pode causar um resultado inesperado de data.

Você pode escolher entre os seguintes curingas com base em data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$HOJE</strong> </p> </td> 
   <td> <p>Recomendamos que você crie filtros sensíveis a data usando esse curinga para evitar a criação do filtro novamente amanhã, na próxima semana ou no próximo mês.</p> <p>Por exemplo, se você quiser exibir todas as tarefas com vencimento antes de hoje, poderá usar a seguinte regra em um filtro de tarefa: <em>Data de Início Planejada Menor que $$TODAY</em>.</p> <p>$$TODAY é sempre igual à meia-noite do dia atual.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Isso é semelhante ao curinga $$TODAY, mas inclui a data e a hora atuais. $$NOW é igual à data e hora atuais.</p> <p>Por exemplo, se você deseja exibir todas as entradas de horas fornecidas até a hora atual, você pode fazer isso usando a seguinte regra em um filtro de horas: <em>Data de Início Planejada Menor que $$NOW</em>.</p> <p>Observação: Este curinga não é suportado no Planejador de Recursos.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para indicar vários períodos de tempo e vários pontos no tempo (futuros ou passados), você pode combinar os curingas acima com o seguinte:

| Atributos |   |
|---|---|
| **q** | trimestre civil |
| **h** | hora |
| **d** | dia |
| **w** | semana |
| **m** | mês |
| **a** | ano |

{style="table-layout:auto"}

| **Qualificadores** | |
|---|---|
| **b** | início do período (sem um atributo especificado, o padrão é início da semana: domingo) |
| **e** | fim do período (sem um atributo especificado, o padrão é fim da semana: sábado) |

{style="table-layout:auto"}

| **Operadores** | |
|---|---|
| **+** | adicionar valor ao valor curinga |
| **-** | subtrair valor do valor curinga |

{style="table-layout:auto"}

Por exemplo, o curinga `$$TODAYb+2w` se refere a &quot;2 semanas a partir do início desta semana&quot;. O curinga *`$$NOW+2h` se refere a &quot;daqui a 2 horas&quot;.

## Variáveis de filtro curinga com base no usuário

>[!IMPORTANT]
>
>Se um filtro ou relatório contiver uma variável de filtro curinga baseada em usuário, os resultados sempre mostrarão informações filtradas pelo usuário que está conectado no momento. Quando você compartilha esse filtro ou relatório com outro usuário, o curinga recupera informações para o usuário que está observando o relatório. Os dois usuários veem resultados diferentes.
>
>Para obter informações sobre como adicionar um curinga baseado no usuário a um relatório, consulte o artigo [Usar curingas baseados no usuário para generalizar relatórios](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Você pode escolher entre as seguintes variáveis baseadas no usuário:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>A variável baseada em usuário mais comum é $$USER.ID. Isso sempre retorna a ID do usuário conectado. Essa é a ID usada para identificar qual usuário criou cada objeto e suas atribuições de trabalho.</p> <p>Quando usado em relatórios, esse curinga diminui o número de relatórios que precisam ser criados em seu sistema. É possível criar um relatório e compartilhá-lo com vários usuários, e os resultados são alterados com base no usuário que está conectado e observando o relatório.</p> <p>Por exemplo, para criar um relatório para todos os problemas atribuídos ao usuário que está conectado, você pode usar a seguinte regra em um filtro de problemas: <em>Atribuído a ID igual a $$USER.ID</em>.</p> <p>O Workfront usa essa variável nos seguintes filtros incorporados:</p> 
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
   <td> <p>A variável $$USER.categoryID se refere a um formulário personalizado específico associado ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>A variável $$USER.accessLevelID se refere à ID do nível de acesso associado ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>A variável $$USER.accessLevelRank se refere à classificação de nível de acesso associada ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>A variável $$USER.companyID refere-se à empresa associada ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>A variável $$USER.customerID se refere à ID da conta do cliente associada ao seu ambiente. Para o seu ambiente, há apenas um valor possível para essa variável e ela normalmente é usada somente ao criar integrações por meio da API.</p> </td> 
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
   <td> <p>A variável $$USER.name se refere ao nome completo do usuário conectado.</p> <p>Nota:   <p>Essa variável curinga funciona somente ao modificar um filtro no modo de texto. Não é possível usar esse curinga em filtros que não oferecem suporte ao modo de texto. Por exemplo, não é possível usar esse curinga nos filtros nas seguintes áreas:</p> 
     <ul> 
      <li> <p>Planejador de recursos</p> </li> 
      <li> <p>Balanceador de carga de trabalho</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>A variável $$USER.homeGroupID se refere à ID do Grupo padrão do usuário conectado. Como um Administrador de grupo, você pode usar essa variável para filtrar somente por itens que pertençam aos usuários no seu grupo padrão.</p> <p>Por exemplo, para ver todas as tarefas incompletas nos projetos do grupo financeiro, use as seguintes regras de filtro em um filtro de tarefa:<br><em>Projeto: ID de Grupo igual a $$USER.homeGroupID </em><br><em>Percentual Concluído menor que 100</em></p> <p>Para ver todas as tarefas incompletas atribuídas a indivíduos em um grupo específico que seja o Grupo inicial do usuário conectado, use as seguintes regras de filtro em um filtro de tarefa:</p> <p><em>Atribuído a: ID de Grupo igual a $$USER.homeGroupID<br>Percentual de Conclusão Menor que 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>A variável $$USER.otherGroupIDs se refere a todos os grupos (incluindo o Grupo inicial) associados ao perfil do usuário conectado.</p> <p>A funcionalidade dessa variável é semelhante à da variável $$USER.homeGroupID, exceto que os resultados exibem informações sobre os usuários que pertencem a qualquer um dos grupos associados ao usuário conectado.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>A variável $$USER.homeTeamID se refere à ID da Equipe inicial do usuário conectado. Como um gerente de equipe, você pode usar essa variável para filtrar apenas por itens que pertencem aos usuários na sua Equipe inicial.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>A variável $$USER.teamIDs retorna uma lista de todas as equipes associadas ao usuário logado.</p> <p>A funcionalidade dessa variável é semelhante à da variável $$USER.homeTeamID, exceto que os resultados exibem informações sobre o usuário que pertence a qualquer uma das equipes identificadas no filtro.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>A variável $$USER.roleID refere-se à Função principal do usuário conectado. Usando essa variável, você pode relatar tarefas ou problemas atribuídos a uma função de trabalho específica.</p> <p>Por exemplo, para ver todas as tarefas atribuídas à função principal do usuário conectado, é possível usar a seguinte regra de filtro em um filtro de tarefa:</p> <p><em>Tarefa: a ID da Função é igual a $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>A variável $$USER.roleIDs se refere a todas as funções de trabalho associadas ao usuário conectado. Usando essa variável, você pode relatar tarefas ou problemas atribuídos a qualquer uma das funções de trabalho associadas ao usuário conectado. </p> <p>Por exemplo, para ver todas as tarefas atribuídas a qualquer uma das funções associadas ao usuário conectado, é possível usar a seguinte regra de filtro em um filtro de tarefa:</p> <p><i>Tarefa: a ID da Função é igual a $$USERID.roleIDs<br></i> </p> <p>Dica: A regra de filtro <i>Tarefa: ID de Função igual a $$USERID.roleIDs</i> existe nos filtros internos Tarefas não atribuídas em minha função e Problemas não atribuídos em minha função. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Variáveis de filtro curinga com base em objeto

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
     <p>Em um formulário personalizado, quando os tipos de objeto selecionados do formulário forem incompatíveis com um campo referenciado em um campo personalizado calculado, você poderá usar esse curinga para evitar a solução alternativa de criar formulários duplicados para esses tipos de objeto.</p> 
     <p>No campo personalizado calculado, faça isso incluindo o curinga em uma expressão IF para que o cálculo possa produzir valores diferentes para cada um dos tipos de objeto do formulário. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
