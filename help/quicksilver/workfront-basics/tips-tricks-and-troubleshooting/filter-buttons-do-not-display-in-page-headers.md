---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Os botões de filtro não são exibidos nos cabeçalhos da página
description: Leia este artigo para solucionar problemas de botões de filtro que não são exibidos nos cabeçalhos da página.
feature: Get Started with Workfront
author: Lisa and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# Os botões de filtro não são exibidos nos cabeçalhos da página

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

Os seguintes botões de filtro não são exibidos em suas respectivas áreas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] area</strong></td> 
   <td><strong>Botões Filtrar</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projetos] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos que estou ativo]</p> </li> 
     <li> <p>[!UICONTROL Projetos possuo]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Folhas de data e hora]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Minhas aprovações de folha de ponto]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Minhas Folhas de Horas]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

Os botões de filtro na [!UICONTROL Projetos e Folhas de Horas] não são exibidos porque os filtros correspondentes não estão incluídos no modelo de layout aplicado ao usuário. O [!DNL Workfront] o administrador deve atribuir um modelo de layout que inclua os filtros.

>[!NOTE]
>
>Às vezes, os filtros são removidos do [!UICONTROL Controles de lista] área em [!UICONTROL Configuração]. O [!DNL Workfront] o administrador deve incluí-los nas listas nesta área para que estejam disponíveis nos templates de layout.

1. Verifique se o modelo de layout exibe os seguintes filtros:

   * [!UICONTROL Projetos em que estou] e [!UICONTROL Projetos que possuo] no [!UICONTROL Projetos] area
   * [!UICONTROL Minhas aprovações de folha de ponto] e [!UICONTROL Minhas Folhas de Horas] no [!UICONTROL Folha de Horas] area

   Para fazer isso:

   1. Acesse o modelo de layout.
   1. Selecionar **[!UICONTROL Listas]** under **[!UICONTROL Personalize o que os usuários veem]**.
   1. Selecionar **[!UICONTROL Projetos]** ou **[!UICONTROL Folhas de Horas]** under **[!UICONTROL Selecione uma lista para personalizar]**.
   1. No **[!UICONTROL Filtro]** verifique se **[!UICONTROL Projetos em que estou]**, **[!UICONTROL Projetos que possuo]** (para projetos) e **[!UICONTROL Minhas aprovações de folha de ponto]** e **[!UICONTROL Minhas Folhas de Horas]** (para folhas de horas) são selecionadas.
   1. Clique em **[!UICONTROL Salvar]**.

   Para obter mais informações, consulte [Personalizar filtros, exibições e agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Atribua o modelo de layout aos usuários, funções, equipes ou grupos corretos. Para obter mais informações, consulte [Atribuir usuários a um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
