---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Carregar pranchetas XD como documentos no Workfront
description: Você pode fazer upload de pranchetas como documentos para uma revisão e aprovação rápidas ou simplesmente para armazená-las no Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# Carregar [!DNL XD] pranchetas como documentos para [!DNL Workfront]

Você pode carregar suas pranchetas como documentos para revisão e aprovação rápidas ou simplesmente armazená-las no [!DNL Adobe Workfront].

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Produto</td> 
   <td>Você deve ter uma licença [!DNL Adobe Creative Cloud] além de uma licença [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a [!UICONTROL Documentos]</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso à [!UICONTROL View] ou superior ao objeto no qual você deseja carregar um documento.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

* Você deve instalar o plug-in [!DNL Adobe Workfront for XD] antes de carregar placas de arte XD como documentos no Workfront.

Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Adicionar um novo documento

1. Clique no ícone **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Você também pode usar o menu para navegar até objetos principais.

   ![](assets/menu-350x440.png)

1. Vá para o item de trabalho no qual deseja carregar um documento.
1. Clique no ícone ![](assets/documents.png) do **[!UICONTROL Documento]** na barra de navegação.

1. Clique em **[!UICONTROL Novo arquivo]** próximo à parte inferior do plug-in.
1. Selecione a prancheta que deseja fazer upload.

   >[!TIP]
   >
   >Para selecionar mais de uma prancheta, clique e arraste o mouse sobre as pranchetas desejadas.
1. (Opcional) Digite um comentário na área **[!UICONTROL Atualizações]**.
1. Escolha o **[!UICONTROL Tipo de ativo]** no menu suspenso:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Formato de Exportação]</td>
     </tr>
     <tr>
      <td role="rowheader">Imagem PNG</td>
      <td>As pranchetas foram carregadas como um arquivo PNG na guia [!UICONTROL Documentos] do item de trabalho em [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>As pranchetas são carregadas como um JPG na guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>As pranchetas são carregadas como um SVG na guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Escolha se deseja que as pranchetas selecionadas sejam carregadas como um <strong>Arquivo de PDF único</strong> ou <strong>Vários arquivos de PDF</strong>. As pranchetas são carregadas como um PDF na guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Clique em **[!UICONTROL Carregar]**.\
   O documento aparece na área [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.

## Adicionar uma nova versão

1. Clique no ícone **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Você também pode usar o menu para navegar até objetos principais.

   ![](assets/menu-350x440.png)

1. Vá para o item de trabalho no qual deseja carregar um documento.
1. Clique no ícone **[!UICONTROL Documento]** ![](assets/documents.png)na barra de navegação.

1. Clique no documento ao qual deseja adicionar uma nova versão.
1. Clique em **[!UICONTROL Nova versão]** próximo à parte inferior do plug-in.
1. Selecione as pranchetas que deseja fazer upload.

   >[!NOTE]
   >
   >Se quiser fazer upload de uma nova versão de um SVG, PNG ou JPG, você poderá fazer upload de apenas uma prancheta.

1. (Opcional) Digite um comentário na área **[!UICONTROL Atualizações]**.

1. Escolha o **[!UICONTROL Tipo de ativo]** no menu suspenso:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Formato de exportação</td>
     </tr>
     <tr>
      <td role="rowheader">Imagem PNG</td>
      <td>A prancheta é carregada como um arquivo PNG na guia [!UICONTROL Documentos] do item de trabalho em [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>A prancheta é carregada como um JPG na guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>A prancheta é carregada como um SVG para a guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>As pranchetas são carregadas como um PDF na guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront].</p>
      <p><strong>Observação</strong>: só é possível carregar uma prancheta para uma nova versão do documento.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Clique em **[!UICONTROL Carregar]**.\
   O documento aparece na área [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.
