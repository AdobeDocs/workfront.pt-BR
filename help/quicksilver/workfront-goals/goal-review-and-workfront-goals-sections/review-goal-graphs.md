---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Analise gráficos para entender as tendências de progresso da meta nas metas do Adobe Workfront
description: Você pode visualizar a integridade geral de suas metas e a tendência de progresso no tempo na seção Gráficos das Metas do Adobe Workfront . Os gráficos desta seção não detalham o progresso de cada meta, mas fornecem um instantâneo holístico do status de progresso de todas as metas, bem como de sua tendência de progresso no tempo durante um período especificado.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: 3989903687f2ea64ebd5ad754119ce1a9d70b9f3
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 0%

---

# Analise gráficos para entender as tendências de progresso da meta nas metas do Adobe Workfront

<!-- drafted mostly for P&P release-->

Você pode visualizar a integridade geral de suas metas e a tendência de progresso no tempo na seção Gráficos das Metas do Adobe Workfront . Os gráficos desta seção não detalham o progresso de cada meta, mas fornecem um instantâneo holístico do status de progresso de todas as metas, bem como de sua tendência de progresso no tempo durante um período especificado.

>[!IMPORTANT]
>
>Você pode ver uma contagem total de suas metas na seção Gráficos de um período selecionado. No entanto, as Metas da Workfront levam em conta apenas as metas com status Ativo e Fechado ao calcular o status geral do progresso da meta e o percentual concluído.

## Requisitos de acesso

<!--drafted for P&P release: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->

Você deve ter o seguinte acesso para executar as ações descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve comprar uma licença adicional para a funcionalidade Metas da Adobe Workfront para acessar descrita neste artigo. </p> <p>Para obter mais informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as metas do Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso às metas</p> <p><b>Nota</b><p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acesso às Metas da Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> 
    <div> 
     <p>Visualizar ou aumentar permissões em metas</p> 
     <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta na Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve ter o seguinte antes de começar:

* Um modelo de layout que inclui a área Metas no Menu principal.

## Tipos de gráficos em metas do Workfront

Os seguintes gráficos estão disponíveis na seção Gráficos ou Metas do Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">O Gráfico de Saúde da Meta</td> 
   <td> <p>Um gráfico de medidor que exibe o seguinte:</p> 
    <ul> 
     <li>Um número total de metas para o período de tempo selecionado. Os objetivos com qualquer status são considerados. </li> 
     <li>O status do progresso das metas com status Ativo e Fechado.</li> 
    </ul> <p>Para obter informações sobre como o Workfront Metas calcula o status do progresso, consulte <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Visão geral do progresso e condição da meta nas Metas da Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">O Gráfico de Progresso da Meta</td> 
   <td> <p>Um gráfico de linhas que exibe atualizações feitas nas metas em incrementos semanais durante a duração da meta. O gráfico de progresso da meta exibe o seguinte:</p> 
    <ul> 
     <li>Uma porcentagem média esperada e real concluída de todas as metas ativas e fechadas no período selecionado. O progresso percentual completo é dividido em incrementos semanais marcados por nós. </li> 
     <li>A porcentagem média geral de progresso para metas ativas e fechadas desde a semana anterior. </li> 
    </ul> <p>Dica: O gráfico de progresso da meta pode não exibir nenhuma informação quando forem feitas atualizações nas metas fora do período selecionado. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Revisar o progresso da meta em gráficos

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) > **Metas** no canto superior direito.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-review-and-workfront-goals-sections/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Isso abre a área Metas do Workfront .

1. Clique em **Gráficos** no painel esquerdo.

   ![](assets/graphs-in-left-panel.png)

   A seção Gráficos é exibida.

   Por padrão, as metas exibidas na seção Gráficos são limitadas pelos seguintes critérios:

   * Os filtros aplicados à área Gráficos.
   * Metas que estão em um status de Ativo e Rascunho.

1. (Opcional) Selecione o tipo de informação que deseja exibir atualizando os filtros no canto superior direito da seção Gráficos.

   Para obter mais informações sobre como filtrar metas, consulte [Filtrar informações em metas do Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   Se você tiver selecionado a exibição de mais de um período, um gráfico de integridade (medidor) e um gráfico de progresso (linha) serão exibidos para cada período.

1. Revise as informações na tabela abaixo ao revisar o Gráfico de Integridade da Meta.

   ![](assets/gauge-graph-wf-align-350x230.png)

   | Número total de metas | O número na parte inferior do gráfico indica o número de metas no período selecionado, em todos os status que você selecionou. |
   |---|---|
   | Porcentagem média concluída | Na parte superior do gráfico, esse número indica a porcentagem média completa de metas ativas e fechadas no período selecionado. |
   | Objetivos e progressos alcançados | O número de metas para cada segmento de status do progresso, quando você passa o mouse sobre os segmentos do gráfico. Somente as metas em um status de Ativa ou Fechada são contadas nos segmentos. |


1. Revise as informações na tabela abaixo ao revisar o Gráfico de Andamento da Meta.

   ![](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Progresso da linha de base</td> 
      <td>A linha de inclinação verde indica a porcentagem total esperada de metas ativas e fechadas para o período de tempo selecionado. Espera-se que todas as metas dentro de um período sejam concluídas, de modo que o progresso da linha de base seja sempre 100% no final do período. </td> 
     </tr> 
     <tr> 
      <td>Progresso real</td> 
      <td> <p>A linha azul indica a porcentagem total real de metas ativas e fechadas para o período de tempo selecionado em incrementos semanais. Cada semana durante a duração da meta é marcada por um nó na linha. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passe o mouse sobre um nó de semana no gráfico de progresso de meta e revise o seguinte:

   * **Data da semana**: O mês, dia e ano da semana selecionada.
   * **Andamento**: Uma média da porcentagem real concluída de todas as metas da semana selecionada.
   * **Linha de base**: Uma média da porcentagem esperada concluída de todas as metas da semana selecionada.

1. (Opcional) Clique em **Andamento** na parte inferior do gráfico de progresso para remover a linha de progresso geral real

   Ou

   Clique em **Linha de base** na parte inferior do gráfico de progresso para remover o progresso esperado do gráfico.

 
