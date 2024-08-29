---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Editar resultados e atividades no Adobe Workfront Goals
description: Depois que o administrador do Adobe Workfront conceder a você o acesso correto às Metas do Adobe Workfront, você poderá criar e editar metas, resultados e atividades.
author: Alina
feature: Workfront Goals
exl-id: 922a05f9-2995-4401-a6d2-e5a331270fd3
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 1%

---

# Editar resultados e atividades no Adobe Workfront Goals

Depois que o administrador do Adobe Workfront conceder a você o acesso correto às Metas do Adobe Workfront, você poderá criar e editar metas, resultados e atividades.

Para obter informações sobre como criar metas, resultados e atividades, consulte os seguintes artigos:

* [Criar metas nas Metas do Adobe Workfront](../../workfront-goals/goal-management/create-goals.md)
* [Introdução a resultados e atividades nas Metas do Adobe Workfront](../../workfront-goals/results-and-activities/get-started-with-results-and-activities.md)
* [Adicionar resultados às metas nas Metas do Adobe Workfront](../../workfront-goals/results-and-activities/add-results-to-goals.md)
* [Adicionar atividades às metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/add-activities-to-goals.md)

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> 
   <p>Para o novo plano e estrutura de licença:
  <ul><li>Um plano Ultimate </li></ul>
   </p>
<p>Para o plano e a estrutura de licença atuais: 
<ul><li> A Pro ou superior </li>
  <li>Uma licença do Adobe Workfront Goals, além de uma licença da Workfront.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licença da Adobe Workfront*</td>
 <td>
 <p>Nova licença: Contributor ou superior</p>
 Ou
 <p>Licença atual: Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">visão geral das licenças da Adobe Workfront</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produto*</td>
 <td>
 <p> Novo requisito de produto, um dos seguintes: </p>
<ul>
<li>Um plano Select ou Prime do Adobe Workfront e uma licença adicional do Adobe Workfront Goals.</li>
<li>Um plano do Ultimate Workfront que inclui o Workfront Goals por padrão. </li></ul>
 <p>Ou</p>
 <p>Requisito atual do produto: um plano do Workfront e uma licença adicional para o Adobe Workfront Goals. </p> <p>Para obter informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as Metas do Workfront</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Nível de acesso</p></td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta no Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclui a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerações ao editar resultados e atividades

<!--
According to Vazgen, access levels will add more considerations.)
-->

* É possível editar resultados e atividades que pertencem às metas criadas ou às metas que você tem permissão para gerenciar.
* Não é possível editar o progresso dos projetos conectados a metas como atividades do Workfront Goals. O progresso dos projetos é atualizado quando as tarefas no projeto são concluídas. Você pode remover projetos da meta do desconectando-os. Para obter mais informações, consulte a seção &quot;Desconectar projetos&quot; no artigo [Remover resultados, atividades e projetos das metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).

  >[!NOTE]
  >
  >Se as seguintes informações do projeto forem atualizadas no nível do projeto, o Workfront Goals as atualizará automaticamente no nível da meta:
  >
  >   
  >   
  >   * Proprietário do projeto
  >   * Nome do projeto
  >   * Percentual concluído do projeto
  >   
  >   
  >Para obter informações sobre como conectar projetos a metas, consulte [Adicionar projetos a metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

* Você pode excluir resultados e atividades das metas quando eles não são mais relevantes para o progresso da meta. Os resultados e as atividades excluídos não podem ser recuperados. Para obter informações sobre como excluir resultados e atividades, consulte [Remover resultados, atividades e projetos das metas no Adobe Workfront Goals](../../workfront-goals/results-and-activities/remove-results-activities-from-goals.md).
* É possível editar resultados e atividades associados a metas de qualquer período, incluindo no passado.
* A edição de resultados e atividades atualiza suas configurações e não atualiza seu progresso. Você deve atualizar o progresso dos resultados e das atividades. Para obter informações sobre como atualizar o progresso de metas, resultados e atividades, consulte [Atualizar progresso da meta em Metas do Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## Editar resultados

<!--
Editing results differs depending on which environment you use.

### Edit results in the Production environment

1. Go to the goal for which you want to edit a result and click the goal name to open the **Goal Details** panel.
1. Click **Results**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the result you want to edit.

   ![](assets/results-gear-icon-options-350x85.png)

1. Click **Edit** to edit the following information:

   | Field |Description|
   |---|---|
   | Name |The name of the result. |
   | Owner |The owner of result.  |
   | Value |How you measure the progress of the result. |
   | Initial |The original value of the result. |
   | Target |The desired value when the result is completed. |

1. Click **Save**.
-->


1. Clique no **Menu principal** ![](assets/main-menu-icon.png) e depois em **Metas**.
1. Na Lista de Metas, clique no nome de uma meta para abrir a página de metas.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. Selecione um resultado na lista Progress indicators e clique no ícone ![](assets/edit-icon.png) **Editar**.

   A caixa Editar resultado é aberta.

   ![](assets/edit-result-box-unshimmed.png)

1. Edite as seguintes informações:
   * **Nome do resultado**: o nome do resultado. Use um nome descritivo que ilustre qual resultado você precisa obter para concluir a meta.
   * **Proprietário do resultado**: o proprietário do resultado. O proprietário deve ser um usuário ativo do Workfront.
   * **Tipo de valor**: como você mede o progresso do resultado.
   * **Valor Inicial**: o valor original do resultado.
   * **Valor de Destino**: o valor desejado quando o resultado é concluído.
Para obter mais informações sobre campos de resultados, consulte [Adicionar resultados às metas](../results-and-activities/add-results-to-goals.md).
1. Clique em **Salvar**.

## Editar atividades

<!--
Editing activities differs depending on which environment you use.

### Edit activities in the Production environment

>[!TIP]
>
>You cannot edit the Activity Type after you saved an activity on a goal.

1. Go to the goal for which you want to edit an activity and click the goal name to open the **Goal Details** panel.
1. Click **Activities**.
1. Click the **gear icon** ![](assets/settings-gear-icon.png) to the right of the activity you want to edit .

   ![](assets/activities-gear-icon-options-350x84.png)

1. Click **Edit** to edit the following information:

   | Field |Description |
   |---|---|
   | Name |The name of the activity. |
   | Owner |The owner of activity.  |

1. Click **Save**.
-->

1. Clique no **Menu principal** ![](assets/main-menu-icon.png) e depois em **Metas**.
1. Na Lista de Metas, clique no nome de uma meta para abrir a página de metas.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. Selecione uma atividade na lista Progress indicators e clique no ícone ![](assets/edit-icon.png) **Editar**.

   A caixa Editar atividade é aberta.

   ![](assets/edit-activity-box-unshimmed.png)

1. Edite as seguintes informações:
   * **Nome da atividade**: o nome da atividade. Use um nome descritivo que ilustre qual atividade você deve executar para indicar que a meta foi concluída.
   * **Proprietário da atividade:** O proprietário da atividade. O proprietário deve ser um usuário ativo do Workfront.\
     Para obter mais informações sobre campos de atividade, consulte [Adicionar atividades às metas](../results-and-activities/add-activities-to-goals.md).
1. Clique em **Salvar**.


