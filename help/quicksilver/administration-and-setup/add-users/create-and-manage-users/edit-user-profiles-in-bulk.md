---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Editar perfis de usuário em massa
description: Como administrador do Adobe Workfront, você pode editar contas de usuário em massa.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: c7b91828e5a4f961fc48e857eb63756b9b38f664
workflow-type: tm+mt
source-wordcount: '2625'
ht-degree: 0%

---

# Editar perfis de usuário em massa

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Você pode editar contas de usuário em massa. Ao editar usuários em massa, somente os campos selecionados especificamente são atualizados com as mesmas informações para todos os usuários selecionados. Todos os outros campos não selecionados permanecem os mesmos para cada usuário individual, mesmo que sejam diferentes para cada usuário.

>[!NOTE]
>
>* Não é possível editar a seção Informações pessoais dos perfis dos usuários em massa, pois essas informações devem ser exclusivas para cada usuário.
>* Para garantir a precisão dos dados e o desempenho ideal, recomendamos que você selecione no máximo 2000 usuários de uma só vez para uma edição em massa.
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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p><p>Ou</p><p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. </li> 
     <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar contas de usuário em massa

{{step-1-to-users}}

1. Selecione mais de um usuário e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png).

1. Na caixa **Editar Usuário**, altere as informações em qualquer uma das seções e clique em **Salvar Alterações** <span class="preview">ou **Salvar**</span> a qualquer momento.

### Preferências

* **Fuso Horário**: o fuso horário do usuário.

  Para obter informações sobre como ajudar usuários a colaborar na Workfront em fusos horários diferentes, consulte [Trabalhando em fusos horários diferentes](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **Localidade de email**: a localidade de email preferencial do usuário. Isso afeta o formato de números e datas nos emails que vêm do Workfront para esse usuário.

  >[!NOTE]
  >
  >Quando sua organização está na Experiência unificada do Adobe, as preferências de idioma do usuário são armazenadas no perfil do Adobe e a localidade do email não é usada. Para obter informações sobre como acessar essas preferências, consulte [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

### Notificações

Selecione as notificações por email que devem ser ativadas para os usuários.

Você pode selecionar notificações de resumo instantâneas e diárias. Todas as notificações de resumo diárias são entregues algum tempo depois do mesmo tempo para todos os usuários selecionados.

Para obter mais informações, consulte [Configurar notificações de eventos para todos no sistema](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

### Acesso

* **Está ativo** / <span class="preview">**O usuário está ativo**</span>: habilite esta opção para indicar que os usuários estão ativos. Usuários ativos usam uma licença Workfront. A desativação do campo desativa os usuários e os impede de fazer logon no Workfront.

* **Nível de Acesso**: selecione o nível de acesso a ser atribuído a esses usuários. Todos os usuários selecionados terão o mesmo nível de acesso.

  Ao atribuir um nível de acesso aos usuários, você pode atribuir um nível igual ou inferior ao seu próprio nível de acesso. (Por exemplo, se o seu nível de acesso for Padrão, você não poderá atribuir o nível de acesso Administrador.)

  No entanto, não é possível atribuir um nível de acesso que, por padrão, seja inferior ao seu próprio nível de acesso se o administrador do Workfront tiver ativado permissões não padrão no nível de acesso que também não estejam ativadas no seu próprio nível de acesso.

  Por exemplo, se você tiver uma licença Standard sem acesso para excluir tarefas, não será possível atribuir uma licença Light a alguém com acesso para excluir tarefas, embora a licença Light seja inferior à licença Standard. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Para obter mais informações sobre níveis de acesso, consulte [Configurar acesso ao Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  >[!NOTE]
  >
  >Se sua organização usar o novo modelo de acesso (Padrão/Claro/Colaborador), você não poderá reatribuir um usuário Padrão ou Light a um nível de acesso de Colaborador se ele já tiver atingido o limite de decisão para o mês.
  >
  >Para obter mais informações sobre o novo modelo de acesso, consulte [Visão geral sobre novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >Para obter informações sobre limites de decisão, consulte [Visão geral sobre documento limitado e decisão de prova para usuários não pagos](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Modelo de layout**: escolha um modelo de layout para os usuários. este modelo de layout tem precedência sobre qualquer modelo de layout atribuído ao Grupo padrão, Equipe padrão ou Função principal. Para obter mais informações sobre a prioridade de atribuição de modelos de layout, consulte [Criar e gerenciar modelos de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

  A lista a seguir descreve como a lista de modelos disponíveis neste campo depende do seu acesso:

   * Como administrador do Workfront, você pode ver todos os modelos de layout de nível de sistema e de grupo.
   * Como administrador de grupo, você pode ver o modelo de layout no nível do sistema, bem como aqueles associados aos grupos que gerencia.
   * Como um usuário com uma licença Padrão ou de Plano e acesso para editar usuários, você pode ver apenas modelos de layout no nível do sistema.

     Para obter mais informações sobre modelos de layout de nível de grupo, consulte [Criar e modificar modelos de layout de um grupo](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organização

* **Empresa**: a empresa dos usuários. Os usuários podem ser associados a apenas uma empresa. Você deve criar uma empresa antes de associá-la a um usuário. Somente empresas ativas são exibidas na lista. Para obter informações sobre como criar empresas, consulte [Criar e editar empresas](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* **Equipe interna**: especifique a equipe interna dos usuários. Os usuários só podem ter uma equipe inicial.
* **Outras equipes**: os usuários podem pertencer a várias equipes.
* **Grupo Doméstico** / <span class="preview">**Grupo Doméstico Atual**</span>: selecione um grupo apropriado para atribuir aos usuários. Isso dá aos usuários a capacidade de acessar objetos que são compartilhados com o grupo. Você também pode compartilhar modelos de layout com um Grupo padrão.

  Este campo é obrigatório. Todos os usuários devem estar associados a um grupo padrão. Se você não selecionar um, seu Grupo Padrão será atribuído como o Grupo Padrão.

  Você pode atribuir um grupo a um usuário somente se um dos seguintes for verdadeiro:

   * você é um administrador do Workfront
   * você é o administrador do grupo
   * o grupo é público

* **Outros grupos**: os usuários podem pertencer a vários grupos. Você pode atribuir um grupo a um usuário somente se for um administrador do Workfront, se for o administrador do grupo ou se o grupo for público.

  >[!IMPORTANT]
  >
  >Adicionar um usuário a mais de 100 grupos pode causar problemas de desempenho em qualquer área do Workfront que carrega a lista de grupos.

  Para obter mais informações sobre grupos públicos, consulte [Criar um grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

  Para obter mais informações sobre grupos, consulte [Visão geral sobre grupos](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Planejamento de recursos

* **Tempo de Trabalho**: representa a porcentagem de tempo FTE (equivalente a tempo completo) em que os usuários estão disponíveis para o trabalho real, sem incluir a sobrecarga. A Hora Útil deve ser um número decimal até 1, e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.

  O campo padrão é 1, indicando que um usuário gasta todo o FTE em trabalho real relacionado ao projeto.

  O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho real relacionado ao projeto.

  Para obter mais informações sobre como criar agendas no Workfront, consulte [Criar uma agenda](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  As exceções de agendamento e a folga também podem afetar a capacidade do usuário.

  O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área Configuração. Para obter mais informações, consulte [Configurar preferências de Gerenciamento de Recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  >[!TIP]
  >
  >Defina o valor de Tempo de trabalho como 1 para indicar que o usuário está disponível para trabalho relacionado ao projeto em todo o equivalente de tempo integral.

* **Agendar Desativação** / <span class="preview">**Definir data de desativação**</span>: marque esta caixa / <span class="preview">clique neste botão</span> se desejar agendar a desativação desses usuários em uma determinada data e em um determinado horário.
* **Data de Desativação Agendada** / <span class="preview">**Data de Desativação**</span>: a data e a hora em que os usuários são desativados. Para obter informações sobre como agendar usuários para desativação, consulte [Agendar usuários para desativação](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation) em [Desativar ou reativar um usuário](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
* **Função principal**: esta é a função principal que os usuários podem desempenhar no Workfront. Todas as tarefas e problemas aos quais os usuários estão atribuídos também são atribuídos a essa função de trabalho. As funções de trabalho são essenciais no gerenciamento de recursos. Você só poderá atualizar esse campo se tiver uma licença Padrão ou de Plano com acesso de usuário administrativo ou se for um administrador do Workfront. Para obter mais informações sobre como configurar usuários com acesso administrativo, consulte [Conceder acesso aos usuários](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  Somente as funções de trabalho ativas são exibidas na lista.

* (Condicional) Se você selecionou uma **Função principal**, o campo **Porcentagem de disponibilidade de FTE** será exibido. Especifique que porcentagem de tempo dos agendamentos dos usuários está alocada para esta função de trabalho. O valor padrão para o Percentual de Disponibilidade de FTE para a Função Principal é 100%.
* **Outras funções**: os usuários podem ter várias funções de trabalho no Workfront. As funções de trabalho são essenciais no gerenciamento de recursos. Não há limite para quantas funções de trabalho um usuário pode realizar. No entanto, recomendamos não atribuir um usuário a um número excessivamente grande de funções de trabalho, pois o gerenciamento de recursos pode se tornar muito complexo para esses usuários.

  Somente as funções de trabalho ativas são exibidas na lista. Para obter mais informações sobre funções de trabalho, consulte [Criar e gerenciar funções de trabalho](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

  Você só poderá atualizar esse campo se tiver uma licença Padrão ou de Plano com acesso de usuário administrativo ou se for um administrador do Workfront.

  Para obter mais informações sobre como configurar usuários com acesso administrativo, consulte [Conceder acesso aos usuários](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Condicional) Se você selecionou uma ou várias **Outras funções**, o campo **Porcentagem de disponibilidade de FTE** será exibido para cada função. Especifique que porcentagem de tempo dos cronogramas dos usuários está alocada para cada função de trabalho. O valor padrão para a Porcentagem de Disponibilidade FTE para as Outras Funções é 0%.

  Se Outras Funções tiverem 0% de Disponibilidade FTE, elas não serão exibidas no Planejador de Recursos, a menos que os usuários sejam atribuídos a tarefas nessas funções.

  A soma de todos os **Percentuais de Disponibilidade de FTE** para todas as funções deve ser igual a 100%. Cada Porcentagem de Disponibilidade de FTE calcula as Horas Disponíveis para cada função por usuário no Planejador de Recursos. As Horas Disponíveis para cada função por usuário dependem do tempo disponível para o usuário.

  O tempo disponível para o usuário é calculado pelo Workfront, dependendo do método selecionado pelo administrador do Workfront para calcular o FTE nas Preferências de gerenciamento de recursos.

  Para obter informações sobre como calcular a disponibilidade do usuário, consulte [Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Para obter informações sobre como configurar preferências de Gerenciamento de Recursos, consulte [Configurar preferências de Gerenciamento de Recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Agendamento**: associe um agendamento aos usuários. O agendamento dos usuários calcula a linha do tempo das tarefas às quais os usuários estão atribuídos.

  Você deve criar um agendamento antes de associá-lo aos usuários. Para obter mais informações sobre como criar agendas, consulte [Criar uma agenda](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  >[!IMPORTANT]
  >
  >O Workfront só usa o agendamento de um usuário quando a configuração **Calcular Disponibilidade de Recursos Usando** está definida como **O Agendamento do Usuário**. Para obter informações sobre como essa configuração afeta qual agendamento é usado para o Gerenciamento de Recursos, consulte [Configurar preferências de Gerenciamento de Recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

* **Perfil de Planilha de Horas**: Associe um Perfil de Planilha de Horas aos usuários para garantir que as planilhas de horas sejam geradas automaticamente.

  A lista de perfis que você tem disponível neste campo depende do seu acesso:

   * Como administrador do Workfront, você pode ver todos os perfis de planilha de horas no nível do sistema e no nível do grupo.
   * Como administrador de grupo, você pode ver os Perfis de planilha de horas no nível do sistema, bem como aqueles associados aos grupos que você gerencia.
   * Como um usuário com uma licença Padrão ou de Plano e acesso para editar usuários, você pode ver somente Perfis de planilha de horas no nível do sistema. Para obter mais informações sobre Perfis de Planilha de Horas no nível do grupo, consulte [Criar, editar e atribuir perfis de planilha de horas](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Tipo de Hora Padrão**: Selecione o tipo de hora padrão para os usuários. Esse é o tipo de hora usado por padrão quando os usuários registram tempo.
* **Tipos de Horas Disponíveis**: Selecione os tipos de horas que devem estar disponíveis para os usuários. Esses tipos de horas estão visíveis em qualquer lugar no Workfront, onde os usuários possam registrar horas. Os usuários só podem ver os tipos de horas que estão ativados no nível do projeto, bem como no nível do usuário. Para obter mais informações sobre quais tipos de horas estão disponíveis para os usuários, consulte [Definir tipos de horas e disponibilidade](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **FTE**: este é o equivalente de tempo integral dos usuários. O Workfront usa esse número para calcular a disponibilidade dos usuários com base na Programação Default apenas quando as Preferências de Gerenciamento de Recursos no nível do sistema são definidas como A Programação Default.

  O FTE indica a quantidade de tempo que os usuários podem gastar no trabalho. Isso inclui as despesas gerais e o tempo gasto no trabalho do projeto. Por exemplo, o tempo gasto em reuniões ou treinamento também é incluído no FTE.

  O FTE deve ser um número decimal até 1 e não pode ser 0. Por exemplo, se o valor de FTE for 0,5 e o Agendamento padrão no Workfront for 40 horas, os usuários estarão disponíveis 20 horas por semana.

  O padrão do campo é 1.

  Exceções de cronograma, folga e o valor de Tempo de trabalho podem afetar a disponibilidade dos usuários.

  O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área Configuração.

  Se as Preferências de Gerenciamento de Recursos no nível do sistema forem definidas como O Cronograma do Usuário, o valor especificado aqui será ignorado e o usuário será considerado disponível de acordo com o especificado em seu cronograma.

  Para obter mais informações, consulte [Configurar preferências de Gerenciamento de Recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Para obter mais informações sobre como criar agendas no Workfront, consulte [Criar uma agenda](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Conjuntos de Recursos**: associe os usuários aos Conjuntos de Recursos.

  >[!NOTE]
  >
  >Somente os conjuntos de recursos comuns a todos os usuários selecionados aparecem nesse campo. Se os usuários selecionados não tiverem conjuntos de recursos compartilhados, esse campo ficará vazio. Se esse campo estiver vazio, os conjuntos de recursos especificados aqui substituirão seus conjuntos de recursos individuais.

  Para obter mais informações sobre pools de recursos, consulte [Associar pools de recursos a usuários](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

* **Taxa de Custo**: a quantidade de custo por hora para o usuário.

  Para taxas de custo atuais, clique em **Adicionar taxa**. Informe o valor da taxa de custo para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A Taxa de Custo 1 não terá uma data inicial e a última taxa de custo não terá uma data final.

  Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de Custo 1 não tiver uma data final e você adicionar a Taxa de Custo 2 com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de Custo 1 para que não haja lacunas.

* **Taxa de Cobrança**: a quantidade de cobrança por hora para o usuário.

  Para taxas de cobrança efetivas por data, clique em **Adicionar taxa**. Informe o valor da taxa de faturamento para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A Taxa de Cobrança 1 não terá uma data inicial e a última taxa de cobrança não terá uma data final.

  Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de cobrança 1 não tiver uma data final e você adicionar um segundo com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de cobrança 1 para que não haja lacunas.

### Formulários personalizados

Associar um formulário personalizado de usuário existente aos usuários. Você deve criar um formulário personalizado antes de associá-lo a um usuário. Somente formulários personalizados ativos são exibidos na lista. Os campos que você não tem acesso para editar não são exibidos em um formulário personalizado individual.

>[!NOTE]
>
>Recursos avançados de formulário personalizado, como campos de pesquisa externos e campos nativos do Workfront, só estão disponíveis quando você abre o registro do usuário na página de detalhes, não na caixa de diálogo Editar usuário. (Na lista de usuários, clique no nome do usuário para abrir os detalhes.)

Opcionalmente, você pode selecionar a opção **Recalcular Expressões Personalizadas** para garantir que todos os campos personalizados calculados em formulários personalizados anexados aos usuários selecionados estejam atualizados.

Para obter informações sobre como criar formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Comentário

Digite o comentário que deseja enviar aos usuários e à área Atualizações dos perfis de usuários.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

