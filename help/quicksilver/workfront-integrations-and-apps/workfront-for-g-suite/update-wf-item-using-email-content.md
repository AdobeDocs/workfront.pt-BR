---
product-area: workfront-integrations;projects
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Atualize um [!DNL Adobe Workfront] item do G Suite usando conteúdo de email
description: Você pode atualizar um projeto, tarefa ou problema existente com informações de um email que não seja da Adobe Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 2ac392f5-98a3-4ab6-a0e3-cda378f0f68b
source-git-commit: 0934ae23a8e80dd18872efef7d274bd57d227647
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Atualize um [!DNL Adobe Workfront] item de [!DNL G Suite] uso de conteúdo de email

>[!NOTE]
>
>Existe um [problema conhecido](https://experienceleague.adobe.com/docs/workfront-known-issues/issues/new-workfront-experience/wf-current/wf-integrations-error-when-opening-wf-for-gsuite.html?lang=en) com a versão atual de [!DNL Workfront for G Suite] não funciona conforme o esperado. Estamos trabalhando em uma nova versão e esperamos que ela seja lançada para o [!DNL Google Marketplace] num futuro próximo.

Você pode atualizar um projeto, tarefa ou problema existente com informações de um[!DNL Adobe Workfront] email.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Antes de atualizar uma [!DNL Workfront] item usando conteúdo de email de [!DNL G Suite], você deve

* Instalar [!DNL Workfront for G suite]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Atualizar um [!DNL Workfront] item usando conteúdo de email de [!DNL G Suite]

1. Se a variável [!UICONTROL Workfront para G Suite] não for exibido, clique no ícone do Workfront ![](assets/wf-lion-icon.png) no [!DNL G Suite] barra lateral dos complementos na extremidade direita da página.
1. Com a mensagem de email aberta em [!DNL G Suite], clique em **[!UICONTROL Publicar como uma nova atualização]** no [!DNL G Suite] painel.
1. Em **[!UICONTROL Tipo]**, clique na seta suspensa e, em seguida, clique no tipo de objeto ao qual deseja adicionar a atualização.
1. Clique no botão **[!UICONTROL Procurar por]** , comece digitando o nome do objeto ao qual deseja adicionar a atualização e selecione o item quando ele for exibido na lista abaixo.

   ![](assets/click-search-for-task-issue.png)

   Essa opção varia, dependendo do que você selecionou na etapa 3. Pode ser **[!UICONTROL Pesquisar um projeto]**, **[!UICONTROL Procurar uma tarefa]** ou **[!UICONTROL Pesquisar por um problema]**.

   >[!NOTE]
   >
   >Ao digitar o nome de uma tarefa, as tarefas pessoais ad hoc são excluídas da lista de nomes exibida abaixo.

1. Faça qualquer uma dessas alterações opcionais:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Atualização]</td> 
      <td>Edite qualquer parte desse texto, que é retirada da linha de assunto e do texto do corpo do email.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir anexos de email]</td> 
      <td><p>(Disponível somente se o email tiver pelo menos um anexo.) Clique nesta opção para salvar anexos na guia [!UICONTROL Documents] da tarefa ou problema. </p><p>Se não quiser salvar um anexo, clique no X à direita do nome. </p><p>Se o email contiver links para documentos em [!DNL Google Drive], os links são salvos na guia [!UICONTROL Visão geral] da tarefa ou problema que você está criando. </p><p>Importante: <span style="color: #ff1493;"><span style="color: #000000;">Para que isso funcione,</span></span>[!DNL Workfront] administrador<span style="color: #ff1493;"><span style="color: #000000;"> deve autorizar [!DNL Google Drive] para trabalhar com [!DNL Workfront]</span></span></p>
      <p>Se você ativar essa opção, ela permanecerá ativada para outros emails convertidos em tarefas, problemas e atualizações.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Notificar</td> 
      <td>Clique em <strong>[!UICONTROL Notificar]</strong>, clique no botão <strong>[!UICONTROL Pesquisar por um usuário ou equipe]</strong> , que é exibida, comece a digitar o nome da pessoa ou equipe e clique nele quando ele for exibido na lista abaixo. Repita isso para cada pessoa e equipe que deseja adicionar e clique em <strong>[!UICONTROL Salvar]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Atualizar]**.

   Ao atualizar o navegador, uma mensagem com um link na parte inferior do [!DNL Workfront for G Suite] O painel confirma que você converteu o email em uma atualização:

   ![](assets/email-was-converted-as-update.png)

   Você pode clicar no link para acessar o [!UICONTROL Atualizações] em [!DNL Workfront] para o objeto especificado na etapa 4.

   Você pode repetir essas etapas para converter o mesmo email em atualizações, tarefas e problemas (consulte [Criar um problema do Adobe Workfront no [!DNL G Suite] usando conteúdo de email](../../workfront-integrations-and-apps/workfront-for-g-suite/create-wf-issue-in-g-suite-using-email-content.md)). Ao atualizar seu navegador ou retornar ao email em outro momento, todos os links criados para o email serão listados na parte inferior da variável [!UICONTROL Workfront para G Suite] painel.

1. (Opcional) Continue a trabalhar com a atualização no [!DNL Workfront] painel complementar executando um dos seguintes procedimentos:

   * Para adicionar outra atualização no **[!UICONTROL Atualizações]** clique em **[!UICONTROL Iniciar uma nova atualização]** e digite as informações.

   * Para responder a uma atualização no **[!UICONTROL Atualizações]** clique em **[!UICONTROL Responder]** e digite sua resposta.

      Para ambas as opções acima, você pode clicar em **[!UICONTROL Notificar]** para especificar destinatários para a resposta, como na etapa 5. Quando estiver pronto, clique em **[!UICONTROL Post]** para adicionar a atualização ou resposta.

   * Clique no botão **[!UICONTROL Detalhes]** para exibir os detalhes do novo projeto, tarefa ou problema.
