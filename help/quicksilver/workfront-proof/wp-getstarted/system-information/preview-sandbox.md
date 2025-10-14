---
content-type: overview;how-to-procedural
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: system-information
title: Visualizar Ambiente de Teste de Sandbox- [!DNL Workfront Proof]
description: A Sandbox de visualização é um ambiente de teste que serve como uma réplica do seu ambiente ativo e é atualizado todos os finais de semana por  [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: cdf269c6-39b1-477a-b9ea-03edf2de77f0
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Visualizar Ambiente de Teste de Sandbox - [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

A sandbox de visualização é um ambiente de teste que serve como uma réplica do seu ambiente ativo e é atualizado todos os finais de semana por [!DNL Workfront Proof].

## Noções básicas sobre a sandbox de visualização

A sandbox de visualização serve como um ambiente em que os usuários em sua organização podem testar e trabalhar com dados do ambiente de produção com segurança, sem afetar o ambiente de produção. É ideal para executar sessões de treinamento, testar novos recursos e determinar a funcionalidade de configuração.

Além disso, novos recursos do produto são carregados no ambiente Pré-visualização de sandbox antes de serem entregues no ambiente de Produção. Seus usuários podem experimentar novas funcionalidades sem afetar seu fluxo de trabalho normal no ambiente de Produção.

A sandbox de visualização contém seus dados de produção reais. Os dados fluem da produção para a pré-visualização, e não ao contrário. Ele é atualizado todos os finais de semana, para que os dados possam estar atrasados em até uma semana no ambiente de produção. Os itens criados desde a última atualização estão no ambiente Visualização da sandbox até a atualização seguinte.

## Acesso à sandbox de visualização

Por padrão, como administrador do sistema, você tem acesso ao ambiente Visualização da sandbox. Se não conseguir acessar o ambiente Visualizar Sandbox conforme descrito nesta seção, contate o administrador do [!DNL Workfront] ou nossa equipe de suporte.

* [Acessando a Sandbox de Visualização como um Cliente Autônomo [!DNL Workfront Proof] &#x200B;](#accessing-the-preview-sandbox-as-a-stand-alone-workfront-proof-customer)
* [Acessando a sandbox de visualização como um cliente do  [!DNL Workfront]+[!DNL Workfront Proof] &#x200B;](#accessing-the-preview-sandbox-as-a-workfrontworkfront-proof-customer)

### Acessando a Sandbox de Visualização como Cliente Autônomo do [!DNL Workfront Proof]

1. Navegue até esta URL: `https://preview.proofhq.com`.
1. Faça logon usando as credenciais de Visualização.\
   Suas credenciais de Visualização devem ser as mesmas que suas credenciais de Produção, a menos que você as tenha alterado na Produção após a atualização da Visualização. Os logons são sincronizados somente quando ocorre uma atualização, que ocorre todos os finais de semana. Eles não são sincronizados automaticamente.

### Acessando a sandbox de visualização como um cliente de prova do [!DNL Workfront+Workfront]

Como administrador do sistema, você pode acessar a Sandbox de Visualização [!DNL Workfront Proof] por meio da interface [!DNL Workfront].

Para acessar a Sandbox de Visualização [!DNL Workfront Proof]:

1. Faça logon no ambiente [!DNL Workfront].
1. Clique em **[!UICONTROL Configuração]** na barra de Navegação Global.
1. Clique em **[!UICONTROL Sistema]** >**[!UICONTROL Preferências]**.

1. Na seção **[!UICONTROL Ambientes de Teste]**, clique em **[!UICONTROL Visualização de Sandbox]**.

1. Faça logon com as credenciais de Visualização.\
   As credenciais de Visualização devem ser iguais às credenciais de Produção, a menos que você as altere na Produção após a atualização da Visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.
1. Clique no ícone [!DNL Workfront Proof] na Barra de Navegação Global.\
   ![proof_access_proofhq.png](assets/proof-access-proofhq-350x39.png)\
   O ambiente de Visualização [!DNL Workfront Proof] é exibido.

## Recebimento de emails da sandbox de visualização

As notificações por email nunca são disparadas do ambiente de Visualização [!DNL Workfront Proof].
