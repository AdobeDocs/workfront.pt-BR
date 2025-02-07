---
title: Definir configurações de aprovação global
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Como administrador do Adobe Workfront, você pode determinar as configurações globais para processos de aprovação no Workfront. Essas configurações afetam todos os processos de aprovação de item de trabalho no sistema.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2fb0c647-bb6d-46d0-a985-6ab820b4a7f2
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 2%

---

# Definir configurações de aprovação global

Como administrador do Adobe Workfront, você pode determinar as configurações globais para processos de aprovação no Workfront. Essas configurações afetam todos os processos de aprovação de item de trabalho no sistema.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um Administrador do sistema ou ter uma licença de Plano com acesso administrativo aos processos de Aprovação</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Definir configurações de aprovação global

{{step-1-to-setup}}

1. Clique em **Processos** > **Aprovações**.

1. Clique no ícone **Configurações** ![ícone de configurações de engrenagem](assets/gear-icon-settings.png) ao lado do nome da área **Aprovações**.

1. Na caixa **Configurações de Aprovação** exibida, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Adicione &lt;number&gt; dias à data planejada de conclusão para acomodar os processos de aprovação</td> 
      <td> <p>Especifique o número de minutos, horas, dias, semanas ou meses para adicionar tempo à data de conclusão planejada da tarefa que precisa de aprovação. Selecione Minutos, horas, dias ou semanas "Decorridos" para adicionar horas que incluam fins de semana, feriados e horas fora do horário de trabalho designados no calendário da programação de trabalho do sistema.</p> 
      <p>Por exemplo, se uma tarefa for atribuída na sexta-feira e tiver uma duração de 3 dias decorridos, a data de conclusão da tarefa será definida para segunda-feira (supondo que sábado e domingo seja um fim de semana). Se a tarefa tiver uma duração de 3 dias (não decorridos), a data de conclusão da tarefa será definida para quarta-feira.</p>
      <p><b>OBSERVAÇÃO</b>: habilitar a adição de tempo extra para acomodar a aprovação em tarefas afetará a linha do tempo da tarefa e a do projeto.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprovador não precisa estar na equipe do projeto (para processos de aprovação que incluem uma função)</td> 
      <td> <p>Selecione esta opção se não for necessário que um aprovador esteja na equipe do projeto quando um processo de aprovação incluir uma função. Ao atribuir a decisão de aprovação a uma função de trabalho, somente os usuários que tiverem uma função associada a eles no projeto verão a aprovação. Se você habilitar essa configuração, qualquer usuário com essa função de trabalho receberá a solicitação de aprovação, esteja ele na equipe do projeto ou não. Para obter informações sobre como editar a função de projeto de um usuário, consulte <a href="../../../manage-work/projects/planning-a-project/manage-project-team.md" class="MCXref xref">Gerenciar a Equipe do Projeto</a>. </p> 
      <p><b>DICA</b>: quando você atribui uma aprovação a uma função e a opção <b>Aprovador não obrigatório na equipe do projeto (para processos de aprovação que incluem uma função)</b> está desabilitada, mas não há funções na equipe do projeto que correspondam à função na aprovação, a aprovação é reatribuída ao Proprietário do Projeto. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desativar a delegação de aprovações</td> 
      <td> <p>Selecione esta opção para desativar a funcionalidade para que os usuários em seu sistema deleguem aprovações a outro usuário. Quando essa opção é selecionada, a opção para delegar aprovações é removida do Workfront e qualquer delegação de aprovação existente é interrompida.</p> <p>Para obter mais informações sobre como delegar aprovações no Workfront, consulte <a href="../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md" class="MCXref xref">Delegar solicitação de aprovação</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permite editar o formulário personalizado quando o projeto, tarefa ou problema está no status de aprovação pendente</td> 
      <td> <p>Selecione esta opção para permitir que os usuários editem o formulário personalizado de projetos, tarefas e problemas quando estiverem no status Aprovação pendente. Esta é a configuração padrão.</p> 
      <p>Quando esta opção é selecionada:</p> 
       <ul> 
       <li>Todos os aprovadores (e quaisquer outros usuários que tenham acesso para editar o formulário personalizado) podem fazer alterações no formulário personalizado quando o objeto estiver com aprovação pendente, independentemente do caminho de aprovação ou da etapa de aprovação atual.</li> 
       <li>As alterações feitas no formulário personalizado durante um processo de aprovação não afetam nenhuma decisão de aprovação tomada antes da alteração.</li> 
       <li> <p>Quaisquer alterações feitas no projeto, tarefa ou problema são controladas da mesma maneira, independentemente dessa configuração. </p> <p>Por exemplo, se você adicionou campos de formulário personalizados para serem rastreados no fluxo de atualização, todas as alterações no formulário serão rastreadas no fluxo de atualização no objeto.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir aos usuários retroceder solicitações recém criadas pendentes de aprovação</td> 
      <td> <p>Selecione esta opção para configurar se os usuários podem cancelar um problema ou uma solicitação com aprovação pendente para seu primeiro status. Você pode associar o primeiro status de um problema ou solicitação a um processo de aprovação configurando filas de solicitações. </p> 
      <p>Para obter mais informações sobre filas de solicitações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>.</p> 
      <p>Siga um destes procedimentos:</p> 
       <ul> 
       <li>Selecione esta opção para permitir que os usuários cancelem uma aprovação para o primeiro status de uma ocorrência ou solicitação. Nesse caso, é possível ver um botão Cancelar&lt; em um novo problema ou solicitação com status de aprovação pendente. Quando eles selecionarem para cancelar o problema, eles receberão um aviso de que o problema também será excluído. O problema é excluído depois que eles confirmam que estão fazendo a recuperação. </li> 
       <li> <p>Desmarque essa opção para impedir que os usuários chamem novamente um problema ou uma solicitação cujo primeiro status seja pendente de aprovação. Eles não podem ver um botão Cancelar&lt; no novo problema ou solicitação e a aprovação deve ser concedida. Esta é a opção padrão.</p> 
       <p>Para obter mais informações sobre como revisar itens aguardando aprovação, consulte <a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Exibir aprovações </a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar alterações.**
