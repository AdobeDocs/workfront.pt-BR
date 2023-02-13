---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp-classic
title: Integrar [!DNL Workfront Proof] com o Basecamp Classic
description: Se você usar [!DNL Basecamp] para o gerenciamento de projetos, você pode oferecer à equipe de projeto ferramentas de revisão e aprovação mais avançadas usando [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: e1f03079-6ccc-4e81-a7f7-184e87d62654
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Integrar [!DNL Workfront Proof] com [!DNL Basecamp Classic]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Se você usar [!DNL Basecamp] para o gerenciamento de projetos, você pode oferecer à equipe de projeto ferramentas de revisão e aprovação mais avançadas usando [!DNL Workfront Proof].

## Noções básicas sobre o [!DNL Basecamp] Integração com [!DNL Workfront]

Integração com [!DNL Basecamp] permite que os usuários visualizem, revisem e aprovem provas em [!DNL Basecamp]. Os usuários podem enviar provas para seu [!DNL Workfront Proof] e conecte-os com sua [!DNL Basecamp] projeto. Seus revisores podem e podem [Tome uma decisão em uma prova no visualizador de prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) via [!DNL Basecamp], usando a mini prova incorporada na mensagem do Basecamp.

Quando integrado ao [!DNL Workfront Proof], [!DNL Basecamp] O permite que os usuários façam o seguinte com provas:

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

* Configurar [!DNL Basecamp] em [Configurações da conta:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Isso permite a integração do Basecamp para toda a organização.
* Para obter mais informações, consulte [Ativar o [!DNL Basecamp] Integração com [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).
* Configurar [!DNL Basecamp] em [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Isso permite que criadores e proprietários de provas se conectem a seus [!DNL Basecamp] e autorizar [!DNL Workfront Proof] acesso. Para obter mais informações, consulte [Definição das Configurações Pessoais](#configuring-personal-settings).

É possível integrar [!DNL Workfront] com [!DNL Basecamp] ou [!DNL Basecamp Classic]. Cada versão de [!DNL Basecamp] O usa uma API diferente e, portanto, requer procedimentos de configuração diferentes.

Para obter informações sobre como configurar [!DNL Basecamp Classic], consulte [Ativar o [!DNL Basecamp] Integração com [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) neste artigo.

Para obter informações sobre como configurar [!DNL Basecamp], consulte [Integrar [!DNL Workfront Proof] com [!DNL Basecamp]](../../../workfront-proof/wp-integrations/basecamp/integrate-workfront-proof-with-basecamp.md).

## Ativar o [!DNL Basecamp] Integração com [!DNL Workfront Proof]

Como um [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) ou [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), é possível configurar a integração do Basecamp para toda a conta no [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. Ir para [Configurações da conta.](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings)
1. Abra o **[!UICONTROL Integrações]** (1).
1. Para habilitar a integração do Basecamp, clique em **[!UICONTROL Habilitar]** (2)
1. Verifique se [!DNL Basecamp Classic] é a versão com a qual você está integrando (3).
1. (Condicional) Se não [!DNL Basecamp] O URL é exibido (4), clique em **[!UICONTROL Editar]** e insira o URL de seu [!DNL Basecamp] conta (sem o http://).
1. Clique em **[!UICONTROL Salvar]** 5.\
   ![Basecamp_account_settings_-_integration.png](assets/basecamp-account-settings---integration-350x192.png)

1. (Opcional) Verifique o [!DNL Basecamp] URL no seu navegador após fazer logon em seu [!DNL Basecamp Classic] conta (6).

   ![Basecamp_URL.png](assets/basecamp-url-350x75.png)

   Depois de integrar [!DNL Workfront Proof] com [!DNL Basecamp], seus usuários podem definir suas configurações pessoais. Para obter informações sobre como configurar configurações pessoais, consulte [Definição das Configurações Pessoais](#configuring-personal-settings).

   Se não for possível ativar [!DNL Basecamp] integração, seu [!DNL Workfront Proof] a ID da conta pode não ser a mesma que a ID da conta usada em [!DNL Basecamp].

## Definição das Configurações Pessoais

Depois de configurar [Configurações da conta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) para sua organização, cada um dos autores que cria/envia provas deve definir seus  [configurações pessoais.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

>[!NOTE]
>
>Concluir essas etapas é mais fácil se você tiver o [!DNL Basecamp] sessão aberta em uma janela do navegador e sua [!DNL Workfront Proof] sessão aberta em outra janela.

* [Recuperar seu [!DNL Basecamp] Token de API](#retrieving-your-basecamp-api-token)
* [Adicionar seu [!DNL Basecamp] Token de API para suas configurações pessoais](#adding-your-basecamp-api-token-to-your-personal-settings)

### Recuperar seu [!DNL Basecamp] Token de API

Para concluir a integração no nível individual em [!DNL Workfront Proof], os usuários precisam de seu token de autenticação individual para a [!DNL Basecamp] API.

Para recuperar o [!DNL Basecamp] Token da API:

1. Faça logon em seu [!DNL Basecamp] conta.
1. Clique em **[!UICONTROL Minhas informações]** (1) no canto superior direito da tela.\
   O [!UICONTROL Minhas informações] será exibida.\
   ![Basecamp_Integration_-_Token1.png](assets/basecamp-integration---token1-350x334.png)

1. No [!UICONTROL Tokens de autenticação] seção , clique em **[!UICONTROL Mostrar seus tokens]** (2) para exibir seus tokens de autenticação pessoais.
1. Selecione o **[!UICONTROL Token para leitores de feed]** ou **[!UICONTROL API do Basecamp]** (3), em seguida, copie o token para a área de transferência.

1. Cole seu [!DNL Basecamp] Token da API no [!UICONTROL Token para leitores de feed] ou [!UICONTROL API do Basecamp] caixa.\
   ![Basecamp_Integration_-_Token2.png](assets/basecamp-integration---token2-350x178.png)

### Adicionar seu [!DNL Basecamp] Token de API para suas configurações pessoais

Para colar o [!DNL Basecamp] Token da API em seu [!DNL Workfront Proof] [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings):

1. Vá para o [[!UICONTROL Integrações] - Configuração do usuário](../../../workfront-proof/wp-getstarted/personal-settings/integrations-user-setup.md) em seu [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) (1)\
   Primeiro, um administrador deve habilitar o [!DNL Basecamp Classic] para habilitar suas configurações pessoais. Para obter informações sobre como configurar a integração, consulte [Ativar o [!DNL Basecamp] Integração com [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof) neste artigo.

1. No [!DNL Basecamp] Caixa de token da API (2), cole o token que você acabou de copiar de sua [!DNL Basecamp] [!UICONTROL Minhas informações] no campo (3).\
   Para obter informações sobre cópia de [!DNL Basecamp] Token de API, consulte [Recuperar seu [!DNL Basecamp] Token de API](#retrieving-your-basecamp-api-token) neste artigo.

1. Clique em **[!UICONTROL Salvar]** (4)

![Basecamp_personal_settings_-_integration.png](assets/basecamp-personal-settings---integration-350x250.png)

Seu [!DNL Workfront Proof] [Configurações pessoais](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings) agora estão integradas ao [!DNL Basecamp Classic] conta.
