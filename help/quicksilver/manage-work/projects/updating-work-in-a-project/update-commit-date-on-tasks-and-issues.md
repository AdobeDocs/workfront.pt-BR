---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar datas de confirmação nas tarefas e problemas
description: Você pode atualizar manualmente a data de confirmação de uma tarefa ou problema atribuído a você. Para obter mais informações sobre Datas de confirmação no Adobe Workfront, consulte Visão geral da Data de confirmação.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 0%

---


# Atualizar datas de confirmação nas tarefas e problemas

{{highlighted-preview}}

Você pode atualizar manualmente a data de confirmação de uma tarefa ou problema atribuído a você. Para obter mais informações sobre Datas de confirmação no Adobe Workfront, consulte [Visão geral da data de compromisso](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisitos de acesso

<!--Audited: 01/2024-->

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
   Para as novas licenças:
   <ul>
   <li><p>Padrão para tarefas</p> </li>
   <li><p>Colaborador ou superior para problemas</p></li>
   </ul>
   Para licenças atuais:
<ul>
   <li><p>Trabalhar ou mais para tarefas</p></li> 
   <li><p>Solicitação ou superior para problemas</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e problemas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões na tarefa ou problema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

Antes de editar a Data de Compromisso de uma tarefa ou problema, você deve ser atribuído à tarefa ou problema cuja Data de Compromisso você precisa atualizar.

## Atualizar datas de confirmação nas tarefas e problemas


Você pode atualizar a Data de confirmação de uma tarefa ou problema nas seguintes áreas do Workfront:

* A seção Detalhes de uma tarefa ou problema
* <span class="preview">O cabeçalho da tarefa ou do problema</span>

  <span class="preview">O administrador do Workfront ou do grupo deve adicionar a Data de confirmação ao cabeçalho da tarefa ou do problema do modelo de layout para exibi-la na página da tarefa ou do problema.
Para obter informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).</span>

A atualização da Data de confirmação é idêntica para tarefas e problemas.

>[!NOTE]
>
>Você pode solicitar que o administrador do sistema ou do grupo adicione o campo Data de confirmação ao painel Resumo para facilitar a atualização em várias áreas do Workfront.
>
>Para obter mais informações, consulte os seguintes artigos:
>
>* [Visão geral do resumo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Personalizar Início e Resumo usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Ir para uma tarefa ou problema atribuído como **Proprietário**.

   Para obter mais informações sobre descobrir quem é o Proprietário da Tarefa para um problema ou tarefa, consulte a seção [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) no artigo [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. <span class="preview">(Condicional e opcional) Se o administrador do Workfront ou do grupo tiver adicionado a Data de confirmação ao cabeçalho da tarefa ou do problema, clique no link **Data de confirmação** no cabeçalho e selecione uma data no calendário. Se a Data de confirmação não estiver no cabeçalho, continue com as etapas a seguir. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>

1. Clique em **Detalhes da tarefa** ou **Detalhes do problema** no painel esquerdo.
1. Clique em **Visão geral** para expandi-la.
1. Atualize o **Data de confirmação** campo.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Clique em **Salvar alterações**.

   Ocorre o seguinte após fazer essa alteração:

   * A Data de confirmação e a Data de conclusão planejada da tarefa ou problema não são mais a mesma.

     Em vez disso, a Data de confirmação e a Data de conclusão projetada da tarefa ou problema tornam-se a mesma.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * O Proprietário do projeto é notificado em uma notificação no aplicativo do Workfront de que você sugeriu uma nova Data de confirmação para a tarefa ou problema.
   * O Proprietário do Projeto é notificado na seção Atualizações de que você sugeriu uma nova Data de Compromisso e, nesse momento, ele pode atualizar a Data de conclusão planejada da tarefa ou problema para corresponder à Data de Compromisso sugerida.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Para obter informações sobre as notificações e atualizações acionadas por essa alteração, consulte a seção &quot;Notificações e atualizações acionadas pela alteração da Data de confirmação&quot; no artigo [Visão geral da data de compromisso](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->