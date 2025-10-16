---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar uma fila de solicitações
description: Você pode configurar uma Fila de solicitações onde os usuários podem inserir solicitações ocasionais que não são trabalhos planejados em um projeto. Por exemplo, uma fila de solicitações de Help Desk pode ser configurada para capturar todas as solicitações de usuário que chegam a um departamento de TI.
author: Becky
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '2843'
ht-degree: 2%

---


# Criar uma fila de solicitações

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--hide/ comment out the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Você pode configurar uma Fila de solicitações onde os usuários podem inserir solicitações ocasionais que não são trabalhos planejados em um projeto. Por exemplo, uma fila de solicitações de Help Desk pode ser configurada para capturar todas as solicitações de usuário que chegam a um departamento de TI.

As solicitações se tornam problemas no Adobe Workfront e são adicionadas aos projetos.

Configurar uma fila de solicitações ajuda a formalizar informações sobre problemas que serão adicionados a um projeto. Todos os problemas enviados ao projeto serão enviados da mesma forma e seguirão o mesmo caminho para a conclusão.

Você pode configurar os seguintes objetos como filas de solicitações no Workfront:

* Projetos
* Modelos. Os projetos criados a partir dos modelos configurados como filas de solicitações se tornarão filas de solicitações.

Para configurar um projeto ou um modelo como uma fila de solicitações, edite a área Detalhes da fila do projeto ou do modelo.

Este artigo descreve como configurar um projeto como uma fila de solicitações, em que os usuários podem enviar solicitações. A configuração de Detalhes da fila para um modelo é semelhante à configuração no projeto.

Para obter informações sobre como enviar uma nova solicitação para uma fila de solicitações, consulte [Copiar e enviar solicitações](../create-requests/copy-and-submit-requests.md).

Para obter informações sobre como configurar um formulário de solicitação no Workfront Planning, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Standard </p>
   <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visão geral das filas de solicitações

Configurar uma fila de solicitações como um projeto. Ao designar o projeto como uma Fila de solicitações, a fila torna-se acessível a partir da área Solicitações do Adobe Workfront. Ao personalizar a Fila de solicitações, você também personaliza o formulário que os usuários preenchem ao enviarem as solicitações.

Este artigo descreve como criar uma fila de solicitações a partir de um projeto existente. No entanto, para criar consistência para o processo de entrada de solicitação ou para adicionar várias camadas a ele para fins de relatório e melhor gerenciamento, também é possível configurar blocos de construção adicionais de uma fila de solicitações, que são descritos na tabela a seguir.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Detalhes da fila</td> 
   <td> <p>Você deve configurar um projeto como uma fila de solicitações na área Detalhes da fila. Esta etapa é obrigatória. </p> <p>Para obter mais informações, consulte a seção <a href="#create-a-request-queue" class="MCXref xref">Criar uma fila de solicitações</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Grupos de Tópicos</td> 
   <td> <p>São menus adicionais que classificam solicitações com base em recursos comuns. Por exemplo, para uma Fila de solicitação de TI, você pode querer ter grupos de tópicos "No local" e "Remoto". </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Criar grupos de tópicos</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enfileirar tópicos</td> 
   <td> <p>São menus adicionais que classificam solicitações que pertencem ao mesmo Grupo de tópicos com base em recursos comuns. Um grupo de tópicos pode conter vários tópicos da fila. </p> <p>Por exemplo, o grupo de tópicos "No local" da Fila de solicitação de TI pode conter os tópicos "Hardware", "Software" e "Rede" da fila. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar tópicos da fila</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Regras de Encaminhamento</td> 
   <td> <p>Eles permitem encaminhar cada solicitação a um usuário, função de trabalho, equipe ou projeto. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar Regras de Roteamento</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar uma fila de solicitações

<!--at production release on April 10, do the following: take the first sentence here out; hide/ comment out the first section (Create a Request Queue in the Production environment); remove the title of the "Create a Request Queue in the Preview environment and leave that section as the only way to create request queues; search for any visible references of production/ preview and remove them from the entire article-->

A criação de uma fila de solicitações difere dependendo do ambiente usado.

<!--

### Create a Request Queue in the Production environment

This section describes how you can define Queue Details for the following objects:

* A project in the Production environment
* A template in the Production or Preview environment

When you set up a project as a Request Queue, the project status must be Current in order to display in the Requests area of Workfront.

>[!TIP]
>
>Your Workfront or group administrator might assign you to a custom Layout Template that might not include some of the sections described in the following steps.


To create a Request Queue:

1. Go to the project that you want to set up as a Request Queue.
1. (Optional) Click **Project Details** in the left panel and add a **Description** to the project in the **Overview** area. This information displays on all new requests.
1. Click **Queue Details** in the left panel. 

   This opens the Queue Details section.

   ![Queue Details top of the section](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)   

1. Specify the following information:

   * **Publish as Help Request Queue:** Select this option to identify this project as a request queue. All incoming issues are considered Requests.  
     When this option is not selected, the project behaves like a standard project in Workfront and all incoming issues are issues.
   
   * **Who can add requests to this queue:** Select which users have access to add requests to this queue. You can allow the following groups of people to see the Request Queue in their Requests area of the Global Navigation Bar when they add a new request:

     |Who can enter requests | Description|
     |---|---|
     | Anyone  |Any Workfront user with an active account can view this request queue and add requests to it |
     | People with view access to this project |Users with View permissions to the project can view and add requests to this queue |
     | People in this project's company |Users who belong to the company associated with this project can view and add requests to this queue. If there is a company associated with the project, the name of the company is listed in parentheses after this setting.  |
     | People in this project's group |Users who belong to the group associated with this project can view and add requests to this queue. If there is a group associated with the project, the name of the group is listed in parentheses after this setting, in gray font.  |

   * **Share with these links:** The following options enable you to provide direct access to the Request Queue and the forms associated with it to users outside of Workfront or to Workfront users using an external page. For information about embedding a request queue in a dashboard as an external page, see [Embed a request queue in a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Users must already have access rights to the Request Queue in order to gain direct access. Using either option described here does not automatically grant access to users.

     >[!TIP]
     >
     >Users must first log in to Workfront before gaining access to the request queue when they access the Request Queue page from another application.

      * **Direct Access URL:** When a user accesses this URL from a browser, the user is taken directly to the New Request  section in the Requests area and this request is selected by default for them.

        ![Share request queue with direct URL embedded in dashboard](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >You can display a Request Queue in a dashboard as an external page. In this case, the request queue is preselected, but you can select any other request queue from the Request Type field. users can change the Request Type. Navigation components of the Requests also display.

      * **Embed Code:** Use this HTML code to embed the request queue form as an iframe within any HTML page.  
        If users are not already authenticated to Workfront when they view the page where the code is embedded, the Workfront login dialog box is displayed. After users log in, the Request Queue form is displayed.

        >[!NOTE]
        >
        >When displaying a Request Queue in an iframe, only the request form displays, the request name is preselected and dimmed. User cannot change the Request type. Navigation components of the Requests area do not display.

        In order for the request queue form to be displayed when using this embed code, you must enable the "Allow embedding of Workfront in an iframe" setting in your system setup. For more information about enabling embedding of Workfront in an iframe, see [Configure system security preferences](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). If this setting is not enabled, the iframe is displayed as blank.

        You can adjust various aspects of how the embedded form is displayed, as follows:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Functionality</strong> </p> </th> 
           <th> <p><strong>Solution</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Adjust the size of the frame</p> </td> 
           <td> <p>Modify the "width" and "height" attributes.</p> <p>By default, the width is "500" and the height is "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direct users to a specific Queue Topic or Topic Group</p> </td> 
           <td> <p>Add the "path" parameter to the src URL. You can find the path parameter by navigating to the desired Queue Topic or Topic Group in the non-embedded form and inspecting the URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Show and allow users to change the pre-configured Topic Group drop-down list</p> </td> 
           <td> <p>Use the "path" parameter by adding the <code>showPreSelectedOptions=true</code> parameter to the <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detect when the form has been submitted</p> </td> 
           <td> <p>Add a "message" event listener to your web page's window and checking if <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> will be set to the ID of the created issue.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Request Types:** Select from the default options below.

     The Workfront administrator can rename the default request types. For more information about renaming the request types, see [Customize default issue types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Bug Report
      * Change Order
      * Issue
      * Request

        This is a required field and you must select at least one option.

     >[!NOTE]
     >
     >Request Types display as a selection in the Requests area only if the Request Type is selected in both the Queue Details and the Queue Topic pages. For information about setting up the Queue Details area of a project, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Each type selected here will be available on the form (you can select more than one). Selecting more than one type can help organize multiple requests coming in.  
     For example, if you are using the form on a request queue for an IT project, the following request types can come in to the queue: hardware, software, bug fixes, and issues.

   * **Default Duration:** The default duration is the length of time it typically takes to complete an issue. This becomes the default for all incoming issues and can be modified manually. Duration is generally set in hours, days, or weeks. The Default Duration of an issue is the same as the Planned Hours on the issue. The Planned Completion Date of the issue calculates based on this field.  
     The default for the issue Duration is 1 day or 8 hours. If your Workfront administrator set the Typical Hours per Work Day as less than 8 hours, the Default Duration for issues is still 8 hours. For example, if the Typical Hours per Work Day is set to 7 hours, the Default Duration for issues is 1.14 Days or 8 hours. For more information about how to set up the system Typical Hours per Work Day, see the "Timeline Calculations" section in the article [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
   
   * **People from the same company will inherit the same permissions for all requests.:** When selected, all requests submitted to the queue are visible for users in the same company. Users can view these requests in the All Requests  section , located within the Requests area. At the time that this setting is enabled or disabled, it impacts all future requests; it does not retroactively impact information. 
   * **When someone makes a request, automatically grant:** When a user makes a request to the request queue, the user is automatically granted the level of permission that you choose to that request. Select from the following permissions levels: 

      * **View Access** 
      * **Contribute Access**. This is the default selection.
      * **Manage Access**

     For information about the Workfront permissions model, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).   
     Setting permissions here saves time, rather than having to grant permissions for each individual incoming request. Choosing this option impacts all future requests, but does not retroactively impact existing requests. 
   
   * **Default Approval**: Associate an approval process with this request queue. Only Issue Approval Processes are visible in this drop-down menu. All issues submitted to this queue will be associated with this approval process. Your Workfront administrator must define system-level approval processes before you can associate them with request queues. Users with administrative access to Approval processes can also create group-specific approval processes.

     >[!IMPORTANT]
     >
     >If the group of the project changes, the group-specific approval process attached to existing issues becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see [How group and approval process changes affect assigned approval processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     If you have multiple queue topics associated with a request queue, we recommend that you associate approval processes with the queue topics instead. For more information about creating queue topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md). 
   
     Consider the following when adding approval processes to request queues:

      * Only active approval processes display in the list. 
      * System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.

   * **Default Route**: Associate a Routing Rule with this request queue. Use Routing Rules to automatically assign new issues submitted to a Request Queue to the correct resource (user, job role, or team), and to the correct project. All issues submitted to this queue will be associated with this Routing Rule. You must configure Routing Rules before they display in the Queue Details section and before you can associate them with request queue.  
     If you have multiple queue topics associated with a request queue, we recommend that you associate routing rules with the queue topics instead. For more information about creating routing rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
   
   * **New Issue Fields:** In the **Show the following selected fields to all users** section, select any fields that you want to be visible to all users who submit a request to the project or add an issue to the project or the tasks.

     >[!TIP]
     >
     >New Issue Fields selected in the Queue Details section are also associated with any new issue added to the project <!--this is confusing: or to the tasks in the Issues section-->.

<!--     When you enable any of the Assigned to, Job Role, or the Team fields, they are always renamed to Assignments in the request form, but you can only specify the type of assignment selected here.

      >[!NOTE]
      >
      >If you selected Assigned To in the Queue Details area, you can enter only users in the Assignments field on the request form. In this case, you cannot enter job roles or a team. 
   
   * **Documents**: If you select to display the Documents section in the new request form, select where the document uploading section should be positioned. Select from the following:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">After custom forms</td> 
        <td><span>The Documents section displays at the bottom of the request form.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Before custom forms</td> 
        <td> <p><span>The Documents section displays between the Workfront fields and the custom fields of the request form.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>   
   
     ![New issue fields area with documents](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Show all selected and unselected fields to:** Select which users you want to see all the fields on the new request form. The following options control the access to the fields on the form.
    
      |Which users can see all fields on the request form | Description|  
      |---|---| 
      | All Users (Plan Licenses) |All users who have a Plan license can see the selected as well as the unselected fields. |
      | People with view access to this project (Plan License) |Those users with a Plan license that also have View rights to this project can see the selected as well as the unselected fields. The rest of the users who can submit requests to this project can see just the selected fields. |
      | No Users |No users can see the unselected fields. All users who can submit requests to this project can only see the fields selected.  |
  
   * **Custom Forms**: Select a custom form to associate with the Request Queue. Only Issue Custom Forms are available to select from this drop-down menu. All issues submitted to the Request Queue will have the selected forms associated with them. You must create issue custom forms before you can see them displayed in the Queue Details section. 
     If you have multiple Queue Topics associated with a Request Queue, we recommend that you associate custom forms with the Queue Topics instead. For more information about creating sub-sections for the Request Queue, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Custom forms on Queue Details](assets/custom-forms-on-queue-details.png)

     If you have multiple custom forms associated with the Request Queue, drag and drop the forms to sort them in the desired order, in the **Reorder Forms** section.

     >[!TIP]
     >
     >Custom forms added to the Queue Details section are also associated with any new issue added to the project <!--this is confusiong: or the tasks in the Issues  section-->.

<!--1. Continue selecting information for the settings in the **Email Queue Settings** area, to allow users to email requests to the request queue project. 

    For more information, see [Enable users to email an issue into a Request Queue project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Click **Save**.  
   Your project has now been configured to be a Request Queue and users can now add requests to it. 

1. (Optional) To enhance the Request Queue functionality, build additional sub-sections for your queue, as well as rules to route the incoming requests to the correct team, assignee or project.

   * For information about creating sub-sections for the Request Queue, see the articles [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) and [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).  
   * For information about routing the requests to the appropriate assignee, team, and appropriate project, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   -->


### Criar uma fila de solicitações

Ao configurar um projeto como uma Fila de solicitações, o status do projeto deve ser Atual para ser exibido na área Solicitações do Workfront.

>[!TIP]
>
>O administrador do Workfront ou do grupo pode atribuir a você um modelo de layout personalizado que pode não incluir algumas das seções descritas nas etapas a seguir.

Para criar uma Fila de solicitações:

1. Vá para o projeto que você deseja configurar como uma Fila de solicitações.
1. (Opcional) Clique em **Detalhes do projeto** no painel esquerdo e adicione uma **Descrição** ao projeto na área **Visão geral**. Essas informações são exibidas em todas as novas solicitações.
1. Clique em **Detalhes da fila** no painel esquerdo.

   Isso abre a seção Detalhes da fila.

   ![Seção Tipo de Fila na área Detalhes da Fila](assets/unshimmed-queue-type-section-queue-details-area.png)

1. Especifique as seguintes informações:

   * **Publicar como Fila de Solicitação de Ajuda**: selecione essa opção para identificar esse projeto como uma fila de solicitações. Todos os problemas recebidos são considerados Solicitações.\
     Quando essa opção não está selecionada, o projeto se comporta como um projeto padrão no Workfront e todos os problemas recebidos são problemas.

   * **Quem pode adicionar solicitações a esta fila?**: Selecione quais usuários têm acesso para adicionar solicitações a esta fila. Você pode permitir que os seguintes grupos de pessoas vejam a Fila de solicitações em sua área Solicitações da Barra de navegação global quando adicionam uma nova solicitação:

     | Quem pode inserir solicitações | Descrição |
     |---|---|
     | Todos | Qualquer usuário do Workfront com uma conta ativa pode visualizar essa fila de solicitações e adicionar solicitações a ela |
     | Pessoas com acesso de visualização a este projeto | Usuários com permissões de Visualização no projeto podem visualizar e adicionar solicitações a esta fila |
     | Pessoas da empresa deste projeto  | Os usuários que pertencem à empresa associada a este projeto podem exibir e adicionar solicitações a esta fila. Se houver uma empresa associada ao projeto, o nome da empresa será listado entre parênteses após essa configuração. |
     | Pessoas do grupo deste projeto  | Os usuários que pertencem ao grupo associado a este projeto podem exibir e adicionar solicitações a esta fila. Se houver um grupo associado ao projeto, o nome do grupo será listado entre parênteses após essa configuração, em fonte cinza. |

     {style="table-layout:auto"}

   * Use as opções a seguir para fornecer acesso direto à Fila de solicitações e aos formulários associados a ela a usuários fora do Workfront ou a usuários do Workfront usando uma página externa incorporada.

   Para obter informações sobre como incorporar uma fila de solicitações em um painel como uma página externa, consulte [Incorporar uma fila de solicitações em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

   Os usuários devem primeiro ter permissões para a Fila de solicitações para obter acesso direto. O uso de qualquer das opções descritas aqui não concede acesso aos usuários automaticamente.

   >[!TIP]
   >
   >Os usuários devem primeiro fazer logon no Workfront antes de obter acesso à fila de solicitações quando acessam a página Fila de solicitações de outro aplicativo.

   * **URL de Acesso Direto:** Quando um usuário acessa esta URL a partir de um navegador, o usuário é levado diretamente para a seção Nova Solicitação na área Solicitações e esta solicitação é selecionada por padrão para ele.

     ![Nova caixa de solicitação do compartilhamento de URL direto](assets/new-request-box-from-direct-url-share.png)

     >[!NOTE]
     >
     >Você pode exibir uma Fila de solicitações em um painel como uma página externa. Nesse caso, a fila de solicitações é pré-selecionada, mas você pode selecionar qualquer outra fila de solicitações no campo Tipo de solicitação. Os usuários que enviam a solicitação podem selecionar outro Tipo de solicitação. Grupos de Tópicos e Tópicos de Fila também são exibidos.

   * **Código incorporado:** Use este código HTML para incorporar o formulário de fila de solicitações como um iframe em qualquer página do HTML.\
     Se os usuários ainda não estiverem autenticados no Workfront quando visualizarem a página em que o código está incorporado, a caixa de diálogo de logon do Workfront será exibida. Depois que os usuários fazem logon, o formulário Fila de solicitações é exibido.

     >[!NOTE]
     >
     >Ao exibir uma Fila de solicitações em um iframe, somente o formulário de solicitação é exibido, o nome da solicitação é pré-selecionado e esmaecido. O usuário não pode alterar o tipo de Solicitação. Os componentes de navegação da área Solicitações não são exibidos.

     Para que o formulário da fila de solicitações seja exibido ao usar esse código incorporado, o administrador do Workfront deve habilitar a configuração &quot;Permitir incorporação do Workfront em um iframe&quot; na área Configuração do sistema.

     Para obter mais informações sobre como habilitar a incorporação do Workfront em um iframe, consulte [Configurar preferências de segurança do sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Se essa configuração não estiver ativada, o iframe será exibido em branco.

     Você pode ajustar vários aspectos de como o formulário incorporado é exibido, da seguinte maneira:

     <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funcionalidade</strong> </p> </th> 
           <th> <p><strong>Solução</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Ajustar o tamanho do quadro</p> </td> 
           <td> <p>Modifique os atributos "width" e "height".</p> <p>A largura padrão é "500" e a altura é "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direcione usuários para um Tópico de Fila ou Grupo de Tópicos específico</p> </td> 
           <td> <p>Adicione o parâmetro "path" ao URL src. Você pode encontrar o parâmetro de caminho navegando até o Tópico da fila ou Grupo de tópicos desejado no formulário não incorporado e inspecionando o URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Mostrar e permitir que os usuários alterem a lista suspensa pré-configurada Grupo de tópicos</p> </td> 
           <td> <p>Use o parâmetro "path" adicionando o parâmetro <code>showPreSelectedOptions=true</code> a <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detectar quando o formulário foi enviado</p> </td> 
           <td> <p>Adicione um ouvinte de eventos de "mensagem" à janela da sua página da Web e verificando se <code>event.data.type</code> é <code>requestSubmitted</code>. <code>event.data.newIssueID</code> será definido como a ID do problema criado.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Tipos de Solicitação:** na seção **Propriedades da Fila**, selecione uma das seguintes opções:

   * Relatório de erro
   * Pedido de alteração
   * Problema
   * Solicitação

   Este campo é obrigatório e você deve selecionar pelo menos uma opção.

   O administrador do Workfront pode renomear os tipos de solicitação padrão. Para obter mais informações sobre como renomear os tipos de solicitação, consulte [Personalizar tipos de problemas padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

   >[!NOTE]
   >
   >Quando os usuários acessam a fila de solicitações na área Solicitações, os Tipos de solicitação são exibidos como uma seleção somente se o Tipo de solicitação for selecionado nas páginas Detalhes da fila e Tópico da fila.
   >
   >Para obter informações sobre como configurar a área Tópicos da Fila de um projeto, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   Cada tipo selecionado aqui estará disponível no formulário (você pode selecionar mais de um). Selecionar mais de um tipo pode ajudar a organizar várias solicitações recebidas.\
   Por exemplo, se você estiver usando o formulário em uma fila de solicitações para um projeto de TI, os seguintes tipos de solicitações poderão entrar na fila: hardware, software, correções de erros e problemas.

   * **Duração Padrão:** Insira um número para a Duração e, no menu suspenso, selecione uma das seguintes unidades de duração:

      * Days
      * Horas
      * Minutes
      * Weeks

   A duração padrão é o tempo normalmente necessário para concluir um problema enviado para essa fila de solicitações. Isso se torna o padrão para todas as questões recebidas e pode ser modificado manualmente.
A duração padrão de um problema é a mesma que o horário planejado para o problema. A Data de conclusão planejada do problema é calculada com base nesse campo.\
   Se deixado inalterado, o padrão para a Duração do problema é 1 dia ou 8 horas.
Se o administrador do Workfront definir as Horas típicas por dia de trabalho como menos de 8 horas na área Configuração, a Duração padrão para problemas ainda será de 8 horas.
Por exemplo, se a opção Horas típicas por dia de trabalho estiver definida como 7 horas na área Configuração do Workfront, a Duração padrão para problemas será 1,14 dia ou 8 horas.
Para obter mais informações sobre como configurar o sistema de Horas Típicas por Dia Útil, consulte a seção &quot;Cálculos de Linha do Tempo&quot; no artigo [Configurar preferências de projeto para todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **As pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações.**: Quando selecionada, todas as solicitações enviadas para a fila ficam visíveis para usuários na mesma empresa. Os usuários podem exibir essas solicitações na seção Todas as solicitações, localizada na área Solicitações. Quando essa configuração é ativada ou desativada, isso afeta todas as solicitações futuras; não afeta as informações retroativamente.
   * **Quando alguém faz uma solicitação, conceder automaticamente...:** Quando um usuário faz uma solicitação para a fila de solicitações, o usuário recebe automaticamente o nível de permissão que você escolher para essa solicitação. Clique no botão Acesso para selecionar entre os seguintes níveis de permissão:

      * **Exibir Acesso**
      * **Acesso ao Contribute**. Esta é a seleção padrão e o nome do botão Acessar.
      * **Gerenciar Acesso**

     Para obter informações sobre o modelo de permissões do Workfront, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Definir as permissões aqui economiza tempo, em vez de precisar conceder permissões individualmente, para cada solicitação recebida. A escolha dessa opção afeta todas as solicitações futuras, mas não afeta retroativamente as solicitações existentes.

   * **Aprovação padrão**: clique no menu suspenso para selecionar um processo de aprovação para esta fila de solicitações. Somente os Processos de aprovação de problemas ficam visíveis nesse menu suspenso. Todos os problemas enviados para essa fila serão associados a esse processo de aprovação. O administrador do Workfront deve definir processos de aprovação no nível do sistema antes que você possa associá-los a filas de solicitações. Os usuários com acesso administrativo aos processos de Aprovação também podem criar processos de aprovação específicos do grupo.

     >[!IMPORTANT]
     >
     >Se o grupo do projeto mudar, o processo de aprovação específico do grupo anexado a problemas existentes se tornará um processo de aprovação de uso único. Para obter mais informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte [Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Se você tiver vários tópicos da fila associados a uma fila de solicitações, recomendamos que você associe os processos de aprovação aos tópicos da fila.

     Para obter mais informações sobre como criar tópicos da fila, consulte [Criar tópicos da fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Considere o seguinte ao adicionar processos de aprovação a filas de solicitações:

      * Somente os processos de aprovação de problemas ativos são exibidos na lista.
      * Os processos de aprovação de problemas específicos de grupo e de todo o sistema são exibidos na lista. Um processo de aprovação associado a um grupo diferente daquele do projeto não é exibido na lista.

   * **Rota Padrão**: Clique no menu suspenso para selecionar uma regra de roteamento para esta fila de solicitações. As regras de roteamento atribuem automaticamente novas ocorrências enviadas a uma fila de solicitações ao recurso correto (usuário, função de trabalho ou equipe) e ao projeto correto. Todos os problemas enviados para essa fila serão associados a essa regra de roteamento. Você deve configurar Regras de Roteamento antes que elas sejam exibidas na seção Detalhes da Fila e antes de associá-las à fila de solicitações.\
     Se você tiver vários tópicos da fila associados a uma fila de solicitações, recomendamos que você associe regras de roteamento aos tópicos da fila. Para obter mais informações sobre como criar regras de roteamento, consulte [Criar Regras de Roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Novos Campos de Problema:** Na seção **Mostrar os seguintes campos selecionados para todos os usuários**, selecione os campos que você deseja que fiquem visíveis para todos os usuários que enviarem uma solicitação para o projeto ou adicionarem um problema a este projeto ou às tarefas do projeto.

     >[!NOTE]
     >
     >* Quando você ativa qualquer um dos campos Atribuído a, Função de trabalho ou Equipe, eles são sempre renomeados para Atribuições no formulário de solicitação quando os usuários enviam a solicitação. Você só pode especificar o tipo de atribuição na área Detalhes da fila.
     >
     >* Se você selecionou Atribuído a na área Detalhes da fila, é possível informar somente usuários no campo Atribuições no formulário de solicitação. Nesse caso, não é possível inserir funções de trabalho ou uma equipe.

   * **Documentos**: selecione essa opção para exibir a seção Documentos no novo formulário de solicitação e, em seguida, selecione onde a seção de carregamento do documento deve ser posicionada. Selecione entre as seguintes opções:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Depois de formulários personalizados</td> 
        <td><span>A seção Documentos é exibida na parte inferior do formulário de solicitação.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Antes dos formulários personalizados</td> 
        <td> <p><span>A seção Documentos é exibida entre os campos do Workfront e os campos personalizados do formulário de solicitação.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![Novos campos e documentos de problema em Detalhes da Fila](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **Mostrar todos os campos selecionados e não selecionados para:** Selecione quais usuários devem ver todos os campos no novo formulário de solicitação. As opções a seguir controlam o acesso aos campos no formulário.

     | Quais usuários podem ver todos os campos no formulário de solicitação | Descrição |
     |---|---| 
     | Todos os usuários (planejar licenças) | Todos os usuários que têm uma licença de Plano podem ver os campos selecionados, bem como os campos não selecionados. |
     | Pessoas com acesso de exibição a este projeto (Licença de plano) | Os usuários com uma licença de Plano que também têm direitos de Exibição para este projeto podem ver os campos selecionados, bem como os campos não selecionados. O restante dos usuários que podem enviar solicitações para esse projeto pode ver apenas os campos selecionados. |
     | Sem usuário | Nenhum usuário pode visualizar os campos não selecionados. Todos os usuários que podem enviar solicitações para este projeto só podem ver os campos selecionados. Esta é a seleção padrão. |

   * **Forms personalizado**: selecione um formulário personalizado para associar à Fila de solicitações no menu suspenso. Você pode selecionar vários formulários, em seguida, arrastá-los e soltá-los na ordem que você deseja que eles sejam exibidos no formulário de solicitação.
Somente formulários de edição personalizados estão disponíveis para seleção nesse menu suspenso. Todos os problemas enviados para essa fila de solicitações, adicionados ao projeto ou às suas tarefas terão os formulários selecionados associados a eles.
Você deve criar formulários personalizados de problemas antes de vê-los exibidos na seção Detalhes da fila.
Se você tiver vários tópicos da fila associados a uma fila de solicitações, recomendamos que você associe formulários personalizados aos tópicos da fila.
Para obter mais informações, consulte [Criar tópicos da fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Caixa Formulários personalizados em Detalhes da Fila](assets/custom-forms-box-on-queue-details.png)

1. Continue selecionando informações para as configurações na área **Configurações da fila de emails**, para permitir que os usuários enviem solicitações por email para o projeto da fila de solicitações.

   Para obter mais informações, consulte [Habilitar usuários a enviar um problema por email para um projeto da Fila de Solicitações](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Clique em **Salvar**.\
   Seu projeto foi configurado para ser uma Fila de solicitações, e os usuários agora podem adicionar solicitações a ela.

1. (Opcional) Para aprimorar a funcionalidade Fila de solicitações, crie subseções adicionais para sua fila, bem como regras para rotear as solicitações recebidas para a equipe, destinatário ou projeto correto.

   * Para obter informações sobre como criar subseções para a Fila de solicitações, consulte os seguintes artigos
   * [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)
   * [Criar Grupos De Tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

     Para obter informações sobre como rotear as solicitações para o responsável, a equipe e o projeto apropriado, consulte [Criar Regras de Roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

