---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mapear uma matriz em [!DNL Adobe] Workfront Fusion
description: Você pode mapear uma matriz para um campo de módulo no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Mapear uma matriz em [!DNL Adobe Workfront Fusion]

Uma matriz é um tipo especial de item que pode conter o seguinte:

* Um ou mais valores de texto (matriz simples)
* Uma ou mais coleções do mesmo tipo (matriz complexa)

>[!INFO]
>
>**Exemplo:** O [!UICONTROL Assistir a emails] retorna uma matriz de anexos para cada email. Cada anexo representa uma coleção que pode conter um nome, conteúdo, tamanho e assim por diante.

Para obter mais informações, consulte [Tipos de dados de item em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## Mapear uma matriz

1. Clique no botão localizado no campo target.

   >[!INFO]
   >
   >  **Exemplo:** No exemplo acima, você clicaria no botão [!UICONTROL Adicionar um anexo] para um email.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Na caixa exibida, digite o item.

   O painel permite mapear campos da mesma forma que com qualquer outro tipo de item. Se você não quiser preencher cada item separadamente, mas quiser mapear outra matriz para o campo de destino, use o [!UICONTROL Mapa] botão. Nesse caso, verifique se ambas as matrizes (a matriz de origem e a matriz de destino) têm a mesma estrutura.

   Você pode adicionar qualquer número de itens a uma matriz.

Você pode dividir um array em pacotes individuais usando um iterador. Para obter mais informações, consulte [[!UICONTROL Iterador] módulo em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
