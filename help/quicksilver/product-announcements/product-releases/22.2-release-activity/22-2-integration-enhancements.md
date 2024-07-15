---
title: 22.2 Aprimoramentos de integração
description: 22.2 Aprimoramentos de integração
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 22.2 Aprimoramentos de integração

Esta página descreve todas as melhorias de Integração feitas com a versão 22.2 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 4 de abril de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.2, consulte a [Visão geral da versão 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## A integração do Adobe Workfront com Anaplan já está disponível

Para oferecer mais flexibilidade e insight sobre os aspectos financeiros dos projetos da Workfront, a Workfront agora pode se integrar à sua conta Anaplan. Ao vincular objetos Workfront a objetos Anaplan, você pode atualizar informações entre as duas contas automaticamente, garantindo que as informações em ambas estejam atualizadas e idênticas. Você também pode acionar processos automatizados no Anaplan com base em ações no Workfront (ou vice-versa).

Por exemplo, você pode criar uma campanha no Anaplan e, em seguida, criar um projeto ou programa do Workfront vinculado à campanha. Quaisquer custos rastreados no Workfront podem ser enviados de volta ao Anaplan para analisar o desempenho da campanha.

Outros fluxos de trabalho que você pode considerar usar a integração Workfront para Anaplan para incluem:

* Criar solicitações de orçamento do Anaplan a partir de novos projetos Workfront
* Criando projetos Workfront a partir de novos Itens da Lista Anaplan
* Iniciando solicitações de fornecedores Anaplan de projetos Workfront

Para obter mais informações, consulte [Adobe Workfront com Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Atualizações aprimoradas de conector do Workfront for Experience Manager

O conector aprimorado do Workfront para Experience Manager agora inclui as seguintes atualizações:

* Agora é possível criar pastas vinculadas entre o Adobe Workfront e o Adobe Experience Manager Assets as a Cloud Service, mesmo se houver várias configurações de pastas vinculadas do projeto.
* Adição de suporte para paginação de subscrição de evento.
* Adição de suporte para AEM 6.4.x
* Adição de suporte para ambientes proxy
* Várias correções de bugs com base no feedback do parceiro e do cliente

Para obter mais informações, consulte [visão geral do conector aprimorado Workfront for Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>A implantação e a configuração deste conector exigem um parceiro certificado. Consulte [Instalar o Workfront para o conector aprimorado do Experience Manager](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) para obter mais informações.

## As integrações do Adobe Creative Cloud agora usam OAuth2

Para maior segurança e para tornar uma experiência mais consistente em todas as integrações, atualizamos as integrações do Adobe Creative Cloud para usar a autenticação OAuth2, uma maneira padrão do setor para autenticar usuários. Agora, quando os usuários fizerem logon, eles poderão ver as ações e áreas específicas às quais as integrações têm acesso e permitir acesso. Depois disso, eles não precisarão fazer logon com a mesma frequência.

Para obter mais informações, consulte [Usar a extensão do Workfront para Illustrator e InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Consulte detalhes do Segredo do cliente para integrações OAuth2 ou JWT personalizadas

Para fornecer transparência no uso das integrações OAuth2 e JWT personalizadas, possibilitamos que você veja detalhes dos Segredos do cliente que suas integrações usam. Agora você pode ver as datas em que o Segredo do cliente foi criado e usado pela última vez. Você também pode adicionar e exibir suas próprias observações sobre o Segredo do cliente.

Anteriormente, esses detalhes estavam indisponíveis.

Para obter mais informações sobre Segredos do cliente em integrações OAuth2 ou JWT personalizadas, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Consulte o tipo de autenticação na lista de aplicativos OAuth2 personalizados

Agora, ao visualizar a lista de aplicativos OAuth2 personalizados em sua organização, você pode ver se cada aplicativo usa autenticação de usuário ou autenticação de servidor.

Anteriormente, só era possível ver essas informações acessando as opções de edição em cada aplicativo.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Defina a expiração para atualizar tokens em suas integrações OAuth2 personalizadas

Para controlar melhor o acesso e a segurança de suas integrações OAuth2 personalizadas, agora é possível personalizar a duração de tokens de atualização. Depois que um token de atualização do usuário expirar, será necessário fazer logon na integração novamente.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Use chaves públicas e privadas em suas integrações OAuth2 personalizadas para aplicativos de servidor para servidor

Agora é possível configurar aplicativos OAuth2 de servidor para servidor em suas integrações personalizadas. Ao configurar chaves públicas e privadas, você pode permitir que o Workfront se comunique com outro aplicativo sem usar credenciais de logon.

Anteriormente, todas as autenticações nos aplicativos OAuth2 personalizados usavam as credenciais de logon do usuário.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## A integração do Google Google Workspace agora usa OAuth2

Para maior segurança e para tornar uma experiência mais consistente em todas as integrações, atualizamos a integração do Google Google Workspace para usar a autenticação OAuth2, uma maneira padrão do setor para autenticar usuários. Agora, quando os usuários fizerem logon, eles poderão ver as ações e áreas específicas às quais as integrações têm acesso e permitir acesso. Depois disso, eles não precisarão fazer logon com a mesma frequência.

Para obter mais informações, consulte [Fazer logon e logoff da Adobe Workfront para o Google Workspace](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
