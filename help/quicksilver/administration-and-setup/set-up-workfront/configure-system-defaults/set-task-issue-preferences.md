---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar preferências de emissão e tarefa em todo o sistema
description: Você pode configurar preferências do sistema para tarefas e problemas. Essas preferências afetam o modo como seus usuários criam tarefas e problemas no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '2089'
ht-degree: 1%

---

# Configurar preferências de emissão e tarefa em todo o sistema

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

Como um [!DNL Adobe Workfront] administrador, você pode configurar as preferências do sistema para tarefas e problemas. Essas preferências afetam o modo como seus usuários criam tarefas e problemas na [!DNL Workfront].

Por padrão, as preferências de tarefa e emissão são bloqueadas e os administradores de grupo não podem modificá-las no nível do grupo, a menos que você as desbloqueie para todos os grupos em todo o sistema. Para obter mais informações, consulte a seção [Bloquear tarefas e emitir preferências para grupos](#lock-task-and-issue-preferences-for-groups) neste artigo.

<!--SPLIT OUT BOTTOM SECTION TO NEW ARTICLE?-->

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

## Configurar preferências de tarefa e problemas para todos em [!DNL Workfront]

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Preferências do projeto]** >**[!UICONTROL Tarefas e problemas].**

1. Na página exibida, continue com uma das 5 seções listadas abaixo para definir as configurações de [!UICONTROL Novos Padrões de Tarefa], [!UICONTROL Problemas], [!UICONTROL Exclusão], [!UICONTROL Datas reais]e [!UICONTROL Acesso].
1. Clique em **[!UICONTROL Salvar]**.

* [[!UICONTROL Padrões de nova tarefa]](#new-task-defaults)
* [[!UICONTROL Problemas]](#issues)
* [[!UICONTROL Exclusão.]](#deletion)
* [[!UICONTROL Datas Efetivas]](#actual-dates)
* [[!UICONTROL Delegação]](#delegation)

   <!--
  <li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Work On It</a> </li>
  -->

* [[!UICONTROL Acesso]](#access)

### [!UICONTROL Padrões de nova tarefa] {#new-task-defaults}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de início em novas tarefas]</td> 
   <td> <p>Determina a data de início padrão de novas tarefas para gerentes de projeto. A data de início de novas tarefas pode ser a data de início planejada do projeto ou o dia em que a tarefa é criada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tipo de duração] </p> </td> 
   <td> <p>Determina a relação entre o número de recursos (e sua porcentagem de alocação) e a duração ou o esforço total da tarefa. Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duração da tarefa e Tipos de duração</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de receita]</td> 
   <td> <p>Calcula estimativas de receita planejadas e reais para uma tarefa. Quando a variável <strong>[!UICONTROL Tipo de receita]</strong> está definida como<strong>[!UICONTROL Não Faturável]</strong>, as horas planejadas e as horas reais registradas não geram uma estimativa de receita para a tarefa e o trabalho na tarefa não contribui para a receita no nível do projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tipo de custo]</td> 
   <td> <p>Calcula estimativas de custo planejadas e reais para uma tarefa. Quando definido como <strong>[!UICONTROL Sem custo]</strong>, as horas planejadas e as horas reais registradas não geram uma estimativa de custo planejada ou real para a tarefa, e o trabalho na tarefa não contribui para os custos a nível do projeto.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Problemas {#issues}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atualizar automaticamente o status do problema resolvido quando o status do objeto de resolução for alterado]</td> 
   <td> <p>Quando alguém converte um problema em um projeto ou tarefa, o problema original e o projeto ou tarefa convertidos tornam-se objetos de resolução. Essa configuração permite correlacionar a resolução do problema original com a resolução de seu objeto resolvível. Para obter mais informações sobre como resolver objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</p> <p>Para que essa configuração tenha qualquer efeito, a opção para <strong>[!UICONTROL Manter o problema original e vincular sua resolução à tarefa]</strong> deve ser selecionado.</p> 
    <ul> 
     <li>Quando essa configuração estiver ativada, você poderá criar status personalizados com a mesma chave para problemas e projetos ou tarefas. Quando o projeto ou a tarefa (como um objeto resolvível) se torna o status personalizado, a alteração também reflete sobre o status do problema. A chave de status deve ser a mesma para o problema e os status do projeto ou da tarefa.</li> 
     <li>Quando essa configuração é desativada, a resolução de status de objeto é automaticamente definida como status padrão, em vez dos personalizados. Para obter mais informações sobre os status padrão, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acesse a lista de status de problemas do sistema</a>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader" [!UICONTROL>Ao converter um problema em uma tarefa]</td> 
   <td> <p>As configurações nesta seção determinam o que acontece durante o processo de conversão de problema a tarefa:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Manter o problema original e vincular sua resolução à tarefa]</strong>: Quando você está convertendo o problema, ele permanece visível como um problema até que a tarefa seja concluída. O status do problema muda automaticamente para [!UICONTROL Fechado] quando a tarefa é concluída. Quando isso é desmarcado, o problema é excluído.</p> <p><b>Nota</b>:  <p>Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema à medida que o convertem, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL Permitir que o contato principal tenha acesso à tarefa]</strong>: Fornece ao contato principal (criador de problemas) acesso à tarefa para revisar a tarefa, fazer atualizações e permanecer informado sobre seu progresso</li> 
     <li> <p><strong>[!UICONTROL Permitir que essas configurações sejam alteradas durante a conversão]</strong>: Permite que o usuário que está convertendo o problema altere essas opções durante a conversão de um problema em uma tarefa.</p> <!--
       Screenshot when possible</p>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ao converter um problema em um projeto]</td> 
   <td> <p>As configurações nesta seção determinam o que acontece durante o processo de conversão de problema para projeto:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Manter o problema original e vincular sua resolução ao projeto]</strong>: Quando você está convertendo o problema, ele permanece visível como um problema até que o projeto seja concluído. O status do problema muda automaticamente para [!UICONTROL Fechado] quando o projeto é concluído. Quando isso é desmarcado, o problema é excluído. </p> <p><b>Nota</b>:  <p>Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema à medida que o convertem, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:</p> 
       <ul> 
        <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a> </p> </li> 
        <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a> </p> </li> 
       </ul> </p> </li> 
     <li><strong>[!UICONTROL Permitir que o contato principal tenha acesso ao projeto]</strong>: Fornece ao contato principal (criador de problemas) acesso ao projeto para revisar o projeto, fazer atualizações e permanecer informado sobre o progresso.</li> 
     <li><strong>[!UICONTROL Permitir que essas configurações sejam alteradas durante a conversão]</strong>: Permite que o usuário que está convertendo o problema altere as opções listadas durante a conversão de um problema em um projeto.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Exclusão.] {#deletion}

**[!UICONTROL Permitir que usuários excluam tarefas e problemas com horas registradas]**: Permite determinar se você permite a exclusão de tarefas ou problemas em que as horas são registradas. Essa opção é selecionada por padrão.

>[!TIP]
>
>Essa configuração também se aplica à exclusão de projetos que tenham tarefas ou problemas com horas registradas neles. Essa configuração não se aplica à exclusão de projetos em que o tempo é registrado diretamente para o projeto.

* Quando for selecionado, você receberá um aviso informativo ao excluir uma tarefa ou problema. O aviso lembra que, se a tarefa ou problema tiver horas registradas, eles serão movidos para o projeto ou excluídos. Você pode configurar se as horas são excluídas ou movidas para o projeto no [!UICONTROL Folha de Horas e Preferências de Horas] área do [!UICONTROL Configuração]. Depois de confirmar que você viu o aviso, a tarefa ou o problema é excluído. Para obter mais informações sobre como configurar a Folha de Horas e as Preferências de Horas, consulte [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   >[!TIP]
   >
   >Ao excluir um projeto com tarefas e problemas que tenham horas registradas, as horas registradas são excluídas ou preservadas de acordo com as configurações na [!UICONTROL Folha de Horas e Preferências de Horas] área de [!UICONTROL Configuração]. A mensagem de aviso não é exibida ao excluir um projeto.

* Ao desmarcar essa opção, você receberá um aviso proibitivo ao excluir uma tarefa ou problema com horas registradas, ou ao excluir um projeto com horas registradas para suas tarefas ou problemas. O aviso especifica que o administrador não permite que tarefas ou problemas com horas registradas sejam excluídos. Não é possível excluir tarefas, problemas ou projetos com horas registradas para tarefas e problemas.

### [!UICONTROL Datas Efetivas] {#actual-dates}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando uma tarefa ou problema passar de "Novo" para "Em progresso", defina a Data de início real como]</td> 
   <td> <p>Selecione uma das opções a seguir para quando a Data de Início Real for registrada em [!DNL Workfront] quando uma tarefa ou problema é proveniente de <strong>[!UICONTROL Novo]</strong> para <strong>[!UICONTROL Em Andamento]</strong>:</p> 
    <ul> 
     <li><strong>[!UICONTROL Agora]:</strong> A Data de Início Real é definida como a data atual.</li> 
     <li><strong>[!UICONTROL A Data De Início Planejada]:</strong> A Data de Início Real é definida como Data de Início Planejada da tarefa ou emissão.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando uma tarefa ou problema é concluído, defina a Data de conclusão real como]</td> 
   <td> <p>Selecione uma das opções a seguir para quando a Data de Conclusão Real for registrada em [!DNL Workfront] quando uma tarefa ou problema é concluído:</p> 
    <ul> 
     <li><strong>[!UICONTROL Agora]:</strong> A Data de Conclusão Real é definida como a data atual.</li> 
     <li> <p><strong>[!UICONTROL A Data De Conclusão Planejada]:</strong> A Data de Conclusão Real é definida como Data de Conclusão Planejada da tarefa ou emissão.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Delegação

Ativar o [!UICONTROL Permitir que usuários deleguem suas tarefas e problemas] permite que todos os usuários do no deleguem temporariamente seu trabalho a outros.

Quando essa configuração é ativada, os usuários podem ver o seguinte:

* O [!UICONTROL Delegar] link em seus [!UICONTROL Início] área. Eles podem delegar aprovações ou tarefas e emitir atribuições aqui.
* Uma indicação de que uma tarefa ou problema é delegado a outro usuário no [!UICONTROL Atribuições e delegações] no cabeçalho da tarefa ou do problema.

Se você desativar o [!UICONTROL Permitir que usuários deleguem suas tarefas e problemas] , as delegações que estão agendadas serão interrompidas e os usuários delegados receberão uma notificação por email de que a delegação foi interrompida.

Para obter informações sobre delegação de trabalho a outros, consulte os seguintes artigos:

* [Visão geral do trabalho delegado](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Gerenciar delegação de tarefa e emissão](../../../manage-work/delegate-work/how-to-delegate-work.md)

<!--
<p><strong>Work On It</strong></p>
This was a Ninja story in Summer/Fall 2020 that may never be implemented Leaving it here drafted in case Ninja decides to add it.</p>
Here's what Jeremy Flores says on 12/1/20:</p>
I have not had a chance to follow up with customers to verify if this is still a need. It has not come up organically. I can follow up with a few customers, but overall I would say that we're probably safe to move on and just mark what we've done to support this as complete. It could still come up but I don't want to push it unless customers really want it.</p>
<p>You can replace the Work On It button with a Start button. When a user assigned to a task or issue clicks Start, the status and Actual Start Date of the work item update automatically, letting others know that the user started work.</p>
<p>Workfront's default Work On It button also signals that a user started work on a task or issue, but it doesn't update the status and Actual Start Date.</p>
<p>To switch to the Start button:</p>
<ol>
<li value="1"> <p>Select <strong>Change the Work On It button to a Start button to automatically update the status of an item</strong>.</p> </li>
<li value="2"> <p>In the lists of check boxes that display below this option, select one or more statuses for each work item type.</p> <p>With multiple statuses selected here, when a user clicks Start on a work item, a drop-down menu lets the user choose a status for the item.</p> </li>
</ol> <note type="note">
<ul class="preview">
<li>Making this change does not affect tasks and issues where the Actual Start Date was already updated. For these, the button displays as Work On It even if it is replaced with the Start button.</li>
<li>If you select New as a status for a work item type (in step 2 above), the Actual Start Date does not update when a user clicks the Start button and then chooses New. This is because a Workfront item is not yet in progress (therefore not yet started) when New is its current status.</li>
<li>This setting is not currently available in
<ul>
<li>The Workfront Mobile App</li>
<li>Workfront for Office 365</li>
<li>Workfront email notifications</li>
</ul></li>
<li>This setting can be configured both at the system level and at the Team level. Enabling the Start button for everyone in the system automatically disables the same setting at the Team level.</li>
<li>If the Work On It setting is enabled, then disabled, tasks and issues function with a Work On It button the way they did before.</li>
</ul>
</note>
-->

### [!UICONTROL Acesso] {#access}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando alguém é atribuído a uma tarefa]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Fornecer a eles ... acesso a uma tarefa]</strong>: Define a permissão padrão que um usuário tem para a tarefa à qual está atribuído. Para obter mais informações sobre permissões de tarefa, consulte<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</li> 
     <li> <p><strong>[!UICONTROL Também concede a eles ... acesso ao projeto]</strong>: Define a permissão padrão que um usuário tem para o projeto no qual ele tem uma tarefa atribuída a ele. Para obter mais informações sobre permissões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando alguém é atribuído a um problema]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Fornecer a eles ... acesso a uma tarefa]</strong>: Define a permissão padrão que um usuário tem para a tarefa à qual está atribuído. Para obter mais informações sobre permissões de tarefa, consulte<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</li> 
     <li> <p><strong>[!UICONTROL Também concede a eles ... acesso ao projeto]</strong>: Define a permissão padrão que um usuário tem para o projeto no qual ele tem uma tarefa atribuída a ele. Para obter mais informações sobre permissões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quando alguém envia uma solicitação]</td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Fornecer a eles ... acesso ao problema]</strong>: Define a permissão padrão que um usuário tem em uma solicitação enviada. Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a>.</li> 
     <li> <p><strong>[!UICONTROL Pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações]</strong>: Permite que os usuários vejam solicitações enviadas por outros usuários da mesma empresa que eles. Eles têm as mesmas permissões nessas solicitações que têm em suas próprias solicitações enviadas.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Bloquear tarefas e emitir preferências para grupos {#lock-task-and-issue-preferences-for-groups}

Se os grupos em sua organização precisarem de uma tarefa ou emitir uma preferência configurada de forma diferente para seus fluxos de trabalho exclusivos, você poderá desbloquear a preferência para todos os grupos em toda a organização para que eles possam configurá-la sozinhos. Quando uma preferência é desbloqueada e o administrador do grupo a modifica, as tarefas ou os problemas associados ao grupo são afetados pela configuração de nível de grupo da preferência, em vez da configuração de nível de sistema.

Para obter informações sobre como um administrador de grupo configura a tarefa e emite preferências para um grupo, consulte [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Depois de um [!DNL Workfront] O administrador desbloqueia uma preferência no nível do sistema, qualquer administrador de grupo pode configurá-la e bloqueá-la para garantir que todos no grupo e nos subgrupos abaixo estejam usando a mesma configuração. Isso é paralelo à capacidade de uma [!DNL Workfront] o administrador precisa configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Bloquear ou desbloquear um projeto, tarefa ou emitir preferência para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Para bloquear ou desbloquear uma tarefa ou preferência de emissão para que os grupos possam configurá-la

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Tarefas e problemas]**.

1. Siga um destes procedimentos:

   * Se você quiser que os administradores de grupos abaixo do seu grupo possam configurar uma preferência para seus grupos, desbloqueie-a ![](assets/unlock-toggle-button.png).
   * Se você quiser que seu grupo e todos os grupos abaixo dele usem sua configuração para uma preferência, verifique se ela está bloqueada (esse é o padrão).

      >[!IMPORTANT]
      >
      >Recomendamos que você se comunique com os administradores e usuários em grupos em todo o sistema para garantir que todas as necessidades sejam contabilizadas na forma como você configura uma preferência bloqueada. Ao bloqueá-lo, sua configuração é herdada por todos os grupos no sistema. E se a preferência tiver sido desbloqueada por algum período de tempo, sua configuração substituirá aquelas que os administradores de grupo podem ter feito.

1. Clique em **[!UICONTROL Salvar]**.
