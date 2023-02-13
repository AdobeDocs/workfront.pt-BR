---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Criar e gerenciar funções de trabalho
description: Como um [!DNL Adobe Workfront] administrador ou um usuário com acesso administrativo às Funções de trabalho, você pode criar funções de trabalho que podem ser atribuídas aos usuários e excluir funções de trabalho padrão que não sejam relevantes para sua organização.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# Criar e gerenciar funções de trabalho

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como um [!DNL Adobe Workfront] administrador ou um usuário com acesso administrativo às Funções de trabalho, você pode criar funções de trabalho que podem ser atribuídas aos usuários e excluir funções de trabalho padrão que não sejam relevantes para sua organização. Para obter informações sobre o acesso administrativo no [!DNL Workfront], consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo às funções de trabalho</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Criar uma função de trabalho

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em &#x200B; **[!UICONTROL Funções do Trabalho].**
1. Clique em **[!UICONTROL Nova Função de Trabalho].**
1. Configure o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indique um nome para a função de trabalho. Esse é o nome que é exibido em todos os locais em [!DNL Workfront] onde o campo [!UICONTROL Função do trabalho] é exibido. </p> <p>Dica: O nome de uma função de trabalho pode conter até 255 caracteres. No entanto, nomes mais longos podem ser truncados em determinadas áreas do [!DNL Workfront]. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Está Ativo]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Selecionar <b>[!UICONTROL Sim]</b> se você quiser que a função esteja ativa e disponível em todos os locais em [!DNL Workfront] ser associado a usuários, itens de trabalho etc. </p> </li> 
        <li> <p>Selecionar <b>[!UICONTROL n.o]</b>, se desejar que a função seja desativada e não esteja disponível para atribuição a usuários, itens de trabalho etc. </p> </li> 
       </ul> <p><span>Para obter informações sobre a desativação de funções de job, consulte</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Desativar funções de trabalho</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Insira uma descrição para a função que indica o que é exclusivo nela. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Moeda de base]</span> </td> 
      <td> <p><span>Esta é a [!UICONTROL Moeda de base], conforme definido na área [!UICONTROL Configuração] pelo administrador do Workfront. Para obter mais informações, consulte</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a> .</p> <p>Dica: <span>Não é possível editar a [!UICONTROL Moeda de base] no nível da função. Este campo está esmaecido e serve como um lembrete do que é a moeda base para o seu sistema.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Custo/ Hr.]</td> 
      <td>Essa é a taxa de custo por hora da função de trabalho. Este valor calcula os custos planejados e reais das tarefas e problemas associados à função e, em última análise, os custos planejados e reais dos projetos. <span>Insira a taxa usando a [!UICONTROL Moeda de base].</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Lista/ Hr.] </td> 
      <td>Essa é a taxa de faturamento por hora da função de trabalho. Este valor calcula as receitas programadas e reais das tarefas e questões associadas à função e, em última análise, as receitas programadas e efetivas dos projetos. Insira a taxa usando a [!UICONTROL Moeda de base]. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Substituir Moeda]</span> </td> 
      <td> 
       <div> 
        <p>Selecione uma moeda associada a esta função de trabalho. Essa é a moeda que [!DNL Workfront] usa para calcular custos e receita associados a esta função de cargo. </p> 
        <p><span>É diferente da [!UICONTROL Moeda de base] configurada pelo seu [!DNL Workfront] na área [!UICONTROL Configuração] e pode ser diferente da moeda associada a um projeto.</span> </p> 
        <p>Dica: Apenas as moedas disponíveis na área [!UICONTROL Taxas de Câmbio] em seu sistema estão disponíveis neste campo.</p> 
       </div> <p><span>Para obter informações sobre como configurar a [!UICONTROL Moeda de base] em [!DNL Workfront], consulte</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.</p> <p><span>Para obter informações sobre como alterar a moeda de um projeto, consulte</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Alterar a moeda do projeto</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Substituir Custo/Hora da Moeda]</span> </td> 
      <td> 
       <div> 
        <p>Esta é a taxa de custo por hora da função de trabalho usando a [!UICONTROL Sobrepor Moeda] selecionada. [!DNL Workfront] usa esse valor para calcular os custos planejados e reais das tarefas e problemas associados à função de trabalho. </p> 
        <p><span>Insira a taxa na [!UICONTROL Override Currency] especificada acima. Isso também atualiza a taxa de Custo/Hora dessa função de trabalho ao usar a [!UICONTROL Moeda de base].</span> </p> 
        <p>Para obter informações sobre como [!DNL Workfront] calcula o custo, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> 
       </div> <p>Dica: Ao atualizar uma função de trabalho existente que já tem uma taxa de Custo/Hora associada a ela, [!DNL Workfront] O calcula a taxa de [!UICONTROL Substituir moeda] com base na taxa de conversão em seu sistema. Se você atualizar o [!UICONTROL Substituir custo/hora da moeda], a função Custo/hora do trabalho também será atualizada automaticamente.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Substituir Faturamento/Hora da Moeda]</span> </td> 
      <td> 
       <div> 
        <p>Esta é a taxa de faturamento por hora da função de trabalho usando a [!UICONTROL Sobrepor Moeda] selecionada. [!DNL Workfront] O usa esse valor para calcular a receita planejada e real das tarefas e problemas associados à função de trabalho. </p> 
        <p><span>Insira a taxa na [!UICONTROL Override Currency] especificada acima. Isso também atualiza a taxa de Faturamento/Hora dessa função de trabalho ao usar a [!UICONTROL Moeda de base].</span> </p> 
        <p>Para obter informações sobre como [!DNL Workfront] calcula a receita, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral da Faturamento e Receita</a>.</p> 
       </div> <p>Dica: Ao atualizar uma função de trabalho existente que já tem uma taxa de Faturamento/Hora associada a ela, [!DNL Workfront] O calcula a taxa de Moeda de Substituição com base na taxa de conversão em seu sistema. Se você atualizar a função Sobrepor Faturamento/Hora da Moeda, a Faturamento/Hora da tarefa também será atualizada automaticamente. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >As funções de trabalho são parte integrante do gerenciamento de recursos. Para usar as ferramentas de planejamento de recursos, as funções de cargo precisam de um custo e uma taxa de faturamento associados a elas. Para obter mais informações, consulte [Introdução ao Gerenciamento de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Clique em **[!UICONTROL Criar função de trabalho]**. A função de trabalho agora está disponível para ser atribuída a tarefas, emissões, aprovações, ou você pode compartilhar modelos de layout ou outros objetos com ela. Para obter informações sobre todos os usos de funções de cargo em [!DNL Workfront], consulte [Visão geral da função de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Para obter informações sobre a exclusão de uma função de trabalho, consulte [Excluir funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
