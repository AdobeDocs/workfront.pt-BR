---
title: Editar o perfil de um usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, você pode criar novos usuários e gerenciar os perfis dos existentes.
author: Courtney, Alina
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 0bf30319978e1ec41a7ba4dc08788e15024cd03f
workflow-type: tm+mt
source-wordcount: '2802'
ht-degree: 0%

---

# Editar o perfil de um usuário

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter instruções sobre como editar o perfil de um usuário no Adobe Admin Console, consulte a seção &quot;Editar detalhes do usuário&quot; no artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ou entre em contato com o administrador do Adobe Admin Console.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe Workfront, você pode criar novos usuários e gerenciar os perfis dos existentes. Para obter informações sobre como criar usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Os usuários com uma licença de Plano também podem criar e gerenciar usuários. Para obter informações sobre o acesso necessário para editar usuários, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do Administrador do sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p><b>Usuários</b> na configuração do seu nível de acesso configurado como <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois <b>Administrador do usuário</b> opções ativadas em <b>Ajustar as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se Usuário <b>Administrador (usuários do grupo)</b> estiver habilitado, você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> <p>Para obter mais informações sobre o <b>Usuários</b> configurar em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Editar um perfil de usuário

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).
1. Selecione o usuário e clique no ícone Editar ![](assets/edit-icon.png).

1. No **Editar usuário** for exibida, altere qualquer uma das informações a seguir e clique em **Salvar alterações**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Informações pessoais </td> 
      <td> 
       <ul> 
        <li><b>Nome</b>, <b>Sobrenome</b></li> 
        <li> <p><b>Endereço de email:</b> O endereço de email de um usuário também é seu nome de usuário no Workfront. Este campo diferencia maiúsculas de minúsculas e deve ser exclusivo. Se qualquer usuário tentar adicionar um endereço de email não exclusivo 3 vezes em uma janela de 10 minutos, uma resposta reCAPTCHA será exibida.</p> <p>Se você usar a  de lista de permissões de email e inserir um domínio de email que não esteja na lista, o usuário não receberá notificações por email. Para obter mais informações sobre a  de lista de permissões, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configurar sua  de lista de permissões de email</a>.</p> </li> 
        <li> <p><b>Redefinir senha</b>: Clique neste link para redefinir a senha do usuário. Você é solicitado a fornecer sua própria senha antes de poder redefinir a senha de um usuário.</p> <p>Para redefinir a senha de outro usuário, você deve ser um administrador do Workfront ou um administrador de grupo.</p> <p><b>Nota</b>:  
          <ul> 
           <li> <p>Se você for um administrador de grupo, poderá redefinir senhas somente para usuários dos grupos designados como tal. Além disso, a permissão Administrador de usuário (usuários do grupo) deve ser ativada em seu nível de acesso:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Esta configuração é desativada por padrão. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </li> 
           <li> <p>Não é possível redefinir a senha de um administrador do Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Nome do usuário</b>: Se o administrador do Workfront ativou uma integração SSO com o Workfront, o nome de usuário SSO será exibido neste campo. O tipo de configuração de SSO ativada para sua instância do Workfront é visível neste campo. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Autenticação</b>: Se o administrador do Workfront ativou uma integração SSO com o Workfront e atualizou todos os usuários para SSO, esse campo será selecionado por padrão. O tipo de configuração de SSO ativada para sua instância do Workfront é visível neste campo.</p> <p>Quando esse campo é selecionado, o usuário precisa fazer logon no Workfront com suas credenciais de SSO. Ao desmarcá-la, será possível fazer logon no Workfront com suas credenciais do Workfront.</p> <p>Para obter mais informações sobre como configurar o Workfront com uma solução SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Visão geral do logon único no Adobe Workfront</a></p> <p>Para obter mais informações sobre como atualizar usuários para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Atualizar usuários para logon único</a>.</p> <p><b>OBSERVAÇÃO</b>: Se você for um administrador de grupo, poderá editar a variável &lt;sso configuration=""&gt; campos somente para usuários nos grupos em que você está designado como tal. Além disso, a permissão Administrador de usuário (usuários do grupo) deve estar ativada em seu nível de acesso.
        <p>Se você for um administrador de grupo e tiver a permissão de Administrador de usuário (todos os usuários) ativada em seu nível de acesso, poderá editar a variável &lt;sso configuration=""&gt; campos para todos os usuários.</p> </li> 
        <li><b>Informações do trabalho:</b> Informações sobre o trabalho, como o cargo e a área de conhecimento pela qual o usuário é responsável.</li> 
        <li><p><b>Informações de contato</b>: O número de telefone e o endereço do usuário.</p>
        <p>Se o usuário estiver habilitado para o Gerenciamento de usuário unificado (UUM) ou para o Sistema Adobe Identity Management (IMS), a variável <b>País</b> na seção Informações de contato só aceita valores de código de país (por exemplo, US, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferências </td> 
      <td> 
       <ul> 
      <li> <p><b>Fuso Horário:</b> O fuso horário do usuário.</p> <p>Para obter informações sobre como ajudar usuários a colaborar no Workfront em vários fusos horários, consulte <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabalhar em vários fusos horários</a>.</p> </li> 
       <li><b>Localidade de email</b>: O local de email preferencial do usuário. Isso afeta o formato de números e datas nos emails provenientes do Workfront.</li>

   <li><b>Receber emails deste ambiente de teste</b>: Marque essa opção se desejar receber notificações por email do ambiente em que você está conectado no momento.
      <p><b>Nota</b></p>
      Essa opção está disponível somente nos ambientes Preview e Sandbox. Por padrão, as notificações por email são ativadas no ambiente Produção. 
      </li>

   <li><b>Mostrar porcentagem concluída no status de atualização</b>: Marque esta opção se desejar exibir uma barra de porcentagem completa dentro da área Atualizar das tarefas deste usuário.</li> 
       <li><b>Enviar trabalho que atribuo a mim mesmo para a guia Trabalhar</b>: Marque essa opção se desejar que tudo o que o usuário atribui a si mesmo apareça diretamente na guia Trabalhar em . O padrão é listar tudo o que é atribuído a um usuário na guia Solicitação de trabalho.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações</td> 
      <td> <p>Selecione as notificações por email que devem ser ativadas para o novo usuário.</p> <p>Você pode selecionar notificações instantâneas e diárias de resumo.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurar notificações de evento para todos no sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acesso</td> 
      <td> 
       <ul> 
      <li><b>Está ativo:</b> Selecione essa caixa para indicar que o usuário está ativo. Usuários ativos usam uma licença do Workfront. Limpar a caixa desativa o usuário.</li> 
       <li> <p><b>Nível de acesso:</b> Selecione o nível de acesso a ser atribuído a este usuário.</p> 
       <p>Ao atribuir um nível de acesso a um usuário, é possível atribuir um nível igual ou inferior ao seu próprio nível de acesso. (Por exemplo, se o nível de acesso for Planejador, você não poderá atribuir o nível de acesso Administrador.) No entanto, não é possível atribuir um nível de acesso que, por padrão, seja menor do que o seu próprio nível de acesso se o administrador do Workfront tiver ativado permissões não padrão no nível de acesso que também não estão ativadas em seu próprio nível de acesso (por meio das configurações de Ajuste Otimizado, conforme descrito em <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>). </p> 
       <p>Para obter mais informações sobre níveis de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configuração do acesso ao Adobe Workfront</a>.</p> </li> 
       <li> <p><b>Modelo de layout</b>: Escolha um modelo de layout para o usuário. Este Modelo de Layout tem precedência sobre qualquer Modelo de Layout atribuído ao Grupo Doméstico do usuário, Equipe Inicial ou função de trabalho principal. Para obter mais informações sobre a prioridade de atribuição de Modelos de Layout, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> <p><b>Nota</b>:  <p>A lista de modelos disponíveis neste campo depende do seu acesso:</p> 
       <ul> 
       <li>Como administrador do Workfront, você pode ver todos os modelos de layout de nível de sistema e de grupo.</li> 
       <li>Como administrador de grupo, você pode ver o modelo de layout no nível do sistema, bem como os associados aos grupos que você gerencia.</li> 
       <li>Como usuário com uma licença de Plano e acesso para editar usuários, você pode ver apenas Modelos de Layout no nível do sistema.</li> 
       </ul> <p>Para obter mais informações sobre Modelos de layout em nível de grupo, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organização </td> 
      <td> 
       <ul> 
      <li><b>Empresa</b>: A empresa do usuário. Os usuários podem ser associados somente a uma empresa. Você deve criar uma empresa antes de associá-la a um usuário. Somente empresas ativas são exibidas na lista. Para obter informações sobre como criar empresas, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Criar e editar empresas</a>.</li> 
      <li><b>Relatórios para:</b> Se você tiver especificado uma empresa para o usuário, também poderá especificar o gerente direto do usuário neste campo. Um usuário pode ter apenas um gerente.</li> 
      <li><b>Relatórios diretos:</b> Se você tiver especificado uma empresa para o usuário, também poderá especificar os relatórios diretos desse usuário. Um usuário pode ter vários relatórios diretos.</li> 
      <li><b>Equipe inicial</b>: Especifique a equipe inicial do usuário. Os usuários só podem ter uma equipe inicial.</li> 
      <li><b>Outras equipes</b>: Os usuários podem pertencer a várias equipes.</li> 
      <li> <p><b>Grupo Doméstico:</b> Selecione um grupo apropriado para atribuir o usuário. Isso dá ao usuário a capacidade de acessar objetos que são compartilhados com o grupo.</p> <p>Este campo é obrigatório. Todos os usuários devem estar associados a um grupo doméstico. Se você não selecionar uma, seu grupo será atribuído como o grupo doméstico do novo usuário.</p> <p><b>OBSERVAÇÃO</b>: Você pode atribuir um grupo a um usuário somente se for um administrador do Workfront, se for o administrador do grupo ou se o grupo for público.</p> </li> 
      <li> <p><b>Outros grupos</b>: Os usuários podem pertencer a vários grupos. Você pode atribuir um grupo a um usuário somente se for um administrador do Workfront, se for o administrador do grupo ou se o grupo for público.</p> <p><b>IMPORTANTE</b>: Adicionar um usuário a mais de 100 grupos pode causar problemas de desempenho em qualquer área do Workfront que carrega a lista de grupos.</p> <p>Para obter mais informações sobre grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Criar um grupo</a>.</p> <p>Para obter mais informações sobre grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral dos grupos</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planejamento de recursos </td> 
      <td> 
       <ul>
       <li>
       <b>Tempo de trabalho</b>: Representa a porcentagem do tempo FTE (Equivalente de Tempo Total) que o usuário está disponível para o trabalho real, não incluindo a sobrecarga. O Tempo de Trabalho deve ser um número decimal de até 1 e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.

   O padrão do campo é 1, indicando que um usuário gasta o FTE inteiro no trabalho real relacionado ao projeto.

   O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho real relacionado ao projeto.

   Para obter mais informações sobre como criar programações no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um agendamento</a>.

   As exceções de agendamento e o tempo limite também podem afetar a capacidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências do Gerenciamento de Recursos na área Configurar . Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências do Gerenciamento de recursos</a>.

   <b>DICA</b>

   Defina o valor Tempo de trabalho como 1 para indicar que o usuário está disponível para trabalho relacionado ao projeto e todo o seu equivalente em tempo integral.
   </li> 
      <li> <b>Agendar desativação</b>: Marque essa caixa se desejar agendar a desativação deste usuário após um período de tempo. </li> 
       <li><b>Data de desativação programada</b>: A data após a qual o usuário se torna desativado. Para obter informações sobre como programar usuários para desativação, consulte o <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Agendar usuários para desativação</a> em <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</li> 
       <li> <p><b>Função principal</b>: Essa é a função de trabalho principal que o usuário pode atender no Workfront. Todas as tarefas e problemas que o usuário está atribuído também são atribuídos a essa função de trabalho. As funções de trabalho são essenciais no gerenciamento de recursos. Você pode atualizar este campo somente se tiver uma licença do Plan com acesso administrativo de usuário ou se for um administrador do Workfront. Para obter mais informações sobre como configurar usuários com acesso administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> <p>Somente as funções de trabalho ativas são exibidas na lista. </p> </li> 
       <li>Se você selecionou um <b>Função principal</b>, o <b>Porcentagem de disponibilidade de FTE</b> é exibido. Especifique a porcentagem de tempo do agendamento do usuário alocada para esta função de trabalho. O valor padrão da Porcentagem de Disponibilidade de FTE para a Função Principal é 100%. </li> 
       <li> <p><b>Outras funções</b>: Um usuário pode ter várias funções de trabalho no Workfront. As funções de trabalho são essenciais no gerenciamento de recursos. Não há limite para quantas funções de trabalho um usuário pode atender. No entanto, recomendamos não atribuir um usuário a um número excessivamente grande de funções de trabalho, pois o gerenciamento de recursos pode se tornar muito complexo para esses usuários.<p>Somente as funções de trabalho ativas são exibidas na lista. Para obter mais informações sobre funções do job, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> <p>Você pode atualizar este campo somente se tiver uma licença do Plan com acesso administrativo de usuário ou se for um administrador do Workfront. <br>Para obter mais informações sobre como configurar usuários com acesso administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
       <li> <p>(Condicional) Se você selecionou um ou vários <b>Outras funções</b>, o <b>Porcentagem de disponibilidade de FTE</b> é exibido para cada função. Especifique qual porcentagem de tempo do agendamento do usuário é alocada para cada função de trabalho. O valor padrão da Porcentagem de Disponibilidade de FTE para outras Funções é 0%.</p> <p><b>OBSERVAÇÃO</b>: Se Outras Funções tiverem uma Disponibilidade de FTE de 0%, elas não serão exibidas no Planejador de Recursos, a menos que os usuários sejam atribuídos a tarefas nessas funções.</p> <p> <img alt="user_settings_role_and_date_boxes_rp_stories.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>Nota</b>: <p>A soma de todos <b>Porcentagens da disponibilidade de FTE</b> para todas as funções devem ser iguais a 100%. Cada Porcentagem da Disponibilidade de FTE calcula as Horas Disponíveis para cada função por usuário no Planejador de Recursos. As Horas Disponíveis para cada função por usuário dependem do tempo disponível para o usuário.</p> <p>O tempo disponível para o usuário é calculado pela Workfront, dependendo do método que foi selecionado pelo administrador do Workfront para calcular o FTE nas Preferências de gerenciamento de recursos.</p> <p>Para obter informações sobre como calcular a disponibilidade para o usuário, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos</a>.</p> <p>Para obter informações sobre como configurar preferências de Gerenciamento de Recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências do Gerenciamento de recursos</a>.</p> </p> </li> 
       <li> <p><b>Agendar</b>: Associe um agendamento ao usuário. O agendamento do usuário calcula a linha do tempo das tarefas às quais o usuário está atribuído.</p> <p>Você deve criar um agendamento antes de associá-lo a um usuário. Para obter mais informações sobre como criar programações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>.</p> <p><b>OBSERVAÇÃO</b>: Recomendamos que o agendamento associado ao usuário corresponda ao Fuso horário do usuário.</p> </li> 
       <li> <p><b>Perfil da folha de horas</b>: Associe um Perfil de folha de horas ao usuário para garantir que as folhas de horas sejam geradas automaticamente para ele.</p> <p><b>OBSERVAÇÃO</b>: A lista de perfis que você tem disponível neste campo depende do seu acesso:
       <ul>
       <li>Como administrador do Workfront, você pode ver todos os perfis de Folha de Horas a nível de sistema e todos os perfis de Folha de Horas a nível de grupo.</li>
       <li>Como administrador de grupo, você pode ver Perfis de Folha de Horas no nível do sistema, bem como os associados aos grupos que você gerencia.</li>
       <li>Como usuário com uma licença de Plano e acesso para editar usuários, você pode ver somente Perfis de Folha de Horas no nível do sistema. Para obter mais informações sobre Perfis de Folha de Horas em nível de grupo, consulte <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Criar, editar e atribuir perfis de folha de ponto</a>.</li>
      </ul></p> </li> 
       <li><b>Tipo de hora padrão</b>: Selecione o tipo de hora padrão para o usuário. Esse é o tipo de hora usado por padrão quando o usuário registra a hora.</li> 
       <li><b>Tipos de hora disponíveis</b>: Selecione os tipos de hora que devem estar disponíveis para o usuário. Esses tipos de hora estão visíveis em qualquer lugar no Workfront, onde o usuário pode registrar o tempo. Um usuário só pode ver os tipos de hora que estão ativados no nível do projeto, bem como o nível do usuário. Para obter mais informações sobre quais tipos de hora estão disponíveis para os usuários, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir os tipos de hora e a disponibilidade das folhas de horas</a>.</li> 
       <li><b>Tempo de logon:</b> Selecione se o usuário deve registrar o tempo nos itens de trabalho em horas ou dias. Para obter mais informações, consulte <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurar se a hora é registrada em horas ou dias</a>.</li>

   <li> <b>FTE</b>: Este é o Equivalente de Tempo Total do usuário. A Workfront usa esse número para calcular a disponibilidade do usuário com base na Programação Padrão somente quando as Preferências de Gerenciamento de Recursos no nível do sistema estão definidas como A Programação Padrão.

   <p>O FTE indica o tempo que o usuário pode gastar no trabalho. Isso inclui despesas gerais, bem como tempo gasto no trabalho do projeto. Por exemplo, o tempo gasto em reuniões ou treinamento também é incluído no ETI.</p>

   O FTE deve ser um número decimal até 1 e não pode ser 0. Por exemplo, se o valor FTE for 0,5 e o Horário padrão no Workfront for de 40 horas, o usuário estará disponível por 20 horas por semana.

   O padrão do campo é 1.

   Exceções de programação, tempo limite e valor de Tempo de Trabalho podem afetar a disponibilidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências do Gerenciamento de Recursos na área Configurar .

   Se as Preferências do Gerenciamento de Recursos no nível do sistema estiverem definidas como O Agendamento do Usuário, o valor especificado aqui será ignorado e o usuário será considerado como disponível de acordo com o que é especificado em seu agendamento.

   Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências do Gerenciamento de recursos</a>.

   Para obter mais informações sobre como criar programações no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um agendamento</a>.
   </li>

   <li><b>Pools de Recursos</b>: Associe o usuário aos Pools de Recursos. Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associar pools de recursos a usuários </a>.</li> 
        <li><b>Custo por hora</b>: A quantidade de custo por hora para o usuário. </li> 
        <li><b>Faturamento por hora</b>: A quantidade de faturamento por hora para o usuário.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulários personalizados</td> 
      <td><p>Associe um formulário personalizado do usuário existente a este usuário. É necessário criar um formulário personalizado antes de associá-lo a um usuário. Somente os formulários personalizados ativos são exibidos na lista. Os campos que você não tem acesso para editar não são exibidos em um formulário personalizado individual.</p> <p>Para obter informações sobre como criar formulários personalizados, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comentário</td> 
      <td>Digite o comentário que deseja enviar aos usuários e à área Atualizações de seus perfis de usuário.</td> 
     </tr> 
    </tbody> 
   </table>
