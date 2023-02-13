---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrar [!DNL Workfront Proof] com [!DNL Basecamp]
description: Se você usar [!DNL Basecamp] para o gerenciamento de projetos, você pode oferecer à equipe de projeto ferramentas de revisão e aprovação mais avançadas usando [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 0%

---

# Integrar [!DNL Workfront Proof] com [!DNL Basecamp]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Se você usar [!DNL Basecamp] para o gerenciamento de projetos, você pode oferecer à equipe de projeto ferramentas de revisão e aprovação mais avançadas usando [!DNL Workfront Proof].

## Noções básicas sobre o [!DNL Basecamp] Integração com [!DNL Workfront]

Integração com [!DNL Basecamp] permite que os usuários visualizem, revisem e aprovem provas em [!DNL Basecamp]. Os usuários podem enviar provas para seu [!DNL Workfront Proof] e conecte-os com sua [!DNL Basecamp] projeto. Seus revisores podem comentar e tomar decisões por meio de [!DNL Basecamp], usando a mini prova incorporada na mensagem do Basecamp.

Quando integrado ao [!DNL Workfront Proof], [!DNL Basecamp] O tem a seguinte funcionalidade de prova:

* Os usuários podem revisar e aprovar provas em [!DNL Basecamp Classic].
* Os usuários têm ferramentas de revisão prontamente disponíveis.
* As equipes de revisão do projeto recebem uma mensagem em [!DNL Basecamp] com uma prova mínima para revisão e aprovação.
* Os usuários podem alternar para uma prova de página inteira para revisão e aprovação.
* Os usuários podem adicionar comentários e marcações a provas em mini e tamanho completo.

   >[!NOTE]
   >
   >Depois que um comentário é respondido, ele não pode ser editado ou excluído.

* Os revisores podem responder às marcações e feitas por outros revisores.
* Os usuários são avisados quando uma nova versão da prova está disponível.
* Usuários que não são [!DNL Workfront Proof] os usuários podem trabalhar em uma prova em [!DNL Basecamp].

A integração de [!DNL Workfront Proof] com [!DNL Basecamp] deve ser configurado em dois níveis:

* Configurar [!DNL Basecamp] em [Configurações da conta:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Isso permite a integração do Basecamp para toda a organização. Para obter mais informações, consulte [Ativar a integração do Basecamp com [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Configurar [!DNL Basecamp] em [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Isso permite que criadores e proprietários de prova se conectem à sua conta pessoal do Basecamp e autorizem [!DNL Workfront Proof] acesso. Para obter mais informações, consulte [Definição das Configurações Pessoais](#configuring-personal-settings).

É possível integrar [!DNL Workfront] com [!DNL Basecamp] ou [!DNL Basecamp Classic]. Cada versão de [!DNL Basecamp] O usa uma API diferente e, portanto, requer procedimentos de configuração diferentes.

Para obter informações sobre como configurar [!DNL Basecamp Classic], consulte [Integração [!DNL Workfront Proof] com [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Ativar o [!DNL Basecamp] Integração com [!DNL Workfront Proof]

Como um [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) ou [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), você pode configurar o [!DNL Basecamp] integração de toda a conta em seu [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Em [!UICONTROL Basecamp], colete as seguintes informações:

   * O URL do seu [!DNL Basecamp] account
   * O URL encontrado no &quot;[!UICONTROL Minhas informações]Seção &quot;

1. Fazer logoff de [!DNL Basecamp].
1. Clique em **[!UICONTROL Configurações da conta]** próximo ao canto superior direito.
1. Clique no botão **[!UICONTROL Integrações]** guia .
1. No **[!UICONTROL [!DNL Basecamp]]** à direita de **[!UICONTROL [!DNL Basecamp]integração]**, clique em **[!UICONTROL Habilitar]**.

1. Próximo a **[!UICONTROL [!DNL Basecamp]version]**, verifique o **[!UICONTROL Versão clássica]** é a versão com a qual você está integrando.

1. (Condicional) Se não [!DNL Basecamp] URL é exibido, clique em **[!UICONTROL Editar]**, digite o URL do [!DNL Basecamp] sem incluir &quot;http://&quot; e, em seguida, clique em **[!UICONTROL Salvar]**.

1. No canto superior direito da janela, clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações pessoais]**.

1. Clique no botão **[!UICONTROL Integrações]** guia .
1. Em **[!DNL Basecamp]**, ao direito de **[!UICONTROL Integração com o Basecamp]**, clique em **[!UICONTROL Habilitar]**.

1. Nas opções exibidas, à direita de **[!UICONTROL [!DNL Basecamp]Token de API]**, clique em **[!UICONTROL Editar]**.

1. Na caixa exibida, digite o URL encontrado no &quot;[!UICONTROL Minhas informações]&quot; na seção [!DNL Basecamp], depois clique em **[!UICONTROL Salvar]**.\
   Depois de integrar [!DNL Workfront Proof] com [!DNL Basecamp], seus usuários podem definir suas configurações pessoais. Para obter informações sobre como configurar configurações pessoais, consulte [Definição das Configurações Pessoais](#configuring-personal-settings)

1. Se não for possível ativar [!DNL Basecamp] integração, seu [!DNL Workfront Proof] a ID da conta pode não ser a mesma que a ID da conta usada em [!DNL Basecamp].
1. Depois de integrar [!DNL Workfront Proof] com [!DNL Basecamp], seus usuários podem definir suas configurações pessoais. Para obter informações sobre como configurar configurações pessoais, consulte [Definição das Configurações Pessoais](#configuring-personal-settings).

## Definição das Configurações Pessoais

Depois de configurar [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) para sua organização, cada um dos autores que criar/enviar provas deve definir seus  [configurações pessoais.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Ir para **[!UICONTROL Configurações pessoais** &#x200B;**]**.

1. Abra o **[!UICONTROL Integrações]** (1).
1. Para ativar o [!DNL Basecamp] integração, clique em **[!UICONTROL Habilitar]** (2)
1. Clique em **[!UICONTROL Conecte-se ao seu [!DNL Basecamp] account]** (3)\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Faça logon no [!DNL Basecamp] conta (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Clique em **[!UICONTROL Sim, vou permitir acesso]** autorizar [!DNL Workfront Proof] acesso à sua conta (2).\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Opcional) Quando sua integração pessoal estiver ativa (3), você poderá alternar facilmente entre as [!DNL Basecamp] contas.

   1. Clicar **[!UICONTROL Switch [!DNL Basecamp] account]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      O [!UICONTROL Alterar Conta do Basecamp] leva você ao [!UICONTROL Configurações pessoais] , onde você pode escolher qual das suas [!DNL Basecamp] contas que você deseja integrar com seu [!DNL Workfront Proof] conta.

   1. Clique em **[!UICONTROL Reintegrar com[!DNL Basecamp]]** (5) antes de escolher a variável [!DNL Basecamp] conta\

      Essa ação atualiza o [!UICONTROL Configurações pessoais] e mostra sua lista mais atualizada de [!DNL Basecamp] contas.

   1. Clique em **[!UICONTROL Integrar a esta conta]** para conectá-lo a [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Agora é possível adicionar provas a [!DNL Basecamp] projetos.
