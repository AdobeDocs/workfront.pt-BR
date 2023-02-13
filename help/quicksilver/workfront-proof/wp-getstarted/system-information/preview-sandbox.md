---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Visualizar ambiente de teste do Sandbox - [!DNL Workfront Proof]
description: A sandbox de visualização é um ambiente de teste que serve como réplica do ambiente ativo e é atualizado a cada fim de semana por [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Visualizar ambiente de teste do Sandbox - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

A sandbox de visualização é um ambiente de teste que serve como réplica do ambiente ativo e é atualizado a cada fim de semana por [!DNL Workfront Proof].

## Noções básicas da caixa de proteção de visualização

A Sandbox de visualização serve como um ambiente em que os usuários em sua organização podem testar e trabalhar com dados com segurança do ambiente de Produção, sem afetar o ambiente de Produção. É ideal para executar sessões de treinamento, testar novos recursos e determinar a funcionalidade de configuração.

Além disso, novos recursos do produto são carregados no ambiente Preview Sandbox antes de serem entregues ao ambiente de Produção. Seus usuários podem experimentar uma nova funcionalidade sem afetar seu fluxo de trabalho normal no ambiente Produção.

A sandbox de visualização contém seus dados de produção reais. Fluxos de dados de Produção para Visualização, e não ao contrário. Ele é atualizado todos os fins de semana, de modo que os dados possam estar até uma semana atrás do ambiente de Produção. Os itens criados desde o último tempo de atualização estão no ambiente Preview Sandbox até a atualização a seguir.

## Acessar o sandbox de visualização

Por padrão, como administrador do sistema, você tem acesso ao ambiente Preview Sandbox . Se não conseguir acessar o ambiente Preview Sandbox conforme descrito nesta seção, entre em contato com seu [!DNL Workfront] administrador ou nossa equipe de suporte.

* [Acessar o sandbox de visualização como independente [!DNL Workfront Proof] Cliente](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Acessar o sandbox de visualização como uma [!DNL Workfront]+[!DNL Workfront Proof] Cliente](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Acessar o sandbox de visualização como independente [!DNL Workfront Proof] Cliente

1. Navegue até este URL:  `https://preview.proofhq.com`.
1. Faça logon usando suas credenciais de Visualização.\
   Suas credenciais de Pré-visualização devem ser iguais às suas credenciais de Produção, a menos que você as tenha alterado em Produção após a atualização de Pré-visualização. Os logons são sincronizados somente quando ocorre uma atualização, que ocorre todo fim de semana. Eles não sincronizam automaticamente.

### Acessar o sandbox de visualização como uma [!DNL Workfront+Workfront] Cliente de prova

Como administrador do sistema, você pode acessar o [!DNL Workfront Proof] Visualizar sandbox por meio da [!DNL Workfront] interface.

Para acessar o [!DNL Workfront Proof] Visualizar sandbox:

1. Faça logon no [!DNL Workfront] ambiente.
1. Clique em **[!UICONTROL Configuração]** na barra Navegação global.
1. Clique em **[!UICONTROL Sistema]** >**[!UICONTROL Preferências]**.

1. No **[!UICONTROL Testar ambientes]** seção , clique em **[!UICONTROL Visualização do Sandbox]**.

1. Faça logon com as credenciais de Visualização.\
   Suas credenciais de Pré-visualização devem ser iguais às credenciais de Produção, a menos que você as tenha alterado em Produção após a atualização de Pré-visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não sincronizam automaticamente.
1. Clique no botão [!DNL Workfront Proof] na Barra de navegação global.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   O [!DNL Workfront Proof] O ambiente de visualização é exibido.

## Recebendo emails da sandbox de visualização

As notificações por email nunca são acionadas pelo [!DNL Workfront Proof] Ambiente de visualização.
