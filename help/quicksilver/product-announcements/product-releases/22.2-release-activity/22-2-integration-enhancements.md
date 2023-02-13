---
title: 2.2 Melhorias da integração
description: 2.2 Melhorias da integração
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: 5e841349-7d76-4ab9-9625-a0c53111bf35
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# 2.2 Melhorias da integração

Esta página descreve todas as melhorias da integração feitas com a versão 2.2 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados no ambiente Produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 4 de abril de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.2, consulte [Visão geral da versão 2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Adobe Workfront com integração com Anaplan agora disponível

Para proporcionar melhor flexibilidade e insights sobre os aspectos financeiros dos projetos da Workfront, a Workfront agora pode se integrar com sua conta Anaplan. Ao vincular objetos Workfront a objetos Anaplan, é possível atualizar as informações entre as duas contas automaticamente, garantindo que as informações em ambas sejam atualizadas e idênticas. Também é possível acionar processos automatizados em Anaplan com base em ações no Workfront (ou vice-versa).

Por exemplo, você pode criar uma campanha em Anaplan e, em seguida, criar um projeto ou programa Workfront vinculado à campanha. Qualquer custo rastreado no Workfront pode ser enviado de volta para Anaplan para analisar o desempenho da campanha.

Outros workflows que você pode considerar o uso da integração Workfront com Anaplan para incluir:

* Criação de solicitações de orçamento do Anaplan a partir de novos projetos do Workfront
* Criando projetos do Workfront a partir de novos itens da lista Anaplan
* Iniciando solicitações de fornecedores Anaplan de projetos da Workfront

Para obter mais informações, consulte [Adobe Workfront com Anaplan](../../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/anaplan-integration.md).

## Atualizações do conector avançado Workfront for Experience Manager

O conector Workfront para Experience Manager aprimorado agora inclui as seguintes atualizações:

* Agora é possível criar pastas vinculadas entre o Adobe Workfront e o Adobe Experience Manager Assets as a Cloud Service, mesmo se houver várias configurações de pastas vinculadas ao projeto.
* Suporte adicionado para paginação de assinatura de evento
* Adição de suporte para AEM 6.4.x
* Suporte adicionado para ambientes proxy
* Várias correções de erros com base no feedback de parceiros e clientes

Para obter mais informações, consulte [Visão geral do conector aprimorado Workfront for Experience Manager](../../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-aem-enhanced-connector-overview.md).

>[!NOTE]
>
>A implantação e a configuração desse conector exigem um parceiro certificado. Consulte [Instalar o Workfront para conector Experience Manager aprimorado](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/workfront-connector-install.html?lang=en#) para obter mais informações.

## As integrações do Adobe Creative Cloud agora usam OAuth2

Para maior segurança e para tornar uma experiência mais consistente em todas as integrações, atualizamos as integrações do Adobe Creative Cloud para usar a autenticação OAuth2, uma maneira padrão do setor para autenticar usuários. Agora, quando os usuários fizerem logon, poderão ver as ações e áreas específicas às quais as integrações têm acesso e permitir o acesso. Depois disso, eles não precisarão fazer logon com a mesma frequência.

Para obter mais informações, consulte [Usar a extensão Workfront para Illustrator e InDesign](../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md).

## Veja os detalhes do Segredo do cliente para integrações OAuth2 ou JWT personalizadas

Para fornecer transparência ao uso de suas integrações OAuth2 e JWT personalizadas, possibilitamos que você veja detalhes dos Segredos do cliente que suas integrações usam. Agora, você pode ver as datas em que o Segredo do cliente foi criado e usado pela última vez. Você também pode adicionar e exibir suas próprias observações sobre o Segredo do cliente.

Anteriormente, esses detalhes não estavam disponíveis.

Para obter mais informações sobre Segredos do cliente nas integrações personalizadas OAuth2 ou JWT, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Veja o tipo de autenticação na lista de aplicativos OAuth2 personalizados

Agora, ao exibir a lista de aplicativos OAuth2 personalizados em sua organização, você pode ver se cada aplicativo usa a autenticação Usuário ou Servidor .

Anteriormente, você podia ver essas informações somente acessando as opções de edição em cada aplicativo.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Defina a expiração para tokens de atualização em suas integrações OAuth2 personalizadas

Para controlar melhor o acesso e a segurança de suas integrações OAuth2 personalizadas, agora é possível personalizar o tempo de vida dos tokens de atualização. Depois que o token de atualização de um usuário expirar, ele precisará fazer logon na integração novamente.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Usar chaves públicas e privadas em suas integrações OAuth2 personalizadas para aplicativos de servidor para servidor

Agora é possível configurar aplicativos OAuth2 de servidor para servidor em suas integrações personalizadas. Ao configurar chaves públicas e privadas, você pode permitir que o Workfront se comunique com outro aplicativo sem usar credenciais de logon.

Anteriormente, todas as autenticações em seus aplicativos OAuth2 personalizados usavam as credenciais de logon do usuário.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## A integração do Google G Suite agora usa OAuth2

Para maior segurança e para tornar uma experiência mais consistente em todas as integrações, atualizamos a integração do Google G Suite para usar a autenticação OAuth2, uma maneira padrão do setor para autenticar usuários. Agora, quando os usuários fizerem logon, poderão ver as ações e áreas específicas às quais as integrações têm acesso e permitir o acesso. Depois disso, eles não precisarão fazer logon com a mesma frequência.

Para obter mais informações, consulte [Fazer logon e sair do Adobe Workfront para G Suite](../../../workfront-integrations-and-apps/workfront-for-g-suite/log-in-and-out-wf-for-gsuite.md).
