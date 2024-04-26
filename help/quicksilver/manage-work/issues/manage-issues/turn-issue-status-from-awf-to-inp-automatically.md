---
product-area: projects
navigation-topic: manage-issues
title: Atualizar automaticamente os status de problemas de Aguardando feedback para Em andamento
description: Quando o contato principal de um problema faz uma atualização do problema atualizando um campo (incluindo um campo personalizado) ou adicionando um comentário, o status do problema é atualizado para Em andamento automaticamente.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Atualizar automaticamente os status de problemas de Aguardando feedback para Em andamento

Quando o contato principal de um problema faz uma atualização do problema atualizando um campo (incluindo um campo personalizado) ou adicionando um comentário, o status do problema é atualizado para Em andamento automaticamente.

Para que essa alteração automática de status ocorra, é necessário:

* O problema deve ser inserido por meio de uma fila de solicitações.

  Para obter informações sobre a criação de filas de solicitações, consulte [Criar e gerenciar filas de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) seção. Para obter informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Os Detalhes da fila na fila de solicitações devem ter estas configurações:
   * **Quando alguém fizer uma solicitação, conceder automaticamente** está definida como **Acesso ao Contribute**
   * **Alterar Status** está selecionado em Configurações avançadas

  ![Detalhes da fila dão acesso ao Contribute e Alterar status é selecionado.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Ao configurar uma fila de solicitações, você pode definir o acesso que os contatos principais têm aos problemas enviados.
  >
  >Ao desmarcar a configuração Alterar status ao configurar a fila de solicitações, lembre-se de que os administradores do sistema sempre têm acesso para alterar o status de problemas, mesmo que a opção Alterar status esteja desmarcada nas configurações da fila de solicitações.

  Para obter mais informações sobre Detalhes da Fila, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* O problema deve estar no status Aguardando feedback.
* Deve haver um status Aguardando feedback (AWF) disponível para problemas no nível do sistema.

  Para obter mais informações sobre os status no nível do sistema, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
