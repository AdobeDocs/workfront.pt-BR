---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: connections-annd-webhooks
title: Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] com medidas de segurança atualizadas
description: A Google introduziu recentemente restrições sobre como os usuários podem usar sua API. Este artigo descreve como se conectar [!DNL Adobe Workfront Fusion] ao Google, considerando essas medidas de segurança de atualização.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] com medidas de segurança atualizadas

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] restrições

O [!DNL Google] introduziu restrições sobre como os usuários podem usar sua API a partir de 1º de junho de 2020. Essas medidas de segurança protegem [!DNL Google] usuários contra vazamento ou uso indevido de seus dados pessoais no [!DNL Google]. As restrições estão relacionadas aos aplicativos [!DNL Gmail] e [!DNL Google Drive]. Para obter mais informações sobre essas restrições, consulte &quot;Requisitos adicionais para escopos de API específicos&quot; na [[!DNL Google] Política de dados do usuário dos serviços de API](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Para acessar escopos restritos, o serviço conectado ([!DNL Adobe Workfront Fusion] ou qualquer outro serviço que deseje acessar os dados do usuário por meio da API) deve ser verificado e deve ter uma Carta de Avaliação para provar que o serviço é seguro e transparente sobre como os dados são usados. [!DNL Workfront Fusion] está em conformidade com todos os requisitos de [!DNL Google] para acesso a escopos restritos. No entanto, a maioria dos serviços conectados de terceiros em [!DNL Workfront Fusion] não tem a Carta de Avaliação e, portanto, não está em conformidade com os termos de [!DNL Google]. Por causa disso, [!DNL Workfront Fusion] não tem permissão para enviar dados para esses serviços.

## Exceções a [!DNL Google Services] restrições

Há algumas exceções que permitem enviar dados a um serviço de terceiros não aprovado que não tenha a Carta de Avaliação sem violar nenhuma das novas restrições. Eles diferem com base em [!DNL Google Workspace] com o cliente OAuth [!DNL Workfront Fusion], [!DNL Google Workspace] com outro cliente OAuth ou [!DNL @gmail.com] e [!DNL @google.mail.com].

* [[!DNL Google Workspace] com  [!DNL Workfront Fusion] cliente OAuth](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] com outro cliente OAuth](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] e [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] com [!DNL Workfront Fusion] cliente OAuth

[!DNL Workfront Fusion] usa a exceção [!UICONTROL Instalação em todo o domínio]. A Instalação em todo o domínio é adequada para [!DNL Google Workspace] usuários e permite que os usuários integrem serviços não aprovados sem qualquer limitação. Se você for um usuário do Google Workspace, não será necessário executar etapas adicionais e poderá se conectar diretamente a serviços não aprovados.

### [!DNL Google Workspace] com outro cliente OAuth

[!DNL Google Workspace] usuários que preferem usar seu próprio cliente OAuth em vez de usar o cliente OAuth [!DNL Workfront Fusion] podem se conectar a [!DNL Google Services] por meio da abordagem de uso [!UICONTROL Interno]. Essa opção destina-se a usuários avançados. Para obter instruções, consulte [Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] e [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

O usuário que acessar [!DNL Google Services] por meio de [!DNL @gmail.com] ou [!DNL @googlemail.com] pode se conectar a [!DNL Google Services] por meio da abordagem de Uso Pessoal. Essa opção destina-se a usuários avançados. Para obter instruções, consulte [Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## Perguntas frequentes

* [Quais aplicativos em  [!DNL Adobe Workfront Fusion]  são afetados?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Eu tenho uma conta  [!DNL Google Workspace] ?](#do-i-have-a-g-suite-account)
* [O que devo fazer se sou [!DNL @gmail.com] ou [!DNL @googlemail.com] usuário?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [O que devo fazer se sou um  [!DNL Google Workspace] usuário?](#what-should-i-do-if-im-a-g-suite-user)

### Quais aplicativos em [!DNL Adobe Workfront Fusion] são afetados? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] e Email (conectado à conta [!DNL Gmail]).

### Tenho uma conta [!DNL Google Workspace]? {#do-i-have-a-g-suite-account}

Se seu endereço de email termina com [!DNL @gmail.com] ou [!DNL @googlemail.com] sua conta não é uma conta [!DNL Google Workspace]. Se a conta do [!DNL Google] terminar com um domínio personalizado como @my-company.com, essa é uma conta do [!DNL Google Workspace].

### O que devo fazer se eu for um usuário do [!DNL @gmail.com] ou do [!DNL @googlemail.com]? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Essas novas restrições só se aplicam se você estiver integrando o [!DNL Google Drive] ou o [!DNL Gmail]. Se quiser se conectar a [!DNL Google Drive] ou [!DNL Gmail], você pode

* Mudar para [!DNL Google Workspace]

  ou

* Crie um cliente OAuth personalizado. Essa opção destina-se a usuários avançados.

  Para obter instruções, consulte [Conectar [!DNL Adobe Workfront Fusion] a [!DNL Google Services] usando um cliente OAuth personalizado](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Se você quiser integrar qualquer serviço diferente de [!DNL Google Drive] ou [!DNL Gmail], essas restrições não se aplicam.

Para obter instruções sobre como conectar outro [!DNL Google Services] a [!DNL Workfront Fusion], consulte [Conectar o aplicativo ou serviço Web do módulo a [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) no artigo [Criar um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### O que devo fazer se eu for um usuário do [!DNL Google Workspace]? {#what-should-i-do-if-im-a-g-suite-user}

Não há nenhuma ação necessária.
