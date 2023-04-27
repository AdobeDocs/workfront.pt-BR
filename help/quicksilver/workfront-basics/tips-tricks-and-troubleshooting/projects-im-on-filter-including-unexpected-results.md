---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtro Projetos que estou ativado , incluindo resultados inesperados
description: Leia este artigo para solucionar problemas no filtro Projetos em que estou, incluindo resultados inesperados.
feature: Get Started with Workfront
author: Nolan
source-git-commit: ba261e5121b4a28f71c58f883c784f4e8d2ada81
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 1%

---

# O filtro Projetos em que estou inclui resultados inesperados

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] licença</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Administrador do sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

O [!UICONTROL **Projetos em que estou**] O filtro inclui resultados que eu não esperaria, pois não estou atribuído ou associado a esses projetos.

## Solução

O [!UICONTROL **Projetos em que estou**] O filtro inclui projetos que contêm o usuário em qualquer um de seus [!UICONTROL **Detalhes do projeto**] campos, incluindo campos facilmente perdidos ou automaticamente preenchidos, como [!UICONTROL **Inserido por**] ou [!UICONTROL **ID do Patrocinador**]. Para remover resultados indesejados, há duas soluções possíveis:

1. Verifique a [!UICONTROL **Detalhes do projeto**] para cada projeto inesperado incluído pelo filtro e remova seu nome de todos os campos.

   OU

1. Tente usar um filtro semelhante, como [!UICONTROL **Projetos que possuo**], que inclui apenas projetos que são especificamente atribuídos a você.

Para obter mais informações sobre o uso de filtros em [!DNL Workfront], consulte [Visão geral dos filtros em [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)