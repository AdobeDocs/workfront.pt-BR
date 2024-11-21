---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulo SOAP
description: Você pode usar o módulo SOAP para se conectar a APIs SOAP no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 752e0766-25f2-4d22-bed5-7c931284258d
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 1%

---

# Módulo [!UICONTROL SOAP]

Você pode usar o módulo [!UICONTROL SOAP] para se conectar às APIs do [!UICONTROL SOAP] no [!UICONTROL Adobe Workfront Fusion].

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
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Limitações do módulo [!UICONTROL SOAP]

>[!NOTE]
>
>Os redirecionamentos são desativados durante o carregamento WDSL. Esse é um recurso de segurança, mas pode significar que redirecionamentos não verificados serão bloqueados quando o módulo for executado.

O módulo [!UICONTROL SOAP] está atualmente na versão beta e não oferece suporte a:

* Redefinir elementos
* Restrições de dígitos de fração
* Restrições de dígitos totais
* Restrições de espaço em branco
* Várias partes nas mensagens de entrada e saída. Somente mensagens de parte única são suportadas
* Elementos de Esquema XML personalizados definidos com a ajuda de esquemas e elementos de [[!UICONTROL SOAP] Codificação](https://schemas.xmlsoap.org).

>[!INFO]
>
>**Exemplo:**
>  
>O seguinte não seria reconhecido corretamente pelo [!UICONTROL Workfront Fusion]:
>
>```
><complexType name="ArrayOfFloat">
>     <complexContent>
>           <restriction base="soapenc:Array">
>                 <attribute ref="soapenc:arrayType"
>                       wsdl:arrayType="xsd:integer[]"/>
>           </restriction>
>     </complexContent>
></complexType>
>```
>
>Este exemplo inclui as referências `soapenc:Array`, `soapenc:arrayType` e `wsdl:arrayType`, que ainda não têm suporte no [!UICONTROL Workfront Fusion].

## Solução alternativa

Se o módulo [!UICONTROL SOAP] se recusar a processar o arquivo WSDL ou lançar vários erros na configuração do módulo, você poderá tentar usar o módulo universal **[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação]**:

1. Em [!DNL Workfront Fusion], crie um novo cenário.
1. Insira o módulo **[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação]** no cenário.
1. Abra a configuração do módulo e preencha os seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Método]</td> 
      <td> <p>[!UICONTROL POST]</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Tipo de corpo]</td> 
      <td> <p>[!UICONTROL Bruto]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de conteúdo]</td> 
      <td> <p>[!UICONTROL XML (application/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Analisar resposta]</td> 
      <td>[!UICONTROL Habilitado]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Abra uma nova janela ou guia do navegador da Web.
1. Cole o URL WSDL na barra de endereços do navegador da Web e busque o arquivo XML.

   A URL WSDL geralmente termina com `?wsdl`, mas não necessariamente, por exemplo `http://voip.ms/api/v1/server.wsdl`.

1. Se o arquivo WSDL não for exibido diretamente no navegador da Web, abra o arquivo baixado em um editor de texto.
1. Pesquisar a marca `<service>` ou `<wsdl:service>`:

   ![](assets/service-350x65.png)

1. Depois de localizado, copie a URL do atributo `location`.
1. Em [!DNL Workfront Fusion], cole a URL no campo de URL do módulo HTTP.
1. Abra o [Cliente [!UICONTROL SOAP] online](https://wsdlbrowser.com/) em uma nova janela/guia do navegador da Web.
1. Cole o URL do WSDL no campo URL do WSDL.
1. Clique em **[!UICONTROL Procurar]**.
1. Escolha na lista de funções à esquerda, por exemplo `getLanguages`.
1. Copie o conteúdo da área de texto [!UICONTROL Solicitar XML].
1. No [!UICONTROL Workfront Fusion], cole o conteúdo copiado no campo de URL do módulo.
1. Forneça valores para os parâmetros selecionados substituindo os pontos de interrogação pelos valores reais:

   ![](assets/request-xml-350x172.png)

1. Feche a configuração do módulo clicando em **[!UICONTROL OK]**.
1. Execute o cenário ou módulo.
