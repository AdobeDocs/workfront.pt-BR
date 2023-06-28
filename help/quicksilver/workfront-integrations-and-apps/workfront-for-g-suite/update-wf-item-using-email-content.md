---
product-area: workfront-integrations;projects
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Atualizar um [!DNL Adobe Workfront] item do G Suite usando conteúdo de email
description: Você pode atualizar um projeto, tarefa ou problema existente com informações de um email que não seja da Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Atualizar um [!DNL Adobe Workfront] item de [!DNL G Suite] uso de conteúdo de email

>[!NOTE]
>
>A versão mais recente do plug-in do Adobe Workfront para Google foi lançada em 26 de junho de 2023.

Você pode atualizar um projeto, tarefa ou problema existente com informações de um[!DNL Adobe Workfront] email.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Pré-requisitos

Antes de atualizar um [!DNL Workfront] item usando o conteúdo de email do [!DNL G Suite], você deve

* Instalar [!DNL Workfront for G suite]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Atualizar um [!DNL Workfront] item usando o conteúdo de email do [!DNL G Suite]

1. Se a variável [!UICONTROL Workfront para G Suite] não for exibido, clique no ícone Workfront ![](assets/wf-lion-icon.png) no [!DNL G Suite] barra lateral de complementos na extremidade direita da página.
1. Com a mensagem de email aberta no [!DNL G Suite], clique em **[!UICONTROL Publicar como uma nova atualização]** no [!DNL G Suite] painel.
1. Em **[!UICONTROL Tipo]**, clique na seta suspensa e clique no tipo de objeto ao qual deseja adicionar a atualização.
1. Clique em **[!UICONTROL Pesquisar por]** , comece digitando o nome do objeto ao qual deseja adicionar a atualização e selecione o item quando ele aparecer na lista abaixo.

   Essa opção varia, dependendo do que você selecionou na etapa 3. Pode ser **[!UICONTROL Procurar um projeto]**, **[!UICONTROL Procurar uma tarefa]** ou **[!UICONTROL Procurar um problema]**.

   >[!NOTE]
   >
   >Quando você estiver digitando o nome de uma tarefa, as tarefas pessoais ad hoc serão excluídas da lista de nomes exibida abaixo.

1. Faça qualquer uma destas alterações opcionais:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Atualizar]</td> 
      <td>Edite qualquer parte deste texto, retirada da linha de assunto e do texto do corpo do email.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir anexos de email]</td> 
      <td><p>(Disponível somente se o email contiver pelo menos um anexo.) Clique nesta opção para salvar anexos na guia [!UICONTROL Documentos] para a tarefa ou problema. </p><p>Para não salvar um anexo, clique no X à direita do seu nome. </p><p>Se o email contiver links para documentos no [!DNL Google Drive], os links serão salvos na guia [!UICONTROL Visão geral] da tarefa ou problema que você está criando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Para que isso funcione, seu</span></span>[!DNL Workfront] administrador<span style="color: #ff1493;"><span style="color: #000000;"> deve autorizar [!DNL Google Drive] para trabalhar com [!DNL Workfront]</span></span></p>
      <p>Se você habilitar essa opção, ela permanecerá habilitada para outros emails convertidos em tarefas, problemas e atualizações.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notificar</td> 
      <td>Clique em <strong>[!UICONTROL Notificar]</strong>, clique no link <strong>[!UICONTROL Pesquisar um usuário ou equipe]</strong> que for exibida, comece digitando o nome da pessoa ou da equipe e clique nele quando ele aparecer na lista abaixo. Repita isso para cada pessoa e equipe que deseja adicionar e clique em <strong>[!UICONTROL Salvar]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Atualizar]**.

   Ao atualizar o navegador, uma mensagem com um link na parte inferior do [!DNL Workfront for G Suite] O painel confirma que você converteu o email em uma atualização:

   Você pode clicar no link para ir para a [!UICONTROL Atualizações] guia em [!DNL Workfront] para o objeto especificado na etapa 4.

   Você pode repetir essas etapas para converter o mesmo email em atualizações, tarefas e problemas (consulte [Criar um problema do Adobe Workfront no [!DNL G Suite] usando conteúdo de email](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Quando você atualiza seu navegador ou retorna ao email em outro momento, todos os links criados para o email são listados na parte inferior do [!UICONTROL Workfront para G Suite] painel.

1. (Opcional) Continue a trabalhar com a atualização no [!DNL Workfront] do painel complementar, seguindo um destes procedimentos:

   * Para adicionar outra atualização no **[!UICONTROL Atualizações]** clique em **[!UICONTROL Iniciar uma nova atualização]** e digite as informações.

   * Para responder a uma atualização sobre o **[!UICONTROL Atualizações]** clique em **[!UICONTROL Responder]** e digite sua resposta.

     Para ambas as opções acima, você pode clicar em **[!UICONTROL Notificar]** para especificar destinatários para a resposta como na etapa 5. Quando estiver pronto, clique em **[!UICONTROL Publicar]** para adicionar a atualização ou resposta.

   * Clique em **[!UICONTROL Detalhes]** para exibir os detalhes do novo projeto, tarefa ou problema.
