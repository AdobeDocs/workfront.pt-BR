---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurar tipos de solicitação
description: Ao trabalhar em um projeto, você pode descobrir que surgem eventos inesperados. Você pode registrar esses eventos inesperados como problemas para um projeto ou tarefa específica. Também é possível enviar solicitações, que são registradas como problemas em um projeto designado como Fila de solicitações. Problemas e solicitações são considerados intercambiáveis no Adobe Workfront.
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

Ao trabalhar em um projeto, você pode descobrir que surgem eventos inesperados. Você pode registrar esses eventos inesperados como problemas para um projeto ou tarefa específica. Também é possível enviar solicitações, que são registradas como problemas em um projeto designado como Fila de solicitações. Problemas e solicitações são considerados intercambiáveis no Adobe Workfront.

Para obter informações sobre como criar problemas em [!DNL Workfront], consulte [Criar problemas](../../../manage-work/issues/manage-issues/create-issues.md). Para obter informações sobre como criar solicitações em [!DNL Workfront], consulte [Criar e enviar [!DNL Adobe Workfront] requests](../../../manage-work/requests/create-requests/create-submit-requests.md). Para obter informações sobre como associar Tipos de solicitação a projetos, consulte [Definir tipos de solicitação para um projeto](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
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

Como um [!DNL Workfront] administrador, você pode configurar os nomes dos tipos de solicitação em seu sistema. Os novos nomes são visíveis em qualquer área do [!DNL Workfront] em que **[!UICONTROL Tipo de problema]** ou **[!UICONTROL Tipo de solicitação]** exibição de campos:

* No **[!UICONTROL Detalhes da fila]** área de um projeto que receberá os problemas ou solicitações.
* Se mais de um tipo de solicitação for selecionado para uma Fila de solicitação, na **[!UICONTROL Novo problema] Formulário** no **[!UICONTROL Tipo de problema]** , ao criar um novo problema ou enviar uma nova solicitação.

   Para obter mais informações sobre como criar problemas em [!DNL Workfront], consulte  [Criar problemas](../../../manage-work/issues/manage-issues/create-issues.md)

   Para obter mais informações sobre como criar solicitações em [!DNL Workfront], consulte  [Criar e enviar [!DNL Adobe Workfront] requests](../../../manage-work/requests/create-requests/create-submit-requests.md).

* No **[!UICONTROL Detalhes do Tópico da Fila]** , ao configurar o Tópico da fila.\
   Para obter mais informações sobre como criar tópicos da fila, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

Para personalizar os nomes dos tipos de solicitação:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Status]**.

1. Clique no botão **[!UICONTROL Problemas]** guia .
1. Na parte superior do **[!UICONTROL Problemas]** , passe o mouse sobre o nome de um tipo de solicitação e clique no botão **[!UICONTROL Editar]** ícone que aparece.

   ![](assets/edit-request-type-name-nwe.png)

1. Na caixa exibida, digite um novo nome e pressione **[!UICONTROL Enter]**.

## Configurar status de problema em diferentes tipos de solicitação

Você pode associar cada tipo de solicitação a diferentes status de ocorrência. Também é possível alterar a ordem em que os status são exibidos em uma ocorrência, dependendo do tipo de problema.

Para obter mais informações sobre como alterar a ordem padrão dos status de ocorrência e configurar os status de ocorrência, consulte o [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) seção em [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
