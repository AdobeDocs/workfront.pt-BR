---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo iterador no Adobe Workfront Fusion
description: Um módulo Iterator é um tipo especial de módulo que converte uma matriz em uma série de pacotes. Cada item de matriz é enviado como um pacote separado.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: a2060e7179f2295bfd42da84bd7bca9862ad0a17
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!UICONTROL Iterador] módulo em [!DNL Adobe Workfront Fusion]

Um [!UICONTROL Iterador] é um tipo especial de módulo que converte uma matriz em uma série de pacotes. Cada item de matriz é enviado como um pacote separado.

Para obter mais informações, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md) e [Mapear uma matriz no Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar o Adobe Workfront Fusion e a Adobe Workfront para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iterador] configuração do módulo

Você configura um [!UICONTROL Iterador] do mesmo modo que você configura qualquer outro módulo. O [!UICONTROL Matriz] contém a matriz a ser convertida ou dividida em pacotes separados.

![](assets/set-up-iterator-350x190.jpg)

Para obter mais informações, consulte [Definir as configurações de um módulo no Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Exemplos:**
>
>* O cenário abaixo mostra como recuperar emails com anexos e salvar os anexos como arquivos únicos em um arquivo selecionado [!DNL Dropbox] pasta.
   >
   >   Os emails podem conter uma matriz de anexos. O [!UICONTROL Iterador] módulo inserido após o primeiro módulo permitirá manipular cada anexo separadamente. O [!UICONTROL Iterador] divide a matriz de anexos em pacotes únicos. Cada pacote, com um anexo, é salvo um de cada vez em um [!DNL Dropbox] pasta. O [!UICONTROL Iterador] a configuração do módulo é mostrada acima: o [!UICONTROL Matriz] O campo deve conter a variável `Attachments` matriz.
   >
   >   ![](assets/attachments-array-350x154.jpg)
>
>* Para sua conveniência, muitos [!DNL Workfront Fusion] oferta de aplicativos especializada [!UICONTROL Iterador] módulos com uma configuração simplificada. Por exemplo, a variável [!UICONTROL Email] o aplicativo contém o especial [!UICONTROL Iterador] módulo [!UICONTROL Email] > [!UICONTROL Iterar anexos] que produzirá os mesmos resultados que o [!UICONTROL Iterador] módulo.
   >
   >   ![](assets/specialized-iterators-350x135.jpg)



## Solução de problemas: O painel Mapeamento não exibe itens mapeáveis em [!UICONTROL Iterador] módulo

Quando uma [!UICONTROL Iterador] não tem informações sobre a estrutura dos itens da matriz, o painel de mapeamento nos módulos que seguem o [!UICONTROL Iterador] o módulo exibe somente 2 itens sob a [!UICONTROL Iterador] módulo :`Total number of bundles` e `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Isso porque cada módulo é responsável por fornecer informações sobre os itens gerados para que esses itens possam ser exibidos corretamente no painel de mapeamento nos módulos subsequentes. No entanto, alguns módulos poderão não ser capazes de fornecer essas informações em alguns casos; por exemplo, [!UICONTROL JSON] > [!UICONTROL Analisar JSON] ou [!UICONTROL Webhooks] > [!UICONTROL Webhook personalizado] módulos com estrutura de dados ausente.

A solução é executar manualmente o cenário para fazer com que o módulo saiba mais sobre os itens gerados para que possa fornecer as informações aos módulos a seguir.

Por exemplo, se você tiver uma [!UICONTROL JSON] > [!UICONTROL Analisar JSON] sem uma estrutura de dados, como abaixo:

![](assets/json-parse-json-350x285.png)

E então se você conectar um [!UICONTROL Iterador] não será possível mapear a saída do módulo para o campo Array no painel de configuração do [!UICONTROL Iterador] módulo :

![](assets/connect-iterator-module-350x146.png)

Para resolver isso, inicie manualmente o cenário no editor de cenário. Você pode desvincular os módulos após a variável [!UICONTROL JSON] > [!UICONTROL Analisar JSON] para impedir que o fluxo continue. Ou você pode clicar com o botão direito do mouse no link [!UICONTROL JSON] > [!UICONTROL Analisar JSON] e escolha **[!UICONTROL Executar este módulo somente]** no menu de contexto para executar somente o [!UICONTROL JSON] > [!UICONTROL Analisar JSON] módulo.

Quando a variável [!UICONTROL JSON] > [!UICONTROL Analisar JSON] é executado, aprende sobre os itens gerados e fornece essas informações para todos os módulos subsequentes, incluindo o módulo Iterator. O painel de mapeamento na configuração do Iterador exibe os itens:

![](assets/mapping-panel-displays-items-350x131.png)

Além disso, o painel de mapeamento nos módulos que são conectados após a [!UICONTROL Iterador] O módulo exibe os itens contidos nos itens da matriz:

![](assets/items-contained-in-array-350x156.png)

Se não for possível ver alguns itens no painel de mapeamento de um módulo, execute o cenário uma vez para que todos os módulos possam aprender sobre os itens enviados e fornecer essas informações aos módulos a seguir.
