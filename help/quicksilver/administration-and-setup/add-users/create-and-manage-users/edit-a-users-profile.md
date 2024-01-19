---
title: Editar o perfil de um usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, você pode criar novos usuários e gerenciar os perfis dos existentes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0343fe74-1be4-43e2-9e3d-8aa1f7ea26fa
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '3381'
ht-degree: 0%

---

# Editar o perfil de um usuário

{{highlighted-preview}}

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter instruções sobre como editar o perfil de um usuário no Adobe Admin Console, consulte a seção &quot;Editar detalhes do usuário&quot; no artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ou entre em contato com o administrador do Adobe Admin Console.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Como administrador do Adobe Workfront, você pode criar usuários e gerenciar os perfis dos existentes. Para obter informações sobre como criar usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

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
   <td> <p>Novo: Padrão</p>
   Ou
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. Para obter informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>. </p> </li> 
     <li> <p>A variável <b>Usuários</b> objeto no seu nível de acesso configurado para <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois critérios seguintes <b>Administrador de Usuários</b> opções ativadas em <b>Ajuste as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> Administrador de Usuários (Todos os usuários)</li>
     <li>Administrador de Usuários (Usuários de Grupo)</li></ul>
     <p>Se  <b>Administrador de Usuários (Usuários de Grupo)</b> estiver ativado, você deve ser um administrador de grupo em um grupo do qual o usuário seja membro para poder editar o usuário.</p> 
     <p>Para obter mais informações sobre o <b>Usuários</b> em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table> 
*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Editar um perfil de usuário

{{step-1-to-users}}

1. Selecione o usuário e clique no botão **Editar** ícone ![](assets/edit-icon.png).

   A caixa Editar Usuário é exibida.

1. No **Editar Usuário** , altere as informações a seguir e clique em **Salvar alterações** a qualquer momento:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Informações pessoais </td> 
      <td> 
       <ul> 
        <li><p><b>Nome</b></p></li>
        <li><p><b>Sobrenome</b></p></li> 
        <li> <p><b>Endereço de email:</b> O endereço de email de um usuário também é seu nome de usuário no Workfront. Esse campo diferencia maiúsculas e minúsculas e deve ser exclusivo. Se qualquer usuário tentar adicionar um endereço de email não exclusivo 3 vezes em uma janela de 10 minutos, uma resposta do reCAPTCHA será exibida.</p> <p> Selecione o <b>Eu não sou um robô</b> antes de continuar.</p><p>Se você usar a inclui na lista de permissões por email e inserir um domínio de email que não esteja na lista, o usuário não receberá notificações por email. Para obter mais informações sobre a inclui na lista de permissões, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configurar a inclui na lista de permissões por email</a>.</p> </li> 
        <li> <p><b>Redefinir senha</b>: Clique neste link para redefinir a senha do usuário. Você deve digitar sua própria senha antes de redefinir a senha de outro usuário.</p> <p>Para redefinir a senha de outro usuário, você deve ser um administrador do Workfront ou um administrador de grupo.</p> <p><b>NOTA</b>:  
          <ul> 
           <li> <p>Se você for um administrador de grupo, poderá redefinir senhas somente para usuários nos grupos em que foi designado como administrador. Além disso, a permissão Administrador de usuários (usuários de grupo) deve estar ativada em seu nível de acesso:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Essa configuração é desativada por padrão. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </li> 
           <li> <p>Não é possível redefinir a senha de um administrador do Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;sso configuration=""&gt; Nome de usuário</b>: Se o administrador do Workfront tiver ativado uma integração de SSO com o Workfront, o Nome de usuário do SSO será exibido nesse campo. O tipo de configuração de SSO ativado para sua instância do Workfront é visível nesse campo. </li> 
        <li> <p><b>OnlyAllow &lt;sso configuration=""&gt; Autenticação</b>: Se o administrador do Workfront tiver habilitado uma integração de SSO com o Workfront e atualizado todos os usuários para SSO, esse campo será selecionado por padrão. O tipo de configuração de SSO ativado para sua instância do Workfront é visível nesse campo.</p> <p>Quando esse campo é selecionado, o usuário precisa fazer logon no Workfront com suas credenciais de SSO. Ao desmarcá-la, você poderá fazer logon no Workfront com as credenciais da Workfront.</p> <p>Para obter mais informações sobre como configurar o Workfront com uma solução SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Visão geral do logon único no Adobe Workfront</a></p> <p>Para obter mais informações sobre a atualização de usuários para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Atualizar usuários para logon único</a>.</p> 
        <p><b>NOTA</b>:</p> 
        <p> Se você for um administrador de grupo, poderá editar a variável &lt;sso configuration=""&gt; campos somente para usuários nos grupos em que você está designado como tal. Além disso, a permissão Administrador de usuário (usuários de grupo) deve estar ativada em seu nível de acesso.
        <p>Se você for um administrador de grupo e tiver a permissão Administrador de usuário (todos os usuários) ativada no seu nível de acesso, poderá editar a variável &lt;sso configuration=""&gt; para todos os usuários.</p> </li> 
        <li><b>Informações da tarefa:</b> Informações sobre o cargo, como o título do cargo (no campo <b>Título</b> domínio de especialização pelo qual o utilizador é responsável (no domínio da <b>Fale comigo sobre</b> campo).</li> 
        <li><p><b>Informações de contato</b>: O número de telefone do usuário (na caixa <b>Número de telefone, ramal</b>, e <b>Celular</b> campos) e endereço (no campo <b>Endereço, Cidade, Estado, CEP, País</b> campos ).</p>
        <p>Se o usuário estiver ativado para o Gerenciamento unificado de usuários (UUM) ou para o Sistema Adobe Identity Management (IMS), a variável <b>País</b> na seção Contact Info (Informações de contato) aceita apenas valores de código de país (por exemplo, EUA, GB, ENTRADA).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferências </td> 
      <td> 
       <ul> 
      <li> <p><b>Fuso Horário:</b> O fuso horário do usuário.</p> <p>Para obter informações sobre como ajudar os usuários a colaborar na Workfront em vários fusos horários, consulte <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabalhar em fusos horários</a>.</p> </li> 
       <li><b>Local de email</b>: a localidade de email preferencial do usuário. Isso afeta o formato de números e datas nos emails que vêm do Workfront para esse usuário.</li>

   <li><b>Receber emails deste ambiente de teste</b>: marque esta opção se desejar receber notificações por email do ambiente em que você está conectado no momento.
      <p><b>Nota</b></p>
      <p>Essa opção está disponível somente nos ambientes Pré-visualização e Sandbox. As notificações por email estão ativadas no ambiente de Produção por padrão. </p>
      </li>

   <li><b>Mostrar o percentual concluído em atualização de status</b>: marque esta opção se desejar exibir uma barra de porcentagem concluída na área de Atualização das tarefas deste usuário, ao usar a experiência de comentário herdada. Para obter informações, consulte <a href="/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md">Nova experiência de comentários</a>.</li> 
       <li><b>Enviar trabalho que eu atribuir a mim mesmo para minha guia Trabalhando em</b>: marque esta opção se desejar que tudo o que o usuário atribuir a si mesmo seja exibido diretamente na lista Em execução na área Página inicial. O padrão é listar tudo atribuído a um usuário nas listas Pronto para iniciar ou Não pronto na área Página inicial.</li> 
       <li><b>Gerar provas automaticamente ao carregar documentos</b>: marque esta opção se desejar que os documentos carregados pelo usuário gerem uma prova imediatamente. </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações</td> 
      <td> <p>Selecione as notificações por email que devem ser ativadas para o novo usuário.</p> <p>Você pode selecionar notificações de resumo instantâneas e diárias.</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurar notificações de eventos para todos no sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acesso</td> 
      <td> 
       <ul> 
      <li><b>Está ativo:</b> Selecione esta caixa para indicar que o usuário está ativo. Usuários ativos usam uma licença Workfront. Limpar a caixa desativa o usuário e impede que ele faça logon no Workfront.</li> 
       <li> <p><b>Nível de acesso:</b> Selecione o nível de acesso a ser atribuído a este usuário.</p> 
       <p>Ao atribuir um nível de acesso a um usuário, você pode atribuir um nível igual ou inferior ao seu próprio nível de acesso.</p>
       <p>Por exemplo, se o seu nível de acesso for Plano, você não poderá atribuir o nível de acesso Administrador. No entanto, não é possível atribuir um nível de acesso que, por padrão, seja inferior ao seu próprio nível de acesso se o administrador do Workfront tiver ativado permissões não padrão no nível de acesso que também não estejam ativadas no seu próprio nível de acesso. </p>
       <p>Por exemplo, se você tiver uma licença de Plano sem acesso para excluir tarefas, não será possível atribuir uma licença de Trabalho a alguém com acesso para excluir tarefas, embora a licença de Trabalho seja inferior à licença de Plano. Para obter mais informações, consulte  <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> 
       <p>Para obter mais informações sobre níveis de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configuração do acesso ao Adobe Workfront</a>.</p>
       <p> <b>NOTA:</b></p> 
       <p> Se sua organização usar o novo modelo de acesso (Padrão/Claro/Colaborador), você não poderá reatribuir um usuário Padrão ou Light a um nível de acesso de Colaborador se ele já tiver atingido o limite de decisão para o mês. </p><p>Para obter mais informações sobre o novo modelo de acesso, consulte <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Visão geral dos novos níveis de acesso</a>. </p><p>Para obter informações sobre limites de decisão, consulte <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Visão geral de documentos e decisões de prova limitados para usuários não pagos</a>.</p></li> 
       <li> <p><b>Modelo de layout</b>: escolha um modelo de layout para o usuário. Este modelo de layout tem prioridade sobre qualquer modelo de layout atribuído ao grupo padrão, à equipe padrão ou à função principal do usuário. Para obter mais informações sobre a prioridade de atribuição dos Modelos de layout, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> <p><b>NOTA</b>:  <p>A lista a seguir descreve como a lista de modelos disponíveis neste campo depende do seu acesso:</p> 
       <ul> 
       <li>Como administrador do Workfront, você pode ver todos os Modelos de layout no nível do sistema e no nível do grupo.</li> 
       <li>Como administrador de grupo, você pode ver o modelo de layout no nível do sistema, bem como aqueles associados aos grupos que gerencia.</li> 
       <li>Como um usuário com uma licença de Plano e acesso para editar usuários, você pode ver apenas Modelos de layout no nível do sistema.</li> 
       </ul> <p>Para obter mais informações sobre Modelos de layout de nível de grupo, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organização </td> 
      <td> 
       <ul> 
      <li><b>Empresa</b>: A empresa do usuário. Os usuários podem ser associados a apenas uma empresa. Você deve criar uma empresa antes de associá-la a um usuário. Somente empresas ativas são exibidas na lista. Para obter informações sobre como criar empresas, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Criar e editar empresas</a>.</li> 
      <li><b>Relatórios para:</b> Se você tiver especificado uma empresa para o usuário, também poderá especificar o gerente direto do usuário neste campo. Um usuário pode ter apenas um gerente. Esse campo não será exibido se o usuário não estiver associado a uma empresa primeiro. </li> 
      <li><b>Relatórios diretos:</b> Se tiver especificado uma empresa para o usuário, você também poderá especificar os subordinados diretos do usuário. Um usuário pode ter vários subordinados diretos. Esse campo não será exibido se o usuário não estiver associado a uma empresa primeiro.</li> 
      <li><b>Equipe interna</b>: especifique a equipe inicial do usuário. Os usuários só podem ter uma equipe inicial. A Equipe interna é importante ao atribuir um modelo de layout ou ao definir o botão Trabalhar na tarefa para as tarefas e problemas atribuídos ao usuário. </li> 
      <li><b>Outras equipes</b>: os usuários podem pertencer a várias equipes. Um usuário pode visualizar itens de trabalho atribuídos a qualquer uma de suas equipes na área Início. </li> 
      <li> <p><b>Grupo Padrão:</b> Selecione um grupo apropriado para atribuir ao usuário. Isso dá ao usuário a capacidade de acessar objetos que são compartilhados com o grupo. Você também pode compartilhar modelos de layout com o Grupo padrão do usuário.</p> <p>Este campo é obrigatório. Todos os usuários devem estar associados a um grupo padrão. Se você não selecionar um, seu grupo será atribuído como o grupo inicial do novo usuário.</p> <p><b>NOTA</b>:</p> 
      <p> Você pode atribuir um grupo a um usuário somente se um dos seguintes for verdadeiro:</p>
      <ul><li>você é um administrador do Workfront</li>
      <li>você é o administrador do grupo</li>
      <li>o grupo é público.</li></ul> 
      <li> <p><b>Outros grupos</b>: os usuários podem pertencer a vários grupos. Você pode atribuir um grupo a um usuário somente se for um administrador do Workfront, se for o administrador do grupo ou se o grupo for público.</p> <p><b>IMPORTANTE</b>:</p> 
      <p>Adicionar um usuário a mais de 100 grupos pode causar problemas de desempenho em qualquer área do Workfront que carrega a lista de grupos.</p> <p>Para obter mais informações sobre grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Criar um grupo</a>.</p> <p>Para obter mais informações sobre grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral dos grupos</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planejamento de recursos </td> 
      <td> 
       <ul>
       <li>
       <b>Horário de trabalho</b>: representa a porcentagem de tempo Equivalente a Tempo Integral (FTE) em que o usuário está disponível para o trabalho real, sem incluir o custo indireto. A Hora Útil deve ser um número decimal até 1, e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.

   O campo padrão é 1, indicando que um usuário gasta todo o FTE em trabalho real relacionado ao projeto.

   O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho real relacionado ao projeto.

   Para obter mais informações sobre como criar agendas no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um agendamento</a>.

   As exceções de agendamento e a folga também podem afetar a capacidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área Configuração. Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de gerenciamento de recursos</a>.

   <b>DICA</b>

   Defina o valor de Tempo de trabalho como 1 para indicar que o usuário está disponível para trabalho relacionado ao projeto em todo o equivalente de tempo integral.
   </li> 
      <li> <b>Desativação programada</b>: marque esta caixa se desejar agendar a desativação desse usuário em uma determinada data e em um determinado horário. </li> 
       <li><b>Data de desativação programada</b>: A data e a hora em que o usuário se torna desativado. Para obter informações sobre como programar usuários para desativação, consulte a <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Programar usuários para desativação</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</li> 
       <li> <p><b>Função Primária</b>: essa é a principal função de trabalho que o usuário pode realizar no Workfront. Todas as tarefas e problemas aos quais o usuário está atribuído também são atribuídos a essa função de trabalho. As funções de trabalho são essenciais no gerenciamento de recursos. Você só poderá atualizar esse campo se tiver uma licença de Plano com acesso de usuário administrativo ou se for um administrador do Workfront. Para obter mais informações sobre a configuração de usuários com acesso de usuário administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> <p>Somente as funções de trabalho ativas são exibidas na lista. </p> </li> 
       <li>Se você selecionou um <b>Função Primária</b>, o <b>Porcentagem de Disponibilidade de FTE</b> é exibido. Especifique o percentual de tempo do agendamento do usuário alocado para esta função de trabalho. O valor padrão para o Percentual de Disponibilidade de FTE para a Função Principal é 100%. </li> 
       <li> <p><b>Outras Funções</b>: um usuário pode ter várias funções de trabalho no Workfront. As funções de trabalho são essenciais no gerenciamento de recursos. Não há limite para quantas funções de trabalho um usuário pode realizar. No entanto, recomendamos não atribuir um usuário a um número excessivamente grande de funções de trabalho, pois o gerenciamento de recursos pode se tornar muito complexo para esses usuários.<p>Somente as funções de trabalho ativas são exibidas na lista. Para obter mais informações sobre funções, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> <p>Você só poderá atualizar esse campo se tiver uma licença de Plano com acesso de usuário administrativo ou se for um administrador do Workfront. <br>Para obter mais informações sobre a configuração de usuários com acesso de usuário administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
       <li> <p>(Condicional) Se você selecionou um ou vários <b>Outras Funções</b>, o <b>Porcentagem de Disponibilidade de FTE</b> é exibido para cada função. Especifique que porcentagem de tempo do cronograma do usuário está alocada para cada função de trabalho. O valor padrão para a Porcentagem de Disponibilidade FTE para as Outras Funções é 0%.</p> <p><b>NOTA</b>: se outras funções tiverem 0% de disponibilidade de FTE, elas não serão exibidas no Planejador de recursos, a menos que os usuários sejam atribuídos a tarefas nessas funções.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTA</b>: <p>A soma de todos <b>Porcentagens de Disponibilidade de FTE</b> para todas as funções, deve ser igual a 100%. Cada Porcentagem de Disponibilidade de FTE calcula as Horas Disponíveis para cada função por usuário no Planejador de Recursos. As Horas Disponíveis para cada função por usuário dependem do tempo disponível para o usuário.</p> <p>O tempo disponível para o usuário é calculado pelo Workfront, dependendo do método selecionado pelo administrador do Workfront para calcular o FTE nas Preferências de gerenciamento de recursos.</p> <p>Para obter informações sobre como calcular a disponibilidade do usuário, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos</a>.</p> <p>Para obter informações sobre a configuração das preferências do Gerenciamento de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências de gerenciamento de recursos</a>.</p> </p>
       <span class="preview"><p>(Opcional) As atribuições de função de trabalho de data de efetivação são usadas nos cálculos financeiros se a função de trabalho do usuário for alterada durante um projeto.</p><p>Clique em <b>Definir funções por data</b>, selecione o <b>Função Primária</b> e <b>Outras Funções</b>e insira a porcentagem de alocação para cada função. As funções podem ser iguais às funções existentes (usando porcentagens diferentes) ou às novas funções. Selecione o <b>Data inicial</b> quando essas funções se tornam ativas. Esta pode ser uma data futura. Quando as funções mais recentes se tornarem ativas, você poderá clicar em <b>Mostrar funções anteriores</b> para ver as funções anteriores e inativas.</p> </li></span>
       <li> <p><b>Agendar</b>: associe um agendamento ao usuário. O agendamento do usuário calcula a linha do tempo das tarefas às quais o usuário está atribuído.</p> <p>Você deve criar um agendamento antes de associá-lo a um usuário. Para obter mais informações sobre a criação de cronogramas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>.</p> <p><b>NOTA</b>: Recomendamos que o agendamento associado ao usuário corresponda ao Fuso horário do usuário.</p> </li> 
       <li> <p><b>Perfil da Planilha de Horas</b>: associe um Perfil de folha de horas ao usuário para garantir que as folhas de horas sejam geradas automaticamente para o usuário.</p> <p><b>NOTA</b>: a lista de perfis que você tem disponível neste campo depende do seu acesso:
       <ul>
       <li>Como administrador do Workfront, você pode ver todos os perfis de planilha de horas no nível do sistema e no nível do grupo.</li>
       <li>Como administrador de grupo, você pode ver os Perfis de planilha de horas no nível do sistema, bem como aqueles associados aos grupos que você gerencia.</li>
       <li>Como um usuário com uma licença de Plano e acesso para editar usuários, você pode ver somente Perfis de Planilha de Horas no nível do sistema. Para obter mais informações sobre os Perfis de Planilha de Horas no nível do grupo, consulte <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Criar, editar e atribuir perfis de planilha de horas</a>.</li>
      </ul></p> </li> 
       <li><b>Tipo de Hora Padrão</b>: selecione o tipo de hora padrão do usuário. Esse é o tipo de hora usado por padrão quando o usuário registra horas.</li> 
       <li><b>Tipos de Hora Disponíveis</b>: selecione os tipos de horas que devem estar disponíveis para o usuário. Esses tipos de horas estão visíveis em qualquer lugar no Workfront, onde o usuário possa registrar horas. Um usuário só pode ver os tipos de horas que estão ativados no nível do projeto, bem como no nível do usuário. Para obter mais informações sobre que tipos de horas estão disponíveis para os usuários, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir tipos de horas e disponibilidade para folhas de horas</a>.</li> 
       <li><b>Registrar Tempo em:</b> Selecione se o usuário deve registrar horas nos itens de trabalho em horas ou dias. Para obter mais informações, consulte <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurar se a hora está conectada em horas ou dias</a>.</li>

   <li> <b>FTE</b>: este é o equivalente de tempo integral do usuário. O Workfront usa esse número para calcular a disponibilidade do usuário com base na Programação Padrão apenas quando as Preferências de Gerenciamento de Recursos no nível do sistema são definidas como A Programação Padrão.

   <p>O FTE indica a quantidade de tempo que o usuário pode gastar no trabalho. Isso inclui as despesas gerais e o tempo gasto no trabalho do projeto. Por exemplo, o tempo gasto em reuniões ou treinamento também é incluído no FTE.</p>

   O FTE deve ser um número decimal até 1 e não pode ser 0. Por exemplo, se o valor de FTE for 0,5 e o Agendamento padrão no Workfront for 40 horas, o usuário estará disponível 20 horas por semana.

   O padrão do campo é 1.

   Exceções de cronograma, tempo de folga pode e o valor de Tempo de trabalho pode afetar a disponibilidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área Configuração.

   Se as Preferências de Gerenciamento de Recursos no nível do sistema forem definidas como O Cronograma do Usuário, o valor especificado aqui será ignorado e o usuário será considerado disponível de acordo com o especificado em seu cronograma.

   Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de gerenciamento de recursos</a>.

   Para obter mais informações sobre como criar agendas no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um agendamento</a>.
   </li>

   <li><b>Conjuntos de recursos</b>: associe o usuário ao Conjunto de recursos. Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associar conjuntos de recursos a usuários </a>.</li>

   <li><b>Taxa de Custo</b>: a quantidade de custo por hora para o usuário.
      <p>Para taxas de custo efetivas por data, clique em <strong>Adicionar taxa</strong>. Informe o valor da taxa de custo para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A Taxa de Custo 1 não terá uma data inicial e a última taxa de custo não terá uma data final.</p><p>Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de Custo 1 não tiver uma data final e você adicionar a Taxa de Custo 2 com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de Custo 1 para que não haja lacunas.</p></li>

   <li><b>Taxa de cobrança</b>: a quantidade de faturamento por hora para o usuário.
      <p>Para taxas de cobrança efetivas por data, clique em <strong>Adicionar taxa</strong>. Informe o valor da taxa de faturamento para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A Taxa de Cobrança 1 não terá uma data inicial e a última taxa de cobrança não terá uma data final.</p> <p>Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de cobrança 1 não tiver uma data final e você adicionar um segundo com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de cobrança 1 para que não haja lacunas.</p><p> <img alt="Custo do usuário e taxas de faturamento" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulários personalizados</td> 
      <td><p>Associar um formulário personalizado de usuário existente a este usuário. Você deve criar um formulário personalizado antes de associá-lo a um usuário. Somente formulários personalizados ativos são exibidos na lista. Os campos que você não tem acesso para editar não são exibidos em um formulário personalizado individual.</p> <p>Para obter informações sobre como criar formulários personalizados, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comentário</td> 
      <td>Digite o comentário que deseja enviar aos usuários e à área Atualizações dos perfis de usuários.</td> 
     </tr> 
    </tbody> 
   </table>
