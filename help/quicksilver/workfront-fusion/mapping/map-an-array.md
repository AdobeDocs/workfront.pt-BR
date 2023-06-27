---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mapear uma matriz no [!DNL Adobe] Workfront Fusion
description: Você pode mapear uma matriz para um campo de módulo no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Mapear uma matriz no [!DNL Adobe Workfront Fusion]

Uma matriz é um tipo especial de item que pode conter o seguinte:

* Um ou mais valores de texto (matriz simples)
* Uma ou mais coleções do mesmo tipo (matriz complexa)

>[!INFO]
>
>**Exemplo:** A variável [!UICONTROL Assistir a emails] O módulo retorna uma matriz de anexos para cada email. Cada anexo representa uma coleção que pode conter um nome, conteúdo, tamanho e assim por diante.

Para obter mais informações, consulte [Tipos de dados de item no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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

## Mapear uma matriz

1. Clique no botão localizado no campo de destino.

   >[!INFO]
   >
   >  **Exemplo:** Para o exemplo acima, você clicaria em [!UICONTROL Adicionar um anexo] para um email.
   >
   >![](assets/add-an-attachment-button-350x152.jpg)

1. Na caixa exibida, insira o item.

   O painel permite mapear campos da mesma forma que com qualquer outro tipo de item. Se não quiser preencher cada item separadamente, mas quiser mapear outra matriz no campo de destino, use o [!UICONTROL Mapa] botão. Nesse caso, verifique se ambos os storages (o storage de origem e o storage de destino) têm a mesma estrutura.

   Você pode adicionar qualquer número de itens a uma matriz.

É possível dividir uma matriz em pacotes individuais usando um iterador. Para obter mais informações, consulte [[!UICONTROL Iterador] módulo no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
