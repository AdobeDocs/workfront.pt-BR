---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] com medidas de segurança atualizadas
description: A Google introduziu recentemente restrições sobre como os usuários podem usar sua API. Este artigo descreve como se conectar [!DNL Adobe Workfront Fusion] para o Google, levando em conta essas medidas de segurança de atualização.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] com medidas de segurança atualizadas

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
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrições

[!DNL Google] introdução de restrições sobre como os usuários podem usar sua API a partir de 1º de junho de 2020. Essas medidas de segurança protegem [!DNL Google] utilizadores de dados pessoais provenientes de fugas ou de utilização [!DNL Google]. As restrições estão relacionadas ao [!DNL Gmail] e [!DNL Google Drive] aplicativos. Para obter mais informações sobre essas restrições, consulte &quot;Requisitos adicionais para escopos específicos da API&quot; no [[!DNL Google] Política de Dados do Usuário dos Serviços de API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Para acessar escopos restritos, o serviço conectado ([!DNL Adobe Workfront Fusion] ou qualquer outro serviço que deseje acessar os dados do usuário por meio da API) devem ser verificados e devem ter uma Carta de Avaliação para provar que o serviço é seguro e transparente sobre como eles usam os dados. [!DNL Workfront Fusion] está em conformidade com todos [!DNL Google]Requisitos do para acessar escopos restritos. No entanto, a maioria dos serviços conectados de terceiros em [!DNL Workfront Fusion] não possuem a Carta de Avaliação e, portanto, não estão em conformidade com [!DNL Google] termos. Por causa disso, [!DNL Workfront Fusion] O não tem permissão para enviar dados para esses serviços.

## Exceções a [!DNL Google Services] restrições

Há algumas exceções que permitem enviar dados a um serviço de terceiros não aprovado que não tenha a Carta de Avaliação sem violar nenhuma das novas restrições. Eles diferem com base em [!DNL G Suite] com o [!DNL Workfront Fusion] cliente OAuth, [!DNL G Suite] com outro cliente OAuth ou [!DNL @gmail.com] e [!DNL @google.mail.com].

* [[!DNL G suite] com [!DNL Workfront Fusion] Cliente OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G suite] com outro cliente OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] e [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] com [!DNL Workfront Fusion] Cliente OAuth

[!DNL Workfront Fusion] usa o [!UICONTROL Instalação em todo o domínio] exceção. A instalação em todo o domínio é adequada para [!DNL G Suite] e permite que os usuários integrem serviços não aprovados sem qualquer limitação. Se você for um usuário do G Suite, não precisará executar etapas adicionais e poderá se conectar diretamente a serviços não aprovados.

### [!DNL G suite] com outro cliente OAuth

[!DNL G Suite] usuários que preferem usar seu próprio cliente OAuth em vez de usar o [!DNL Workfront Fusion] O cliente OAuth pode se conectar a [!DNL Google Services] por meio da [!UICONTROL Interno] Use a abordagem. Essa opção destina-se a usuários avançados. Para obter instruções, consulte [Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] uso de um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] e [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Usuário que acessa [!DNL Google Services] até [!DNL @gmail.com] ou [!DNL @googlemail.com] pode se conectar a [!DNL Google Services] através da abordagem de uso pessoal. Essa opção destina-se a usuários avançados. Para obter instruções, consulte [Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] uso de um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Perguntas frequentes

* [Quais aplicativos estão em [!DNL Adobe Workfront Fusion] são afetados?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Tenho uma conta do [!DNL G Suite]?](#do-i-have-a-g-suite-account)
* [O que devo fazer se for [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [O que devo fazer se sou um usuário do [!DNL G Suite]?](#what-should-i-do-if-im-a-g-suite-user)

### Quais aplicativos estão em [!DNL Adobe Workfront Fusion] são afetados? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail], e Email (conectado a [!DNL Gmail] conta).

### Eu tenho um [!DNL G Suite] conta? {#do-i-have-a-g-suite-account}

Se o seu endereço de email terminar com [!DNL @gmail.com] ou [!DNL @googlemail.com] sua conta não é uma [!DNL G Suite] conta. Se o seu [!DNL Google] conta termina com um domínio personalizado, como @my-company.com, então é um [!DNL G Suite] conta.

### O que devo fazer se for [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Essas novas restrições só se aplicam se você estiver integrando [!DNL Google Drive] ou [!DNL Gmail]. Se quiser se conectar a [!DNL Google Drive] ou [!DNL Gmail], você pode

* Alternar para [!DNL G Suite]

  ou

* Crie um cliente OAuth personalizado. Essa opção destina-se a usuários avançados.

  Para obter instruções, consulte [Conectar [!DNL Adobe Workfront Fusion] para [!DNL Google Services] uso de um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Se quiser integrar qualquer serviço diferente do [!DNL Google Drive] ou [!DNL Gmail], essas restrições não se aplicam.

Para obter instruções sobre como conectar outros [!DNL Google Services] para [!DNL Workfront Fusion], consulte [Conecte o aplicativo ou serviço Web do módulo ao [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) no artigo [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### O que devo fazer se sou um [!DNL G Suite] usuário? {#what-should-i-do-if-im-a-g-suite-user}

Não há nenhuma ação necessária.
