---
title: Configurar preferências de tarefas e problemas para um grupo
user-type: administrator
product-area: system-administration;user-management;setup
keywords: grupo,preferências,tarefa,problema,desbloquear
navigation-topic: create-and-manage-groups
description: Se os grupos em sua organização precisarem configurar uma preferência de tarefa ou problema independentemente da forma como é configurada no nível do sistema, um administrador do Adobe Workfront poderá desbloquear a preferência. Em seguida, como administrador de grupo, você pode configurar a preferência para seu grupo e ela afetará todas as tarefas ou problemas associados ao seu grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 36c4505b396f38617a7e82ae637596ff6c046d57
workflow-type: tm+mt
source-wordcount: '1885'
ht-degree: 2%

---

# Configurar preferências de tarefas e problemas para um grupo

Se os grupos em sua organização precisarem configurar uma preferência de tarefa ou problema independentemente da forma como é configurada no nível do sistema, um administrador do Adobe Workfront poderá desbloquear a preferência. Em seguida, como administrador de grupo, você pode configurar a preferência para seu grupo e ela afetará todas as tarefas ou problemas associados ao seu grupo.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Para obter informações sobre como o administrador do Workfront desbloqueia preferências, consulte [Bloquear ou desbloquear preferências do projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>A configuração no nível do grupo também é possível para as preferências do projeto. Para obter informações, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* Normalmente, uma preferência desbloqueada permanece desbloqueada indefinidamente. Se o administrador do Workfront o bloquear novamente, a configuração do sistema será aplicada novamente e as configurações da preferência feita pelos administradores de grupo serão perdidas.
>* As preferências definidas para o grupo associado a um projeto têm precedência sobre as preferências definidas para o Grupo padrão do usuário que cria o projeto.
>* Algumas preferências de nível de grupo afetam os modelos de projeto criados para o grupo. Para obter mais informações, consulte a seção [Exibir, trabalhar com e criar modelos para seu grupo da área Grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) no artigo [Criar e modificar os modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Depois que um administrador do Workfront desbloqueia uma preferência no nível do sistema, você pode configurá-la e bloqueá-la para garantir que todos no seu grupo e em seus subgrupos usem a mesma configuração. Isso é paralelo à capacidade que um administrador do Workfront tem de configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear uma preferência de projeto, tarefa ou problema para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar preferências de tarefas e problemas desbloqueadas para um grupo de nível superior

>[!TIP]
>
>Se você for um administrador do Workfront, ignore as etapas 1 a 4. Para isso, acesse Configurar > Preferências do projeto > Tarefas e problemas e, em seguida, procure o nome do grupo na caixa na parte superior da página.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo para o qual deseja configurar preferências de tarefas e problemas desbloqueadas.
1. Na página exibida para o grupo, no painel esquerdo, clique em **Preferências de tarefas e problemas**.
1. Na página exibida, continue com uma das 5 seções listadas abaixo dessas etapas para definir as configurações para as áreas Padrões de Novas Tarefas, Problemas, Exclusão, Datas Efetivas e Acesso, depois clique em **Salvar**.

   Se você passar o mouse sobre o ícone de bloqueio ![](assets/lock-toggle-button-dimmed.png) de uma preferência que precisa ser configurada e uma dica de ferramenta for exibida informando que o está bloqueado, você poderá solicitar que o administrador do Workfront o desbloqueie para todos os grupos da organização.

   Quando estiver desbloqueado, você e outros administradores de grupo poderão configurá-lo separadamente para seus próprios grupos. Além disso, você pode bloqueá-lo para o seu grupo e qualquer subgrupo abaixo dele.

   * [Padrões de nova tarefa](#new-task-defaults)
   * [Problemas](#issues)
   * [Exclusão](#deletion)

   <!--* <span class="preview">[Move](#move)</span>-->

   * [Datas Efetivas](#actual-dates)
   * [Acesso](#access)

### Padrões de nova tarefa {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Data de Início em Novas Tarefas</td> 
      <td> <p>Determina a data de início padrão para novas tarefas para gerentes de projeto. A data de início das novas tarefas pode ser a data planejada de início do projeto ou o dia em que a tarefa é criada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tipo de Duração </p> </td> 
      <td> <p>Determina a relação entre o número de recursos (e sua porcentagem de alocação) e a duração ou o esforço total da tarefa. Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duração da tarefa e tipos de duração: índice do artigo</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Receita</td> 
      <td> <p>Calcula as estimativas de receita planejadas e reais para uma tarefa. Quando o <strong>Tipo de Receita</strong> está definido como<strong>Não Faturável</strong>, as horas planejadas e as horas reais registradas não geram uma estimativa de receita para a tarefa e o trabalho na tarefa não contribui para a receita no nível do projeto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Custo</td> 
      <td> <p>Calcula as estimativas de custo planejadas e reais para uma tarefa. Quando definido como <strong>Sem Custo</strong>, as horas planejadas e as horas reais registradas não geram uma estimativa de custo planejada ou real para a tarefa, e o trabalho na tarefa não contribui para os custos no nível do projeto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

### Problemas {#issues}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Atualizar automaticamente o status de Problema resolvível quando o status do Objeto de resolução é alterado</td> 
      <td> <p>Quando alguém converte um problema em um projeto ou tarefa, tanto o problema original quanto o projeto ou tarefa convertido se tornam objetos de resolução. Essa configuração permite correlacionar a resolução da ocorrência original com a resolução de seu objeto resolvível. Para obter mais informações sobre a resolução de objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral de Objetos Resolventes e Resolvíveis </a>.</p> <p>Para que esta configuração tenha algum efeito, a opção para <strong>Manter o problema original e vincular sua resolução à tarefa</strong> deve ser selecionada.</p> 
       <ul> 
        <li>Quando essa configuração estiver ativada, você poderá criar status personalizados com a mesma chave para problemas e projetos ou tarefas. Quando o projeto ou a tarefa (como um objeto que pode ser resolvido) se transforma em um status personalizado, a alteração também reflete no status do problema. A chave de status deve ser a mesma para os status de problema e de projeto ou tarefa.</li> 
        <li>Quando essa configuração é desativada, a resolução dos status dos objetos é automaticamente definida para o status padrão, em vez dos personalizados. Para obter mais informações sobre os status padrão, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acessar a lista de status de problemas do sistema</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ao converter um problema em uma tarefa</td> 
      <td> <p>As configurações nesta seção determinam o que acontece durante o processo de conversão de problema em tarefa:</p> 
       <ul> 
        <li><strong>Mantenha o problema original e vincule sua resolução à tarefa</strong>: quando você está convertendo o problema, ele permanece visível como um problema até que a tarefa seja concluída. O status do problema muda automaticamente para Closed quando a tarefa é concluída.</li> 
        <li><strong>Permitir que o Contato Principal tenha acesso à tarefa</strong>: concede ao contato principal (criador de problemas) acesso à tarefa para revisar a tarefa, fazer atualizações e permanecer informado sobre seu progresso</li> 
        <li> <p><strong>Permitir que estas configurações sejam alteradas durante a conversão</strong>: permite que o usuário que está convertendo o problema altere estas opções durante a conversão de um problema em uma tarefa.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ao converter um problema em um projeto</td> 
      <td> <p>As configurações nesta seção determinam o que acontece durante o processo de conversão de problema em projeto:</p> 
       <ul> 
        <li><strong>Manter o problema original e vincular sua resolução ao projeto</strong>: quando você está convertendo o problema, ele permanece visível como um problema até que o projeto seja concluído. O status do problema muda automaticamente para Fechado quando o projeto é concluído.</li> 
        <li><strong>Permitir que o contato primário tenha acesso ao projeto</strong>: concede ao contato primário (criador da edição) acesso ao projeto para revisar o projeto, fazer atualizações e permanecer informado sobre o progresso.</li> 
        <li><strong>Permitir que estas configurações sejam alteradas durante a conversão</strong>: permite que o usuário que está convertendo o problema altere as opções listadas durante a conversão de um problema em um projeto.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Exclusão. {#deletion}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Permitir que os usuários excluam tarefas e problemas com horas reportadas</td> 
      <td> <p> Permite determinar se você permite a exclusão de tarefas ou problemas em que as horas são registradas. Essa opção é selecionada por padrão.</p> 
       <div> 
        <p><b>Dica</b>: esta configuração também se aplica à exclusão de projetos que tenham tarefas ou problemas com horas registradas. Essa configuração não se aplica à exclusão de projetos em que o tempo é registrado diretamente para o projeto. </p> 
        <p>Considere o seguinte:</p> 
        <ul> 
         <li> <p>Quando essa opção estiver selecionada, você receberá um aviso informativo ao excluir uma tarefa ou problema. O aviso lembra que, se a tarefa ou o problema tiver registrado horas, eles serão movidos para o projeto ou excluídos. Você pode configurar se as horas serão excluídas ou movidas para o projeto na área Planilha de horas e preferências de horas da Configuração. Depois de confirmar que você viu o aviso, a tarefa ou o problema é excluído. Para obter mais informações sobre como configurar as Preferências de Horas e Planilha de Horas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurar preferências de horas e Planilha de Horas</a>. </p> <p>Dica: <span>Quando você exclui um projeto com tarefas e problemas que têm horas reportadas, as horas reportadas são excluídas ou preservadas de acordo com as configurações na área Preferências de Horas e Planilha de Horas da Configuração</span>. </p> </li> 
         <li><span>Ao desmarcar esta opção, você receberá um aviso proibitivo ao excluir uma tarefa ou problema com horas reportadas, ou ao excluir um projeto com horas reportadas para suas tarefas ou problemas</span> <span>.</span> O aviso especifica que o administrador não permite que tarefas ou problemas com horas reportadas sejam excluídos. Não é possível excluir tarefas, problemas<span> ou projetos com horas registradas para tarefas e problemas</span>. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>


<!-- *****also replace the & with "and" in the Deletion section

<div class="preview">

### Move

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Allow users to move tasks and issues with logged hours</td> 
      <td> <p> Lets you determine whether you allow the move of tasks or issues where hours are logged. This option is selected by default.</p> 
       <p>Consider the following:</p> 
        <ul> 
         <li> When it is selected, you can move tasks and issues that have time logged. The hours also move with the tasks or issues. </li>
      <li>When you deselect this option, you receive a prohibitive warning when you move a task or issue with logged hours. The warning specifies that the administrator does not allow for tasks or issues with logged hours to be moved. The tasks or issues that have hours logged cannot be moved. </li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

</div>

-->

### Datas Efetivas {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Quando uma tarefa ou problema mudar de "Novo" para "Em andamento", definir a Data de início efetiva como</td> 
      <td> <p>Selecione uma das seguintes opções para quando a Data de Início Efetivo for registrada no Workfront quando uma tarefa ou problema mudar de <strong>Novo</strong> para <strong>Em Andamento</strong>:</p> 
       <ul> 
        <li><strong>Agora:</strong> A Data de Início Efetivo está definida como a data atual.</li> 
        <li><strong>A Data de Início Planejada:</strong> A Data de Início Efetivo está definida como a Data de Início Planejada da tarefa ou problema.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando uma tarefa ou problema for concluído, definir a Data de conclusão atual como</td> 
      <td> <p>Selecione uma das seguintes opções para quando a Data de conclusão efetiva for registrada no Workfront quando uma tarefa ou problema for concluído:</p> 
       <ul> 
        <li><strong>Agora:</strong> a data de conclusão efetiva está definida para a data atual.</li> 
        <li> <p><strong>A Data de Conclusão Planejada:</strong> A Data de Conclusão Efetiva está definida como a Data de Conclusão Planejada da tarefa ou problema.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--
   This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it. Here's what Jeremy Flores says on 12/1/20:
   
   I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.
   You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.
   Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.

   To switch to the Start button:
   
   Select Change the Work On It button to a Start button to automatically update the status of an item. 
   In the lists of check boxes that display below this option, select one or more statuses for each work item type. With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item. 
     
   Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.
   If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.
   This setting is not currently available in
   
   The Workfront Mobile App
   Workfront for Office 365
   Workfront email notifications
   
   This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.
   If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.
   -->

### Acesso {#access}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Quando alguém é designado a uma tarefa</td> 
      <td> 
       <ul> 
        <li><strong>Conceder a eles... acesso a uma tarefa</strong>: define a permissão padrão que um usuário tem para a tarefa à qual está atribuído. Para obter mais informações sobre permissões de tarefas, consulte<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Conceder acesso aos usuários</a>.</li> 
        <li> <p><strong>Também conceder a eles... acesso ao projeto</strong>: define a permissão padrão que um usuário tem para o projeto no qual ele tem uma tarefa atribuída a ele. Para obter mais informações sobre permissões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto do sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando alguém é designado a um problema</td> 
      <td> 
       <ul> 
        <li><strong>Conceder a eles... acesso a uma tarefa</strong>: define a permissão padrão que um usuário tem para a tarefa à qual está atribuído. Para obter mais informações sobre permissões de tarefas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</li> 
        <li> <p><strong>Também conceder a eles... acesso ao projeto</strong>: define a permissão padrão que um usuário tem para o projeto no qual ele tem uma tarefa atribuída a ele. Para obter mais informações sobre permissões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto do sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando alguém envia uma solicitação</td> 
      <td> 
       <ul> 
        <li><strong>Conceder a eles... acesso ao problema</strong>: define a permissão padrão que um usuário tem em uma solicitação que enviou. Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema</a>.</li> 
        <li> <p><strong>As pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações</strong>: permite que os usuários vejam as solicitações enviadas por outros usuários da mesma empresa que eles. Nessas solicitações, eles têm as mesmas permissões que têm em suas próprias solicitações enviadas.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
