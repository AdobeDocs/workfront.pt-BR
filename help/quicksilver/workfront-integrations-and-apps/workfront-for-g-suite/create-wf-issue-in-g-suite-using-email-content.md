---
product-area: workfront-integrations;projects
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Criar um  [!DNL Adobe Workfront] problema no Google Workspace usando conteúdo de email
description: Você pode converter um email externo (não gerado por [!DNL Adobe Workfront)] em um problema [!DNL Workfront] a.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 7a15f557-67d8-4be8-8538-4bce06536c0a
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Criar um problema do [!DNL Adobe Workfront] no [!DNL Google Workspace] usando conteúdo de email

>[!NOTE]
>
>A versão mais recente do plug-in do Adobe Workfront para Google foi lançada em 26 de junho de 2023.

Você pode converter um email externo (não gerado por [!DNL Adobe Workfront]) em um problema de [!DNL Workfront].

Você também pode converter um email externo em uma atualização sobre um problema existente. Para obter mais informações, consulte [Atualizar um [!DNL Adobe Workfront] item de [!DNL Google Workspace] usando conteúdo de email](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Para obter informações sobre como usar o [!DNL Google Workspace] para trabalhar com emails de notificação enviados por [!DNL Workfront], consulte [Gerenciar [!DNL Adobe Workfront] detalhes de notificação de [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Antes de criar um problema com o [!DNL Google Workspace], você deve

* Instalar [!DNL Workfront for Google Workspace]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Criar um problema do [!DNL Adobe Workfront] no [!DNL Google Workspace] usando conteúdo de email

1. Se o painel [!UICONTROL Workfront para Google Workspace] não for exibido, clique no [!DNL Workfront] ícone ![Workfront ícone](assets/wf-lion-icon.png) na barra lateral de complementos [!DNL Google Workspace] na extremidade direita da página.
1. Com a mensagem de email aberta no [!DNL Google Workspace], clique em uma opção no [!DNL Workfront for Google Workspace] para converter o email em um novo problema do [!DNL Workfront].

   ![Converter email](assets/convert-email-task-issue-update.png)

1. Se quiser anexar o problema a um projeto pai, clique em **[!UICONTROL Nome do projeto]**, comece digitando o nome do projeto no qual deseja o problema e clique no nome do projeto quando ele aparecer na lista abaixo.
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
      <td>Clique em <strong>[!UICONTROL Atribuir a]</strong>, clique na opção <strong>[!UICONTROL Atribuir a]</strong> que é exibida, em seguida, comece a digitar o nome da pessoa e clique nele quando ele aparecer na lista abaixo. Repita isso para cada pessoa que deseja adicionar e clique em <strong>[!UICONTROL Salvar]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Prioridade]</td> 
      <td>Clique na seta suspensa e, em seguida, clique na prioridade desejada para a ocorrência.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir anexos de email]</td> 
      <td> <p>(Disponível somente se o email contiver pelo menos um anexo.) Clique nesta opção para salvar anexos no email na área [!UICONTROL Documentos] do problema. </p> <p>Para não salvar um anexo, clique no X à direita do seu nome. </p> <p>Se o email contiver links para documentos no [!DNL Google Drive], eles serão salvos na guia [!UICONTROL Visão geral] do problema que você está criando. </p> <p>Importante: para que isso funcione, o administrador do [!DNL Workfront] deve autorizar o [!DNL Google Drive] a trabalhar com documentos no [!DNL Workfront], conforme descrito na seção <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurar integrações para gerenciar documentos</a> do artigo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurar integrações de documentos</a>.</p> <p>Se você habilitar essa opção, ela permanecerá habilitada para outros emails convertidos em tarefas, problemas e atualizações.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Incluir arquivo de email</td> 
      <td> <p>Clique nesta opção para salvar o email original como um arquivo de Email (EML) (Email) <span>na área [!UICONTROL Documentos]</span> do problema. A partir daí, você pode clicar duas vezes no arquivo para abrir o email em seu aplicativo de email.</p> <p>Se você habilitar essa opção, ela permanecerá habilitada para outros emails convertidos em tarefas, problemas e atualizações.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar Problema]**.

   A guia **[!UICONTROL Detalhes]** do novo problema é exibida no painel [!DNL Workfront for Google Workspace]. Você pode clicar em **[!UICONTROL Atualizações]** e começar a se comunicar com os colaboradores imediatamente, sem deixar sua caixa de entrada.

   Na parte inferior da guia **[!UICONTROL Detalhes]**, você também pode clicar em **[!UICONTROL Exibir no Workfront]** para ir para o novo problema no Workfront.

   Quando você atualiza o navegador, uma mensagem com um link na parte inferior do painel [!UICONTROL Workfront para Google Workspace] confirma que você converteu o email em um problema:

   Você pode clicar no link para ir para o modo de exibição Detalhes, no painel [!DNL Workfront for Google Workspace], do problema que você criou.

   Você pode repetir essas etapas para converter o mesmo email em vários problemas. Quando você atualizar o navegador ou retornar ao email em outro momento, todos os links criados para o email serão listados na parte inferior do painel do [!UICONTROL Workfront para Google Workspace].

1. (Opcional) Continue a trabalhar com o problema no painel [!DNL Workfront for Google Workspace] seguindo um destes procedimentos:

   * Para adicionar uma atualização na guia **[!UICONTROL Atualizações]**, clique em **[!UICONTROL Iniciar uma nova atualização]** e digite a atualização.

   * Para responder a uma atualização na guia **[!UICONTROL Atualizações]**, clique em **[!UICONTROL Responder]** e digite sua resposta.

     Para ambas as ações acima, você pode notificar usuários específicos sobre seu comentário. Clique em **[!UICONTROL Notificar]**, comece a digitar o nome de um usuário e depois clique no nome quando ele aparecer na lista suspensa. Repita esse processo para outros usuários que deseja notificar e clique em **[!UICONTROL Postar]**.

   * Clique na guia **[!UICONTROL Documentos]** para ver todos os documentos salvos com o problema.
