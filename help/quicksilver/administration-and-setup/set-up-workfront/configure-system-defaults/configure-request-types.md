---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurar tipos de solicitação
description: Ao trabalhar em um projeto, você pode descobrir que eventos inesperados surgem. Você pode registrar esses eventos inesperados como problemas para um projeto ou tarefa específica. Também é possível enviar solicitações, que são registradas como ocorrências em um projeto designado como Fila de solicitações. Problemas e solicitações são considerados intercambiáveis no Adobe Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Configurar tipos de solicitação

Ao trabalhar em um projeto, você pode descobrir que eventos inesperados surgem. Você pode registrar esses eventos inesperados como problemas para um projeto ou tarefa específica. Também é possível enviar solicitações, que são registradas como ocorrências em um projeto designado como Fila de solicitações. Problemas e solicitações são considerados intercambiáveis no Adobe Workfront.

Para obter informações sobre como criar problemas no [!DNL Workfront], consulte [Criar problemas](../../../manage-work/issues/manage-issues/create-issues.md). Para obter informações sobre como criar solicitações em [!DNL Workfront], consulte [Criar e enviar [!DNL Adobe Workfront] solicitações](../../../manage-work/requests/create-requests/create-submit-requests.md). Para obter informações sobre como associar Tipos de Solicitação a projetos, consulte [Definir Tipos de Solicitação para um projeto](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront].</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## Personalizar os nomes dos tipos de solicitação

Como administrador do [!DNL Workfront], você pode configurar os nomes dos tipos de solicitação no sistema. Os novos nomes estão visíveis em qualquer área de [!DNL Workfront] onde os campos **[!UICONTROL Tipo de Problema]** ou **[!UICONTROL Tipo de Solicitação]** exibam:

* Na área **[!UICONTROL Detalhes da fila]** de um projeto que receberá os problemas ou solicitações.
* Se mais de um tipo de solicitação for selecionado para uma Fila de solicitações, no Formulário **[!UICONTROL Novo problema]** no campo **[!UICONTROL Tipo de problema]**, ao criar um novo problema ou enviar uma nova solicitação.

  Para obter mais informações sobre como criar problemas no [!DNL Workfront], consulte [Criar problemas](../../../manage-work/issues/manage-issues/create-issues.md)

  Para obter mais informações sobre como criar solicitações em [!DNL Workfront], consulte [Criar e enviar [!DNL Adobe Workfront] solicitações](../../../manage-work/requests/create-requests/create-submit-requests.md).

* No formulário **[!UICONTROL Detalhes do tópico da fila]**, ao configurar o Tópico da fila.\
   Para obter mais informações sobre como criar Tópicos da Fila, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Para personalizar os nomes dos tipos de solicitação:

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Status]**.

1. Clique na guia **[!UICONTROL Problemas]**.
1. Na parte superior da guia **[!UICONTROL Problemas]**, passe o mouse sobre o nome de um tipo de solicitação e clique no ícone **[!UICONTROL Editar]** que aparece.

   ![](assets/edit-request-type-name-nwe.png)

1. Na caixa exibida, digite um novo nome e pressione **[!UICONTROL Enter]**.

## Configurar status de problemas em diferentes tipos de solicitação

Você pode associar cada tipo de solicitação a diferentes status de ocorrência. Você também pode alterar a ordem na qual os status são exibidos em uma ocorrência, dependendo do tipo de ocorrência.

Para obter mais informações sobre como alterar a ordem padrão dos status de problemas e configurar esses status, consulte a seção [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) em [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
