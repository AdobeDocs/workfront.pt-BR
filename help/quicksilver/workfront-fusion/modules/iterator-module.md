---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo Iterador no Adobe Workfront Fusion
description: Um módulo Iterador é um tipo especial de módulo que converte uma matriz em uma série de pacotes. Cada item de matriz é emitido como um pacote separado.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 0%

---

# [!UICONTROL Iterador] módulo no [!DNL Adobe Workfront Fusion]

Um [!UICONTROL Iterador] módulo é um tipo especial de módulo que converte uma matriz em uma série de pacotes. Cada item de matriz é emitido como um pacote separado.

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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar o Adobe Workfront Fusion e o Adobe Workfront para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Iterador] configuração do módulo

Você configurou um [!UICONTROL Iterador] o mesmo que você configurou qualquer outro módulo. A variável [!UICONTROL Matriz] o campo contém a matriz a ser convertida ou dividida em pacotes separados.

![](assets/set-up-iterator-350x190.jpg)

Para obter mais informações, consulte [Definir as configurações de um módulo no Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Exemplos:**
>
>* O cenário abaixo mostra como recuperar emails com anexos e salvar os anexos como arquivos únicos em um [!DNL Dropbox] pasta.
>
>   Os e-mails podem conter uma matriz de anexos. A variável [!UICONTROL Iterador] módulo inserido após o primeiro módulo permitirá que você lide com cada anexo separadamente. A variável [!UICONTROL Iterador] O módulo divide a matriz de anexos em pacotes únicos. Cada pacote, com um anexo, é salvo um de cada vez em um [!DNL Dropbox] pasta. A variável [!UICONTROL Iterador] a configuração do módulo é mostrada acima: a variável [!UICONTROL Matriz] o campo deve conter a `Attachments` matriz.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Para sua conveniência, muitos [!DNL Workfront Fusion] aplicativos oferecem especializados [!UICONTROL Iterador] módulos com uma configuração simplificada. Por exemplo, a variável [!UICONTROL E-mail] O aplicativo contém o [!UICONTROL Iterador] módulo [!UICONTROL E-mail] > [!UICONTROL Iterar anexos] que produzirão os mesmos resultados que os [!UICONTROL Iterador] módulo.
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Solução de problemas: o painel Mapeamento não exibe itens mapeáveis em [!UICONTROL Iterador] módulo

Quando um [!UICONTROL Iterador] não possui informações sobre a estrutura dos itens da matriz, o painel de mapeamento nos módulos após o [!UICONTROL Iterador] o módulo exibe somente 2 itens sob a [!UICONTROL Iterador] módulo:`Total number of bundles` e `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Isso ocorre porque cada módulo é responsável por fornecer informações sobre os itens gerados para que esses itens possam ser exibidos corretamente no painel de mapeamento nos módulos subsequentes. No entanto, vários módulos podem não conseguir fornecer essas informações em alguns casos; por exemplo, [!UICONTROL JSON] > [!UICONTROL Analisar JSON] ou [!UICONTROL Webhooks] > [!UICONTROL Webhook personalizado] módulos com estrutura de dados ausente.

A solução é executar manualmente o cenário para que o módulo aprenda sobre os itens gerados, de modo que possa fornecer as informações aos seguintes módulos.

Por exemplo, se você tiver uma [!UICONTROL JSON] > [!UICONTROL Analisar JSON] módulo sem uma estrutura de dados como abaixo:

![](assets/json-parse-json-350x285.png)

E, em seguida, se você conectar um [!UICONTROL Iterador] para ele, você não poderá mapear a saída do módulo para o campo Array no painel de configuração do [!UICONTROL Iterador] módulo:

![](assets/connect-iterator-module-350x146.png)

Para resolver isso, inicie manualmente o cenário no editor de cenários. É possível desvincular os módulos após a variável [!UICONTROL JSON] > [!UICONTROL Analisar JSON] para impedir que o fluxo continue. Ou você pode clicar com o botão direito do mouse no [!UICONTROL JSON] > [!UICONTROL Analisar JSON] módulo e escolha **[!UICONTROL Executar este módulo somente]** no menu de contexto para executar somente as [!UICONTROL JSON] > [!UICONTROL Analisar JSON] módulo.

Quando a variável [!UICONTROL JSON] > [!UICONTROL Analisar JSON] O executa, aprende sobre os itens gerados e fornece essas informações a todos os módulos subsequentes, incluindo o módulo Iterador. O painel de mapeamento na configuração do Iterador exibe os itens:

![](assets/mapping-panel-displays-items-350x131.png)

Além disso, o painel de mapeamento nos módulos que são conectados após a [!UICONTROL Iterador] O módulo exibe os itens contidos nos itens da matriz:

![](assets/items-contained-in-array-350x156.png)

Se não conseguir ver alguns itens no painel de mapeamento de um módulo, execute o cenário uma vez para que todos os módulos possam aprender sobre os itens gerados e fornecer essas informações aos módulos a seguir.
