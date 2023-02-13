---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo de roteador no Adobe Workfront Fusion
description: O módulo Roteador permite ramificar seu fluxo para várias rotas e processar os dados em cada rota de forma diferente. Quando um módulo de Roteador recebe um pacote, ele o encaminha para cada rota conectada na ordem em que as rotas foram anexadas ao módulo de Roteador.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# [!UICONTROL Roteador] módulo em [!DNL Adobe Workfront Fusion]

O [!UICONTROL Roteador] permite ramificar seu fluxo em várias rotas e processar os dados em cada rota de forma diferente. Uma vez [!UICONTROL Roteador] O módulo recebe um pacote, ele o encaminha para cada rota conectada na ordem em que as rotas foram anexadas ao [!UICONTROL Roteador] módulo.

>[!NOTE]
>
>* Para verificar a ordem das rotas, clique no botão [!UICONTROL Alinhamento automático] ícone , que organizará as rotas de acordo com a ordem de cima para baixo.
>
>  Para alterar o pedido, remova o [!UICONTROL Roteador] e reconecte as rotas na ordem desejada.
>
>* As rotas são processadas sequencialmente, não em paralelo. Um pacote não é enviado para a próxima rota até que tenha sido completamente processado pela rota anterior.
>




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
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Adicionar um [!UICONTROL Roteador] para um cenário

A [!UICONTROL Roteador] pode ser adicionado a um cenário de uma das seguintes maneiras:

* Se quiser conectar o [!UICONTROL Roteador] depois de um módulo, clique na alça direita do módulo, comece a digitar **[!UICONTROL roteador]** para pesquisá-lo, escolha **[!UICONTROL Controle de fluxo]** > **[!UICONTROL Roteador]** na lista de módulos que é exibida.

   ![](assets/connect-the-router-350x108.png)

* Se quiser inserir o [!UICONTROL Roteador] entre dois módulos, clique no ícone da chave de fenda abaixo da rota que conecta os dois módulos (ou clique com o botão direito do mouse na rota) e escolha **[!UICONTROL Adicionar um roteador]** no menu .

   ![](assets/insert-router-350x191.png)

* Você pode inserir um [!UICONTROL Roteador] automaticamente. Por exemplo, na imagem abaixo, para conectar o módulo no canto inferior direito ao módulo no canto superior esquerdo (que já está conectado ao módulo no canto superior direito), arraste a alça esquerda do módulo inferior direito e solte-o no módulo superior esquerdo.

   ![](assets/insert-router-automatically-350x379.png)

## Filtros

Você pode colocar um filtro em uma rota após a variável [!UICONTROL Roteador] módulo para filtrar pacotes como em qualquer outra rota:

1. Clique em um dos pontos na rota.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. No **[!UICONTROL Configurar um filtro]** caixa que é exibida, adicione condições e clique em **[!UICONTROL OK]** para salvar a configuração do filtro.

   ![](assets/set-up-a-filter-2-350x242.png)

Para obter mais informações, consulte [Adicione um filtro a um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## A rota de fallback

A configuração do filtro em uma rota após um [!UICONTROL Roteador] O módulo contém uma opção especial: A rota de fallback:

![](assets/fallback-route-350x260.png)

Quando ativado, essa rota é usada no caso em que um pacote não pode continuar a partir do [!UICONTROL Roteador] módulo via qualquer outra rota porque os filtros nas outras rotas o filtraram.

A rota de fallback é diferenciada por um sinal de seta diferente dentro da [!UICONTROL Roteador] módulo:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Um caso de uso típico da rota de fallback é continuar o fluxo com uma rota se a condição for atendida e com outra rota, se não for, como nas etapas a seguir:

1. Insira um [!UICONTROL Roteador] em seu cenário.
1. Conecte ambas as rotas ao [!UICONTROL Roteador] módulo .
1. Clique na primeira rota e especifique uma condição:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Clique na segunda rota e habilite o [!UICONTROL rota de fallback] opção:

   ![](assets/enable-fallback-route-option-350x238.png)
