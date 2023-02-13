---
product-area: workfront-integrations;projects
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Crie um [!DNL Adobe Workfront] tarefa no G Suite usando conteúdo de email
description: Você pode converter um email externo (não gerado pelo Adobe) [!DNL Workfront]) a uma tarefa do Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 6bbb4301-2791-4d72-bad8-fef63d6e892a
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# Crie um [!DNL Adobe Workfront] tarefa em [!DNL G Suite] uso de conteúdo de email

Você pode converter um email externo (não gerado por [!DNL Adobe Workfront]) a um [!DNL Workfront] tarefa.

Também é possível converter um email externo em uma atualização de uma tarefa existente. Para obter mais informações, consulte [Atualize um [!DNL Adobe Workfront] item do [!DNL G Suite] usando conteúdo de email](../../workfront-integrations-and-apps/workfront-for-g-suite/update-wf-item-using-email-content.md).

Para obter informações sobre como usar [!DNL G Suite] para trabalhar com emails de notificação enviados por [!DNL Workfront], consulte [Gerenciar [!DNL Adobe Workfront] detalhes da notificação do [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/manage-wf-email-notification-details-in-gsuite.md).

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

Antes de criar um [!DNL Workfront] tarefa em [!DNL G Suite], você deve

* Instalar [!DNL Workfront for G suite]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Crie um [!DNL Adobe Workfront] tarefa em [!DNL G Suite] uso de conteúdo de email

1. Se a variável [!UICONTROL Workfront para G Suite] não for exibido, clique no botão [!DNL Workfront] ícone ![](assets/wf-lion-icon.png) no [!DNL G Suite] barra lateral dos complementos na extremidade direita da página.
1. Com a mensagem de email aberta em [!DNL G Suite], clique em uma opção em [!DNL Workfront for G Suite] para converter o email em um novo [!DNL Workfront] tarefa.

   ![](assets/convert-email-task-issue-update.png)

1. Selecione um **[!UICONTROL Criar novo]** opção para indicar se a tarefa fará parte de um projeto ou de uma tarefa pessoal independente de um projeto.
1. Se quiser anexar a tarefa a um projeto pai, clique em **[!UICONTROL Nome do projeto]**, comece digitando o nome do projeto onde deseja que a tarefa seja executada e clique no nome do projeto quando ele for exibido na lista abaixo.
1. Faça qualquer uma dessas alterações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da tarefa]</td> 
      <td>Edite qualquer parte desse texto, que é retirada da linha de assunto do email.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Edite qualquer parte desse texto, que é retirada do corpo do email.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Atribuir a]</td> 
      <td>Clique em <strong>[!UICONTROL Atribuir a]</strong>, clique no botão <strong>[!UICONTROL Atribuir a]</strong> , que é exibida, comece a digitar o nome da pessoa e clique nele quando ele for exibido na lista abaixo. Repita isso para cada pessoa que deseja adicionar e clique em <strong>[!UICONTROL Salvar]</strong>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Duração planejada]</td> 
      <td> <p>Clique em <strong>[!UICONTROL Duração planejada]</strong>e digite o número de dias que deseja que a tarefa leve. </p> <p>Observação: Essa opção pode ser configurada para sua organização de diferentes maneiras. Por exemplo, para sua organização, talvez seja necessário digitar um número de horas em vez de dias. Se precisar de mais informações, consulte [!DNL Workfront] administrador. Se desejar especificar um período de tempo diferente do padrão configurado, digite <strong>m</strong>, <strong>h</strong>, <strong>d</strong>, <strong>w</strong>ou <strong>mo</strong> após o número para indicar minutos, horas, dias, semanas ou meses.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Prioridade]</td> 
      <td>Clique na seta suspensa e, em seguida, clique na prioridade desejada para a tarefa.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir anexos de email]</td> 
      <td> <p>(Disponível somente se o email tiver pelo menos um anexo.) Clique nesta opção para salvar anexos no email na área [!UICONTROL Documents] da tarefa. </p> <p>Se não quiser salvar um anexo, clique no X à direita do nome. </p> <p>Se o email contiver links para documentos em [!DNL Google Drive], eles são salvos na guia [!UICONTROL Visão geral] da tarefa que você está criando. </p> <p>Importante: Para que isso funcione, [!DNL Workfront] o administrador deve autorizar [!DNL Google Drive] para trabalhar com documentos em [!DNL Workfront], conforme descrito na seção <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md#configur" class="MCXref xref">Configurar integrações para gerenciar documentos</a> no artigo <a href="../../administration-and-setup/configure-integrations/configure-document-integrations.md" class="MCXref xref">Configurar integrações de documentos</a>.</p> <p>Se você ativar essa opção, ela permanecerá ativada para outros emails convertidos em tarefas, problemas e atualizações.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Incluir arquivo de email]</td> 
      <td> <p>Clique nesta opção para salvar o email original como um arquivo de email (EML) <span>à área [!UICONTROL Documents]</span> da tarefa. A partir daí, você pode clicar duas vezes no arquivo para abrir o email em seu aplicativo de email.</p> <p>Se você ativar essa opção, ela permanecerá ativada para outros emails convertidos em tarefas, problemas e atualizações.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar tarefa]**.

   O **[!UICONTROL Detalhes]** para a nova tarefa é exibida na guia [!DNL Workfront for G Suite] painel. Você pode clicar em **[!UICONTROL Atualizações]** e comece a se comunicar com colaboradores imediatamente, sem deixar sua caixa.

   Na parte inferior do **[!UICONTROL Detalhes]** , você também pode clicar em **[!UICONTROL Exibir em[!DNL Workfront]]** para acessar a nova tarefa no Workfront.

   Ao atualizar o navegador, uma mensagem com um link na parte inferior do [!DNL Workfront for G Suite] O painel confirma que você converteu o email em uma tarefa:

   ![](assets/email-was-converted.png)

   Você pode clicar no link para ir para a exibição Detalhes, dentro do [!DNL Workfront for G Suite] painel, para a tarefa criada.

   Você pode repetir essas etapas para converter o mesmo email em várias tarefas. Ao atualizar seu navegador ou retornar ao email em outro momento, todos os links criados para o email serão listados na parte inferior da variável [!UICONTROL Workfront para G Suite] painel.

1. (Opcional) Continue a trabalhar com a tarefa na [!DNL Workfront for G Suite] , executando um dos seguintes procedimentos:

   * Para adicionar uma atualização no **[!UICONTROL Atualizações]** clique em **[!UICONTROL Iniciar uma nova atualização]** e digite a atualização.

   * Para responder a uma atualização no **[!UICONTROL Atualizações]** clique em **[!UICONTROL Responder]** e digite sua resposta.

      Para ambas as ações acima, você pode notificar usuários específicos sobre seu comentário. Clique em **[!UICONTROL Notificar]**, comece a digitar o nome de um usuário e clique no nome quando ele for exibido na lista suspensa. Repita esse processo para outros usuários que deseja notificar e clique em **[!UICONTROL Post]**.

   * Clique no botão **[!UICONTROL Documentos]** para ver quaisquer documentos salvos com a tarefa.

Você pode repetir essas etapas para converter o mesmo email em várias tarefas. Ao atualizar seu navegador ou retornar ao email em outro momento, todos os links criados para o email serão listados na parte inferior da variável [!DNL Workfront for G Suite] painel.
