---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtro Projetos em que estou trabalhando, incluindo resultados inesperados
description: Leia este artigo para solucionar problemas do filtro Projetos em que estou trabalhando, incluindo resultados inesperados.
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 3%

---

# O filtro Projetos em que estou trabalhando inclui resultados inesperados

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table>
  <tr>
   <td>Pacote do Adobe Workfront
   </td>
   <td> <p>Prime ou Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
  <tr>
   <td>Licenças do Adobe Workfront
   </td>
   <td><p>Standard</p>
   <p>Plano</p>
   </td>
  </tr>
   <tr>
   <td>Configurações de nível de acesso
   </td>
   <td>Você deve ser um administrador [!DNL Workfront].
   </td>
  </tr>
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Problema

O filtro [!UICONTROL **Projetos em que estou**] inclui resultados que eu não esperaria, pois não estou atribuído ou associado a esses projetos.

## Solução

O filtro [!UICONTROL **Projetos em que estou**] inclui projetos que contêm o usuário em qualquer um de seus campos [!UICONTROL **Detalhes do Projeto**], incluindo campos que podem ser perdidos facilmente ou que são preenchidos automaticamente, como [!UICONTROL **Informado por**] ou [!UICONTROL **ID do Patrocinador**]. Para remover resultados indesejados, há duas soluções possíveis:

1. Verifique os [!UICONTROL **Detalhes do Projeto**] para cada projeto inesperado incluído pelo filtro e remova seu nome de todos os campos.

   OR

1. Tente usar um filtro semelhante, como [!UICONTROL **Projetos dos quais sou proprietário**], que inclui apenas projetos que são atribuídos especificamente a você.

Para obter mais informações sobre o uso de filtros no [!DNL Workfront], consulte [Visão Geral de Filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
