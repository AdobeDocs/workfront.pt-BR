---
product-area: projects
navigation-topic: approvals
title: Associar um processo de aprovação novo ou existente ao trabalho
description: Este artigo descreve como você pode associar processos de aprovação a itens de trabalho. Para obter informações sobre como associar aprovações a provas ou documentos, consulte os seguintes artigos.
author: Courtney and Alina
feature: Work Management
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 7dbb9ca9b26f17710a7897e98dca109b5c886bd7
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# Associar um processo de aprovação novo ou existente ao trabalho

Este artigo descreve como você pode associar processos de aprovação a itens de trabalho. Para obter informações sobre como associar aprovações a provas ou documentos, consulte os seguintes artigos:

* [Criar uma prova avançada com um fluxo de trabalho Automatizado](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Solicitar aprovações de documento](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

Você pode associar um processo de aprovação global ou de uso único a um item de trabalho no Adobe Workfront. Os seguintes cenários existem:

* Associe um processo de aprovação global existente a um projeto, tarefa, problema, modelo ou tarefa de modelo. Alguns processos de aprovação global estão disponíveis para todos os grupos no sistema. Os processos de aprovação global em nível de grupo estão disponíveis somente para determinados grupos.
* Crie um processo de aprovação de uso único e associe-o a um projeto, tarefa, problema, modelo ou tarefa de modelo existente.

>[!NOTE]
>
>Este artigo usa o termo &quot;processo de aprovação global&quot; para diferenciar do &quot;processo de aprovação de uso único&quot;. Um processo de aprovação global pode ser usado repetidamente.
>
>O termo &quot;processo de aprovação global a nível de grupo&quot; refere-se a um processo de aprovação que pode ser utilizado repetidamente em itens e com status associados apenas a um grupo específico.

Para obter informações mais gerais sobre processos de aprovação, consulte [Visão geral do processo de aprovação](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Para obter informações sobre como criar um processo de aprovação global, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar acesso ou superior a Projetos, Tarefas, Problemas ou Modelos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para o projeto, tarefa, problema ou modelo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre a associação de processos de aprovação a itens de trabalho

Além das considerações descritas abaixo, recomendamos que você revisite as considerações gerais sobre os processos de aprovação no Workfront. Para obter mais informações, consulte [Visão geral do processo de aprovação](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* Você deve criar o projeto, a tarefa, a emissão, o modelo ou a tarefa do modelo antes que o processo de aprovação possa ser associado a eles.
* Ao anexar um processo de aprovação a um item para um status que foi aprovado e no qual o item está no momento, o processo de aprovação não será acionado e nenhuma notificação será enviada aos aprovadores.

   **Exemplo:** Se uma tarefa estiver no status de Concluído e você anexar um processo de aprovação associado ao status Concluído, a aprovação não será acionada.

* Quando você anexa um processo de aprovação ao primeiro status de um item (usando um modelo para tarefas e projetos, usando as configurações de Configuração da fila para problemas ou definindo as Configurações da tarefa de um projeto para novas tarefas), os processos de aprovação são ignorados se a aprovação enviada for recuperada. Nesse caso, os aprovadores não recebem notificações.

   Para obter mais informações sobre como recuperar aprovações, consulte [Exibir aprovações](../../review-and-approve-work/manage-approvals/view-approvals.md).

   >[!TIP]
   >
   >O primeiro status para uma tarefa ou problema é New. O primeiro status de um projeto é o status selecionado pelo administrador do Workfront nas Preferências do projeto no sistema. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* A associação de processos de aprovação com um objeto não é registrada na área Atualizações do objeto.
* Não é possível associar um processo de aprovação a uma tarefa pai.
* Adicionar um usuário, equipe ou função como aprovador não concede automaticamente permissões ao objeto associado à aprovação. Eles recebem permissões do objeto quando a etapa de aprovação é acionada. Caso contrário, os objetos devem ser compartilhados com eles antes que possam tomar uma decisão de aprovação.

As seções a seguir descrevem os diferentes métodos de associação de um processo de aprovação a um projeto, tarefa ou problema.

## Associar um processo de aprovação global a um item de trabalho {#associate-a-global-approval-process-with-a-work-item}

Você pode associar um processo de aprovação global a um item de trabalho (projeto, tarefa, emissão, modelo, tarefa do modelo).

O processo de aprovação global deve estar disponível para o grupo associado ao item de trabalho ou para todos os grupos no sistema.

>[!NOTE]
Você pode anexar processos de aprovação de projeto a um modelo e processos de aprovação de tarefa a uma tarefa de modelo. Depois disso, quando alguém usa o modelo para criar um projeto, o processo de aprovação se torna um processo de aprovação de projeto ou tarefa, respectivamente. Um processo de aprovação de uso único anexado a uma tarefa de modelo ou modelo permanece um processo de aprovação de uso único para projetos e tarefas.

Para obter informações sobre como os administradores do Workfront podem configurar um processo de aprovação global para todos os grupos no sistema e como os administradores de grupo podem criar aprovações para um grupo, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
Você também pode modificar um processo de aprovação global para atender às suas necessidades específicas. Para obter mais informações, consulte a seção [Modificar um processo de aprovação global para uso em um objeto específico](#modify-a-global-approval-process-for-use-on-a-specific-object) neste artigo.

Para associar um processo de aprovação global existente a um projeto, tarefa, problema, modelo ou tarefa do modelo:

1. Vá para o item de trabalho ao qual deseja associar um processo de aprovação.
1. Clique em **Aprovações** no painel esquerdo.

   Talvez seja necessário clicar em **Mostrar mais**, depois clique em **Aprovações**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   O processo de aprovação selecionado é exibido.

1. Expanda o **Usar existentes** e selecione um processo de aprovação existente.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   O processo de aprovação selecionado é exibido.

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Clique em **Salvar**.
1. (Opcional) Clique em Editar Processo de Aprovação se desejar modificar a aprovação existente anexada ao item. Isso altera o processo de aprovação global para um processo de aprovação de uso único. Para obter mais informações, consulte a seção [Modificar um processo de aprovação global para uso em um objeto específico](#modify-a-global-approval-process-for-use-on-a-specific-object) neste artigo.

## Modificar um processo de aprovação global para uso em um objeto específico {#modify-a-global-approval-process-for-use-on-a-specific-object}

O administrador ou administrador de grupo da Workfront cria processos de aprovação global para você usar, conforme descrito em [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Modificar um processo de aprovação global anexado a um item é idêntico ao processo de aprovação de uso único.

Você pode modificar um processo de aprovação global para atender a quaisquer necessidades específicas do projeto, tarefa ou problema associado a ele.

>[!IMPORTANT]
Quando você modifica um processo de aprovação global, ele se torna um processo de aprovação de uso único que pode ser usado somente no objeto em que você o modificou. O processo de aprovação global permanece inalterado.
Considere as seguintes limitações ao modificar um processo de aprovação global:
* O processo de aprovação é modificado somente para o projeto, tarefa ou problema com o qual você está associando o processo de aprovação.
* Quaisquer alterações futuras feitas por um administrador ao processo de aprovação global original não refletirão no processo de aprovação global que você modificou.
>


Para modificar um processo de aprovação já anexado a um item:

1. Adicione um processo de aprovação global ao projeto, tarefa ou problema.

   Para obter instruções, consulte a seção [Associar um processo de aprovação global a um item de trabalho](#associate-a-global-approval-process-with-a-work-item) neste artigo.

   >[!IMPORTANT]
   Certifique-se de clicar em **Salvar** ao adicionar a aprovação.

1. Após adicionar o processo de aprovação global, clique no botão **Editar**&#x200B;ícone ![](assets/edit-icon.png) no canto superior direito da página de aprovação. Essa ação transforma o processo de aprovação global ou de nível de grupo em um processo de aprovação de uso único.
1. Faça alterações no processo de aprovação existente. Para obter mais informações, consulte a seção [Associar um processo de aprovação de uso único a um projeto, tarefa, problema, modelo ou tarefa de modelo](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) neste artigo.
1. Clique em **Salvar**, depois clique em **Salvar** novamente para confirmar que você deseja converter o processo de aprovação global em um processo de aprovação de uso único disponível somente neste objeto.

## Associar um processo de aprovação de uso único a um projeto, tarefa, problema, modelo ou tarefa de modelo {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

Você pode criar um processo de aprovação de uso único para uso somente em um projeto, tarefa ou problema específico.

Você também pode associar um processo de aprovação de uso único a uma tarefa de modelo ou modelo, de modo que ele esteja disponível em projetos e tarefas criados a partir do modelo.

>[!NOTE]
Você pode associar um processo de aprovação de uso único a qualquer status de nível de sistema ou de grupo para um projeto, tarefa, problema, modelo ou tarefa de modelo. Para obter informações sobre os status do Workfront, consulte [Criar ou editar um status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Criar um processo de aprovação dessa forma permite criar um processo de aprovação personalizado para atender às suas necessidades. No entanto, o processo de aprovação não pode ser associado a outros itens de trabalho no futuro.

Como alternativa, você pode modificar um processo de aprovação global de um item específico e que também se torna um processo de aprovação de uso único. Para obter mais informações, consulte a seção [Modificar um processo de aprovação global para uso em um objeto específico](#modify-a-global-approval-process-for-use-on-a-specific-object) neste artigo.

Para criar um processo de aprovação de uso único:

1. Vá para o projeto, tarefa, emissão, modelo ou tarefa do modelo onde deseja associar um processo de aprovação.
1. Clique em **Aprovações** no painel esquerdo.

   Talvez seja necessário clicar em **Mostrar mais** > **Aprovações**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Clique em **Criar uso único**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Complete as etapas a partir da etapa 6 da seção &quot;Criar um processo de aprovação global a nível de sistema ou de grupo para itens de trabalho&quot; no artigo [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   Depois de anexar o processo de aprovação de uso único, ele é exibido como &quot;`<Custom>`&quot; no campo Processo de aprovação dentro da caixa Editar de modelos e tarefas do modelo. Para obter informações sobre como editar modelos ou tarefas de modelo, consulte os seguintes artigos:
   * [Editar modelos de projeto](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   * [Editar uma tarefa de modelo](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)


   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Remover ou excluir um processo de aprovação de um item de trabalho

Você pode remover um processo de aprovação global ou de nível de grupo ou pode excluir um processo de aprovação de uso único de um projeto, tarefa ou problema anteriormente associado a ele.

Os seguintes cenários existem: 

* Remover o processo de aprovação global ou de nível de grupo não exclui a aprovação. A aprovação permanece disponível para uso futuro.
* A exclusão de um processo de aprovação de usuário único o exclui do Workfront e não pode ser recuperada.

Para remover ou excluir um processo de aprovação de um item de trabalho:

1. Vá para o projeto, tarefa, emissão, modelo ou tarefa do modelo em que deseja remover um processo de aprovação adicionado anteriormente.
1. Clique em **Aprovações** no painel esquerdo.

   Talvez seja necessário clicar em **Mostrar mais** > **Aprovações**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Clique em um dos ícones a seguir no canto superior direito da seção Aprovações , dependendo do tipo de aprovação associada ao item:

   * **A remoção**&#x200B;ícone ![](assets/remove-icon---x-in-circle.png) para aprovações globais ou de nível de grupo.
   * **A Exclusão**&#x200B;ícone ![](assets/delete.png) para aprovações de utilização única.

1. Clique em **Remover** ou **Excluir** para confirmar.

   O processo de aprovação é removido do item de trabalho.

## Associar automaticamente um processo de aprovação a itens de trabalho

Você pode associar um processo de aprovação automaticamente a itens de trabalho usando os seguintes workflows:

* Para projetos e tarefas, é possível associar um processo de aprovação usando um template. Você pode anexar um processo de aprovação existente à guia Aprovações de modelo ou à guia Aprovações de tarefa de modelo . Para obter informações sobre como associar uma aprovação existente a um item de trabalho, consulte [Associar um processo de aprovação global a um item de trabalho](#associate-a-global-approval-process-with-a-work-item) neste artigo.
* Para novas tarefas em um projeto existente, você pode associar um processo de aprovação global ou um processo de aprovação global em nível de grupo na área Configurações da tarefa da caixa Editar projeto . Para obter informações, consulte a seção &quot;Configurações da tarefa&quot; no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).
* Para problemas, é possível associar uma aprovação a cada novo problema adicionado a um projeto associando um processo de aprovação existente a uma fila de solicitações. Para obter informações sobre como configurar filas de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
