---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: http-modules
title: Usar TLS mútuo em módulos HTTP no Adobe Workfront Fusion
description: Você pode usar TLS Mútuo em seus módulos HTTP do Adobe Workfront Fusion, permitindo que ambos os lados da transação de informações verifiquem a identidade do outro.
author: Becky
feature: Workfront Fusion
exl-id: ace9c404-34de-4bc5-bc77-2e53df36dbd9
source-git-commit: 595d6e3e0a7d87240644bf20efd425917f4d953d
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Usar TLS mútuo em módulos HTTP em [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>O Adobe Workfront Fusion requer um [!DNL Adobe Workfront Fusion] além de uma licença da Adobe Workfront.

## Visão geral do TLS mútuo

Ao enviar dados pela Internet, é importante garantir que eles vão para ou vêm do local correto e que somente o recipient pretendido possa lê-los. Com o TLS ativado, o cliente (computador solicitando informações) usa certificados para verificar a identidade do servidor (computador fornecendo informações). Isso faz conexões HTTP seguras.

O TLS mútuo permite que essa confirmação de identidade siga ambas as maneiras. Quando o servidor envia seu certificado para verificar sua identidade ao cliente, ele também solicita o certificado do cliente. Isso garante que o servidor não envie informações para um site ou usuário que as usaria incorretamente.

>[!INFO]
>
>**Exemplo:**
>
>* **TLS**: Quando uma pessoa digita &quot;MyGreatBank.com&quot; em um navegador, ela quer ter certeza de que está indo para Meu Grande Banco, não um site que possa usar incorretamente ou vender suas informações bancárias. Eles também querem ter certeza de que suas informações de conta bancária estão criptografadas.
   >
   >   Quando o navegador (o cliente) se conecta a MyGreatBank.com (o servidor), o TLS requer um certificado de MyGreatBank.com para verificar sua identidade. O certificado é fornecido por uma autoridade de certificação, como [!DNL DigiCert] ou [!DNL Thawte]. Como o navegador confia na autoridade de certificado, ele permite a conexão.
>
>* **TLS mútuo**: MySoftware.com é um cliente de software que precisa de informações da API MyGreatBank.com. O MyGreatBank permite que apenas clientes confiáveis se conectem aos seus servidores. Assim, além do TLS regular que verifica a identidade do MyGreatBank.com, o processo de autoridade de certificação/TLS também verifica a solicitação do MySoftware.com.


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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Fornecer [!DNL Workfront Fusion] certificado público


Quando você se conecta a um serviço da Web com uma solicitação HTTP, o serviço da Web geralmente requer um [!DNL Workfront Fusion] certificado público para verificação. Isso permite que o serviço da Web compare o certificado apresentado na solicitação HTTP com o certificado no arquivo, como uma maneira de garantir que o certificado esteja na  lista de permissões do serviço da Web.

Para obter instruções sobre como fazer upload do [!DNL Adobe Workfront Fusion] certificado público para um serviço da Web, consulte a documentação do serviço da Web.

>[!NOTE]
>
>Talvez seja necessário fornecer outras informações além do certificado. Para obter informações sobre o que um serviço da Web requer, consulte a documentação da API do serviço da Web.

Você pode usar os seguintes links para baixar os certificados públicos do Workfront Fusion:

### Certificados para 14 de novembro de 2022 - 15 de julho de 2023

>[!IMPORTANT]
>
>Esses [!DNL Workfront Fusion] os certificados públicos expiram em 15 de julho de 2023. Depois que o seu expirar, você precisará fazer upload de um novo certificado para o serviço da Web. Recomendamos que você:
>
>* Anote a data de expiração e defina um lembrete para você fazer upload do certificado em seu serviço da Web.
>* Marque esta página como favorito para localizar facilmente os novos certificados.
>


* [Baixar [!DNL Workfront Fusion] Certificado 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com-jul-15-2023+updated.cer)
* [Baixar [!DNL Workfront Fusion] Certificado UE 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app-eu_workfrontfusion_com-jul-15-2023.cer)

   Para utilização na UE

<!--

Previous US cert

* [Download [!DNL Workfront Fusion] Certificate 2023](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/app_workfrontfusion_com-jul-15-2023.cer)

### Certificates for November 17, 2021 - November 14, 2022

>[!IMPORTANT]
>
>These certificates expire on November 14, 2022. Upload the new certificates to the web service as soon as possible.

* [Download Workfront Fusion Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app_workfrontfusion_com_certificate-chain-2022.crt) 
* [Download Workfront Fusion EU Certificate 2022](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion+2.0+public+certificates/app-eu_workfrontfusion_com_certificate-chain-2022.crt)

  For use in the EU

  -->

## Ativar TLS mútuo no [!DNL Workfront Fusion] Módulos HTTP

Todos [!DNL Workfront Fusion] [!UICONTROL HTTP] Os módulos de solicitação têm a opção de habilitar o TLS mútuo.

Para ativar o TLS mútuo em um [!UICONTROL HTTP] módulo de solicitação:

1. Adicione um [!UICONTROL HTTP] solicite o módulo para o seu cenário.
1. Comece a configurar o módulo.

   Para obter instruções sobre como configurar um [!UICONTROL HTTP] módulo de solicitação, consulte o artigo apropriado em [[!UICONTROL HTTP] módulos](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

1. Habilitar **[!UICONTROL Mostrar configurações avançadas]** próximo à parte inferior do módulo.
1. Habilitar **[!UICONTROL Usar TLS mútuo]**.
