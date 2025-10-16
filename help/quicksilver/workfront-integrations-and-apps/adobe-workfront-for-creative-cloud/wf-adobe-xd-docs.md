---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Fazer upload de pranchetas do XD como documentos para o Workfront
description: Você pode fazer upload de pranchetas como documentos para uma revisão e aprovação rápidas ou simplesmente para armazená-las no Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---


# Carregar [!DNL XD] pranchetas como documentos para [!DNL Workfront]

Você pode carregar suas pranchetas como documentos para revisão e aprovação rápidas ou simplesmente armazená-las no [!DNL Adobe Workfront].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> 
   <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Produtos adicionais</td> 
   <td>Você deve ter uma licença [!DNL Adobe Creative Cloud] além de uma licença [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a [!UICONTROL Documentos]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso à [!UICONTROL View] ou superior ao objeto no qual você deseja carregar um documento.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* Você deve instalar o plug-in [!DNL Adobe Workfront for XD] antes de carregar quadros de arte do XD como documentos no Workfront.

Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Adicionar um novo documento

1. Clique no ícone **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Você também pode usar o menu para navegar até objetos principais.

   ![Ícone de menu](assets/menu-350x440.png)

1. Vá para o item de trabalho no qual deseja carregar um documento.
1. Clique no ícone **[!UICONTROL Documento]** ![Ícone Documento](assets/documents.png) na barra de navegação.

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
      <td>Escolha se deseja que as pranchetas selecionadas sejam carregadas como um <strong>Único arquivo PDF</strong> ou <strong>Vários arquivos PDF</strong>. As pranchetas são carregadas como um PDF na guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Clique em **[!UICONTROL Carregar]**.\
   O documento aparece na área [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.

## Adicionar uma nova versão

1. Clique no ícone **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Você também pode usar o menu para navegar até objetos principais.

   ![Ícone de menu](assets/menu-350x440.png)

1. Vá para o item de trabalho no qual deseja carregar um documento.
1. Clique no ícone **[!UICONTROL Documento]** ![Ícone Documento](assets/documents.png)na barra de navegação.

1. Clique no documento ao qual deseja adicionar uma nova versão.
1. Clique em **[!UICONTROL Nova versão]** próximo à parte inferior do plug-in.
1. Selecione as pranchetas que deseja fazer upload.

   >[!NOTE]
   >
   >Para fazer upload de uma nova versão de uma SVG, PNG ou JPG, você pode fazer upload de apenas uma prancheta.

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
      <td>A prancheta é carregada como uma JPG na guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>A prancheta é carregada como uma SVG na guia [!UICONTROL Documentos] do item de trabalho no [!DNL Workfront]. </td>
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
