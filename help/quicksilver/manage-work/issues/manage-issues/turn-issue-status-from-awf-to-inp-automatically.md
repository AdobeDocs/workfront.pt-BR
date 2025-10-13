---
product-area: projects
navigation-topic: manage-issues
title: Atualizar automaticamente os status de problemas de Aguardando feedback para Em andamento
description: Quando o contato principal de um problema faz uma atualização do problema atualizando um campo (incluindo um campo personalizado) ou adicionando um comentário, o status do problema é atualizado para Em andamento automaticamente.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Atualizar automaticamente os status de problemas de Aguardando feedback para Em andamento

<!--Audited: 109/2025-->

Quando o contato principal de um problema faz uma atualização do problema atualizando um campo (incluindo um campo personalizado) ou adicionando um comentário, o status do problema é atualizado para Em andamento automaticamente.

Para que essa alteração automática de status ocorra, é necessário:

* O problema deve ser adicionado usando uma fila de solicitações.

  Para obter informações sobre como criar filas de solicitações, consulte a seção [Criar e gerenciar Filas de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md).

  Para obter informações sobre o envio de solicitações para uma fila de solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Os Detalhes da fila na fila de solicitações devem ter estas configurações:
   * **Quando alguém faz uma solicitação, conceder automaticamente** está definido como **Acesso ao Contribute**
   * **Alterar Status** está selecionado

  ![Os Detalhes da Fila dão acesso ao Contribute e Alterar Status está selecionado.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Ao configurar uma fila de solicitações, você pode definir o acesso que os contatos principais têm aos problemas enviados.
  >
  >Ao desmarcar a configuração Alterar status ao configurar a fila de solicitações, lembre-se de que os administradores do sistema sempre têm acesso para alterar o status de problemas, mesmo que a opção Alterar status esteja desmarcada nas configurações da fila de solicitações.

  Para obter mais informações sobre Detalhes da Fila, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* O problema deve estar no status Aguardando feedback.
* Deve haver um status Aguardando feedback (AWF) disponível para problemas no nível do sistema.

  Para obter mais informações sobre status de nível de sistema, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
