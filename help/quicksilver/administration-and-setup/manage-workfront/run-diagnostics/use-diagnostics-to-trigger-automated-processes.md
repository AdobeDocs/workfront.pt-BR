---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Usar diagnósticos para acionar processos automatizados
description: Você pode usar o Diagnóstico para acionar manualmente processos automatizados, como scripts baseados em tempo, recálculos ou notificações por email.
feature: System Setup and Administration
role: Admin
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 6%

---

# Usar diagnósticos para acionar processos automatizados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Você pode usar o Diagnóstico para acionar manualmente processos automatizados, como scripts baseados em tempo, recálculos ou notificações por email.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano do Adobe Workfront</a> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças</a> </td> 
   <td> <p>Plano </p>Você deve ser um administrador do Workfront. Para obter informações sobre administradores do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</td> 
  </tr> 
 </tbody> 
</table>

## Usar diagnósticos para acionar processos automatizados

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Expanda **Sistema** e clique em **Diagnósticos**.
1. Selecione uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Envia notificações de vencimentos</td> 
      <td> <p>Envia manualmente as notificações automáticas de lembrete sobre tarefas e problemas vencidos. </p> <p>Para obter mais informações sobre como configurar lembretes automáticos, consulte <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurar lembretes automáticos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envia notificações de antecipação</td> 
      <td> <p>Envia manualmente as notificações automáticas de lembrete para tarefas e problemas que estão se aproximando de suas datas de vencimento.</p> <p>Para obter mais informações sobre como configurar lembretes automáticos, consulte <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Configurar lembretes automáticos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Envia Lembretes de Notificações</td> 
      <td> <p>Envia manualmente notificações de lembrete. </p> <p>Para obter mais informações sobre como configurar notificações de lembrete, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurar notificações de lembrete</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verifica todas as contas POP</td> 
      <td> <p>Verifica se novos emails foram enviados para contas POP vinculadas ao Workfront. </p> <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information about Workfront and POP account integrations, see and <a href="../../../manage-work/requests/create-and-manage-request-queues/queue-details-tab-overview.md" class="MCXref xref">Overview of the Queue Details tab in a project</a>.</p>
       --> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recalcular Linhas de Tempo</td> 
      <td> <p>Recalcula a linha do tempo de todos os projetos no Workfront com o status Atual. </p> <p>Para obter mais informações sobre como calcular a linha de tempo de projetos automática ou manualmente, um projeto por vez, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular linhas de tempo do projeto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recupera Relatórios Padrão do Cliente</td> 
      <td>Restaura os relatórios padrão originalmente fornecidos com o Workfront, para que fiquem visíveis na seção <strong>Relatórios</strong> para todos os usuários.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerar planilha de horas</td> 
      <td>Gera planilhas de horas para usuários baseado em seus perfis de planilhas de horas recorrentes. Essa opção precisa ser executada somente se o perfil da folha de horas tiver sido alterado significativamente depois de ter sido atribuído aos usuários e somente após qualquer folha de horas atual e futura ter sido excluída.</td> 
     </tr> 
    </tbody> 
   </table>
