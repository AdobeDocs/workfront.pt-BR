---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Estruturas de dados no [!DNL Adobe Workfront Fusion]
description: Uma estrutura de dados é um documento que descreve em detalhes o formato dos dados que estão sendo transferidos para o Adobe Workfront Fusion. Com base nesse documento, o editor de cenários pode descobrir qual módulo retorna ou recebe qual tipo de dados. Os documentos de estrutura de dados são usados com mais frequência para serializar/analisar formatos de dados, como JSON, XML, CSV e outros.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Estruturas de dados no [!DNL Adobe Workfront Fusion]

Uma estrutura de dados é um documento que descreve em detalhes o formato dos dados que estão sendo transferidos para o [!DNL Adobe Workfront Fusion]. Com base nesse documento, o editor de cenários pode descobrir qual módulo retorna ou recebe qual tipo de dados. Os documentos de estrutura de dados são usados com mais frequência para serializar/analisar formatos de dados, como JSON, XML, CSV e outros.

Você pode criar uma estrutura de dados clicando no ícone [!UICONTROL Criar uma nova estrutura de dados] botão na caixa [!UICONTROL Visão geral da estrutura de dados] ou nas configurações do módulo que requer especificação de estrutura de dados.

Os tipos de dados compatíveis estão descritos no [[!UICONTROL Tipos de módulos]](../../workfront-fusion/modules/module-types.md) artigo.

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

## Gerador de estrutura de dados

Nem sempre as estruturas de dados precisam ser criadas. Você pode tornar mais fácil usando um modelo do nosso gerador integrado. Ao fornecer uma amostra de dados, o gerador criará automaticamente uma estrutura de dados com base na amostra de dados inserida. A estrutura de dados criada pode ser modificada manualmente.

![](assets/data-structure-generator-350x341.jpg)
