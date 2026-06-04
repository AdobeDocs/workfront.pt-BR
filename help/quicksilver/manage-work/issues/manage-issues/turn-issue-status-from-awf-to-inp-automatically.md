---
product-area: projects
navigation-topic: manage-issues
title: Atualizar automaticamente os status de problemas de Aguardando feedback para Em andamento
description: Quando o contato principal de um problema faz uma atualização do problema atualizando um campo (incluindo um campo personalizado) ou adicionando um comentário, o status do problema é atualizado para Em andamento automaticamente.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
TQID: https://experienceleague.adobe.com/axgDUT8M6p79omHTSO8OrvM7qAM81AjG0Fug2JUl4ck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 3%

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
