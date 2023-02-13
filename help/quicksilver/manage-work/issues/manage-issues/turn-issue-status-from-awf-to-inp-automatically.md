---
product-area: projects
navigation-topic: manage-issues
title: Atualizar automaticamente os status de problema de Aguardando Feedback para Em Andamento
description: Quando o Contato principal de um problema atualiza o problema atualizando um campo (incluindo um campo personalizado) ou adicionando um comentário, o status do problema é atualizado automaticamente para Em andamento.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Atualizar automaticamente os status de problema de Aguardando Feedback para Em Andamento

Quando o Contato principal de um problema atualiza o problema atualizando um campo (incluindo um campo personalizado) ou adicionando um comentário, o status do problema é atualizado automaticamente para Em andamento.

Para que essa alteração automática de status ocorra, é necessário o seguinte:

* O problema deve ser inserido por meio de uma fila de solicitações.

   Para obter informações sobre como criar filas de solicitações, consulte o [Criar e gerenciar filas de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) seção. Para obter informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Os Detalhes da fila na fila de solicitações devem ter estas configurações:
   * **Quando alguém faz uma solicitação, concede automaticamente** está definida como **Acesso ao Contribute**
   * **Alterar Status** está selecionada em Configurações avançadas

   ![Detalhes da fila fornecem acesso ao contribuinte e o status de alteração é selecionado.](assets/queuedetails-contributeaccess-changestatus.png)

   Para obter mais informações sobre Detalhes da fila, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* O problema deve estar em Aguardando status de Feedback.
* Deve haver um status Aguardando feedback (AWF) disponível para problemas no nível do sistema.

   Para obter mais informações sobre status no nível do sistema, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
