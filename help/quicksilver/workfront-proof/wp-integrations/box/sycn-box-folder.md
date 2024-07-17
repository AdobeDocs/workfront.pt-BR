---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Sincronizar Pastas De Caixa Com  [!DNL Workfront Proof]
description: É possível sincronizar uma pasta do Box com uma pasta no Workfront Proof. Cada alteração feita em seus arquivos na pasta Box será refletida no Workfront Proof (como fazer upload de um novo arquivo, adicionar uma nova versão, renomear um arquivo etc.).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Sincronizar [!DNL Box] Pastas Com [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Você pode sincronizar uma pasta do [!DNL Box] com uma pasta no [!DNL Workfront Proof]. Cada alteração feita em seus arquivos na pasta Box será refletida no Workfront Proof (como fazer upload de um novo arquivo, adicionar uma nova versão, renomear um arquivo etc.).

Para obter mais informações sobre pastas, consulte [Gerenciar Pastas e seus Conteúdos em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Somente usuários com perfis de [!UICONTROL Gerentes] ou superior podem sincronizar pastas. O usuário [!DNL Box] que carregar o arquivo para uma pasta sincronizada com [!DNL Workfront Proof] será o proprietário da prova criada em [!DNL Workfront Proof] (se for um usuário dentro da mesma conta [!DNL Workfront Proof]). Se o usuário [!DNL Box] for um usuário em uma conta diferente do [!DNL Workfront Proof] ou não tiver uma conta com [!DNL Workfront Proof], a pessoa que criou a sincronização entre as pastas se tornará o proprietário da prova. Para obter mais informações, consulte *&quot;Editando Perfis de Usuário e Permissões.&quot;*

Para sincronizar uma pasta [!DNL Box] com uma pasta em [!DNL Workfront Proof]:

1. Na sua conta do [!DNL Box], vá para a página [!UICONTROL Todos os Arquivos e Pastas].
1. Clique no menu **[!UICONTROL Mais opções]** ao lado da pasta com a qual você deseja sincronizar [!DNL Workfront Proof] (1).
1. Selecione **[!UICONTROL Mais Ações]** (2).
1. Clique em **[!UICONTROL Sincronizar com[!DNL Workfront Proof]]** (3).
1. Na caixa [!UICONTROL Sincronizar pasta] exibida (se você estiver conectado ao [!DNL Workfront Proof]), siga um destes procedimentos:

   * Clique em um nome de pasta [!DNL Workfront Proof] para sincronizá-lo com a pasta correspondente na Caixa (4).
   * Clique em **[!UICONTROL Nova pasta]** para criar uma nova pasta em [!DNL Workfront Proof] (5).\

     ![folder_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Se você optar por criar uma nova pasta, será solicitado a fornecer detalhes sobre ela.

1. Clique em **[!UICONTROL Salvar]**.\
   A página [!UICONTROL Detalhes da pasta] da pasta sincronizada é aberta em [!DNL Workfront Proof]. Esta página contém informações sobre a pasta.\
   Esta página também permite pausar e desativar a sincronização. Se você pausar a sincronização, a pasta não será mais atualizada com as alterações de [!DNL Box], mas a sincronização poderá ser retomada a qualquer momento. Desabilitar a sincronização significa que a conexão entre as pastas foi interrompida e a sincronização precisaria ser restabelecida a partir da conta [!DNL Box].\
   A página [!UICONTROL Detalhes da pasta] contém as seguintes informações e funções em relação à sua pasta no [!DNL Box]:

   * **[!UICONTROL Pausar sincronização]**: a pasta [!DNL Workfront Proof] não será mais atualizada com as alterações do Box. A sincronização pode ser retomada a qualquer momento (1).
   * **[!UICONTROL Desabilitar sincronização de pastas]**: a conexão entre pastas foi perdida, e a sincronização terá que ser configurada novamente da conta [!DNL Box] (2).

   * Somente o usuário que iniciou a sincronização de pastas pode desabilitá-la ou pausá-la. Para obter mais informações, consulte [Gerenciar pastas e seus conteúdos em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Ir para [!DNL Box] pasta**: se você compartilhou a URL da pasta (nas opções de pasta [!DNL Box]), essa opção ficará disponível e o levará diretamente à pasta [!DNL Box] (3).
   * **[!UICONTROL Detalhes da sincronização de pastas]**: esta seção contém informações sobre a pasta [!DNL Box] (4).
   * Link da pasta **[!UICONTROL [!DNL Box]]**: URL para a pasta [!DNL Box] (5).
   * **[!UICONTROL Atividade]:** Mostra os logs de atividades da pasta [!DNL Workfront Proof], onde você pode verificar quem iniciou a sincronização de pastas (6).
   * ![detalhes_da_pasta_1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* Você também pode sincronizar a pasta [!DNL Box] no menu [!UICONTROL Opções de pasta].
>* Se você tiver sua própria página de logon com a marca [!DNL Workfront Proof], será direcionado para essa página em vez da página de logon padrão [!DNL Workfront Proof]. Consulte os artigos em [Marcas](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) se precisar de mais informações.
>* Se você tiver habilitado a funcionalidade [!UICONTROL Logon Único (SSO)] em sua conta [!DNL Workfront Proof], será direcionado para a página de logon com SSO e solicitará que você insira suas credenciais de logon com SSO, mas somente se estiver usando o mesmo endereço de email da conta [!DNL Box] e do [!DNL Workfront Proof]. Se precisar de mais informações, consulte [[!UICONTROL Logon Único] em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Se você não estiver usando o mesmo endereço de email para a conta [!DNL Box] e para a conta [!DNL Workfront Proof], você sempre será direcionado à página de logon padrão [!DNL Workfront Proof].
>


