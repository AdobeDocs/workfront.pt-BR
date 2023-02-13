---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar datas de confirmação em tarefas e problemas
description: Você pode atualizar manualmente a Data de confirmação de uma tarefa ou um problema ao qual está atribuído. Para obter mais informações sobre Datas de confirmação no Adobe Workfront, consulte Visão geral da Data de confirmação .
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Atualizar datas de confirmação em tarefas e problemas

Você pode atualizar manualmente a Data de confirmação de uma tarefa ou um problema ao qual está atribuído. Para obter mais informações sobre datas de confirmação no Adobe Workfront, consulte [Visão geral da data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Requisitos de acesso

<!--drafted for P&P

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   For the current licenses:
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   For legacy licenses:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior para tarefas</p> 
   <p>Solicitação ou superior para problemas</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões na tarefa ou no problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar, você deve ser atribuído à tarefa ou ocorrência para a qual precisa atualizar a Data de confirmação.

## Atualizar datas de confirmação em tarefas e problemas

A atualização da Data da confirmação é idêntica para tarefas e problemas.

1. Vá para uma tarefa ou problema atribuído como **Proprietário da Tarefa**.

   Para obter mais informações sobre como descobrir quem é o Proprietário da Tarefa de um problema ou tarefa, consulte a seção [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) no artigo [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Clique em Trabalhar nele no cabeçalho da tarefa ou do problema

   Ou

   Clique em **Iniciar tarefa** ou **Problema inicial** se o botão Trabalhar nele tiver sido personalizado em seu ambiente para indicar que você está trabalhando no item de trabalho.

   Nesse momento, a Data da confirmação e a Data de conclusão planejada da tarefa ou emissão são as mesmas.

1. (Opcional) Se você clicou em Iniciar tarefa ou Iniciar problema, clique em **Desfazer** no canto inferior esquerdo da tela. A Data de confirmação é removida.

   Para obter informações sobre a substituição do botão Trabalho nele por um botão Iniciar, consulte  [Substitua o botão Trabalho nele por um botão Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

   >[!TIP]
   >
   >A opção de desfazer sua seleção para iniciar seu trabalho não está disponível ao clicar em **Trabalhe nele**.

1. Clique em **Atualizações** no painel esquerdo, em seguida, clique no botão **Iniciar uma nova atualização** >**Data de confirmação**

   Ou

   Clique em **Detalhes da tarefa** ou **Detalhes do problema** no painel esquerdo, em seguida, clique duas vezes **Data de confirmação** e selecione uma nova data no calendário, em seguida, clique em **Salvar alterações**.
   ![](assets/commit-date-calendar-picker-in-updates-stream-nwe-350x452.png)

   As seguintes coisas acontecem após fazer essa alteração: 

   * A Data de confirmação e a Data de conclusão planejada não são mais as mesmas.

      Em vez disso, a Data de confirmação e a Data de conclusão projetada da tarefa ou emissão se tornam iguais.

      ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * As alterações são salvas automaticamente ao selecionar uma nova data na área Atualizações .
   * O Proprietário do Projeto é notificado de que você sugeriu uma nova Data de Confirmação para a tarefa ou emissão e pode, no momento, atualizar a Data de Conclusão Planejada da tarefa ou emissão para corresponder à Data de Confirmação sugerida.

      ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)

      Para obter informações sobre as notificações e atualizações acionadas por essa alteração, consulte a seção [Notificações e atualizações acionadas pela alteração da Data de Confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md#notifica) no artigo [Visão geral da data de confirmação](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).
