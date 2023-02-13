---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Estruturas de dados em [!DNL Adobe Workfront Fusion]
description: Uma estrutura de dados é um documento que descreve detalhadamente o formato dos dados que estão sendo transferidos para o Adobe Workfront Fusion. Com base nesse documento, o editor de cenário é capaz de descobrir qual módulo retorna ou recebe qual tipo de dados. Os documentos da estrutura de dados são usados com mais frequência para serializar/analisar formatos de dados, como JSON, XML, CSV e outros.
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Estruturas de dados em [!DNL Adobe Workfront Fusion]

Uma estrutura de dados é um documento que descreve detalhadamente o formato dos dados que estão sendo transferidos para [!DNL Adobe Workfront Fusion]. Com base nesse documento, o editor de cenário é capaz de descobrir qual módulo retorna ou recebe qual tipo de dados. Os documentos da estrutura de dados são usados com mais frequência para serializar/analisar formatos de dados, como JSON, XML, CSV e outros.

Você pode criar uma estrutura de dados clicando no botão [!UICONTROL Criar uma nova estrutura de dados] no botão [!UICONTROL Visão geral da estrutura de dados] ou nas configurações do módulo que requer especificação de estrutura de dados.

Os tipos de dados compatíveis são descritos na seção [[!UICONTROL Tipos de módulos]](../../workfront-fusion/modules/module-types.md) artigo 10. o

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

## Gerador de estrutura de dados

As estruturas de dados nem sempre precisam ser criadas. Você pode facilitar usando um modelo do nosso gerador incorporado. Ao fornecer uma amostra de dados, o gerador criará automaticamente uma estrutura de dados com base na amostra de dados inserida. A estrutura de dados criada pode ser modificada manualmente.

![](assets/data-structure-generator-350x341.jpg)
