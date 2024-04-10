---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Formato de domínio para chamadas de API do Adobe Workfront
description: Localize seu domínio para usar na API do Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---

# Formato de domínio para chamadas de API do Adobe Workfront

Ao fazer uma chamada de API para a API do Workfront, você usa o domínio de sua organização na chamada. O formato desse URL de domínio difere com base no fato de sua organização ter sido integrada ao Adobe Unified Shell.

Para saber se sua organização está no Adobe Unified Shell, examine o URL que é exibido quando você está visualizando uma página do Workfront.

| O URL do Workfront começa com: | URL para chamadas de API: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

Para localizar seu domínio:

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Configuração]** ![Ícone de Configuração](/help/_includes/assets/gear-icon-setup.png).
1. Selecionar **Sistema** e selecione **Informações do cliente**.

   Seu domínio está listado à direita da tela.

   ![Domínio](assets/domain.png)

