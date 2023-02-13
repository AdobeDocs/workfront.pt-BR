---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] para [!DNL Google Services] com medidas de segurança atualizadas
description: A Google introduziu recentemente restrições sobre como os usuários podem usar sua API. Este artigo descreve como se conectar [!DNL Adobe Workfront Fusion] para a Google, contabilizando essas medidas de segurança de atualização.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Connect [!DNL Adobe Workfront Fusion] para [!DNL Google Services] com medidas de segurança atualizadas

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrições

[!DNL Google] introduziu restrições sobre como os usuários podem usar sua API a partir de 1º de junho de 2020. Estas medidas de segurança protegem [!DNL Google] usuários de fugas ou uso indevido de seus dados pessoais em [!DNL Google]. As restrições estão relacionadas com a [!DNL Gmail] e [!DNL Google Drive] aplicativos. Para obter mais informações sobre essas restrições, consulte &quot;Requisitos adicionais para escopos de API específicos&quot; na seção [[!DNL Google] Política de dados do usuário dos serviços de API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Para acessar escopos restritos, o serviço conectado ([!DNL Adobe Workfront Fusion] ou qualquer outro serviço que deseje acessar os dados do usuário por meio da API) deve ser verificado e deve ter uma Carta de Avaliação para provar que o serviço é seguro e transparente sobre como eles usam os dados. [!DNL Workfront Fusion] cumpre com todas as [!DNL Google]Exigências de acesso aos escopos restritos. No entanto, a maioria dos serviços conectados de terceiros em [!DNL Workfront Fusion] não têm a Carta de Avaliação e, portanto, não estão em conformidade com [!DNL Google] termos. Por causa disso, [!DNL Workfront Fusion] não tem permissão para enviar dados para esses serviços.

## Exceções a [!DNL Google Services] restrições

Existem algumas exceções que permitem enviar dados para um serviço de terceiros não aprovado que não tem a Carta de Avaliação sem violar qualquer uma das novas restrições. Elas diferem com base em [!DNL G Suite] com o [!DNL Workfront Fusion] cliente OAuth, [!DNL G Suite] com outro cliente OAuth, ou [!DNL @gmail.com] e [!DNL @google.mail.com].

* [[!DNL G suite] com [!DNL Workfront Fusion] Cliente OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] com outro cliente OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] e [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] com [!DNL Workfront Fusion] Cliente OAuth

[!DNL Workfront Fusion] usa a variável [!UICONTROL Instalação em todo o domínio] exceção. A Instalação em todo o domínio é adequada para [!DNL G Suite] e permite que os usuários integrem serviços não aprovados sem limitações. Se você for um usuário do G Suite, não precisará executar etapas adicionais e poderá se conectar diretamente a serviços não aprovados.

### [!DNL G suite] com outro cliente OAuth

[!DNL G Suite] usuários que preferem usar seu próprio cliente OAuth em vez de usar o [!DNL Workfront Fusion] O cliente OAuth pode se conectar a [!DNL Google Services] através da [!UICONTROL Interno] Abordagem de uso. Essa opção destina-se a usuários avançados. Para obter instruções, consulte [Connect [!DNL Adobe Workfront Fusion] para [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] e [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Usuário que acessa [!DNL Google Services] through [!DNL @gmail.com] ou [!DNL @googlemail.com] pode se conectar a [!DNL Google Services] através da abordagem de uso pessoal. Essa opção destina-se a usuários avançados. Para obter instruções, consulte [Connect [!DNL Adobe Workfront Fusion] para [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Perguntas frequentes

* [Quais aplicativos são [!DNL Adobe Workfront Fusion] são afetadas?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Tenho uma conta do [!DNL G Suite]?](#do-i-have-a-g-suite-account)
* [O que devo fazer se eu estiver [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [O que devo fazer se for um usuário do [!DNL G Suite]?](#what-should-i-do-if-im-a-g-suite-user)

### Quais aplicativos são [!DNL Adobe Workfront Fusion] são afetadas? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]e Email (conectado ao [!DNL Gmail] conta).

### Eu tenho um [!DNL G Suite] conta? {#do-i-have-a-g-suite-account}

Se seu endereço de email terminar com [!DNL @gmail.com] ou [!DNL @googlemail.com] sua conta não é [!DNL G Suite] conta. Se o seu [!DNL Google] a conta termina com um domínio personalizado, como @my-company.com , então é uma [!DNL G Suite] conta.

### O que devo fazer se eu estiver [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Essas novas restrições só se aplicam se você estiver integrando o [!DNL Google Drive] ou [!DNL Gmail]. Se você deseja se conectar ao [!DNL Google Drive] ou [!DNL Gmail], você pode

* Mudar para [!DNL G Suite]

   ou

* Crie um cliente OAuth personalizado. Essa opção destina-se a usuários avançados.

   Para obter instruções, consulte [Connect [!DNL Adobe Workfront Fusion] para [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Se quiser integrar qualquer outro serviço que não [!DNL Google Drive] ou [!DNL Gmail], estas restrições não se aplicam.

Para obter instruções sobre como conectar outros [!DNL Google Services] para [!DNL Workfront Fusion], consulte [Conecte o aplicativo ou o serviço da Web do módulo ao [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) no artigo [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### O que devo fazer se eu for um [!DNL G Suite] usuário? {#what-should-i-do-if-im-a-g-suite-user}

Não há ação necessária.
