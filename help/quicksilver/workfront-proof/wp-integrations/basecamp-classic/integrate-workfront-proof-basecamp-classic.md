---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integrar  [!DNL Workfront Proof]  ao Basecamp Classic
description: Se você usar o [!DNL Basecamp] para gerenciamento de projetos, poderá oferecer à sua equipe de projetos ferramentas de revisão e aprovação mais avançadas usando o [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Integrar [!DNL Workfront Proof] a [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se você usar o [!DNL Basecamp] para gerenciamento de projetos, poderá oferecer à sua equipe de projetos ferramentas de revisão e aprovação mais avançadas usando o [!DNL Workfront Proof].

## Compreendendo a Integração do [!DNL Basecamp] com o [!DNL Workfront]

A integração com [!DNL Basecamp] permite que os usuários exibam, revisem e aprovem provas tudo dentro de [!DNL Basecamp]. Os usuários podem enviar provas para sua conta do [!DNL Workfront Proof] e conectá-las ao seu projeto do [!DNL Basecamp]. Seus revisores podem fazer [Tomar uma decisão sobre uma prova no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp], usando a miniprova incorporada na mensagem do Carimbo de Base.

Quando integrado ao [!DNL Workfront Proof], o [!DNL Basecamp] permite que os usuários façam o seguinte com provas:

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

* Configurar [!DNL Basecamp] em [Configurações da conta:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) permite a integração do Carimbo de base para toda a organização.
* Para obter mais informações, consulte [Habilitando a [!DNL Basecamp] Integração com [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Configurar [!DNL Basecamp] em [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): permite que os criadores e proprietários de provas se conectem à sua conta pessoal [!DNL Basecamp] e autorizem o acesso de [!DNL Workfront Proof]. Para obter mais informações, consulte [Definindo Configurações Pessoais](#configuring-personal-settings).

Você pode integrar [!DNL Workfront] com [!DNL Basecamp] ou [!DNL Basecamp Classic]. Cada versão do [!DNL Basecamp] usa uma API diferente e, portanto, requer procedimentos de configuração diferentes.

Para obter informações sobre como configurar o [!DNL Basecamp Classic], consulte [Habilitar a [!DNL Basecamp] Integração com o [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) neste artigo.

Para obter informações sobre como configurar o [!DNL Basecamp], consulte [Integrar [!DNL Workfront Proof] com [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Habilitando a Integração do [!DNL Basecamp] com o [!DNL Workfront Proof]

Como um [Perfis de Permissões de Prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) ou [Perfis de Permissões de Prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), você pode configurar a integração do Carimbo de Base para toda a conta nas [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Ir para [Configurações da conta.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Abra a guia **[!UICONTROL Integrações]** (1).
1. Para habilitar a integração com o Carimbo de Base, clique em **[!UICONTROL Habilitar]** (2).
1. Verifique se [!DNL Basecamp Classic] é a versão com a qual você está integrando (3).
1. (Condicional) Se nenhuma URL [!DNL Basecamp] for exibida (4), clique em **[!UICONTROL Editar]** e insira a URL da sua conta [!DNL Basecamp] (sem o http://).
1. Clique em **[!UICONTROL Salvar]** (5).\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Opcional) Verifique a URL do [!DNL Basecamp] no navegador depois de fazer logon na conta do [!DNL Basecamp Classic] (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   Depois de integrar [!DNL Workfront Proof] com [!DNL Basecamp], seus usuários poderão definir suas configurações pessoais. Para obter informações sobre como definir configurações pessoais, consulte [Definindo Configurações Pessoais](#configuring-personal-settings).

   Se você não puder habilitar a integração do [!DNL Basecamp], a ID da conta do [!DNL Workfront Proof] pode não ser a mesma que a ID da conta usada no [!DNL Basecamp].

## Definição de configurações pessoais

Depois de configurar as [configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) para sua organização, cada autor que criar/enviar provas deve definir suas [configurações pessoais.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Concluir essas etapas é mais fácil se você tiver a sessão do [!DNL Basecamp] aberta em uma janela do navegador e a sessão do [!DNL Workfront Proof] aberta em outra janela.

* [Recuperando o Token de API  [!DNL Basecamp] ](#retrieving-your-basecamp-api-token)
* [Adicionar o token de API  [!DNL Basecamp]  às suas configurações pessoais](#adding-your-basecamp-api-token-to-your-personal-settings)

### Recuperando seu token de API [!DNL Basecamp]

Para concluir a integração em nível individual no [!DNL Workfront Proof], os usuários precisam de seus tokens de autenticação individuais para a API [!DNL Basecamp].

Para recuperar o token de API [!DNL Basecamp]:

1. Entre na sua conta [!DNL Basecamp].
1. Clique em **[!UICONTROL Minhas informações]** (1) no canto superior direito da tela.\
   A página [!UICONTROL Minhas Informações] é exibida.\
   ![Integração_do_Carimbo_Base_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. Na seção [!UICONTROL Tokens de autenticação], clique em **[!UICONTROL Mostrar seus tokens]** (2) para exibir seus tokens de autenticação pessoal.
1. Selecione o **[!UICONTROL Token para leitores de feed]** ou a **[!UICONTROL API Basecamp]** (3) e copie o token para a área de transferência.

1. Cole seu token de API [!DNL Basecamp] no [!UICONTROL Token para leitores de feed] ou na caixa [!UICONTROL API Basecamp].\
   ![Integração_do_Carimbo_Base_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Adicionar o token de API [!DNL Basecamp] às suas configurações pessoais

Para colar o token de API [!DNL Basecamp] nas [!DNL Workfront Proof] [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Vá para as [[!UICONTROL Integrações] - Configuração do Usuário](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) em suas [Configurações Pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1).\
   Um administrador precisa primeiro habilitar a integração com o [!DNL Basecamp Classic] para que você possa habilitar suas configurações pessoais. Para obter informações sobre como configurar a integração, consulte [Habilitar a [!DNL Basecamp] Integração com o [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) neste artigo.

1. Na caixa de token da API [!DNL Basecamp] (2), cole o token que você acabou de copiar da sua página [!DNL Basecamp] [!UICONTROL Minhas Informações] no campo (3).\
   Para obter informações sobre como copiar o token de API [!DNL Basecamp], consulte [Recuperando o  [!DNL Basecamp] Token de API](#retrieving-your-basecamp-api-token) neste artigo.

1. Clique em **[!UICONTROL Salvar]** (4).

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Suas [!DNL Workfront Proof] [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) agora estão integradas à sua conta do [!DNL Basecamp Classic].
