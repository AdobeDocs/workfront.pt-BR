---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Mover usuários entre contas usando  [!DNL Workfront Proof]
description: Se você for um  [!DNL Workfront Proof] administrador e tiver uma ou mais contas satélite conectadas à sua conta principal, poderá mover os usuários entre todas essas contas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Mover usuários entre contas usando [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se você for um administrador de Prova [!DNL Workfront] e tiver uma ou mais contas satélite conectadas à sua conta principal, poderá mover os usuários entre todas essas contas.

## Movendo usuários entre contas conectadas

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações de conta]**.

1. Abra a guia **[!UICONTROL Usuários]**.
1. Clique no ícone (1) **[!UICONTROL Mover usuário]**. ![Move_user2.png](assets/move-user2-350x95.png)

1. Na caixa Mover usuário exibida, confirme o usuário que deseja mover (1).
1. Selecione uma conta de destino na lista de contas conectadas (2).
1. Atribua a permissão de perfil (3) que este usuário deve ter na nova conta.
1. Selecione um usuário (4) que deve assumir a propriedade dos itens que não serão movidos.
Isso inclui os itens que você decidirá deixar na conta antiga e os itens que não podem ser movidos (consulte [Itens que não podem ser movidos](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) abaixo).

1. Marque as caixas de seleção se desejar mover as provas (5) e os arquivos (6) junto com o usuário.
1. Crie um nome para a pasta (7) na qual todos os itens movidos serão colocados na nova conta.
1. Clique em **[!UICONTROL Mover usuário]** (8) para iniciar o processo.
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

Se você optar por mover o usuário sem suas provas e arquivos, essa ação será executada imediatamente. Se você optar por mover o usuário junto com suas provas e arquivos, o perfil do usuário será reatribuído imediatamente, mas as provas e os arquivos aparecerão gradualmente na conta de destino, pois essa operação requer tempo para transferir os dados.

Dependendo do número de arquivos e do processo de movimentação de provas, pode levar de alguns minutos a algumas horas.

>[!NOTE]
>
>Se você suspeitar que o processo demora mais do que o esperado ou que as provas e/ou os arquivos movidos não aparecem na nova conta, entre em contato com nossa equipe de suporte.

## Itens que não podem ser movidos

### Pastas criadas ou pertencentes ao usuário movido

Devido à natureza de várias permissões aplicadas a pastas e seu conteúdo (por exemplo, elas podem ser compartilhadas com outros usuários e contas), não é possível mover as estruturas de pastas com o usuário.

Se uma pasta pertencer ao usuário movido, a propriedade será transferida para o usuário selecionado (4) na janela pop-up &quot;Mover usuário&quot;.

>[!NOTE]
>
>Se uma pasta tiver sido criada pelo usuário movido, ele permanecerá seu criador, somente a propriedade será transferida. A pasta permanecerá visível para o usuário movido na barra lateral da nova conta. O usuário movido ainda terá acesso &quot;Somente leitura&quot; aos itens colocados nessas pastas.

Se você não quiser que o usuário movido mantenha essas permissões ou se o usuário movido não quiser ver suas pastas antigas na conta &amp; antiga, a solução aqui seria excluir as pastas da seguinte maneira:

1. Crie uma nova pasta na conta antiga.
1. Mova todos os itens das pastas do usuário movido para a pasta recém-criada.
1. Excluir todas as pastas deixadas pelo usuário movido.

### Conjuntos de versões com proprietários diferentes

Se uma prova tiver algumas versões e cada uma delas for de propriedade de um usuário diferente, as versões de propriedade do usuário movido não serão movidas. A propriedade dessas versões será transferida para outro usuário de acordo com sua escolha (4) na caixa Mover usuário. (Para obter mais informações, consulte .)

>[!NOTE]
>
>Um usuário movido precisa ser o proprietário de todas as versões de prova no conjunto para que a prova seja movida.

### Grupos

Os grupos precisarão ser recriados pelo usuário movido em sua nova conta. Para obter mais informações, consulte [Criar grupos de revisão usando [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### Exibições personalizadas

As Exibições personalizadas pessoais precisarão ser recriadas pelo usuário movido em sua nova conta. Para obter mais informações, consulte [Criar e gerenciar exibições personalizadas [!DNL Workfront Proof] Prova](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Campos personalizados

Os campos personalizados não podem ser movidos e os dados de campos personalizados serão perdidos, portanto, gere os relatórios dos itens necessários antes da movimentação.

### Modelos de fluxo de trabalho automatizados

Os Modelos de fluxo de trabalho automatizados precisam ser recriados na nova conta, mas os estágios serão retidos nas provas movidas criadas com os modelos.

### Ações em comentários

As ações em Comentários permanecerão nas provas, mas não será possível filtrar mais por elas. A solução seria criar Ações correspondentes na nova conta e sinalizar novamente os comentários com as novas ações, se necessário.
