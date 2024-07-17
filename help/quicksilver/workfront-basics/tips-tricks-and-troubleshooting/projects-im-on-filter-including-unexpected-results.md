---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtro Projetos em que estou trabalhando, incluindo resultados inesperados
description: Leia este artigo para solucionar problemas do filtro Projetos em que estou trabalhando, incluindo resultados inesperados.
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# O filtro Projetos em que estou trabalhando inclui resultados inesperados

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>licença do Adobe [!DNL Workfront]</strong></td> 
   <td> <p>[!UICONTROL Plano] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Administrador do sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

O filtro [!UICONTROL **Projetos em que estou**] inclui resultados que eu não esperaria, pois não estou atribuído ou associado a esses projetos.

## Solução

O filtro [!UICONTROL **Projetos em que estou**] inclui projetos que contêm o usuário em qualquer um de seus campos [!UICONTROL **Detalhes do Projeto**], incluindo campos que podem ser perdidos facilmente ou que são preenchidos automaticamente, como [!UICONTROL **Informado por**] ou [!UICONTROL **ID do Patrocinador**]. Para remover resultados indesejados, há duas soluções possíveis:

1. Verifique os [!UICONTROL **Detalhes do Projeto**] para cada projeto inesperado incluído pelo filtro e remova seu nome de todos os campos.

   OU

1. Tente usar um filtro semelhante, como [!UICONTROL **Projetos dos quais sou proprietário**], que inclui apenas projetos que são atribuídos especificamente a você.

Para obter mais informações sobre o uso de filtros no [!DNL Workfront], consulte [Visão Geral de Filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
