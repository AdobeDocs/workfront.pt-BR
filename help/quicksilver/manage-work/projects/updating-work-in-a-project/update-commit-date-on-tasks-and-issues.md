---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar datas de confirmação nas tarefas e problemas
description: Você pode atualizar manualmente a data de confirmação de uma tarefa ou problema atribuído a você. Para obter mais informações sobre Datas de confirmação no Adobe Workfront, consulte Visão geral da Data de confirmação.
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Atualizar datas de confirmação nas tarefas e problemas

Você pode atualizar manualmente a data de confirmação de uma tarefa ou problema atribuído a você. Para obter mais informações sobre Datas de confirmação no Adobe Workfront, consulte [Visão geral da data de compromisso](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisitos de acesso

<!--Audited: 01/2024-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
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

Antes de começar, você deve estar atribuído à tarefa ou problema para o qual precisa atualizar a Data de confirmação.

## Atualizar datas de confirmação nas tarefas e problemas

A atualização da Data de confirmação é idêntica para tarefas e problemas.

1. Ir para uma tarefa ou problema atribuído como **Proprietário**.

   Para obter mais informações sobre descobrir quem é o Proprietário da Tarefa para um problema ou tarefa, consulte a seção [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) no artigo [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Clique em **Detalhes da tarefa** ou **Detalhes do problema** no painel esquerdo.
1. Clique em **Visão geral** para expandi-la.
1. Atualize o **Data de confirmação** campo.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Clique em **Salvar alterações**.

   Ocorre o seguinte após fazer essa alteração: 

   * A Data de confirmação e a Data de conclusão planejada da tarefa ou problema não são mais a mesma.

     Em vez disso, a Data de confirmação e a Data de conclusão projetada da tarefa ou problema tornam-se a mesma.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Se você estiver usando a área Atualizações herdadas, o Proprietário do projeto será notificado de que você sugeriu uma nova Data de confirmação para a tarefa ou problema e poderá, nesse momento, atualizar a Data de conclusão planejada da tarefa ou problema para que corresponda à Data de confirmação sugerida. Esta funcionalidade não é suportada na nova experiência de comentários. Para obter informações, consulte [A nova experiência de comentários](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

     Para obter informações sobre as notificações e atualizações acionadas por essa alteração, consulte a seção [Notificações e atualizações acionadas pela alteração da Data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) no artigo [Visão geral da data de compromisso](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
