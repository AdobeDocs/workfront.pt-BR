---
product-area: workfront-integrations;projects
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Criar uma tarefa  [!DNL Adobe Workfront]  no Google Workspace usando conteúdo de email
description: Você pode converter um email externo (não gerado pelo Adobe [!DNL Workfront]) em uma tarefa do Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 0%

---

# Criar uma tarefa [!DNL Adobe Workfront] em [!DNL Google Workspace] usando conteúdo de email

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a seguinte funcionalidade do Workfront para Google Workspace não estará disponível após **28 de fevereiro de 2026**:
>
>* Acesso à funcionalidade Google Workspace no Workfront
>
>* Exibir e gerenciar tarefas do Workfront no Gmail ou no painel do site Calendário do Google
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Google Workspace.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Google Workspace, consulte [módulos do Gmail](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) e [módulos do Google Calendar](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Você pode converter um email externo (não gerado por [!DNL Adobe Workfront]) em uma tarefa [!DNL Workfront].

Você também pode converter um email externo em uma atualização em uma tarefa existente. Para obter mais informações, consulte [Atualizar um [!DNL Adobe Workfront] item de [!DNL Google Workspace] usando conteúdo de email](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Para obter informações sobre como usar o [!DNL Google Workspace] para trabalhar com emails de notificação enviados por [!DNL Workfront], consulte [Gerenciar [!DNL Adobe Workfront] detalhes de notificação de [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p><p>Trabalhar ou superior</p>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de criar uma tarefa [!DNL Workfront] em [!DNL Google Workspace], você deve

* Instalar [!DNL Workfront for Google Workspace]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Criar uma tarefa [!DNL Adobe Workfront] em [!DNL Google Workspace] usando conteúdo de email

1. Se o painel [!UICONTROL Workfront para Google Workspace] não for exibido, clique no [!DNL Workfront] ícone ![Workfront ícone](assets/wf-lion-icon.png) na barra lateral de complementos [!DNL Google Workspace] na extremidade direita da página.
1. Com a mensagem de email aberta no [!DNL Google Workspace], clique em uma opção no [!DNL Workfront for Google Workspace] para converter o email em uma nova tarefa do [!DNL Workfront].

1. Selecione uma opção **[!UICONTROL Criar novo]** para indicar se a tarefa fará parte de um projeto ou de uma tarefa pessoal que seja independente de um projeto.
1. Se quiser anexar a tarefa a um projeto pai, clique em **[!UICONTROL Nome do projeto]**, comece digitando o nome do projeto no qual deseja a tarefa e clique no nome do projeto quando ele aparecer na lista abaixo.
1. Faça qualquer uma destas alterações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da tarefa]</td> 
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
      <td role="rowheader">[!UICONTROL Duração planejada]</td> 
      <td> <p>Clique em <strong>[!UICONTROL Duração planejada]</strong> e digite o número de dias que deseja que a tarefa dure. </p> <p>Observação: essa opção pode ser configurada para sua organização de diferentes maneiras. Por exemplo, para sua organização, talvez seja necessário digitar um número de horas em vez de dias. Se precisar de mais informações, consulte o administrador do [!DNL Workfront]. Se quiser especificar um período diferente do padrão configurado, digite <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong> ou <strong>mo</strong> após o número para indicar minutos, horas, dias, semanas ou meses.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Prioridade]</td> 
      <td>Clique na seta suspensa e clique na prioridade desejada para a tarefa.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir anexos de email]</td> 
      <td> <p>(Disponível somente se o email contiver pelo menos um anexo.) Clique nesta opção para salvar anexos no email na área [!UICONTROL Documentos] da tarefa. </p> <p>Para não salvar um anexo, clique no X à direita do seu nome. </p> <p>Se o email contiver links para documentos em [!DNL Google Drive], eles serão salvos na guia [!UICONTROL Visão geral] da tarefa que você está criando. </p> <p>Importante: para que isso funcione, o administrador do [!DNL Workfront] deve autorizar o [!DNL Google Drive] a trabalhar com documentos no [!DNL Workfront], conforme descrito na seção <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurar integrações para gerenciar documentos</a> do artigo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurar integrações de documentos</a>.</p> <p>Se você habilitar essa opção, ela permanecerá habilitada para outros emails convertidos em tarefas, problemas e atualizações.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir arquivo de email]</td> 
      <td> <p>Clique nesta opção para salvar o email original como um arquivo de email (EML) <span>na área [!UICONTROL Documentos]</span> da tarefa. A partir daí, você pode clicar duas vezes no arquivo para abrir o email em seu aplicativo de email.</p> <p>Se você habilitar essa opção, ela permanecerá habilitada para outros emails convertidos em tarefas, problemas e atualizações.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar tarefa]**.

   A guia **[!UICONTROL Detalhes]** da nova tarefa é exibida no painel [!DNL Workfront for Google Workspace]. Você pode clicar em **[!UICONTROL Atualizações]** e começar a se comunicar com os colaboradores imediatamente, sem deixar sua caixa de entrada.

   Na parte inferior da guia **[!UICONTROL Detalhes]**, você também pode clicar em **[!UICONTROL Exibir em[!DNL Workfront]]** para ir para a nova tarefa no Workfront.

   Quando você atualiza o navegador, uma mensagem com um link na parte inferior do painel do [!DNL Workfront for Google Workspace] confirma que você converteu o email em uma tarefa:

   Você pode clicar no link para ir para o modo de exibição Detalhes, no painel [!DNL Workfront for Google Workspace], da tarefa que você criou.

   Você pode repetir essas etapas para converter o mesmo email em várias tarefas. Quando você atualizar o navegador ou retornar ao email em outro momento, todos os links criados para o email serão listados na parte inferior do painel do [!UICONTROL Workfront para Google Workspace].

1. (Opcional) Continue a trabalhar com a tarefa no painel [!DNL Workfront for Google Workspace] seguindo um destes procedimentos:

   * Para adicionar uma atualização na guia **[!UICONTROL Atualizações]**, clique em **[!UICONTROL Iniciar uma nova atualização]** e digite a atualização.

   * Para responder a uma atualização na guia **[!UICONTROL Atualizações]**, clique em **[!UICONTROL Responder]** e digite sua resposta.

     Para ambas as ações acima, você pode notificar usuários específicos sobre seu comentário. Clique em **[!UICONTROL Notificar]**, comece a digitar o nome de um usuário e depois clique no nome quando ele aparecer na lista suspensa. Repita esse processo para outros usuários que deseja notificar e clique em **[!UICONTROL Postar]**.

   * Clique na guia **[!UICONTROL Documentos]** para ver todos os documentos salvos com a tarefa.

Você pode repetir essas etapas para converter o mesmo email em várias tarefas. Quando você atualizar o navegador ou retornar ao email em outro momento, todos os links criados para o email serão listados na parte inferior do painel do [!DNL Workfront for Google Workspace].
