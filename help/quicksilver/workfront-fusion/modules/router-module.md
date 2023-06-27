---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo de roteador no Adobe Workfront Fusion
description: O módulo de Roteador permite ramificar seu fluxo em várias rotas e processar os dados em cada rota de forma diferente. Depois que um módulo de roteador recebe um pacote, ele o encaminha para cada rota conectada na ordem em que as rotas foram anexadas ao módulo de roteador.
author: Becky
feature: Workfront Fusion
exl-id: 3c39c562-1cee-4f8e-89cc-0ed554079a2b
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 0%

---

# [!UICONTROL Roteador] módulo no [!DNL Adobe Workfront Fusion]

A variável [!UICONTROL Roteador] permite ramificar seu fluxo em várias rotas e processar os dados dentro de cada rota de forma diferente. Uma vez a [!UICONTROL Roteador] recebe um pacote, ele o encaminha para cada rota conectada na ordem em que as rotas foram anexadas ao [!UICONTROL Roteador] módulo.

>[!NOTE]
>
>* Para verificar a ordem das rotas, clique no link [!UICONTROL Alinhamento automático] ícone, que organizará as rotas de acordo com a ordem de cima para baixo.
>
>  Para alterar a ordem, remova a variável [!UICONTROL Roteador] e reconecte as rotas na ordem desejada.
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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
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

## Adicionar um [!UICONTROL Roteador] módulo para um cenário

A [!UICONTROL Roteador] pode ser adicionado a um cenário de uma das seguintes maneiras:

* Se quiser conectar o [!UICONTROL Roteador] após um módulo, clique na alça direita do módulo e comece a digitar **[!UICONTROL roteador]** para pesquisá-la, escolha **[!UICONTROL Controle de fluxo]** > **[!UICONTROL Roteador]** na lista de módulos que é exibida.

  ![](assets/connect-the-router-350x108.png)

* Se desejar inserir o [!UICONTROL Roteador] módulo entre dois módulos, clique no ícone de chave inglesa abaixo da rota que conecta os dois módulos (ou clique com o botão direito do mouse na rota) e escolha **[!UICONTROL Adicionar um roteador]** no menu.

  ![](assets/insert-router-350x191.png)

* É possível inserir um [!UICONTROL Roteador] automaticamente. Por exemplo, na imagem abaixo, para conectar o módulo no canto inferior direito ao do canto superior esquerdo (que já está conectado ao do canto superior direito), arraste a alça esquerda do módulo inferior direito e solte-a no módulo superior esquerdo.

  ![](assets/insert-router-automatically-350x379.png)

## Filtros

Você pode colocar um filtro em uma rota após a variável [!UICONTROL Roteador] módulo para filtrar pacotes como em qualquer outra rota:

1. Clique em um dos pontos na rota.

   ![](assets/router-click-a-dot-in-route-350x339.png)

1. No **[!UICONTROL Configurar um filtro]** que é exibida, adicione condições e clique em **[!UICONTROL OK]** para salvar a configuração do filtro.

   ![](assets/set-up-a-filter-2-350x242.png)

Para obter mais informações, consulte [Adicionar um filtro a um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

## A rota de fallback

A configuração de filtro em um roteiro depois de um [!UICONTROL Roteador] O módulo contém uma opção especial: a rota de fallback:

![](assets/fallback-route-350x260.png)

Quando habilitada, essa rota é usada quando um pacote não pode continuar do estado [!UICONTROL Roteador] via qualquer outra rota porque os filtros nas outras rotas a filtravam.

A rota de Fallback é diferenciada por um sinal de seta diferente dentro do [!UICONTROL Roteador] módulo:

![](assets/arrow-sign-in-router-module-350x361.png)

## If/Else

Um caso de uso típico da rota de fallback é continuar o fluxo com uma rota se a condição for atendida e com outra rota se não for, como nos seguintes passos:

1. Inserir um [!UICONTROL Roteador] em seu cenário.
1. Conecte ambas as rotas à [!UICONTROL Roteador] módulo .
1. Clique na primeira rota e especifique uma condição:

   ![](assets/set-up-a-filter-2-350x242.png)

1. Clique na segunda rota e habilite a opção [!UICONTROL rota de fallback] opção:

   ![](assets/enable-fallback-route-option-350x238.png)
