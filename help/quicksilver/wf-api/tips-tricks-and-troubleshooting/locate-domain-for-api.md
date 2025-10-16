---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Formato de domínio para chamadas de API do Adobe Workfront
description: Localize seu domínio para usar na API do Adobe Workfront
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: e9a9e45720c8b9ad25e3fa9340c813a73989fb4a
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 1%

---

# Formato de domínio para chamadas de API do Adobe Workfront

Ao fazer uma chamada de API para a API do Workfront, você usa o domínio de sua organização na chamada. O formato desse URL de domínio difere com base no fato de sua organização ter sido integrada ao Adobe Unified Shell.

Para saber se sua organização está no Adobe Unified Shell, examine o URL que é exibido quando você está visualizando uma página do Workfront.

| O URL do Workfront começa com: | URL para chamadas de API: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Para localizar seu domínio:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique no ícone **[!UICONTROL Instalação]** ![Instalação](/help/_includes/assets/gear-icon-setup.png).
1. Selecione **Sistema** e, em seguida, **Informações do cliente**.

   Seu domínio está listado à direita da tela.

   ![Domínio](assets/domain.png)

