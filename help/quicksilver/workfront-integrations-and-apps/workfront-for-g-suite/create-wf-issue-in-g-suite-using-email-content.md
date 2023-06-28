---
product-area: workfront-integrations;projects
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Criar um [!DNL Adobe Workfront] problema no G Suite usando conteúdo de email
description: Você pode converter um email externo (não gerado por [!DNL Adobe Workfront)] para um [!DNL Workfront] problema.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 4b95828dc3e6a67c4dbefb46f173303c519643a9
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Criar um [!DNL Adobe Workfront] problema no [!DNL G Suite] uso de conteúdo de email

>[!NOTE]
>
>A versão mais recente do plug-in do Adobe Workfront para Google foi lançada em 26 de junho de 2023.

Você pode converter um email externo (não gerado por [!DNL Adobe Workfront]) para um [!DNL Workfront] problema.

Você também pode converter um email externo em uma atualização sobre um problema existente. Para obter mais informações, consulte [Atualizar um [!DNL Adobe Workfront] item do [!DNL G Suite] usando conteúdo de email](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Para obter informações sobre o uso de [!DNL G Suite] para trabalhar com emails de notificação enviados por [!DNL Workfront], consulte [Gerenciar [!DNL Adobe Workfront] detalhes da notificação do [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Antes de criar um problema no [!DNL G Suite], você deve

* Instalar [!DNL Workfront for G suite]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Criar um [!DNL Adobe Workfront] problema no [!DNL G Suite] uso de conteúdo de email

1. Se a variável [!UICONTROL Workfront para G Suite] não for exibido, clique na guia [!DNL Workfront] ícone ![](assets/wf-lion-icon.png) no [!DNL G Suite] barra lateral de complementos na extremidade direita da página.
1. Com a mensagem de email aberta no [!DNL G Suite], clique em uma opção no [!DNL Workfront for G Suite] para converter o email em um novo [!DNL Workfront] problema.

   ![](assets/convert-email-task-issue-update.png)

1. Se quiser anexar o problema a um projeto principal, clique em **[!UICONTROL Nome do projeto]**, comece digitando o nome do projeto no qual deseja solucionar o problema e clique no nome do projeto quando ele aparecer na lista abaixo.
1. Faça qualquer uma destas alterações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do Problema]</td> 
      <td>Edite qualquer parte deste texto, retirada da linha de assunto do email.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Edite qualquer parte deste texto, que é retirada do corpo do email.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Atribuir a]</td> 
      <td>Clique em <strong>[!UICONTROL Atribuir a]</strong>, clique no link <strong>[!UICONTROL Atribuir esta a]</strong> que é exibida, comece digitando o nome da pessoa e clique nele quando ele for exibido na lista abaixo. Repita isso para cada pessoa que deseja adicionar e clique em <strong>[!UICONTROL Salvar]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Prioridade]</td> 
      <td>Clique na seta suspensa e, em seguida, clique na prioridade desejada para a ocorrência.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir anexos de email]</td> 
      <td> <p>(Disponível somente se o email contiver pelo menos um anexo.) Clique nesta opção para salvar anexos no email na área [!UICONTROL Documentos] do problema. </p> <p>Para não salvar um anexo, clique no X à direita do seu nome. </p> <p>Se o email contiver links para documentos no [!DNL Google Drive], elas serão salvas na guia [!UICONTROL Visão geral] do problema que você está criando. </p> <p>Importante: para que isso funcione, seu [!DNL Workfront] o administrador deve autorizar [!DNL Google Drive] para trabalhar com documentos no [!DNL Workfront], conforme descrito na seção <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurar integrações para gerenciar documentos</a> no artigo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurar integrações de documentos</a>.</p> <p>Se você habilitar essa opção, ela permanecerá habilitada para outros emails convertidos em tarefas, problemas e atualizações.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Incluir arquivo de email</td> 
      <td> <p>Clique nessa opção para salvar o email original como um arquivo de email (EML) (Email) <span>à área [!UICONTROL Documentos]</span> do problema. A partir daí, você pode clicar duas vezes no arquivo para abrir o email em seu aplicativo de email.</p> <p>Se você habilitar essa opção, ela permanecerá habilitada para outros emails convertidos em tarefas, problemas e atualizações.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar Problema]**.

   A variável **[!UICONTROL Detalhes]** para o novo problema é exibida na guia [!DNL Workfront for G Suite] painel. Você pode clicar em **[!UICONTROL Atualizações]** e comece a se comunicar com os colaboradores imediatamente, sem deixar sua caixa de entrada.

   Na parte inferior do **[!UICONTROL Detalhes]** , você também pode clicar em **[!UICONTROL Exibir no Workfront]** para ver o novo problema no Workfront.

   Ao atualizar o navegador, uma mensagem com um link na parte inferior do [!UICONTROL Workfront para G Suite] O painel confirma que você converteu o email em um problema:

   Você pode clicar no link para ir para a visualização de Detalhes, na [!DNL Workfront for G Suite] para o problema criado.

   Você pode repetir essas etapas para converter o mesmo email em vários problemas. Quando você atualiza seu navegador ou retorna ao email em outro momento, todos os links criados para o email são listados na parte inferior do [!UICONTROL Workfront para G Suite] painel.

1. (Opcional) Continue a trabalhar com o problema na [!DNL Workfront for G Suite] ao executar uma das ações a seguir:

   * Para adicionar uma atualização no **[!UICONTROL Atualizações]** clique em **[!UICONTROL Iniciar uma nova atualização]** e digite a atualização.

   * Para responder a uma atualização sobre o **[!UICONTROL Atualizações]** clique em **[!UICONTROL Responder]** e digite sua resposta.

     Para ambas as ações acima, você pode notificar usuários específicos sobre seu comentário. Clique em **[!UICONTROL Notificar]**, comece digitando o nome de um usuário e clique no nome quando ele for exibido na lista suspensa. Repita esse processo para outros usuários que deseja notificar e, em seguida, clique em **[!UICONTROL Publicar]**.

   * Clique em **[!UICONTROL Documentos]** para ver todos os documentos salvos com a ocorrência.
