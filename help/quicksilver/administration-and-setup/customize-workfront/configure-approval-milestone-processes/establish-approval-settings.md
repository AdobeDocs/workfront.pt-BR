---
title: Definir configurações de aprovação global
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Como administrador do Adobe Workfront, você pode determinar as configurações globais para processos de aprovação no Workfront. Essas configurações afetam todos os processos de aprovação de itens de trabalho em seu sistema.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 2%

---

# Definir configurações de aprovação global

Como administrador do Adobe Workfront, você pode determinar as configurações globais para processos de aprovação no Workfront. Essas configurações afetam todos os processos de aprovação de itens de trabalho em seu sistema.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um Administrador do Sistema ou ter uma licença de Plano com acesso administrativo aos processos de Aprovação</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Definir configurações de aprovação global

1. Faça logon no Workfront as a Workfront Administrator .
1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Processos** > **Aprovações** .

1. Clique no botão **Configurações** ícone ![](assets/gear-icon-settings.png) ao lado do **Aprovações** nome da área.

1. No **Configurações de aprovação** na caixa exibida, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Adicionar &lt;number&gt; Dias até a data de conclusão planejada para acomodar os processos de aprovação</td> 
      <td> <p>Especifique o número de minutos, horas, dias, semanas ou meses para adicionar tempo à data de conclusão planejada da tarefa que precisa de aprovação. Selecione minutos, horas, dias ou semanas "Aproveitados" para adicionar tempo que inclua fins de semana, feriados e horas que não estejam funcionando designados no calendário de agendamento do sistema.</p> 
      <p>Por exemplo, se uma tarefa for atribuída na sexta-feira e tiver uma duração de 3 dias decorridos, a data de conclusão da tarefa será definida para Segunda-feira (supondo que sábado e domingo seja um fim de semana). Se a tarefa tiver uma duração de 3 dias (não decorrido), a data de conclusão da tarefa será definida para quarta-feira.</p>
      <p><b>OBSERVAÇÃO</b>: Habilitar a adição de tempo extra para acomodar a aprovação em tarefas afetará a linha do tempo da tarefa e a do projeto.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprovador não precisa estar na equipe do projeto (para processos de aprovação que incluem uma função)</td> 
      <td> <p>Selecione essa opção se um aprovador não precisar estar na equipe do projeto quando um processo de aprovação incluir uma função. Ao atribuir a decisão de aprovação a uma função de trabalho, somente os usuários que têm uma função associada a eles no projeto visualizarão a aprovação. Se você habilitar essa configuração, qualquer usuário com essa função de trabalho receberá a solicitação de aprovação se estiver ou não na equipe do projeto. Para obter informações sobre como editar a função de projeto de um usuário, consulte <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gerenciar a equipe do projeto</a>. </p> 
      <p><b>DICA</b>: Ao atribuir uma aprovação a uma função e à opção <b>Aprovador não precisa estar na equipe do projeto (para processos de aprovação que incluem uma função)</b> estiver desativado, mas não houver funções na equipe do projeto que correspondam à função na aprovação, a aprovação será reatribuída ao Proprietário do projeto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desativar a delegação de aprovações</td> 
      <td> <p>Selecione essa opção para desativar a funcionalidade para que usuários em seu sistema deleguem aprovações a outro usuário. Quando essa opção é selecionada, a opção para delegar aprovações é removida do Workfront e qualquer delegação de aprovação existente é interrompida.</p> <p>Para obter mais informações sobre delegação de aprovações no Workfront, consulte <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegar solicitação de aprovação</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir edição do formulário personalizado quando o projeto, a tarefa ou o problema estiver no status de aprovação pendente</td> 
      <td> <p>Selecione essa opção para permitir que os usuários editem o formulário personalizado de projetos, tarefas e problemas quando estiverem no status de Aprovação pendente. Esta é a configuração padrão.</p> 
      <p>Quando esta opção é selecionada:</p> 
       <ul> 
       <li>Todos os aprovadores (e qualquer outro usuário que tenha acesso para editar o formulário personalizado) podem fazer alterações no formulário personalizado quando o objeto estiver pendente de aprovação, independentemente do caminho de aprovação ou da etapa de aprovação atual.</li> 
       <li>As alterações feitas no formulário personalizado durante um processo de aprovação não afetam as decisões de aprovação feitas antes da alteração.</li> 
       <li> <p>Todas as alterações feitas no projeto, tarefa ou problema são rastreadas da mesma maneira, independentemente dessa configuração. </p> <p>Por exemplo, se você tiver adicionado campos de formulário personalizados para serem rastreados no fluxo de atualização, quaisquer alterações no formulário serão rastreadas no fluxo de atualização no objeto.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir aos usuários retroceder solicitações recém criadas pendentes de aprovação</td> 
      <td> <p>Selecione essa opção para configurar se os usuários podem recuperar um problema ou uma solicitação pendente de aprovação para seu primeiro status. Você pode associar o primeiro status de um problema ou de uma solicitação a um processo de aprovação configurando filas de solicitações. </p> 
      <p>Para obter mais informações sobre filas de solicitação, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>.</p> 
      <p>Siga um destes procedimentos:</p> 
       <ul> 
       <li>Selecione essa opção para permitir que os usuários recuperem uma aprovação para o primeiro status de um problema ou de uma solicitação. Nesse caso, eles podem ver um botão Recall&lt; em um novo problema ou solicitação que está pendente de status de aprovação. Ao optar por cancelar o problema, eles receberão um aviso de que o problema também será excluído. O problema é excluído depois de terem confirmado sua evocação. </li> 
       <li> <p>Desmarque essa opção para impedir que os usuários lembrem um problema ou uma solicitação cujo primeiro status está pendente de aprovação. Eles não podem ver um botão Recall&lt; na nova edição ou solicitação e a aprovação deve ser concedida. Esta é a opção padrão.</p> 
       <p>Para obter mais informações sobre a revisão de itens aguardando aprovação, consulte <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Exibir aprovações </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar alterações.**
