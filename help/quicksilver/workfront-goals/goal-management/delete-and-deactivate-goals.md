---
product-previous: workfront-goals
navigation-topic: old-workfront-goals-articles
title: Excluir e desativar metas no Adobe Workfront Goals
description: Quando você começa a trabalhar em uma meta do e ela se torna irrelevante em sua organização, recomendamos desativá-la, em vez de excluí-la. Desativar uma meta mantém suas informações históricas e oferece a você a chance de reativá-la posteriormente. Entretanto, há momentos em que a exclusão de uma meta pode fazer sentido, para manter a precisão da sua lista de metas.
author: Alina
feature: Workfront Goals
exl-id: 3089adeb-3e56-492a-82fe-536f57079b73
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 3%

---

# Excluir e desativar metas no Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Quando você começa a trabalhar em uma meta do e ela se torna irrelevante em sua organização, recomendamos desativá-la, em vez de excluí-la. Desativar uma meta mantém suas informações históricas e oferece a você a chance de reativá-la posteriormente. Entretanto, há momentos em que a exclusão de uma meta pode fazer sentido, para manter a precisão da sua lista de metas.

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
 <p>Or</p>
  <p>Current product requirement: In addition to a Workfront license, you must purchase a license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
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

## Desativar metas

Você pode desativar uma meta que não é mais relevante e que talvez queira reativar no futuro.

* [Considerações ao desativar metas](#considerations-when-deactivating-goals)
* [Desativar metas](#deactivate-goals)

### Considerações ao desativar metas

Lembre-se do seguinte ao desativar metas:

* Você só pode desativar metas em um status Ativo. Para obter informações sobre como ativar uma meta, consulte [Ativar metas no Adobe Workfront Goals](../../workfront-goals/goal-management/activate-goals.md).

  >[!TIP]
  >
  >Não é possível desativar metas em um status de Rascunho.

* O Workfront para de calcular o progresso das metas desativadas.
* As metas inativas não são mais exibidas em ou são consideradas na seção Gráficos das Metas do Workfront. Para obter informações sobre gráficos de metas do Workfront, consulte [Revisar gráficos para entender as tendências de progresso das metas no Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/review-goal-graphs.md).

  <!--* The Check-in section. For information about the Check-in page, see [Update goal progress in Adobe Workfront Goals](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md). -->

* Você não pode mais fazer atualizações em metas desativadas.
* É possível editar informações sobre a meta e seu alinhamento.
* Você pode reativar uma meta desativada anteriormente.

### Desativar metas

<!--
Deactivating goals differs depending on which environment you use.

### Deactivate goals in the Production environment


1. Go to the goal that you want to deactivate.

   For example, go to the Goal List and click the name of a goal.

   The Goal Details panel opens on the right.

   >[!TIP]
   >
   >You can open goals from any sections of Workfront Goals.

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Deactivate**.

   ![Deactivate goal](assets/deactivate-goal-highlighted.png)

   The goal status changes to Inactive. 

1. Click the **X** icon in the upper-right to close Goal Details.
-->

{{step1-to-goals}}

A lista de metas é exibida.


1. (Opcional) Modifique seus filtros para exibir somente as metas que estão ativas.

   Para obter informações sobre como filtrar informações no Workfront Goals, consulte [Informações de filtro no Adobe Workfront Goals](../goal-management/filter-information-wf-goals.md).

1. Clique em uma meta ativa.

   A página de meta é aberta.

   ![Página de meta](assets/goal-page-unshimmed.png)

1. Clique no **Mais** ícone ![Mais](assets/more-icon.png) à direita do nome da meta e clique em **Desativar**.

1. A meta é desativada e seu status torna-se Inativo.

## Excluir metas

Você pode excluir metas que não são mais relevantes ou que talvez nunca sejam relevantes.

* [Considerações ao excluir metas](#considerations-when-deleting-goals)
* [Excluir metas](#delete-goals)

### Considerações ao excluir metas {#considerations-when-deleting-goals}

* É possível excluir metas em qualquer status, incluindo metas fechadas.
* Não é possível recuperar metas excluídas.
* As atividades Resultados e Barra de progresso manual anexadas à meta também são excluídas.
* Os projetos associados às metas não são excluídos, mas a associação deles com a meta é removida.

### Excluir metas

<!--
Deleting  goals differs depending on which environment you use.

#### Delete goals in the Production environment

1. Go to the goal that you want to delete.

   For example, go to the Goal List and click a goal.

   The Goal Details panel opens on the right. 

1. Click the **More icon** ![More icon](assets/more-icon.png), then click **Delete**.

   ![Delete goal](assets/delete-goal-highlighted.png)

1. Click **Yes, delete**.

   The goal is removed from the Goal List and cannot be recovered.
-->

{{step1-to-goals}}

A lista de metas é exibida.

1. Clique no nome de uma meta. Isso abre a página de meta.
1. Clique no menu **Mais** ![Mais ícone](assets/more-icon.png) à direita do nome da meta e clique em **Excluir meta** e depois em **Excluir**.

   A meta e suas atividades e resultados também são excluídos e não podem ser recuperados. Os projetos que foram associados à meta ou às metas secundárias não são excluídos.


