---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo Iterador no Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Módulo [!UICONTROL Iterador] em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Módulo Iterador](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/iterator-module.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Um módulo [!UICONTROL Iterador] é um tipo especial de módulo que converte uma matriz em uma série de conjuntos. Cada item de matriz é emitido como um pacote separado.

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
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
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

## Configuração do módulo [!UICONTROL Iterador]

Você configurou um módulo [!UICONTROL Iterador] da mesma forma que configurou qualquer outro módulo. O campo [!UICONTROL Matriz] contém a matriz a ser convertida ou dividida em conjuntos separados.

![](assets/set-up-iterator-350x190.jpg)

Para obter mais informações, consulte [Definir as configurações de um módulo no Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Exemplos:**
>
>* O cenário abaixo mostra como recuperar emails com anexos e salvar os anexos como arquivos únicos em uma pasta [!DNL Dropbox] selecionada.
>
>   Os e-mails podem conter uma matriz de anexos. O módulo [!UICONTROL Iterador] inserido após o primeiro módulo permitirá que você manipule cada anexo separadamente. O módulo [!UICONTROL Iterador] divide a matriz de anexos em conjuntos únicos. Cada pacote, com um anexo, é salvo um de cada vez em uma pasta [!DNL Dropbox] selecionada. A configuração do módulo [!UICONTROL Iterador] é mostrada acima: o campo [!UICONTROL Matriz] deve conter a matriz `Attachments`.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* Para sua conveniência, muitos aplicativos [!DNL Workfront Fusion] oferecem módulos [!UICONTROL Iterador] especializados com uma configuração simplificada. Por exemplo, o aplicativo [!UICONTROL Email] contém o módulo [!UICONTROL Iterador] especial [!UICONTROL Email] > [!UICONTROL Iterar anexos] que produzirá os mesmos resultados que o módulo [!UICONTROL Iterador] geral.
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Solução de problemas: o painel Mapeamento não exibe itens mapeáveis no módulo [!UICONTROL Iterador]

Quando um módulo [!UICONTROL Iterador] não tem informações sobre a estrutura dos itens da matriz, o painel de mapeamento nos módulos após o módulo [!UICONTROL Iterador] exibe apenas 2 itens sob o módulo [!UICONTROL Iterador]: `Total number of bundles` e `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Isso ocorre porque cada módulo é responsável por fornecer informações sobre os itens gerados para que esses itens possam ser exibidos corretamente no painel de mapeamento nos módulos subsequentes. No entanto, vários módulos podem não ser capazes de fornecer essas informações em alguns casos; por exemplo, [!UICONTROL JSON] > [!UICONTROL Parse JSON] ou [!UICONTROL Webhooks] > [!UICONTROL Webhook personalizado] módulos com estrutura de dados ausente.

A solução é executar manualmente o cenário para que o módulo aprenda sobre os itens gerados, de modo que possa fornecer as informações aos seguintes módulos.

Por exemplo, se você tiver um módulo [!UICONTROL JSON] > [!UICONTROL Parse JSON] sem uma estrutura de Dados como abaixo:

![](assets/json-parse-json-350x285.png)

Se você conectar um módulo [!UICONTROL Iterador] a ele, não será possível mapear a saída do módulo para o campo Matriz no painel de configuração do módulo [!UICONTROL Iterador]:

![](assets/connect-iterator-module-350x146.png)

Para resolver isso, inicie manualmente o cenário no editor de cenários. Você pode desvincular os módulos após o módulo [!UICONTROL JSON] > [!UICONTROL Parse JSON] para impedir que o fluxo continue. Ou você pode clicar com o botão direito do mouse no módulo [!UICONTROL JSON] > [!UICONTROL Analisar JSON] e escolher **[!UICONTROL Executar somente este módulo]** no menu de contexto para executar somente o módulo [!UICONTROL JSON] > [!UICONTROL Analisar JSON].

Quando o [!UICONTROL JSON] > [!UICONTROL Parse JSON] é executado, ele aprende sobre os itens gerados e fornece essas informações a todos os módulos subsequentes, incluindo o módulo Iterador. O painel de mapeamento na configuração do Iterador exibe os itens:

![](assets/mapping-panel-displays-items-350x131.png)

Além disso, o painel de mapeamento nos módulos conectados após o módulo [!UICONTROL Iterador] exibe os itens contidos nos itens da matriz:

![](assets/items-contained-in-array-350x156.png)

Se não conseguir ver alguns itens no painel de mapeamento de um módulo, execute o cenário uma vez para que todos os módulos possam aprender sobre os itens gerados e fornecer essas informações aos módulos a seguir.
