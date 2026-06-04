---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Filtro Projetos em que estou trabalhando, incluindo resultados inesperados
description: Leia este artigo para solucionar problemas do filtro Projetos em que estou trabalhando, incluindo resultados inesperados.
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
TQID: https://experienceleague.adobe.com/xE5RW947MUFg5d2X6ikKhHSftQDUMxDJlC05un0oDH0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 23%

---

# O filtro “Projetos em que estou envolvido” inclui resultados inesperados

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table>
  <tr>
   <td>Pacote do Adobe Workfront
   </td>
   <td>Qualquer</td>
  </tr>
  <tr>
   <td>Licenças do Adobe Workfront
   </td>
   <td><p>Padrão</p>
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
