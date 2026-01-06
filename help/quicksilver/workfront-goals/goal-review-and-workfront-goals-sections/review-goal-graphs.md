---
product-previous: workfront-goals
navigation-topic: goal-review-and-sections
title: Revise os gráficos para entender as tendências de progresso das metas no Adobe Workfront Goals
description: Você pode visualizar a integridade geral de suas metas e a tendência do progresso delas no tempo na seção Gráficos das Metas do Adobe Workfront. Os gráficos nesta seção não detalham o progresso de cada meta, mas fornecem um instantâneo holístico do status de progresso de todas as metas, bem como sua tendência de progresso no tempo durante um período especificado.
author: Alina
feature: Workfront Goals
exl-id: 8d5f3617-c7bf-44ce-99b0-d4ebda106f25
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 2%

---

# Revise gráficos para entender as tendências de progresso das metas no Adobe Workfront Goals

<!--Audited for P&P only: 4/2025-->

Você pode visualizar a integridade geral de suas metas e a tendência do progresso delas no tempo na seção Gráficos das Metas do Adobe Workfront. Os gráficos nesta seção não detalham o progresso de cada meta, mas fornecem um instantâneo holístico do status de progresso de todas as metas, bem como sua tendência de progresso no tempo durante um período especificado.

>[!IMPORTANT]
>
>Você pode ver uma contagem total de suas metas na seção Gráficos para um período selecionado. No entanto, o Workfront Goals leva em conta apenas metas com status Ativo e Fechado ao calcular o status do progresso geral da meta e o percentual concluído.

## Requisitos de acesso

>[!NOTE]
>
>Sua empresa pode optar por continuar usando o Adobe Workfront Goals se ele comprou esse pacote no passado. Você precisa falar com o seu representante de conta para obter mais detalhes.
>
>O Adobe Workfront Goals não está mais disponível para compra.

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacote do Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licença do Adobe Workfront</td>
 <td>
 <p>Colaborador ou superior</p>
<p>Solicitação ou superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuração do nível de acesso</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo Administradores do sistema, devem receber um modelo de layout que inclua a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td>  
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
    <p> New product requirement: Workfront</p>
    Or
    <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p> </td>
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
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Tipos de gráficos nas Metas do Workfront

Os gráficos a seguir estão disponíveis na seção Gráficos ou Metas do Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Gráfico de integridade da meta</td> 
   <td> <p>Um gráfico de medidores que mostra o seguinte:</p> 
    <ul> 
     <li>Um número total de metas para o período selecionado. Metas com qualquer status são consideradas. </li> 
     <li>O status do progresso das metas com status Ativo e Fechado.</li> 
    </ul> <p>Para obter informações sobre como o Workfront Goals calcula o status do progresso, consulte <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Visão geral do progresso e da condição da meta no Adobe Workfront Goals</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">O Gráfico de Progresso da Meta</td> 
   <td> <p>Um gráfico de linha que mostra as atualizações feitas nas metas em incrementos semanais durante a duração da meta. O gráfico de progresso da meta exibe o seguinte:</p> 
    <ul> 
     <li>Uma porcentagem média de conclusão esperada e real de todas as metas ativas e fechadas no período selecionado. O progresso do percentual de conclusão é dividido em incrementos semanais marcados por nós. </li> 
     <li>A porcentagem média geral de progresso de metas ativas e fechadas desde a semana anterior. </li> 
    </ul> <p>Dica: o gráfico de progresso da meta pode não exibir nenhuma informação quando as atualizações são feitas nas metas fora do período selecionado. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Revisar o progresso da meta em gráficos

{{step1-to-goals}}

Isso abre a área Metas do Workfront.

1. Clique em **Gráficos** no painel esquerdo.

   ![Gráficos no painel esquerdo](assets/graphs-in-left-panel.png)

   A seção Gráficos é exibida.

   Por padrão, as metas exibidas na seção Gráficos são limitadas pelos seguintes critérios:

   * Os filtros aplicados à área Gráficos.
   * Metas com status Ativo e Rascunho.

1. (Opcional) Selecione o tipo de informação que deseja exibir, atualizando os filtros no canto superior direito da seção Gráficos.

   Para obter mais informações sobre como filtrar metas, consulte [Filtrar informações em Metas da Adobe Workfront](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   >[!TIP]
   >
   >Se você optou por exibir mais de um período, um gráfico de integridade (medidor) e um gráfico de progresso (linha) serão exibidos para cada período.

1. Revise as informações na tabela abaixo ao revisar o Gráfico de integridade da meta.

   ![Gráfico de medição](assets/gauge-graph-wf-align-350x230.png)

   | Número total de metas | O número na parte inferior do gráfico indica o número de todas as metas no período selecionado, em todos os status selecionados. |
   |---|---|
   | Percentual médio concluído | Na parte superior do gráfico, esse número indica o percentual médio de conclusão de metas ativas e fechadas no período selecionado. |
   | Metas e seu progresso | O número de metas para cada segmento de status de progresso, quando você passa o mouse sobre os segmentos do gráfico. Somente metas em um status Ativo ou Fechado são contadas nos segmentos. |


1. Revise as informações na tabela abaixo ao revisar o Gráfico de Progresso da Meta.

   ![Gráfico de linhas](assets/line-graph-wf-align-350x161.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Progresso da linha de base</td> 
      <td>A linha de inclinação verde indica a média geral concluída esperada de metas ativas e fechadas para o período selecionado. Espera-se que todas as metas em um período sejam concluídas, de modo que o progresso da linha de base seja sempre 100% no final do período. </td> 
     </tr> 
     <tr> 
      <td>Progresso real</td> 
      <td> <p>A linha azul indica a média geral de porcentagem concluída real de metas ativas e fechadas para o período selecionado em incrementos semanais. Cada semana durante a duração da meta é marcada por um nó na linha. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Passe o mouse sobre um nó semanal no gráfico de progresso da meta e analise o seguinte:

   * **Data da semana**: o mês, o dia e o ano da semana selecionada.
   * **Progresso**: uma média do percentual de conclusão real de todas as metas para a semana selecionada.
   * **Linha de Base**: uma média da porcentagem concluída esperada de todas as metas para a semana selecionada.

1. (Opcional) Clique em **Progresso** na parte inferior do gráfico de progresso para remover a linha de progresso geral real

   Ou

   Clique em **Linha de Base** na parte inferior do gráfico de progresso para remover o progresso esperado do gráfico.


