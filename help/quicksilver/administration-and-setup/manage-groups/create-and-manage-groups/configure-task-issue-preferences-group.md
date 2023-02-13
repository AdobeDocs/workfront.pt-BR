---
title: Configurar preferências de tarefa e emissão para um grupo
user-type: administrator
product-area: system-administration;user-management;setup
keywords: grupo,preferências,tarefa,problema,desbloquear
navigation-topic: create-and-manage-groups
description: Se os grupos em sua organização precisarem configurar uma tarefa ou emitir uma preferência independentemente da forma como é configurada no nível do sistema, um administrador do Adobe Workfront poderá desbloquear a preferência. Em seguida, como administrador de grupo, você pode configurar a preferência para seu grupo e isso afetará todas as tarefas ou problemas associados ao grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 6889b94a-1be6-4be9-8397-c38f890f9103
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '1894'
ht-degree: 3%

---

# Configurar preferências de tarefa e emissão para um grupo

Se os grupos em sua organização precisarem configurar uma tarefa ou emitir uma preferência independentemente da forma como é configurada no nível do sistema, um administrador do Adobe Workfront poderá desbloquear a preferência. Em seguida, como administrador de grupo, você pode configurar a preferência para seu grupo e isso afetará todas as tarefas ou problemas associados ao grupo.

Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Para obter informações sobre como o administrador do Workfront desbloqueia preferências, consulte [Bloquear ou desbloquear preferências de projeto para todos os grupos no sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

>[!TIP]
>
>A configuração em nível de grupo também é possível para preferências de projeto. Para obter mais informações, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

>[!NOTE]
>
>* Normalmente, uma preferência desbloqueada permanece desbloqueada indefinidamente. Se o administrador do Workfront rebloquear, a configuração do sistema entrará em vigor novamente e as configurações da preferência feitas pelos administradores do grupo serão perdidas.
>* As preferências definidas para o grupo associado a um projeto têm prioridade sobre as preferências definidas para o Grupo inicial do usuário que cria o projeto.
>* Algumas preferências de nível de grupo afetam os modelos de projeto criados para o grupo. Para obter mais informações, consulte a seção [Exibir, trabalhar e criar modelos para seu grupo na área Grupos](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#view) no artigo [Criar e modificar modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
>
>* Depois que um administrador do Workfront desbloquear uma preferência no nível do sistema, você pode configurá-la e bloqueá-la para garantir que todos no seu grupo e em seus subgrupos estejam usando a mesma configuração. Isso é paralelo à capacidade de um administrador do Workfront configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear um projeto, tarefa ou emitir preferência para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).
>


## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Configurar a tarefa desbloqueada e emitir preferências para um grupo de nível superior

>[!TIP]
>
>Se você for um administrador do Workfront, é possível ignorar as etapas 1 a 4 acessando Configurar > Preferências do projeto > Tarefas e problemas e depois pesquisando o nome do grupo na caixa na parte superior da página.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo para o qual você deseja configurar a tarefa desbloqueada e emitir preferências.
1. Na página que é exibida para o grupo, no painel esquerdo, clique em **Preferências de tarefa e emissão**.
1. Na página exibida, continue com uma das 5 seções listadas abaixo para definir as configurações das áreas Novos padrões da tarefa, problemas, exclusão, datas reais e acesso, em seguida, clique em **Salvar**.

   Se você passar o mouse sobre o ícone de cadeado ![](assets/lock-toggle-button-dimmed.png) para obter uma preferência que você precisa configurar e uma dica de ferramenta for exibida para informá-lo que está bloqueada, você pode solicitar ao administrador do Workfront que a desbloqueie para todos os grupos na organização.

   Quando ele é desbloqueado, você e outros administradores de grupo podem configurá-lo separadamente para seus próprios grupos. Além disso, você pode bloqueá-lo para seu grupo e para qualquer subgrupo abaixo do seu grupo.

   * [Padrões de nova tarefa](#new-task-defaults)
   * [Problemas](#issues)
   * [Exclusão.](#deletion)
   * [Datas Efetivas](#actual-dates)

      <!--   
     <li><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>   
     -->

   * [Acesso](#access)

### Padrões de nova tarefa {#new-task-defaults}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Data de início em novas tarefas</td> 
      <td> <p>Determina a data de início padrão de novas tarefas para gerentes de projeto. A data de início de novas tarefas pode ser a data de início planejada do projeto ou o dia em que a tarefa é criada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Tipo de Duração </p> </td> 
      <td> <p>Determina a relação entre o número de recursos (e sua porcentagem de alocação) e a duração ou o esforço total da tarefa. Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duração da tarefa e Tipos de duração</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Receita</td> 
      <td> <p>Calcula estimativas de receita planejadas e reais para uma tarefa. Quando a variável <strong>Tipo de receita</strong> está definida como<strong>Não Faturável</strong>, as horas planejadas e as horas reais registradas não geram uma estimativa de receita para a tarefa e o trabalho na tarefa não contribui para a receita no nível do projeto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Custo</td> 
      <td> <p>Calcula estimativas de custo planejadas e reais para uma tarefa. Quando definido como <strong>Sem custo</strong>, as horas planejadas e as horas reais registradas não geram uma estimativa de custo planejada ou real para a tarefa, e o trabalho na tarefa não contribui para os custos a nível do projeto.</p> </td> 
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
      <td> <p>Quando alguém converte um problema em um projeto ou tarefa, o problema original e o projeto ou tarefa convertidos tornam-se objetos de resolução. Essa configuração permite correlacionar a resolução do problema original com a resolução de seu objeto resolvível. Para obter mais informações sobre como resolver objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</p> <p>Para que essa configuração tenha qualquer efeito, a opção para <strong>Mantenha o problema original e vincule sua resolução à tarefa</strong> deve ser selecionado.</p> 
       <ul> 
        <li>Quando essa configuração estiver ativada, você poderá criar status personalizados com a mesma chave para problemas e projetos ou tarefas. Quando o projeto ou a tarefa (como um objeto resolvível) se torna o status personalizado, a alteração também reflete sobre o status do problema. A chave de status deve ser a mesma para o problema e os status do projeto ou da tarefa.</li> 
        <li>Quando essa configuração é desativada, a resolução de status de objeto é automaticamente definida como status padrão, em vez dos personalizados. Para obter mais informações sobre os status padrão, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acesse a lista de status de problemas do sistema</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ao converter um problema em uma tarefa</td> 
      <td> <p>As configurações nesta seção determinam o que acontece durante o processo de conversão de problema a tarefa:</p> 
       <ul> 
        <li><strong>Mantenha o problema original e vincule sua resolução à tarefa</strong>: Quando você está convertendo o problema, ele permanece visível como um problema até que a tarefa seja concluída. O status do problema muda automaticamente para Closed quando a tarefa é concluída.</li> 
        <li><strong>Permitir que o Contato Principal tenha acesso à tarefa</strong>: Fornece ao contato principal (criador de problemas) acesso à tarefa para revisar a tarefa, fazer atualizações e permanecer informado sobre seu progresso</li> 
        <li> <p><strong>Permitir que essas configurações sejam alteradas durante a conversão</strong>: Permite que o usuário que está convertendo o problema altere essas opções durante a conversão de um problema em uma tarefa.</p> <!--
          Screenshot when possible</p>
         --> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ao converter um problema em um projeto</td> 
      <td> <p>As configurações nesta seção determinam o que acontece durante o processo de conversão de problema para projeto:</p> 
       <ul> 
        <li><strong>Mantenha o problema original e vincule sua resolução ao projeto</strong>: Quando você está convertendo o problema, ele permanece visível como um problema até que o projeto seja concluído. O status do problema muda automaticamente para Closed quando o projeto é concluído.</li> 
        <li><strong>Permitir que o Contato Principal tenha acesso ao projeto</strong>: Fornece ao contato principal (criador de problemas) acesso ao projeto para revisar o projeto, fazer atualizações e permanecer informado sobre o progresso.</li> 
        <li><strong>Permitir que essas configurações sejam alteradas durante a conversão</strong>: Permite que o usuário que está convertendo o problema altere as opções listadas durante a conversão de um problema em um projeto.</li> 
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
        <p><b>Ponta</b>: Essa configuração também se aplica à exclusão de projetos que tenham tarefas ou problemas com horas registradas neles. Essa configuração não se aplica à exclusão de projetos em que o tempo é registrado diretamente para o projeto. </p> 
        <p>Considere o seguinte:</p> 
        <ul> 
         <li> <p>Quando for selecionado, você receberá um aviso informativo ao excluir uma tarefa ou problema. O aviso lembra que, se a tarefa ou problema tiver horas registradas, eles serão movidos para o projeto ou excluídos. Você pode configurar se as horas são excluídas ou movidas para o projeto na área Folha de Horas e Preferências de Horas da Instalação. Depois de confirmar que você viu o aviso, a tarefa ou o problema é excluído. Para obter mais informações sobre como configurar a Folha de Horas e as Preferências de Horas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md" class="MCXref xref">Configurar preferências de hora e folha de ponto</a>. </p> <p>Dica: <span>Quando você exclui um projeto com tarefas e problemas que tenham horas registradas, as horas registradas são excluídas ou são preservadas de acordo com as configurações na área Folha de horas e preferências de horas da Configuração</span>. </p> </li> 
         <li><span>Ao desmarcar essa opção, você receberá um aviso proibitivo ao excluir uma tarefa ou problema com horas registradas, ou ao excluir um projeto com horas registradas para suas tarefas ou problemas</span> <span>.</span> O aviso especifica que o administrador não permite que tarefas ou problemas com horas registradas sejam excluídos. Tarefas, problemas<span>ou projetos com horas registradas para tarefas e problemas</span> não pode ser excluído. </li> 
        </ul> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

### Datas Efetivas {#actual-dates}

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Quando uma tarefa ou problema passar de "Novo" para "Em Andamento", defina a Data de Início Real como</td> 
      <td> <p>Selecione uma das seguintes opções para quando a Data de início real for registrada no Workfront quando uma tarefa ou problema for de <strong>Novo</strong> para <strong>Em Andamento</strong>:</p> 
       <ul> 
        <li><strong>Agora:</strong> A Data de Início Real é definida como a data atual.</li> 
        <li><strong>A Data Inicial Planejada:</strong> A Data de Início Real é definida como Data de Início Planejada da tarefa ou emissão.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando uma tarefa ou problema for concluído, definir a Data de conclusão atual como</td> 
      <td> <p>Selecione uma das seguintes opções para quando a Data de conclusão real for registrada no Workfront quando uma tarefa ou problema for concluído:</p> 
       <ul> 
        <li><strong>Agora:</strong> A Data de Conclusão Real é definida como a data atual.</li> 
        <li> <p><strong>Data de Conclusão Planejada:</strong> A Data de Conclusão Real é definida como Data de Conclusão Planejada da tarefa ou emissão.</p> </li> 
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
      <td role="rowheader">Quando alguém é atribuído a uma tarefa</td> 
      <td> 
       <ul> 
        <li><strong>Conceder-lhes ... acesso a uma tarefa</strong>: Define a permissão padrão que um usuário tem para a tarefa à qual está atribuído. Para obter mais informações sobre permissões de tarefa, consulte<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref"> Conceder acesso aos usuários</a>.</li> 
        <li> <p><strong>Conceder-lhes também ... acesso ao projeto</strong>: Define a permissão padrão que um usuário tem para o projeto no qual ele tem uma tarefa atribuída a ele. Para obter mais informações sobre permissões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando alguém é atribuído a um problema</td> 
      <td> 
       <ul> 
        <li><strong>Conceder-lhes ... acesso a uma tarefa</strong>: Define a permissão padrão que um usuário tem para a tarefa à qual está atribuído. Para obter mais informações sobre permissões de tarefa, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</li> 
        <li> <p><strong>Conceder-lhes também ... acesso ao projeto</strong>: Define a permissão padrão que um usuário tem para o projeto no qual ele tem uma tarefa atribuída a ele. Para obter mais informações sobre permissões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quando alguém envia uma solicitação</td> 
      <td> 
       <ul> 
        <li><strong>Conceder-lhes ... acesso à questão</strong>: Define a permissão padrão que um usuário tem em uma solicitação enviada. Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema</a>.</li> 
        <li> <p><strong>Pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações</strong>: Permite que os usuários vejam solicitações enviadas por outros usuários da mesma empresa que eles. Eles têm as mesmas permissões nessas solicitações que têm em suas próprias solicitações enviadas.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
