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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---

# [!UICONTROL SOAP] módulo

Você pode usar o [!UICONTROL SOAP] módulo ao qual se conectar [!UICONTROL SOAP] APIs em [!UICONTROL Adobe Workfront Fusion].

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

## Usar o [!UICONTROL SOAP] módulo

A variável [!UICONTROL SOAP] no momento, o módulo está na versão beta e não oferece suporte a:

* Redefinir elementos
* Restrições de dígitos de fração
* Restrições de dígitos totais
* Restrições de espaço em branco
* Várias partes nas mensagens de entrada e saída. Somente mensagens de parte única são suportadas
* Elementos personalizados do esquema XML definidos com a ajuda de [[!UICONTROL SOAP] Codificação](http://schemas.xmlsoap.org) esquemas e elementos.

>[!INFO]
>
>**Exemplo:**
>  
>Os seguintes itens não seriam reconhecidos corretamente pelo [!UICONTROL Workfront Fusion]:
>
>```
><complexType name="ArrayOfFloat">
>
>   
  <complexContent>
>
>      
     <restriction base="soapenc:Array">
>
>         
        <attribute ref="soapenc:arrayType"
>
>            
           wsdl:arrayType="xsd:integer[]"/>
>
>      
     </restriction>
>
>   
  </complexContent>
>
>
</complexType>
>```

Inclui a `soapenc:Array`, `soapenc:arrayType` e `wsdl:arrayType` referências, que ainda não são compatíveis com o [!UICONTROL Workfront Fusion].

## Solução alternativa

Se a variável [!UICONTROL SOAP] módulo se recusa a processar o arquivo WSDL ou lança vários erros na configuração do módulo, você pode tentar usar o universal **[!UICONTROL HTTP] > [!UICONTROL Fazer uma solicitação]** módulo em vez disso:

1. Entrada [!DNL Workfront Fusion], crie um novo cenário.
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

   O URL WSDL geralmente termina com `?wsdl`, mas não necessariamente, por exemplo `http://voip.ms/api/v1/server.wsdl`.

1. Se o arquivo WSDL não for exibido diretamente no navegador da Web, abra o arquivo baixado em um editor de texto.
1. Procure por `<service>` ou `<wsdl:service>` tag:

   ![](assets/service-350x65.png)

1. Depois de localizado, copie o URL do `location` atributo.
1. Entrada [!DNL Workfront Fusion], cole o URL no campo URL do módulo HTTP.
1. Abra o [Online [!UICONTROL SOAP] Cliente](https://wsdlbrowser.com/) em uma nova janela/guia do navegador da web.
1. Cole o URL do WSDL no campo URL do WSDL.
1. Clique em **[!UICONTROL Procurar]**.
1. Selecione na lista de funções à esquerda, por exemplo `getLanguages`.
1. Copie o conteúdo do [!UICONTROL XML de solicitação] área de texto.
1. Entrada [!UICONTROL Workfront Fusion], cole o conteúdo copiado no campo URL do módulo.
1. Forneça valores para os parâmetros selecionados substituindo os pontos de interrogação pelos valores reais:

   ![](assets/request-xml-350x172.png)

1. Feche a configuração do módulo clicando em **[!UICONTROL OK]**.
1. Execute o cenário ou módulo.
