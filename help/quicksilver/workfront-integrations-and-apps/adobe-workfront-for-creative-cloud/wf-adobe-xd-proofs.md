---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-xd
title: Carregar pranchetas XD como provas no Workfront
description: Você pode fazer upload de pranchetas como provas diretamente no Adobe Workfront para uma revisão e aprovação completas.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d6699fd7-f130-4231-8713-0cfa8dc3c910
source-git-commit: d5255968a96452d9501a285408f67be7da10d933
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# Carregar [!DNL XD] pranchetas como provas para [!DNL Workfront]

Você pode fazer upload de pranchetas como provas diretamente no [!DNL Adobe Workfront] para uma revisão e aprovação completas.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Plano atual: [!UICONTROL Pro] ou superior</p> <p>ou</p> <p>Plano herdado: [!UICONTROL Premium]</p> <p>Para obter mais informações sobre acesso de prova com os diferentes planos, consulte .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>Plano atual: [!UICONTROL Trabalho] ou [!UICONTROL Prova]</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Você deve ter uma licença [!DNL Adobe Creative Cloud] além de uma licença [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>[!UICONTROL Manager] ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Editar acesso a [!UICONTROL Documentos]</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do [!DNL Workfront] ou do [!DNL Workfront Proof].

## Pré-requisitos

* Você deve instalar o plug-in [!DNL Adobe Workfront for XD] antes de carregar provas no [!DNL Adobe XD].

  Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for XD]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-xd-install.md).

## Carregar uma prova estática

1. Clique no ícone **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Você também pode usar o menu para navegar até objetos principais.

   ![](assets/menu-350x440.png)

1. Vá para o item de trabalho no qual deseja carregar uma prova estática.
1. Clique no ícone ![](assets/documents.png) do **[!UICONTROL Documento]** na barra de navegação.

1. Clique em **[!UICONTROL Novo arquivo]** próximo à parte inferior do plug-in.
1. Selecione as pranchetas que deseja fazer upload.

   >[!TIP]
   >
   >* As pranchetas aparecerão na prova na ordem em que foram selecionadas. A primeira prancheta selecionada será a primeira página na prova e assim por diante.
   >* Para selecionar rapidamente mais de uma prancheta, clique e arraste o mouse sobre as pranchetas desejadas. Isso não permite controlar a ordem das pranchetas na prova.

1. Habilitar **[!UICONTROL Criar uma prova]**.

1. Nomeie a prova.

1. Escolha o tipo de aprovação de prova desejado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Os processos básicos de aprovação são ad hoc e podem incluir diferentes revisores, conforme necessário: </p> 
       <ul> 
        <li> <p>(Opcional) Adicione <strong>Aprovadores</strong> à caixa.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Os processos de aprovação automatizados são pré-criados pelos administradores e incluem revisores e estágios específicos. Para obter mais informações, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Visão geral do Fluxo de Trabalho Automatizado</a>.</p> 
       <ul> 
        <li> <p>Escolha um [!UICONTROL Modelo de Fluxo de Trabalho] no menu suspenso.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Opcional) Digite um comentário na área **[!UICONTROL Atualizações]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. Escolha o formato de exportação no menu suspenso **[!UICONTROL Tipo de ativo]**.


1. (Opcional) Se você selecionar PDF como tipo de ativo e tiver mais de uma prancheta selecionada, escolha se deseja exportar suas pranchetas como **[!UICONTROL Arquivo de PDF único]s** ou **M[!UICONTROL vários arquivos de PDF]**.

1. (Opcional) Nomeie o PDF.

   ![](assets/pdf-options.png)

1. Clique em **[!UICONTROL Carregar]**.\
   O documento aparece na área [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.

## Carregar uma prova interativa {#upload-an-interactive-proof}

Você pode criar uma prova interativa para suas pranchetas com o plug-in [!DNL Workfront for Adobe]. É um processo de duas etapas. Primeiro, é necessário criar um link interativo e, em seguida, carregar a prova em um item de trabalho.

### Criar um link interativo para a prancheta  {#create-an-interactive-link-for-your-art-board}

1. Abra a prancheta e clique em **[!UICONTROL Compartilhar]** na área superior esquerda da tela.
1. Especifique as configurações de link:

   1. Nomeie o link.
   1. Escolha uma configuração de exibição.
   1. Na seção **[!UICONTROL Acesso ao Link]**, verifique se **[!UICONTROL Qualquer pessoa com este link]** está selecionada.

      Você deve ativar esse tipo de acesso para gerar uma prova interativa.

   1. Clique em **[!UICONTROL Criar link]**.

1. Clique novamente em **[!UICONTROL Design]** na área superior esquerda da tela. Prossiga para a seção [Carregar uma prova interativa](#upload-an-interactive-proof) abaixo.

   >[!NOTE]
   >
   >Talvez seja necessário reabrir o painel de plug-in no canto inferior esquerdo da tela.

### Carregar uma prova interativa

1. Clique no ícone **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Você também pode usar o menu para navegar até objetos principais.

   ![](assets/menu-350x440.png)

1. Vá para o item de trabalho no qual deseja carregar uma prova interativa.
1. Clique no ícone ![](assets/documents.png) do **[!UICONTROL Documento]** na barra de navegação.

1. Clique em **[!UICONTROL Novo arquivo]** próximo à parte inferior do plug-in.
1. Habilitar **[!UICONTROL Criar uma prova]**.

1. Escolha o tipo de aprovação de prova desejado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Os processos básicos de aprovação são ad hoc e podem incluir diferentes revisores, conforme necessário: </p> 
       <ul> 
        <li> <p>(Opcional) Adicione <strong>Aprovadores</strong> à caixa.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Os processos de aprovação automatizados são pré-criados pelos administradores e incluem revisores e estágios específicos. Para obter mais informações, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Visão geral do Fluxo de Trabalho Automatizado</a>.</p> 
       <ul> 
        <li> <p>Escolha um [!UICONTROL Modelo de Fluxo de Trabalho] no menu suspenso.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. (Opcional) Digite um comentário na área **[!UICONTROL Atualizações]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. No menu suspenso **[!UICONTROL Tipo de ativo]**, escolha o link que acabou de criar na guia **Links compartilhados**. Para obter mais informações, consulte [Criar um link interativo para sua prancheta](#create-an-interactive-link-for-your-artboard).\
   ![](assets/shared-links-xd-350x870.png)

1. Clique em **[!UICONTROL Carregar]**.

   O documento aparece na área [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.

   >[!IMPORTANT]
   >
   >Os usuários devem ter acesso ao [!UICONTROL Desktop Proofing Viewer] para revisar e aprovar provas interativas. Para obter mais informações, consulte [Instalar o [!UICONTROL Desktop Proofing Viewer]](../../review-and-approve-work/proofing/use-the-desktop-proofing-viewer/installing-desktop-proofing-viewer.md).

## Carregar uma nova versão de prova

Você pode fazer upload de uma nova versão de uma prova. O plug-in lembra o fluxo de trabalho de prova definido na versão anterior, mas você pode alterá-lo se desejar.

1. Clique no ícone **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Você também pode usar o menu para navegar até objetos principais.

   ![](assets/menu-350x440.png)

1. Vá para o item de trabalho para o qual você precisa carregar um documento.
1. Clique no ícone **[!UICONTROL Documento]** ![](assets/documents.png)na barra de navegação.

1. Clique em **[!UICONTROL Nova versão]** próximo à parte inferior do plug-in.
1. Habilitar **[!UICONTROL Criar uma prova]**.
1. Selecione as pranchetas que deseja fazer upload.

   >[!NOTE]
   >
   >Se quiser fazer upload de uma nova versão de um arquivo .svg, .png ou .jpg, você poderá fazer upload de apenas uma prancheta.

1. Escolha o tipo de aprovação de prova desejado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Básico]: </td> 
      <td> <p>Os processos básicos de aprovação são ad hoc e podem incluir diferentes revisores, conforme necessário: </p> 
       <ul> 
        <li> <p>(Opcional) Adicione <strong>Aprovadores</strong> à caixa.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Automatizado]</td> 
      <td> <p>Os processos de aprovação automatizados são pré-criados pelos administradores e incluem revisores e estágios específicos. Para obter mais informações, consulte <a href="../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Visão geral do Fluxo de Trabalho Automatizado</a>.</p> 
       <ul> 
        <li> <p>Escolha um [!UICONTROL Modelo de Fluxo de Trabalho] no menu suspenso.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

{{adjust-proof-settings}}

1. Escolha o formato de exportação no menu suspenso **[!UICONTROL Tipo de ativo]**.

   ![](assets/create-a-proof-xd-350x202.png)

1. (Opcional) Digite um comentário na área **[!UICONTROL Atualizações]**.

   ![](assets/proof-approvals-xd-350x396.png)

1. (Opcional) Se você selecionar PDF como tipo de ativo e tiver mais de uma prancheta selecionada, escolha se deseja exportar suas pranchetas como **[!UICONTROL Arquivo de PDF único]s** ou **M[!UICONTROL vários arquivos de PDF]**.

1. (Opcional) Nomeie o PDF.

   ![](assets/pdf-options.png)

1. Clique em **[!UICONTROL Carregar]**.\
   O documento aparece na área [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.
