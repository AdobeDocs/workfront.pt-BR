---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Criar e gerenciar funções de trabalho
description: Como um [!DNL Adobe Workfront] administrador ou um usuário com acesso administrativo a Funções de trabalho, você pode criar funções de trabalho que podem ser atribuídas a usuários e excluir funções de trabalho padrão que não são relevantes para sua organização.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# Criar e gerenciar funções de trabalho

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como um [!DNL Adobe Workfront] administrador ou um usuário com acesso administrativo a Funções de trabalho, você pode criar funções de trabalho que podem ser atribuídas a usuários e excluir funções de trabalho padrão que não são relevantes para sua organização. Para obter informações sobre acesso administrativo no [!DNL Workfront], consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>Atual: [!UICONTROL Plano]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a funções de trabalho</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

+++

## Criar uma função de trabalho

Para criar uma função de trabalho:

{{step-1-to-setup}}

1. No painel esquerdo, clique em&#x200B; **[!UICONTROL Funções de trabalho].**
1. Clique em **[!UICONTROL Nova Função].**
1. Configure o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td> <p>Indique um nome para o cargo. Este é o nome que é exibido em qualquer lugar no [!DNL Workfront] onde é exibido o campo [!UICONTROL Função de trabalho]. </p> <p>Dica: o nome de uma função de trabalho pode conter até 255 caracteres. No entanto, nomes mais longos podem estar truncados em determinadas áreas do [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Informe uma descrição para a função que indique o que é exclusivo sobre ela. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Está Ativo]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Selecionar <b>[!UICONTROL Sim]</b> se você quiser que a função fique ativa e disponível em qualquer lugar no [!DNL Workfront] para ser associado a usuários, itens de trabalho etc. </p> </li> 
        <li> <p>Selecionar <b>[!UICONTROL Não]</b>, se desejar que a função seja desativada e não esteja disponível para atribuição a usuários, itens de trabalho etc. </p> </li> 
       </ul> <p><span>Para obter informações sobre como desativar funções de trabalho, consulte</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Desativar funções de trabalho</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Moeda Base]</span> </td> 
      <td> <p><span>Essa é a [!UICONTROL Moeda base], conforme definido na área [!UICONTROL Configuração] pelo administrador do Workfront. Para obter informações, consulte</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a> .</p> <p>Dica: <span>Não é possível editar a [!UICONTROL Moeda Base] no nível de função de trabalho. Esse campo fica esmaecido e serve como um lembrete da moeda base do sistema.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Taxa de Custo]</td> 
      <td><p>Esta é a taxa de custo por hora da função de trabalho. Esse valor calcula os custos planejados e reais de tarefas e problemas associados à função e, por fim, os custos planejados e reais dos projetos. Insira a taxa usando a [!UICONTROL Moeda base].</p> 
      <p>Para taxas de custo efetivas por data, clique em <strong>[!UICONTROL Adicionar Taxa]</strong>. Insira o valor de custo/hora para o período e atribua uma [!UICONTROL Data de Início] e uma [!UICONTROL Data de Término] conforme necessário. A primeira taxa de custo não terá uma data inicial e a última taxa de custo não terá uma data final.</p> <p>Algumas datas são adicionadas automaticamente. Por exemplo, se a primeira taxa de custo não tiver uma data final e você adicionar uma segunda taxa de custo com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à primeira taxa de custo para que não haja lacunas.</p> <p>Dica: ao editar uma função de trabalho existente, você pode selecionar <strong>Classificar por data de início</strong> para ver a data de início mais recente no topo da lista de taxas.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Taxa de Cobrança] </td> 
      <td><p>Esta é a taxa de cobrança por hora da função de trabalho. Esse valor calcula as receitas planejadas e reais de tarefas e problemas associados à função e, por fim, as receitas planejadas e reais dos projetos. Insira a taxa usando a [!UICONTROL Moeda base].</p> <p>Para taxas de cobrança efetivas por data, clique em <strong>[!UICONTROL Adicionar Taxa]</strong>. Insira o valor de faturamento/hora para o período e atribua uma [!UICONTROL Data de Início] e uma [!UICONTROL Data de Término] conforme necessário. A primeira taxa de cobrança não terá uma data inicial e a última taxa de cobrança não terá uma data final.</p> <p>Algumas datas são adicionadas automaticamente. Por exemplo, se a primeira taxa de cobrança não tiver uma data final e você adicionar um segundo com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à primeira taxa de cobrança para que não haja lacunas.</p> <p>Dica: ao editar uma função de trabalho existente, você pode selecionar <strong>Classificar por data de início</strong> para ver a data de início mais recente no topo da lista de taxas.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Substituir Moeda]</span> </td> 
      <td>
        <p>Selecione uma moeda associada a esta função de trabalho. Essa é a moeda que [!DNL Workfront] usa para calcular custos e receita associados a esta função de trabalho. </p> 
        <p><span>Isso é diferente da [!UICONTROL Moeda Base] configurada pelo seu [!DNL Workfront] administrador na área [!UICONTROL Setup] e pode ser diferente da moeda associada a um projeto.</span> </p> 
        <p>Dica: somente as moedas disponíveis na área [!UICONTROL Taxas de Câmbio] do sistema estão disponíveis neste campo. Se você tiver apenas uma moeda configurada, esse campo não será exibido.</p> 
       <p><span>Para obter informações sobre como configurar a [!UICONTROL Moeda Base] em [!DNL Workfront], consulte</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.</p> <p><span>Para obter informações sobre como alterar a moeda de um projeto, consulte</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Alterar a moeda do projeto</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Substituir Taxa de Custo da Moeda]</span> </td> 
      <td>
        <p>Essa é a taxa de custo por hora da função de trabalho que usa a [!UICONTROL Substituir Moeda] selecionada. [!DNL Workfront] O usa esse valor para calcular os custos planejados e reais de tarefas e problemas associados à função de trabalho. </p> 
        <p><span>Insira a taxa na [!UICONTROL Substituir moeda] especificada acima. Isso também atualiza a Taxa de Custo para essa função de trabalho ao usar a [!UICONTROL Moeda Base].</span> </p> 
        <p>Para obter informações sobre como [!DNL Workfront] calcula o custo, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> 
       <p>Dica: Ao atualizar uma função de trabalho existente que já tenha uma Taxa de Custo associada a ela, [!DNL Workfront] O calcula a taxa de [!UICONTROL Substituir moeda] com base no índice de conversão do sistema. Se você atualizar a [!UICONTROL Substituir Taxa de Custo da Moeda], a Taxa de Custo da função de trabalho também será atualizada automaticamente.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Substituir Taxa de Cobrança da Moeda]</span> </td> 
      <td>
        <p>Essa é a taxa de cobrança por hora da função de trabalho usando a [!UICONTROL Substituir Moeda] selecionada. [!DNL Workfront] O usa esse valor para calcular a receita planejada e real de tarefas e problemas associados à função de trabalho. </p>
        <p><span>Insira a taxa na [!UICONTROL Substituir moeda] especificada acima. Isso também atualiza a Taxa de Cobrança dessa função de trabalho ao usar a [!UICONTROL Moeda Base].</span> </p>
        <p>Para obter informações sobre como [!DNL Workfront] calcula a receita, consulte <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão geral de faturamento e receita</a>.</p>
        <p>Dica: ao atualizar uma função de trabalho existente que já tenha uma Taxa de cobrança associada a ela, [!DNL Workfront] O calcula a taxa de Sobreposição de Moeda com base na taxa de conversão do seu sistema. Se você atualizar a Taxa de Faturamento da Moeda de Sobreposição, a Taxa de Faturamento da função de trabalho também será atualizada automaticamente. </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >As funções de trabalho são parte integral do gerenciamento de recursos. Para usar as ferramentas de planejamento de recursos, as funções de trabalho precisam de um custo e uma taxa de faturamento associados a elas. Para obter informações, consulte [Introdução ao gerenciamento de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. Clique em **[!UICONTROL Criar função de trabalho]**. A função de trabalho agora está disponível para ser atribuída a tarefas, problemas, aprovações ou você pode compartilhar modelos de layout ou outros objetos com ela. Para obter informações sobre todos os usos de funções de trabalho no [!DNL Workfront], consulte [Visão geral das funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Para obter informações sobre a exclusão de uma função de trabalho, consulte [Excluir funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
