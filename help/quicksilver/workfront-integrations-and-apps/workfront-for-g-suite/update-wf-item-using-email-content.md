---
product-area: workfront-integrations;projects
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Atualizar um  [!DNL Adobe Workfront]  item do Google Workspace usando conteúdo de email
description: Você pode atualizar um projeto, tarefa ou problema existente com informações de um email que não seja da Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Atualizar um item [!DNL Adobe Workfront] de [!DNL Google Workspace] usando conteúdo de email

>[!NOTE]
>
>A versão mais recente do plug-in do Adobe Workfront para Google foi lançada em 26 de junho de 2023.

Você pode atualizar um projeto, tarefa ou problema existente com informações de um email não-[!DNL Adobe Workfront].

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

Antes de atualizar um item [!DNL Workfront] usando o conteúdo de email de [!DNL Google Workspace], você deve

* Instalar [!DNL Workfront for Google Workspace]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Atualizar um item [!DNL Workfront] usando o conteúdo de email de [!DNL Google Workspace]

1. Se o painel [!UICONTROL Workfront para Google Workspace] não for exibido, clique no ícone do Workfront ![ícone do Workfront](assets/wf-lion-icon.png) na barra lateral de complementos [!DNL Google Workspace] na extremidade direita da página.
1. Com a mensagem de email aberta no [!DNL Google Workspace], clique em **[!UICONTROL Postar como uma nova atualização]** no painel [!DNL Google Workspace].
1. Em **[!UICONTROL Tipo]**, clique na seta suspensa e, em seguida, clique no tipo de objeto ao qual deseja adicionar a atualização.
1. Clique na opção **[!UICONTROL Pesquisar por]**, comece digitando o nome do objeto ao qual deseja adicionar a atualização e selecione o item quando ele aparecer na lista abaixo.

   Essa opção varia, dependendo do que você selecionou na etapa 3. Pode ser **[!UICONTROL Pesquisar um projeto]**, **[!UICONTROL Pesquisar uma tarefa]** ou **[!UICONTROL Pesquisar um problema]**.

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
      <td>Edite qualquer parte desse texto, retirada da linha de assunto e do texto do corpo do email.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir anexos de email]</td> 
      <td><p>(Disponível somente se o email contiver pelo menos um anexo.) Clique nesta opção para salvar anexos na guia [!UICONTROL Documentos] para a tarefa ou problema. </p><p>Para não salvar um anexo, clique no X à direita do seu nome. </p><p>Se o email contiver links para documentos em [!DNL Google Drive], os links serão salvos na guia [!UICONTROL Visão geral] da tarefa ou problema que você está criando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Para que isso funcione, seu</span></span>[!DNL Workfront] administrador<span style="color: #ff1493;"><span style="color: #000000;"> deve autorizar [!DNL Google Drive] a trabalhar com [!DNL Workfront]</span></span></p>
      <p>Se você habilitar essa opção, ela permanecerá habilitada para outros emails convertidos em tarefas, problemas e atualizações.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notificar</td> 
      <td>Clique em <strong>[!UICONTROL Notify]</strong>, clique na opção <strong>[!UICONTROL Pesquisar um usuário ou equipe]</strong> que é exibida, em seguida, comece a digitar o nome da pessoa ou equipe e clique nele quando ele aparecer na lista abaixo. Repita isso para cada pessoa e equipe que deseja adicionar e clique em <strong>[!UICONTROL Salvar]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Atualizar]**.

   Quando você atualiza o navegador, uma mensagem com um link na parte inferior do painel [!DNL Workfront for Google Workspace] confirma que você converteu o email em uma atualização:

   Você pode clicar no link para ir até a guia [!UICONTROL Atualizações] no [!DNL Workfront] para o objeto especificado na etapa 4.

   Você pode repetir essas etapas para converter o mesmo email em atualizações, tarefas e problemas (consulte [Criar um problema do Adobe Workfront [!DNL Google Workspace] usando conteúdo de email](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Quando você atualizar o navegador ou retornar ao email em outro momento, todos os links criados para o email serão listados na parte inferior do painel do [!UICONTROL Workfront para Google Workspace].

1. (Opcional) Continue a trabalhar com a atualização no painel complementar do [!DNL Workfront] seguindo um destes procedimentos:

   * Para adicionar outra atualização na guia **[!UICONTROL Atualizações]**, clique em **[!UICONTROL Iniciar uma nova atualização]** e digite as informações.

   * Para responder a uma atualização na guia **[!UICONTROL Atualizações]**, clique em **[!UICONTROL Responder]** e digite sua resposta.

     Para ambas as opções acima, você pode clicar em **[!UICONTROL Notificar]** para especificar destinatários para a resposta como na etapa 5. Quando estiver pronto, clique em **[!UICONTROL Postar]** para adicionar a atualização ou a resposta.

   * Clique na guia **[!UICONTROL Detalhes]** para exibir os detalhes do novo projeto, tarefa ou problema.
