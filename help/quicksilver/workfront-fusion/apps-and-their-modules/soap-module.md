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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# [!UICONTROL SOAP] módulo

Você pode usar o [!UICONTROL SOAP] módulo a ser conectado [!UICONTROL SOAP] APIs em [!UICONTROL Adobe Workfront Fusion].

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

## Usar o [!UICONTROL SOAP] módulo

O [!UICONTROL SOAP] no momento, o módulo está em beta e não oferece suporte a:

* Redefinir elementos
* Restrições de dígitos de Fração
* Total de restrições de dígitos
* Restrições de espaço em branco
* Várias partes nas mensagens de entrada e saída. Somente mensagens de parte única são suportadas
* Elementos personalizados do esquema XML definidos com a ajuda de [[!UICONTROL SOAP] Codificação](http://schemas.xmlsoap.org) esquemas e elementos.

>[!INFO]
>
>**Exemplo:**
>  
>Os itens a seguir não seriam reconhecidos corretamente por [!UICONTROL Workfront Fusion]:
>
>```
><complexType name="ArrayOfFloat">
>
>   <complexContent>
>
>      <restriction base="soapenc:Array">
>
>         <attribute ref="soapenc:arrayType"
>
>            wsdl:arrayType="xsd:integer[]"/>
>
>      </restriction>
>
>   </complexContent>
>
></complexType>
>```

Inclui a variável `soapenc:Array`, `soapenc:arrayType` e `wsdl:arrayType` referências, que ainda não são compatíveis em [!UICONTROL Workfront Fusion].

## Solução alternativa

Se a variável [!UICONTROL SOAP] o módulo se recusa a processar o arquivo WSDL ou lança vários erros na configuração do módulo, você pode tentar usar o **[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação]** em vez disso:

1. Em [!DNL Workfront Fusion], crie um novo cenário.
1. Insira o **[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação]** no cenário.
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
      <td> <p>[!UICONTROL bruto]</p> </td> [!UICONTROL ]
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de conteúdo]</td> 
      <td> <p>[!UICONTROL XML (aplicativo/xml)]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Analisar resposta]</td> 
      <td>[!UICONTROL Ativado]</td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/workaround-350x443.png)

1. Abra uma nova janela ou guia do navegador da Web.
1. Cole o URL WSDL na barra de endereços do navegador da Web e busque o arquivo XML.

   O URL WSDL geralmente termina com `?wsdl`, mas não necessariamente, por exemplo `http://voip.ms/api/v1/server.wsdl`.

1. Se o arquivo WSDL não for exibido diretamente no navegador da Web, abra o arquivo baixado em um editor de texto.
1. Procure a variável `<service>` ou `<wsdl:service>` tag:

   ![](assets/service-350x65.png)

1. Depois de localizada, copie o URL do `location` atributo.
1. Em [!DNL Workfront Fusion], cole o URL no campo URL do módulo HTTP.
1. Abra o [Online [!UICONTROL SOAP] Cliente](https://wsdlbrowser.com/) em uma nova janela/guia do navegador da Web.
1. Cole o URL WSDL no campo URL WSDL.
1. Clique em **[!UICONTROL Procurar]**.
1. Escolha na lista de funções à esquerda, por exemplo `getLanguages`.
1. Copie o conteúdo da [!UICONTROL Solicitar XML] área de texto.
1. Em [!UICONTROL Workfront Fusion], cole o conteúdo copiado no campo URL do módulo.
1. Forneça valores para os parâmetros selecionados ao substituir os pontos de interrogação por valores reais:

   ![](assets/request-xml-350x172.png)

1. Feche a configuração do módulo clicando em **[!UICONTROL OK]**.
1. Execute o cenário ou módulo.
