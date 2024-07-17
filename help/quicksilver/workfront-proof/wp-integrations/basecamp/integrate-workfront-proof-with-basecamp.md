---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrar [!DNL Workfront Proof] com [!DNL Basecamp]
description: Se você usar o [!DNL Basecamp] para gerenciamento de projetos, poderá oferecer à sua equipe de projetos ferramentas de revisão e aprovação mais avançadas usando o [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Integrar [!DNL Workfront Proof] a [!DNL Basecamp]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se você usar o [!DNL Basecamp] para gerenciamento de projetos, poderá oferecer à sua equipe de projetos ferramentas de revisão e aprovação mais avançadas usando o [!DNL Workfront Proof].

## Compreendendo a Integração do [!DNL Basecamp] com o [!DNL Workfront]

A integração com [!DNL Basecamp] permite que os usuários exibam, revisem e aprovem provas tudo dentro de [!DNL Basecamp]. Os usuários podem enviar provas para sua conta do [!DNL Workfront Proof] e conectá-las ao seu projeto do [!DNL Basecamp]. Os revisores podem comentar e tomar decisões por meio do [!DNL Basecamp], usando a miniprova incorporada na mensagem do Carimbo de Base.

Quando integrado a [!DNL Workfront Proof], [!DNL Basecamp] tem a seguinte funcionalidade de prova:

* Os usuários podem revisar e aprovar provas em [!DNL Basecamp Classic].
* Os usuários têm ferramentas de análise prontamente disponíveis.
* As equipes de revisão de projetos recebem uma mensagem em [!DNL Basecamp] com uma minitorprova para revisão e aprovação.
* Os usuários podem alternar para uma prova de página inteira para revisão e aprovação.
* Os usuários podem adicionar comentários e marcações a provas de tamanho menor e maior.

  >[!NOTE]
  >
  >Depois que um comentário é respondido, ele não pode ser editado ou excluído.

* Os revisores podem responder às marcações e feitas por outros revisores.
* Os usuários são alertados quando uma nova versão da prova está disponível.
* Os usuários que não são [!DNL Workfront Proof] podem trabalhar em uma prova no [!DNL Basecamp].

A integração do [!DNL Workfront Proof] com o [!DNL Basecamp] deve ser configurada em dois níveis:

* Configurar [!DNL Basecamp] em [Configurações da conta:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) permite a integração do Carimbo de base para toda a organização. Para obter mais informações, consulte [Habilitando a Integração do Carimbo de Base com [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Configurar [!DNL Basecamp] em [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): permite que os criadores e proprietários de provas se conectem à sua conta pessoal do Carimbo de Base e autorizem o acesso de [!DNL Workfront Proof]. Para obter mais informações, consulte [Definindo Configurações Pessoais](#configuring-personal-settings).

Você pode integrar [!DNL Workfront] com [!DNL Basecamp] ou [!DNL Basecamp Classic]. Cada versão do [!DNL Basecamp] usa uma API diferente e, portanto, requer procedimentos de configuração diferentes.

Para obter informações sobre como configurar o [!DNL Basecamp Classic], consulte [Integração [!DNL Workfront Proof] com [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Habilitando a Integração do [!DNL Basecamp] com o [!DNL Workfront Proof]

Como um [Perfis de Permissões de Prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) ou [Perfis de Permissões de Prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), você pode configurar a integração do [!DNL Basecamp] para toda a conta nas [configurações da Conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Em [!UICONTROL Basecamp], colete as seguintes informações:

   * A URL da sua conta [!DNL Basecamp]
   * A URL encontrada na seção &quot;[!UICONTROL Minhas informações]&quot;

1. Faça logout de [!DNL Basecamp].
1. Clique em **[!UICONTROL Configurações da conta]** próximo ao canto superior direito.
1. Clique na guia **[!UICONTROL Integrações]**.
1. Na seção **[!UICONTROL [!DNL Basecamp]]**, à direita de **[!UICONTROL [!DNL Basecamp]integração]**, clique em **[!UICONTROL Habilitar]**.

1. Ao lado da **[!UICONTROL [!DNL Basecamp]versão]**, verifique se a **[!UICONTROL versão Clássica]** é a versão com a qual você está integrando.

1. (Condicional) Se nenhuma URL [!DNL Basecamp] for exibida, clique em **[!UICONTROL Editar]**, digite a URL da sua conta [!DNL Basecamp], sem incluir &quot;http://&quot;, e clique em **[!UICONTROL Salvar]**.

1. No canto superior direito da janela, clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações pessoais]**.

1. Clique na guia **[!UICONTROL Integrações]**.
1. Em **[!DNL Basecamp]**, à direita de **[!UICONTROL Integração com o mapa de base]**, clique em **[!UICONTROL Habilitar]**.

1. Nas opções exibidas, à direita de **[!UICONTROL [!DNL Basecamp]Token de API]**, clique em **[!UICONTROL Editar]**.

1. Na caixa exibida, digite a URL localizada na seção &quot;[!UICONTROL Minhas informações]&quot; em [!DNL Basecamp] e clique em **[!UICONTROL Salvar]**.\
   Depois de integrar [!DNL Workfront Proof] com [!DNL Basecamp], seus usuários poderão definir suas configurações pessoais. Para obter informações sobre como definir configurações pessoais, consulte [Definindo Configurações Pessoais](#configuring-personal-settings)

1. Se você não puder habilitar a integração do [!DNL Basecamp], a ID da conta do [!DNL Workfront Proof] pode não ser a mesma que a ID da conta usada no [!DNL Basecamp].
1. Depois de integrar [!DNL Workfront Proof] com [!DNL Basecamp], seus usuários poderão definir suas configurações pessoais. Para obter informações sobre como definir configurações pessoais, consulte [Definindo Configurações Pessoais](#configuring-personal-settings).

## Definição de configurações pessoais

Depois de definir as [configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) para sua Organização, cada um dos autores que criar/enviar provas deve definir suas [configurações pessoais.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Ir para **[!UICONTROL Configurações&#x200B;pessoais***]**.

1. Abra a guia **[!UICONTROL Integrações]** (1).
1. Para habilitar a integração do [!DNL Basecamp], clique em **[!UICONTROL Habilitar]** (2).
1. Clique em **[!UICONTROL Conectar-se à sua conta [!DNL Basecamp]]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Faça logon em sua conta do [!DNL Basecamp] (1).\
   ![Basecamp_login_page.png](assets/basecamp-login-page-350x107.png)

1. Clique em **[!UICONTROL Sim, concederei acesso]** para autorizar o acesso [!DNL Workfront Proof] à sua conta (2).\
   ![Basecamp_authorization_page.png](assets/basecamp-authorization-page-350x173.png)

1. (Opcional) Quando sua integração pessoal estiver ativa (3), você poderá alternar facilmente entre suas contas do [!DNL Basecamp].

   1. Clicando em **[!UICONTROL Alternar [!DNL Basecamp] conta]** (4).\

      ![Basecamp_switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      A [!UICONTROL Conta do Carimbo de Base do Comutador] direciona você à página [!UICONTROL Configurações Pessoais], na qual é possível escolher qual das [!DNL Basecamp] contas você deseja integrar à sua conta do [!DNL Workfront Proof].

   1. Clique em **[!UICONTROL Reintegrar com[!DNL Basecamp]]** (5) antes de escolher a conta [!DNL Basecamp]\

      Isso atualiza a página [!UICONTROL Configurações Pessoais] e mostra sua lista mais atualizada de contas do [!DNL Basecamp].

   1. Clique em **[!UICONTROL Integrar a esta conta]** para conectá-la a [!DNL Workfront Proof].\

      ![Basecamp_switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Agora você pode adicionar provas a [!DNL Basecamp] projetos.
