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

Os botões de filtro na área [!UICONTROL Projetos e Planilhas de Horas] não são exibidos porque os filtros correspondentes não estão incluídos no modelo de layout aplicado ao usuário. O administrador do [!DNL Workfront] deve atribuir um modelo de layout que inclua os filtros.

>[!NOTE]
>
>Às vezes, os filtros são removidos da área [!UICONTROL Controles de Lista] na [!UICONTROL Instalação]. O administrador [!DNL Workfront] deve incluí-los nas listas desta área para que eles fiquem disponíveis nos modelos de layout.

1. Verifique se o modelo de layout exibe os seguintes filtros:

   * [!UICONTROL Projetos dos quais sou proprietário] e [!UICONTROL Projetos dos quais sou proprietário] na área [!UICONTROL Projetos]
   * [!UICONTROL Minhas Aprovações de Planilha de Horas] e [!UICONTROL Minhas Planilhas de Horas] na área [!UICONTROL Planilha de Horas]

   Para fazer isso:

   1. Acesse o modelo de layout.
   1. Selecione **[!UICONTROL Listas]** em **[!UICONTROL Personalize o que os usuários veem]**.
   1. Selecione **[!UICONTROL Projetos]** ou **[!UICONTROL Folhas de horas]** em **[!UICONTROL Selecione uma lista para personalizar]**.
   1. Na seção **[!UICONTROL Filtro]**, verifique se **[!UICONTROL Projetos dos quais sou proprietário]**, **[!UICONTROL Projetos dos quais sou proprietário]** (para projetos) e **[!UICONTROL Minhas aprovações de folha de horas]** e **[!UICONTROL Minhas folhas de horas]** (para folhas de horas) estão selecionados.
   1. Clique em **[!UICONTROL Salvar]**.

   Para obter mais informações, consulte [Personalizar Filtros, Exibições e Agrupamentos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. Atribua o modelo de layout aos usuários, funções de trabalho, equipes ou grupos corretos. Para obter informações, consulte [Atribuir usuários a um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).
