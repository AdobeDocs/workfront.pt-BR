---
product-area: projects
navigation-topic: manage-issues
title: Criar problemas
description: Ao trabalhar em um projeto, você pode descobrir que eventos inesperados surgem. Você pode registrar esses eventos inesperados como problemas para um projeto específico ou de uma tarefa. Os usuários com acesso apropriado podem visualizar e monitorar o status dos problemas à medida que o projeto ou a tarefa avança até a conclusão, eliminando a necessidade de longas cadeias de email ou reuniões de status. Ao contrário das tarefas, que são eventos planejados, os problemas representam itens de trabalho não planejados no Adobe Workfront.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1540'
ht-degree: 0%

---

# Criar problemas

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

Ao trabalhar em um projeto, você pode descobrir que eventos inesperados surgem. Você pode registrar esses eventos inesperados como problemas para um projeto específico ou de uma tarefa. Os usuários com acesso apropriado podem visualizar e monitorar o status dos problemas à medida que o projeto ou a tarefa avança até a conclusão, eliminando a necessidade de longas cadeias de email ou reuniões de status. Ao contrário das tarefas, que são eventos planejados, os problemas representam itens de trabalho não planejados no Adobe Workfront.

Você também pode adicionar problemas a projetos como solicitações. Para obter informações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Problemas e solicitações são usados alternadamente no Workfront. Você pode registrar problemas em projetos e tarefas para indicar trabalho imprevisto que precisa ser resolvido. Você também pode enviar solicitações que são registradas como ocorrências em um projeto designado como uma Fila de solicitações.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior para adicionar problemas a um projeto ou tarefa</p> <p>Solicitação ou mais recente para adicionar problemas como solicitações, usando uma Fila de solicitações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior a projetos e tarefas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre acesso a problemas em seu Nível de Acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões do Contribute ou superior com capacidade para adicionar problemas à tarefa ou projeto em que você cria o problema</p> <p> Para obter informações sobre a concessão de permissões para problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a></p> <p>Para obter informações sobre como solicitar permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

+++

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitações na criação de problemas

Quando você tem o acesso e as permissões corretas, é possível criar problemas em um projeto ou tarefa. No entanto, os seguintes casos ocorrem quando talvez você não consiga criar problemas:

* O administrador do Workfront ou um administrador de grupo deve ativar a adição de problemas a um projeto com status Concluído ou Inativo na área Preferências do projeto. Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Não é possível adicionar problemas a um projeto que está em Aprovação pendente.

## Preparar o formulário Novo problema

Sua organização deve ter um processo bem definido para quando e como registrar um problema. Ao configurar esse processo, a primeira etapa é criar o formulário necessário para enviar um problema. Se você permitir que problemas sejam adicionados diretamente a tarefas e projetos, ou se tiver filas de solicitações em que problemas são enviados, será possível definir quais campos do Workfront, bem como quais campos personalizados estão disponíveis para os usuários quando eles enviam novos problemas e devem ser concluídos. O formulário Novo problema pode conter informações importantes que serão úteis para resolver o problema rapidamente.

Os campos para os novos problemas em um projeto são definidos na seção Detalhes da fila do projeto onde os problemas serão registrados. Para obter informações sobre como configurar a seção Detalhes da Fila do projeto, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Para obter informações sobre como criar problemas enviando-os para uma fila de solicitações, consulte a seção [Criar problemas inserindo uma nova solicitação](#create-issues-by-entering-a-new-request) neste artigo.

## Criar problemas em uma tarefa ou projeto usando o botão Novo Problema

Depois de definir os campos de um novo formulário de problema em seu projeto, você pode começar a criar problemas.

<!-- OLD UI: redesigned on Oct 26, 2023:

Creating issues differs depending on which environment you choose to create the issue. 

### Create issues on a task or project using the New Issue button in the Production environment

To create an issue on a task or a project:

1. Go to a project where you want to create the issue. 
1. (Optional) If you want to log the issue for a task, go to the **Tasks** area, then click the name of a task. 
1. Click the **Issues** section.

   
1. Click **New Issue**.

  

1. (Conditional) If the project creator created Queue Topics or Topic Groups on the project they are added to the new issue form. Specify the **Topic Group** or the **Queue Topic** of your new issue. Topic Groups and Queue Topics have names customized to your environment.  
   For more information about creating Topic Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![New issue screen](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * If there is only one Queue Topic set on the project, it is displayed automatically.
   * If the Topic Group does not have any Queue Topics or Topic Groups under it, nothing is available in the Topic Group drop-down.

1. (Conditional) If the project creator allowed for the **Request Type** field to display on the New Issue form, select the type of your issue from the following options:

   * Bug Report
   * Change Order
   * Issue
   * Request  
     Depending on how your Workfront administrator has configured your Project Preferences, the names of the issue types might be different for you. 

   >[!TIP]
   >
   >The Request Types must be enabled in the Queue Details and as well as when creating the Queue Topic to display as a selection in the New Issue form. For information, see the following articles: 
   >* [Create a Request Queue](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Create Queue Topics](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Add a name for the new issue in the **Issue Name** field. 
1. Continue specifying the fields available in the **New Issue** form. For more information about the fields available as you enter a new issue, see [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Not all the issue-related fields are available in the New Issue form. The project creator enables the fields available when creating an issue when they define the Queue Details area of the project. For more information, see [Create a Requests Queue](../../requests/create-and-manage-request-queues/create-request-queue.md). 


1. (Conditional) If the Queue Topics are associated with a custom form, that custom form will display in the **New Issue** form.  
   Or  
   If the project is associated with an issue custom form through the Queue Details area, the form displays in the **New Issue** form, after the default Workfront fields.

   For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click **Save New Issue.**

Issues can be assigned to multiple users, job roles or to a team. For more information about assigning and managing requests, see [Manage work and team requests](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content:
-->

Para criar um problema em uma tarefa ou um projeto:

1. Vá para um projeto em que deseja criar o problema.
1. (Opcional) Se quiser registrar o problema de uma tarefa, vá para a área **Tarefas** e clique no nome de uma tarefa.
1. Clique na seção **Problemas**.

   A lista de problemas do projeto é exibida

1. Clique em **Novo problema** na parte superior da lista de problemas.
A caixa Nova ocorrência é exibida.

   ![Caixa Novo problema](assets/new-issue-box-matches-new-request-ui.png)

1. (Condicional) Se o criador do projeto criou Tópicos de fila ou Grupos de tópicos no projeto, eles serão adicionados ao novo formulário de problema. Especifique o **Grupo de Tópicos** ou o **Tópico da Fila** do novo problema. Grupos de tópicos e Tópicos de fila têm nomes personalizados para o seu ambiente.\
   Para obter mais informações sobre como criar Grupos de Tópicos, consulte [Criar Grupos de Tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obter mais informações sobre como criar Tópicos da Fila, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Se houver apenas um Tópico da fila definido no projeto, ele será exibido automaticamente.
   * Se o Grupo de tópicos não tiver nenhum Tópico ou Grupo de tópicos na fila, nada estará disponível no menu suspenso Grupo de tópicos.

1. Adicione o nome do problema no campo **Assunto** e adicione uma **Descrição**.

1. (Condicional) Se o criador do projeto permitiu que o campo **Tipo de solicitação** fosse exibido no formulário Novo problema, selecione o tipo do seu problema dentre as seguintes opções:

   * Relatório de erro
   * Pedido de alteração
   * Problema
   * Solicitar\
     Dependendo de como o administrador do Workfront configurou as Preferências do projeto, os nomes dos tipos de problemas podem ser diferentes para você.

   >[!TIP]
   >
   >Os Tipos de solicitação devem ser ativados em Detalhes da fila e ao criar o Tópico da fila para ser exibido como uma seleção no formulário Novo problema. Para obter informações, consulte os seguintes artigos:
   >* [Criar uma Fila de Solicitações](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Criar Tópicos de Fila](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Continue especificando os campos disponíveis no formulário **Novo problema**. Para obter mais informações sobre os campos disponíveis quando você insere um novo problema, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Nem todos os campos relacionados a problemas estão disponíveis no formulário Novo problema. O criador do projeto ativa os campos disponíveis ao criar um problema ao definir a área Detalhes da fila do projeto. Para obter mais informações, consulte [Criar uma fila de solicitações](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Condicional) Se os Tópicos da fila estiverem associados a um formulário personalizado, ele será exibido no formulário **Novo problema**.\
   Ou\
   Se o projeto estiver associado a um formulário personalizado de problema por meio da área Detalhes da fila, o formulário será exibido no formulário **Novo problema**, após os campos padrão do Workfront.

   Para obter informações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clique em **Enviar**.

   Problemas podem ser atribuídos a vários usuários, funções de trabalho ou a uma equipe. Para obter mais informações sobre como atribuir e gerenciar solicitações, consulte [Gerenciar solicitações de trabalho e de equipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).


## Criar problemas em uma tarefa ou projeto em linha

>[!IMPORTANT]
>
>O proprietário do projeto deve habilitar **Permitir que os usuários adicionem problemas embutidos** ao definir configurações de problemas para o projeto antes que você possa adicionar problemas embutidos no projeto ou nas tarefas. Para obter informações sobre como definir configurações de problemas em um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Quando quiser adicionar vários problemas rapidamente, você pode criar problemas para uma tarefa ou um projeto em linha, adicionando-os a uma lista de problemas.

>[!NOTE]
>
>Ao adicionar problemas em linha, a Workfront não aplica o formulário Novo problema aos novos problemas. Não recomendamos adicionar problemas em linha se você quiser que os usuários forneçam determinadas informações ao inserir problemas. Isso pode ter um impacto negativo no relatório de problemas e, posteriormente, na capacidade do usuário atribuído ao problema de ter todas as informações necessárias para resolvê-lo.

Para criar problemas em linha:

1. Vá para um projeto em que deseja criar o problema.
1. (Opcional) Se quiser registrar o problema de uma tarefa, vá para a seção **Tarefas** e clique no nome de uma tarefa.
1. Clique na seção **Problemas** no painel esquerdo.
1. Clique em **Adicionar mais problemas** na parte inferior da lista de problemas.

   Uma nova linha é criada na lista de problemas na seção Problemas.

   >[!TIP]
   >
   >Essa opção estará esmaecida se a configuração Permitir que os usuários adicionem problemas em linha estiver desmarcada na caixa Editar projeto. Para obter informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![Botão Adicionar mais problemas](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Comece digitando o nome do problema no campo Nome e continue adicionando mais informações sobre o problema em linha.

   >[!TIP]
   >
   >Os campos disponíveis para edição em linha são disponibilizados pela visualização aplicada à lista de problemas. Talvez não seja possível editar em linha os seguintes tipos de campos:
   >   
   >* Campos que pertencem a outro objeto
   >* Campos que você não tem acesso para editar
   >* Campos que são cálculos e que são atualizados automaticamente pelo Workfront

1. Clique em Inserir para concluir a edição em linha e adicionar o problema ao projeto ou tarefa.

## Criar problemas inserindo uma nova solicitação {#create-issues-by-entering-a-new-request}

Você pode designar projetos para serem recipientes de problemas de recebimento. Esses tipos de projetos são chamados de Filas de solicitações no Workfront. Você pode acessar Filas de solicitações por meio da área Solicitações no Menu principal.

>[!TIP]
>
>Os termos &quot;problema&quot; e &quot;solicitação&quot; são intercambiáveis no Workfront.

Para obter mais informações sobre como configurar projetos como Filas de solicitações para receber problemas, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Para obter informações sobre o envio de solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
