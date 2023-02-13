---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Sincronizar pastas de caixa com [!DNL Workfront Proof]
description: Você pode sincronizar uma pasta de Caixa com uma pasta na Workfront Proof. Todas as alterações feitas nos arquivos na pasta Caixa serão refletidas na Workfront Proof (portanto, upload de um novo arquivo, adição de uma nova versão, renomeação de um arquivo, etc.).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Sincronizar [!DNL Box] Pastas com [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Você pode sincronizar um [!DNL Box] com uma pasta em [!DNL Workfront Proof]. Todas as alterações feitas nos arquivos na pasta Caixa serão refletidas na Workfront Proof (portanto, upload de um novo arquivo, adição de uma nova versão, renomeação de um arquivo, etc.).

Para obter mais informações sobre pastas, consulte [Gerenciar pastas e seu conteúdo em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Somente usuários com perfis de [!UICONTROL Gerentes] ou superior podem sincronizar pastas. O [!DNL Box] usuário que faz upload do arquivo para uma pasta sincronizada com [!DNL Workfront Proof], será o proprietário da prova criada em [!DNL Workfront Proof] (se forem um usuário dentro do mesmo [!DNL Workfront Proof] conta). Se a variável [!DNL Box] usuário é um usuário em um [!DNL Workfront Proof] conta ou não tem uma conta com [!DNL Workfront Proof], a pessoa que criou a sincronização entre as pastas se tornará a proprietária da prova. Para obter mais informações, consulte *&quot;Editando perfis de usuário e permissões.&quot;*

Para sincronizar um [!DNL Box] com uma pasta em [!DNL Workfront Proof]:

1. Em seu [!DNL Box] , vá para a [!UICONTROL Todos os arquivos e pastas] página.
1. Clique no botão **[!UICONTROL Mais opções]** ao lado da pasta com a qual deseja sincronizar [!DNL Workfront Proof] (1)
1. Selecionar **[!UICONTROL Mais ações]** (2)
1. Clique em **[!UICONTROL Sincronizar com[!DNL Workfront Proof]]** (3)
1. No [!UICONTROL Pasta de sincronização] que é exibida (se você estiver conectado [!DNL Workfront Proof]), execute um dos seguintes procedimentos:

   * Clique em um [!DNL Workfront Proof] nome da pasta para sincronizá-la com a pasta correspondente na caixa 4.
   * Clique em **[!UICONTROL Nova pasta]** para criar uma nova pasta em [!DNL Workfront Proof] (5).\

      ![folder_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Se você optar por criar uma nova pasta, será solicitado a fornecer detalhes sobre ela.

1. Clique em **[!UICONTROL Salvar]**.\
   O [!UICONTROL Detalhes da pasta] a página para a pasta sincronizada é aberta em [!DNL Workfront Proof]. Esta página contém informações sobre a pasta.\
   Esta página também permite pausar e desativar a sincronização. Se você pausar a sincronização, a pasta não será mais atualizada com as alterações de [!DNL Box], mas a sincronização pode ser retomada a qualquer momento. Desativar a sincronização significa que a conexão entre as pastas está quebrada e a sincronização precisaria ser restabelecida a partir do [!DNL Box] conta.\
   O [!UICONTROL Detalhes da pasta] contém as seguintes informações e funções em relação à sua pasta em [!DNL Box]:

   * **[!UICONTROL Pausar sincronização]**: O [!DNL Workfront Proof] não será mais atualizada com as alterações da caixa. A sincronização pode ser retomada a qualquer momento (1).
   * **[!UICONTROL Desativar sincronização de pastas]**: A conexão entre pastas é perdida, e a sincronização terá que ser configurada novamente a partir do [!DNL Box] conta (2).

   * Somente o usuário que iniciou a sincronização de pastas pode desabilitá-la ou pausá-la. Para obter mais informações, consulte  [Gerenciar pastas e seu conteúdo em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Ir para [!DNL Box] pasta**: Se você compartilhou o URL da pasta (no [!DNL Box] opções de pasta), essa opção ficará disponível e o levará diretamente para a [!DNL Box] pasta (3).
   * **[!UICONTROL Detalhes de sincronização de pastas]**: Esta seção contém informações sobre o [!DNL Box] pasta (4).
   * **[!UICONTROL [!DNL Box]link da pasta]**: URL para a [!DNL Box] pasta (5).
   * **[!UICONTROL Atividade]:** Mostra os logs de atividades do [!DNL Workfront Proof] , aqui você pode verificar quem iniciou a sincronização de pastas (6).
   * ![folder_details_1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* Você também pode sincronizar o [!DNL Box] da pasta de [!UICONTROL Opções de pasta] menu.
>* Se você tiver sua própria marca [!DNL Workfront Proof] fazer logon na página, você será direcionado para essa página em vez do padrão [!DNL Workfront Proof] página de logon. Veja os artigos em [Marca](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) se precisar de mais informações.
>* Se você ativou a variável [!UICONTROL Logon único (SSO)] em sua [!DNL Workfront Proof] , você será levado à página de logon SSO e solicitado a inserir suas credenciais de logon SSO, mas somente se estiver usando o mesmo endereço de email para sua [!DNL Box] e [!DNL Workfront Proof]. Se precisar de mais informações, consulte [[!UICONTROL Logon único] em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Se você não estiver usando o mesmo endereço de email para [!DNL Box] e sua [!DNL Workfront Proof] você sempre será levado para o padrão [!DNL Workfront Proof] página de logon.
>



