---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Fazer upload de provas do Adobe Photoshop
description: Você pode fazer upload de seus quadros de arte como provas diretamente no Adobe Workfront para obter uma análise e aprovação completas.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
source-git-commit: 698affafa8771e9e91b725908d4782a2af12c0b8
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Fazer upload de provas de [!DNL Photoshop]

Você pode fazer upload de seus quadros de arte diretamente para [!DNL Adobe Workfront] para uma análise e aprovação completas.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Plano atual: [!UICONTROL Pro] ou superior</p> <p>ou</p> <p>Plano herdado: [!UICONTROL Premium]</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>Plano atual: [!UICONTROL Trabalho] ou [!UICONTROL Prova]</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Você deve ter um [!DNL Adobe Creative Cloud] além de um [!DNL Workfront] licença.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>[!UICONTROL Manager] ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Editar acesso aos [!UICONTROL Documents]</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Pré-requisitos

* Você deve instalar o [!DNL Adobe Workfront for Photoshop] antes de fazer upload de provas do [!DNL Adobe Photoshop].

   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## Fazer upload de uma prova básica

1. Clique no botão **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Também é possível usar o menu para navegar até os objetos pai.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vá para o item de trabalho onde deseja carregar uma prova.
1. Clique no botão **[!UICONTROL Documento]** ícone ![](assets/documents.png) na barra de navegação.
1. Clique em **[!UICONTROL Novo arquivo]** próximo à parte inferior do plug-in.
1. Ative o **[!UICONTROL Criar uma prova]** alternar.
1. (Opcional) Digite um nome para a prova no **[!UICONTROL Nome da prova]** caixa de texto.
1. No **[!UICONTROL Aprovações de prova]** seção , selecione **[!UICONTROL Básico]**.
1. (Opcional) Adicione aprovadores.
1. (Opcional) Digite um comentário no **[!UICONTROL Atualizações]** área.

   ![](assets/add-comment.png)

1. Escolha a **[!UICONTROL Tipo de ativo]** no menu suspenso.

1. (Opcional) Selecione **[!UICONTROL Adicionar arquivo externo]** para adicionar um arquivo de seu computador.
1. Clique em **[!UICONTROL Upload]**, configure as opções de exportação desejadas com base no tipo de ativo escolhido acima.

   ![](assets/plugin-files-350x307.png)\
   O documento é exibido na [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.


## Fazer upload de uma prova automatizada

1. Clique no botão **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Também é possível usar o menu para navegar até os objetos pai.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vá para o item de trabalho onde deseja carregar uma prova.
1. Clique no botão **[!UICONTROL Documento]** ícone ![](assets/documents.png) na barra de navegação.

1. Clique em **[!UICONTROL Novo arquivo]** próximo à parte inferior do plug-in.
1. Ative o **[!UICONTROL Criar uma prova]** alternar.
1. (Opcional) Digite um nome para a prova no **[!UICONTROL Nome da prova]** caixa de texto.
1. No **[!UICONTROL Aprovações de prova]** seção , selecione **[!UICONTROL Automatizado]**.
1. (Opcional) Na seção **[!UICONTROL Modelo de fluxo de trabalho]** digite o nome de um template de workflow de prova.

{{adjust-proof-settings}}

>[!NOTE]
>
> Se houver campos obrigatórios em branco no modelo de fluxo de trabalho, as configurações de prova automatizada serão abertas automaticamente e você deverá preencher esses campos para fazer upload da prova.


1. (Opcional) Digite um comentário no **[!UICONTROL Atualizações]** área.

   ![](assets/add-comment-automated-approval.png)

1. Escolha a **[!UICONTROL Tipo de ativo]** no menu suspenso.
1. (Opcional) Selecione **[!UICONTROL Adicionar arquivo externo]** para adicionar um arquivo de seu computador.
1. Clique em **[!UICONTROL Upload]**, configure as opções de exportação desejadas com base no tipo de ativo escolhido acima.
O documento é exibido na [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.

## Fazer upload de uma nova versão de prova

Você pode fazer upload de uma nova versão de uma prova. O plug-in lembra do fluxo de trabalho de prova definido na versão anterior, mas você pode alterá-lo se desejar.

1. Clique no botão **[!UICONTROL Menu]** no canto superior direito e selecione **[!UICONTROL Lista de Trabalho]**. Também é possível usar o menu para navegar até os objetos pai.

   ![](assets/go-back-to-work-list-350x314.png)

1. Vá para o item de trabalho para o qual você precisa carregar um documento.
1. Clique no botão **[!UICONTROL Documento]** ícone ![](assets/documents.png)na barra de navegação.

1. Clique em **[!UICONTROL Nova versão]** próximo à parte inferior do plug-in.
1. Ative o **[!UICONTROL Criar uma prova]** alternar.

1. No *[!UICONTROL *Aprovações de prova]**, escolha **[!UICONTROL Básico]** ou **[!UICONTROL Automatizado]**.

1. Adicionar **[!UICONTROL Revisores]** ou **[!UICONTROL Modelo de fluxo de trabalho]** com base no tipo de aprovação selecionado na etapa 7.

1. (Opcional) Digite um comentário no **[!UICONTROL Atualizações]** área.
1. Escolha a **[!UICONTROL Tipo de ativo]** no menu suspenso.
1. Clique em **[!UICONTROL Upload]**, configure as opções de exportação desejadas com base no tipo de ativo escolhido acima.
O documento é exibido na [!UICONTROL Documentos] no plug-in e no aplicativo de desktop.
