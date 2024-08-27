---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Configurar preferências de tarefas e problemas em todo o sistema
description: Você pode configurar preferências de todo o sistema para tarefas e problemas. Essas preferências afetam a maneira como seus usuários criam tarefas e problemas no Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8b99f939-12fe-4470-9dc8-f8a92c6db334
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# Configurar preferências de tarefas e problemas em todo o sistema

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
Linked to Converting Issues.-->

Como administrador do [!DNL Adobe Workfront], você pode configurar preferências de todo o sistema para tarefas e problemas. Essas preferências afetam a maneira como seus usuários criam tarefas e problemas no [!DNL Workfront].

Por padrão, as preferências de tarefas e problemas são bloqueadas e os administradores de grupos não podem modificá-las no nível do grupo, a menos que você as desbloqueie para todos os grupos no sistema. Para obter mais informações, consulte a seção [Preferências de tarefas e problemas para grupos](#lock-task-and-issue-preferences-for-groups) neste artigo.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td><p>Novo: [!UICONTROL Padrão]</p>
   ou
   <p>Atual: [!UICONTROL Plano]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar preferências de tarefas e problemas para todos em [!DNL Workfront]

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Preferências do projeto]** >**[!UICONTROL Tarefas e problemas].**

1. Na página exibida, continue com uma das 5 seções listadas abaixo para definir as configurações para [!UICONTROL Novos Padrões de Tarefa], [!UICONTROL Problemas], [!UICONTROL Exclusão], [!UICONTROL Datas Efetivas] e [!UICONTROL Acesso]:

   * [[!UICONTROL Padrões de nova tarefa]](#new-task-defaults)
   * [[!UICONTROL Problemas]](#issues)
   * [[!UICONTROL Exclusão]](#deletion)
   * [[!UICONTROL Datas efetivas]](#actual-dates)
   * [[!UICONTROL Delegação]](#delegation)

   <!--
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#work-on-it" class="MCXref xref">Trabalhar Nele</a> </li>
  --&gt;

* [[!UICONTROL Acesso]](#access)

### [!UICONTROL Padrões de nova tarefa] {#new-task-defaults}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Data de Início]</td> 
    <td> <p>Determina a data de início padrão para novas tarefas para gerentes de projeto. A data de início das novas tarefas pode ser a data planejada de início do projeto ou o dia em que a tarefa é criada.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader"> <p>[!UICONTROL Tipo de Duração] </p> </td> 
    <td> <p>Determina a relação entre o número de recursos (e sua porcentagem de alocação) e a duração ou o esforço total da tarefa. Para obter mais informações, consulte <a href="../../../manage-work/tasks/taskdurtn/task-duration-duration-type.md" class="MCXref xref">Duração e tipos de duração da tarefa</a></p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Tipo de Receita]</td> 
    <td> <p>Calcula as estimativas de receita planejadas e reais para uma tarefa. Quando o <strong>[!UICONTROL Tipo de Receita]</strong> está definido como <strong>[!UICONTROL Não Faturável]</strong>, as horas planejadas e as horas reais registradas não geram uma estimativa de receita para a tarefa e o trabalho na tarefa não contribui para a receita no nível do projeto.</p> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Tipo de Custo]</td> 
    <td> <p>Calcula as estimativas de custo planejadas e reais para uma tarefa. Quando definido como <strong>[!UICONTROL Sem Custo]</strong>, as horas planejadas e as horas reais registradas não geram uma estimativa de custo planejada ou real para a tarefa, e o trabalho na tarefa não contribui para os custos no nível do projeto.</p> </td> 
    </tr> 
  </tbody> 
</table>

### Problemas {#issues}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Atualiza automaticamente o status de Problema resolvível quando o status do Objeto de resolução é alterado]</td> 
    <td> <p>Quando alguém converte um problema em um projeto ou tarefa, tanto o problema original quanto o projeto ou tarefa convertido se tornam objetos de resolução. Essa configuração permite correlacionar a resolução da ocorrência original com a resolução de seu objeto resolvível. Para obter mais informações sobre a resolução de objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral de Objetos Resolventes e Resolvíveis </a>.</p> <p>Para que esta configuração tenha algum efeito, a opção para <strong>[!UICONTROL Manter o problema original e vincular sua resolução à tarefa]</strong> deve ser selecionada.</p> 
      <ul> 
      <li>Quando essa configuração estiver ativada, você poderá criar status personalizados com a mesma chave para problemas e projetos ou tarefas. Quando o projeto ou a tarefa (como um objeto que pode ser resolvido) se transforma em um status personalizado, a alteração também reflete no status do problema. A chave de status deve ser a mesma para os status de problema e de projeto ou tarefa.</li> 
      <li>Quando essa configuração é desativada, a resolução dos status dos objetos é automaticamente definida para o status padrão, em vez dos personalizados. Para obter mais informações sobre os status padrão, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Acessar a lista de status de problemas do sistema</a>.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Ao converter um problema em uma tarefa]</td> 
    <td> <p>As configurações nesta seção determinam o que acontece durante o processo de conversão de problema em tarefa:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Manter o problema original e vincular sua resolução à tarefa]</strong>: quando você está convertendo o problema, ele permanece visível como um problema até que a tarefa seja concluída. O status do problema muda automaticamente para [!UICONTROL Fechado] quando a tarefa é concluída. Quando essa opção não está selecionada, o problema é excluído.</p> <p><b>NOTA</b>:  <p>Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema como estão convertendo-o, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso aos problemas</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Permitir que o Contato Primário tenha acesso à tarefa]</strong>: Concede ao contato primário (criador de problemas) o acesso de Exibição à tarefa para revisar a tarefa, permanecer informado sobre seu progresso e fazer comentários na seção Atualizações da tarefa.</li> 
      <li> <p><strong>[!UICONTROL Permitir que essas configurações sejam alteradas durante a conversão]</strong>: Permite que o usuário que está convertendo o problema altere essas opções durante a conversão de um problema em uma tarefa.</p></li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Ao converter um problema em um projeto]</td> 
    <td> <p>As configurações nesta seção determinam o que acontece durante o processo de conversão de problema em projeto:</p> 
      <ul> 
      <li> <p><strong>[!UICONTROL Manter o problema original e vincular sua resolução ao projeto]</strong>: quando você está convertendo o problema, ele permanece visível como um problema até que o projeto seja concluído. O status do problema muda automaticamente para [!UICONTROL Encerrado] quando o projeto é concluído. Quando essa opção não está selecionada, o problema é excluído. </p> <p><b>NOTA</b>:  <p>Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema como estão convertendo-o, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:</p> 
        <ul> 
          <li> <p><a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso aos problemas</a> </p> </li> 
          <li> <p><a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a> </p> </li> 
        </ul> </p> </li> 
      <li><strong>[!UICONTROL Permitir que contato primário tenha acesso ao projeto]</strong>: Dá ao contato primário (criador da edição) acesso de Visualização ao projeto para revisar o projeto, manter-se informado sobre seu progresso e fazer comentários na seção Atualizações do projeto.</li> 
      <li><strong>[!UICONTROL Permitir que essas configurações sejam alteradas durante a conversão]</strong>: Permite que o usuário que está convertendo o problema altere as opções listadas durante a conversão de um problema em um projeto.</li> 
      </ul> </td>
    </tr> 
  </tbody> 
  </table>

### [!UICONTROL Exclusão] {#deletion}

**[!UICONTROL Permitir que usuários excluam tarefas e problemas com horas reportadas]**: Permite que você determine se permite a exclusão de tarefas ou problemas em que horas são reportadas. Essa opção é selecionada por padrão.

>[!TIP]
>
>Essa configuração também se aplica à exclusão de projetos que têm tarefas ou problemas com horas registradas. Essa configuração não se aplica à exclusão de projetos em que o tempo é registrado diretamente para o projeto.

* Quando essa opção estiver selecionada, você receberá um aviso informativo ao excluir uma tarefa ou problema. O aviso lembra que, se a tarefa ou o problema tiver registrado horas, eles serão movidos para o projeto ou excluídos. Você pode configurar se as horas serão excluídas ou movidas para o projeto na área [!UICONTROL Planilha de Horas e Preferências de Horas] da [!UICONTROL Instalação]. Depois de confirmar que você viu o aviso, a tarefa ou o problema é excluído. Para obter mais informações sobre como configurar as Preferências de Horas e Planilha de Horas, consulte [Configurar preferências de horas e Planilha de Horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

  >[!TIP]
  >
  >Quando você exclui um projeto com tarefas e problemas que têm horas reportadas, as horas reportadas são excluídas ou preservadas de acordo com as configurações na área [!UICONTROL Preferências de Planilha de Horas e Horas] da [!UICONTROL Instalação]. A mensagem de aviso não é exibida ao excluir um projeto.

* Ao desmarcar essa opção, você receberá um aviso proibitivo ao excluir uma tarefa ou problema com horas reportadas ou ao excluir um projeto com horas reportadas para suas tarefas ou problemas. O aviso especifica que o administrador não permite que tarefas ou problemas com horas reportadas sejam excluídos. As tarefas, problemas ou projetos que têm horas registradas para tarefas e problemas não podem ser excluídos.

### [!UICONTROL Datas efetivas] {#actual-dates}

<table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando uma tarefa ou problema muda de "Novo" para "Em andamento", defina a Data de início efetiva como]</td> 
    <td> <p>Selecione uma das seguintes opções para quando a Data de Início Efetivo for registrada em [!DNL Workfront] quando uma tarefa ou problema passar de <strong>[!UICONTROL Novo]</strong> para <strong>[!UICONTROL Em Andamento]</strong>:</p> 
      <ul> 
      <li><strong>[!UICONTROL Agora]:</strong> A Data de Início Efetivo está definida como a data atual.</li> 
      <li><strong>[!UICONTROL A Data de Início Planejada]:</strong> A Data de Início Efetiva está definida como a Data de Início Planejada da tarefa ou problema.</li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando uma tarefa ou problema é concluído, definir a Data de conclusão atual como]</td> 
    <td> <p>Selecione uma das seguintes opções para quando a Data de Término Efetivo for registrada em [!DNL Workfront] quando uma tarefa ou problema for concluído:</p> 
      <ul> 
      <li><strong>[!UICONTROL Agora]:</strong> A Data de Término Efetivo está definida como a data atual.</li> 
      <li> <p><strong>[!UICONTROL A Data de Conclusão Planejada]:</strong> A Data de Conclusão Efetiva está definida como a Data de Conclusão Planejada da tarefa ou problema.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

### Delegação

Habilitar a configuração **[!UICONTROL Permitir que usuários deleguem tarefas e problemas]** permite que todos os usuários no deleguem temporariamente seu trabalho a outras pessoas.

Quando essa configuração estiver ativada, os usuários poderão ver o seguinte:

* O link [!UICONTROL Delegar] em sua área [!UICONTROL Residência]. Eles podem delegar aprovações ou atribuições de tarefas e problemas daqui.
* Uma indicação de que uma tarefa ou problema é delegada a outro usuário na área [!UICONTROL Atribuições e delegações] no cabeçalho da tarefa ou problema.

  Se você desabilitar a configuração [!UICONTROL Permitir que os usuários deleguem tarefas e problemas], as delegações agendadas no momento serão interrompidas e os usuários delegados receberão uma notificação por email de que a delegação foi interrompida.

Para obter informações sobre como delegar trabalho a outras pessoas, consulte os seguintes artigos:

* [Delegar visão geral do trabalho](../../../manage-work/delegate-work/delegate-work-overview.md)
* [Gerenciar delegação de tarefas e problemas](../../../manage-work/delegate-work/how-to-delegate-work.md)

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
      <li><strong>[!UICONTROL Conceder a eles... acesso a uma tarefa]</strong>: define a permissão padrão que um usuário tem para a tarefa à qual está atribuído. Para obter mais informações sobre permissões de tarefas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</li> 
      <li> <p><strong>[!UICONTROL Também conceder a eles ... acesso ao projeto]</strong>: define a permissão padrão que um usuário tem para o projeto no qual tem uma tarefa atribuída a ele. Para obter mais informações sobre permissões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto do sistema</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando alguém é atribuído a um problema]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Conceder a eles... acesso a uma tarefa]</strong>: define a permissão padrão que um usuário tem para a tarefa à qual está atribuído. Para obter mais informações sobre permissões de tarefas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</li> 
      <li> <p><strong>[!UICONTROL Também conceder a eles ... acesso ao projeto]</strong>: define a permissão padrão que um usuário tem para o projeto no qual tem uma tarefa atribuída a ele. Para obter mais informações sobre permissões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto do sistema</a>.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td role="rowheader">[!UICONTROL Quando alguém envia uma solicitação]</td> 
    <td> 
      <ul> 
      <li><strong>[!UICONTROL Conceder a eles... acesso ao problema]</strong>: define a permissão padrão que um usuário tem em uma solicitação enviada. Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a>.</li> 
      <li> <p><strong>[!UICONTROL Pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações]</strong>: permite que os usuários vejam solicitações enviadas por outros usuários da mesma empresa que eles. Nessas solicitações, eles têm as mesmas permissões que têm em suas próprias solicitações enviadas.</p> </li> 
      </ul> </td> 
    </tr> 
  </tbody> 
</table>

1. Clique em **[!UICONTROL Salvar]**.

## Bloquear preferências de tarefas e problemas para grupos {#lock-task-and-issue-preferences-for-groups}

Se os grupos em sua organização precisarem de uma preferência de tarefa ou problema configurada de forma diferente para seus fluxos de trabalho exclusivos, você poderá desbloquear a preferência para todos os grupos em toda a organização para que eles possam configurá-la por conta própria. Quando uma preferência é desbloqueada e o administrador do grupo a modifica, as tarefas ou problemas associados ao grupo são afetados pela configuração do nível do grupo para a preferência em vez da configuração do nível do sistema.

Para obter informações sobre como um administrador de grupo configura preferências de tarefas e problemas para um grupo, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

>[!NOTE]
>
>Depois que um administrador do [!DNL Workfront] desbloqueia uma preferência no nível do sistema, qualquer administrador de grupo pode configurá-la e bloqueá-la para garantir que todos no grupo e nos subgrupos abaixo estejam usando a mesma configuração. Isso é paralelo à capacidade que um administrador do [!DNL Workfront] tem de configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Bloquear ou desbloquear uma preferência de projeto, tarefa ou problema para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

Para bloquear ou desbloquear uma preferência de tarefa ou problema para que os grupos possam configurá-la:

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Tarefas e problemas]**.

1. Siga um destes procedimentos:

   * Se quiser que os administradores de grupos abaixo do seu grupo possam configurar uma preferência para seus grupos, desbloqueie-a ![](assets/unlock-toggle-button.png).
   * Se quiser que o seu grupo e todos os grupos abaixo dele usem sua configuração como uma preferência, verifique se ele está bloqueado (esse é o padrão).

     >[!IMPORTANT]
     >
     >Recomendamos que você se comunique com os administradores e usuários em grupos em todo o sistema para garantir que todas as necessidades sejam consideradas na maneira como você configura uma preferência bloqueada. Ao bloqueá-lo, sua configuração para ele é herdada por todos os grupos no sistema. E se a preferência tiver sido desbloqueada por qualquer período, sua configuração substituirá aquelas que os administradores de grupo podem ter feito.

1. Clique em **[!UICONTROL Salvar]**.
