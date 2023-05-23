---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Os botões de filtro não são exibidos nos cabeçalhos da página
description: Leia este artigo para solucionar problemas de botões de filtro que não são exibidos nos cabeçalhos da página.
feature: Get Started with Workfront
author: Nolan and Alina
exl-id: 327564ed-60df-441a-a38b-a17a8c57adb0
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 1%

---

# Os botões de filtro não são exibidos nos cabeçalhos da página

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td> <p>[!UICONTROL Plano] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Administrador do sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problema

Os botões de filtro a seguir não são exibidos nas respectivas áreas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>[!DNL Adobe Workfront] área</strong></td> 
   <td><strong>Botões de filtro</strong></td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Projetos] </p> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Projetos em que estou]</p> </li> 
     <li> <p>[!UICONTROL Projetos dos quais sou proprietário]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><span>[!UICONTROL Planilha de Horas]</span> </td> 
   <td> 
    <ul> 
     <li> <p><span>[!UICONTROL Minhas planilhas de horas aprovadas]</span> </p> </li> 
     <li> <p><span>[!UICONTROL Minhas Planilhas de Horas]</span> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

Os botões de filtro no [!UICONTROL Projetos e planilha de horas] não são exibidos porque os filtros correspondentes não estão incluídos no modelo de layout aplicado ao usuário. A variável [!DNL Workfront] O administrador deve atribuir um modelo de layout que inclua os filtros.

>[!NOTE]
>
>Às vezes, os filtros são removidos da variável [!UICONTROL Controles de Lista] área em [!UICONTROL Configuração]. A variável [!DNL Workfront] o administrador precisa incluí-los nas listas desta área para que estejam disponíveis nos templates de layout.

1. Verifique se o modelo de layout exibe os seguintes filtros:

   * [!UICONTROL Projetos em que estou trabalhando] e [!UICONTROL Projetos dos quais sou proprietário] no [!UICONTROL Projetos] área
   * [!UICONTROL Minhas planilhas de horas aprovadas] e [!UICONTROL Minhas Planilhas de Horas] no [!UICONTROL Planilha de horas] área

   Para fazer isso:

   1. Acesse o modelo de layout.
   1. Selecionar **[!UICONTROL Listas]** em **[!UICONTROL Personalize o que os usuários veem]**.
   1. Selecionar **[!UICONTROL Projetos]** ou **[!UICONTROL Planilhas de Horas]** em **[!UICONTROL Selecione uma lista para personalizar]**.
   1. No **[!UICONTROL Filtro]** , verifique se **[!UICONTROL Projetos em que estou trabalhando]**, **[!UICONTROL Projetos dos quais sou proprietário]** (para projetos) e **[!UICONTROL Minhas planilhas de horas aprovadas]** e **[!UICONTROL Minhas Planilhas de Horas]** (para folhas de horas) são selecionadas.
   1. Clique em **[!UICONTROL Salvar]**.

   Para obter mais informações, consulte [Personalizar filtros, visualizações e agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Atribua o modelo de layout aos usuários, funções de trabalho, equipes ou grupos corretos. Para obter informações, consulte [Atribuir usuários a um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
