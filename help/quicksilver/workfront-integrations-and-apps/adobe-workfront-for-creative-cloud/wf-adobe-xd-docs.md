---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Fazer upload XD pranchetas como documentos para o Workfront
description: Você pode fazer upload de suas pranchetas como documentos para uma revisão e aprovação rápidas ou simplesmente armazenar no Adobe Workfront.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 710035f7-339c-457c-b9b0-e51bc0e0061d
source-git-commit: bf47ae15d2972e8ee11f76741f8e5c676d79e626
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---


# Upload [!DNL XD] pranchetas como documentos para [!DNL Workfront]

Você pode fazer upload de suas pranchetas como documentos para uma revisão e aprovação rápidas ou simplesmente armazenar em [!DNL Adobe Workfront].

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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
   <td>Você deve ter um [!DNL Adobe Creative Cloud] além de um [!DNL Workfront] licença.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso aos [!UICONTROL Documents]</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso à [!UICONTROL View] ou superior ao objeto no qual você deseja fazer upload de um documento.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

* Você deve instalar o [!DNL Adobe Workfront for XD] antes de fazer upload XD quadros de arte como documentos para o Workfront.

Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Adicionar um novo documento

1. Clique no botão **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Também é possível usar o menu para navegar até os objetos pai.

   ![](assets/menu-350x440.png)

1. Vá para o item de trabalho onde deseja carregar um documento.
1. Clique no botão **[!UICONTROL Documento]** ícone ![](assets/documents.png) na barra de navegação.

1. Clique em **[!UICONTROL Novo arquivo]** próximo à parte inferior do plug-in.
1. Selecione o quadro que deseja fazer upload.

   >[!TIP]
   >
   >Para selecionar mais de uma prancheta, clique e arraste o mouse sobre as pranchetas desejadas.
1. (Opcional) Digite um comentário no **[!UICONTROL Atualizações]** área.
1. Escolha a **[!UICONTROL Tipo de ativo]** no menu suspenso:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">[!UICONTROL Exportar formato]</td>
     </tr>
     <tr>
      <td role="rowheader">Imagem PNG</td>
      <td>As pranchetas são carregadas como um PNG na guia [!UICONTROL Documents] do item de trabalho em [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>As pranchetas são carregadas como JPG para a guia [!UICONTROL Documents] do item de trabalho em [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>As pranchetas são carregadas como SVG para a guia [!UICONTROL Documents] do item de trabalho em [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td>Escolha se deseja que os pranchetas selecionados sejam carregados como um <strong>Arquivo PDF único</strong> ou <strong>Vários arquivos PDF</strong>. As pranchetas são carregadas como PDF para a guia [!UICONTROL Documents] do item de trabalho em [!DNL Workfront].</td>
     </tr>
    </tbody>
   </table>


1. Clique em **[!UICONTROL Upload]**.\
   O documento é exibido na [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.

## Adicionar uma nova versão

1. Clique no botão **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Também é possível usar o menu para navegar até os objetos pai.

   ![](assets/menu-350x440.png)

1. Vá para o item de trabalho onde deseja carregar um documento.
1. Clique no botão **[!UICONTROL Documento]** ícone ![](assets/documents.png)na barra de navegação.

1. Clique no documento ao qual deseja adicionar uma nova versão.
1. Clique em **[!UICONTROL Nova versão]** próximo à parte inferior do plug-in.
1. Selecione as pranchetas que deseja fazer upload.

   >[!NOTE]
   >
   >Se quiser fazer upload de uma nova versão de um SVG, PNG ou JPG, é possível fazer upload de apenas uma prancheta.

1. (Opcional) Digite um comentário no **[!UICONTROL Atualizações]** área.

1. Escolha a **[!UICONTROL Tipo de ativo]** no menu suspenso:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td colspan="2" role="rowheader">Formato de exportação</td>
     </tr>
     <tr>
      <td role="rowheader">Imagem PNG</td>
      <td>O quadro é carregado como um PNG na guia [!UICONTROL Documents] do item de trabalho em [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">JPG</td>
      <td>O quadro é carregado como JPG para a guia [!UICONTROL Documents] do item de trabalho em [!DNL Workfront]. <br></td>
     </tr>
     <tr>
      <td role="rowheader">SVG</td>
      <td>O quadro é carregado como um SVG para a guia [!UICONTROL Documents] do item de trabalho em [!DNL Workfront]. </td>
     </tr>
     <tr>
      <td role="rowheader">PDF</td>
      <td><p>As pranchetas são carregadas como PDF para a guia [!UICONTROL Documents] do item de trabalho em [!DNL Workfront].</p>
      <p><strong>Observação</strong>: Você pode fazer upload de apenas uma prancheta para uma nova versão do documento.</p>
      </td>
     </tr>
    </tbody>
   </table>

1. Clique em **[!UICONTROL Upload]**.\
   O documento é exibido na [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.
