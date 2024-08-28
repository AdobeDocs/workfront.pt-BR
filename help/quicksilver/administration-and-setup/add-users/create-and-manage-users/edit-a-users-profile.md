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
source-git-commit: 1e70620514f180d547c61970c0dd49d281377ce5
workflow-type: tm+mt
source-wordcount: '3336'
ht-degree: 0%

---

# Editar o perfil de um usuário

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Como administrador do Adobe Workfront, você pode criar usuários e gerenciar os perfis dos existentes. Para obter informações sobre como criar usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
     <li> <p>O objeto <b>Usuários</b> em seu nível de acesso configurado para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas <b>Administrador de Usuários</b> a seguir, habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
     <ul><li> Administrador de Usuários (Todos os usuários)</li>
     <li>Administrador de Usuários (Usuários de Grupo)</li></ul>
     <p>Se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo para um grupo do qual o usuário seja membro para poder editar o usuário.</p> 
     <p>Para obter mais informações sobre a configuração <b>Usuários</b> em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

+++

## Editar um perfil de usuário

{{step-1-to-users}}

1. Selecione o usuário e clique no ícone **Editar** ![](assets/edit-icon.png).

   A caixa Editar Usuário é exibida.

1. Na caixa **Editar Usuário**, altere qualquer uma das informações a seguir e clique em **Salvar Alterações** a qualquer momento:

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
        <li> <p><b>Endereço de email:</b> O endereço de email de um usuário também é seu nome de usuário no Workfront. Esse campo diferencia maiúsculas e minúsculas e deve ser exclusivo. Se qualquer usuário tentar adicionar um endereço de email não exclusivo 3 vezes em uma janela de 10 minutos, uma resposta do reCAPTCHA será exibida.</p> <p> Selecione a configuração <b>Não sou um robô</b> antes de continuar.</p><p>Se você usar a inclui na lista de permissões por email e inserir um domínio de email que não esteja na lista, o usuário não receberá notificações por email. Para obter mais informações sobre a incluir na lista de permissões inclui na lista de permissões, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md" class="MCXref xref">Configurar a pesquisa por email</a>.</p> </li> 
        <li> <p><b>Redefinir Senha</b>: clique neste link para redefinir a senha do usuário. Você deve digitar sua própria senha antes de redefinir a senha de outro usuário.</p> <p>Para redefinir a senha de outro usuário, você deve ser um administrador do Workfront ou um administrador de grupo.</p> <p><b>NOTA</b>:  
          <ul> 
           <li> <p>Se você for um administrador de grupo, poderá redefinir senhas somente para usuários nos grupos em que foi designado como administrador. Além disso, a permissão Administrador de usuários (usuários de grupo) deve estar ativada em seu nível de acesso:</p> <p> <img src="assets/group-admin-user.png" > </p> <p>Essa configuração é desativada por padrão. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </li> 
           <li> <p>Não é possível redefinir a senha de um administrador do Workfront.</p> </li> 
          </ul> </p> </li> 
        <li><b>&lt;Configuração de SSO&gt; Nome de usuário</b>: se o administrador do Workfront habilitou uma integração de SSO com o Workfront, o Nome de Usuário de SSO é exibido neste campo. O tipo de configuração de SSO ativado para sua instância do Workfront é visível nesse campo. </li> 
        <li> <p><b>Permitir &lt;Configuração de SSO&gt; Autenticação</b>: se o administrador do Workfront habilitou uma integração de SSO com o Workfront e atualizou todos os usuários para SSO, esse campo será selecionado por padrão. O tipo de configuração de SSO ativado para sua instância do Workfront é visível nesse campo.</p> <p>Quando esse campo é selecionado, o usuário precisa fazer logon no Workfront com suas credenciais de SSO. Ao desmarcá-la, você poderá fazer logon no Workfront com as credenciais da Workfront.</p> <p>Para obter mais informações sobre como configurar o Workfront com uma solução SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md" class="MCXref xref">Visão geral do logon único no Adobe Workfront</a></p> <p>Para obter mais informações sobre como atualizar usuários para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Atualizar usuários para logon único</a>.</p> 
        <p><b>NOTA</b>:</p> 
        <p> Se você for um administrador de grupo, poderá editar os campos &lt;Configuração de SSO&gt; somente para usuários nos grupos em que estiver designado como tal. Além disso, a permissão Administrador de usuário (usuários de grupo) deve estar ativada em seu nível de acesso.
        <p>Se você for um administrador de grupo e tiver a permissão Administrador de Usuário (Todos os Usuários) ativada em seu nível de acesso, poderá editar os campos &lt;Configuração do SSO&gt; para todos os usuários.</p> </li> 
        <li><b>Informações do Trabalho:</b> Informações sobre o trabalho, como o cargo (no campo <b>Título</b>), e a área de conhecimento pela qual o usuário é responsável (no campo <b>Fale Comigo Sobre</b>).</li> 
        <li><p><b>Informações de contato</b>: o número de telefone do usuário (no <b>Número de telefone, ramal).</b> e <b>Número de celular</b> campos) e endereço (nos campos <b>Endereço, Cidade, Estado, CEP, País</b> ).</p>
        <p>Se o usuário estiver habilitado para o Unified User Management (UUM) ou para o Adobe Identity Management System (IMS), o campo <b>País</b> na seção Informações de Contato só aceitará valores de código de país (por exemplo, EUA, GB, IN).</p></li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preferências </td> 
      <td> 
       <ul> 
      <li> <p><b>Fuso Horário:</b> O fuso horário do usuário.</p> <p>Para obter informações sobre como ajudar usuários a colaborar na Workfront em fusos horários diferentes, consulte <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Trabalhando em fusos horários diferentes</a>.</p> </li>

   <li><p><b>Localidade de email</b>: a localidade de email preferencial do usuário. Isso afeta o formato de números e datas nos emails que vêm do Workfront para esse usuário.</p>
      <p><b>OBSERVAÇÃO:</b> quando sua organização está no Adobe da Experiência unificada, as preferências de idioma do usuário são armazenadas no perfil de Adobe e a localidade de email não é usada. Para obter informações sobre como acessar essas preferências, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>.</p></li>

   <li><b>Receber emails deste ambiente de teste</b>: marque esta opção se desejar receber notificações por email do ambiente em que você está conectado no momento.
      <p><b>Nota</b></p>
      <p>Essa opção está disponível somente nos ambientes Pré-visualização e Sandbox. As notificações por email estão ativadas no ambiente de Produção por padrão. </p>
      </li>

   </li> 
       <li><b>Enviar trabalho que eu atribuir a mim mesmo para minha guia Trabalhando em</b>: marque esta opção se desejar que tudo o que o usuário atribuir a si mesmo apareça diretamente na lista Trabalhando em na área Página Inicial. O padrão é listar tudo atribuído a um usuário nas listas Pronto para iniciar ou Não pronto na área Página inicial.</li> 
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
      <li><b>Está Ativo:</b> marque esta caixa para indicar que o usuário está ativo. Usuários ativos usam uma licença Workfront. Limpar a caixa desativa o usuário e impede que ele faça logon no Workfront.</li> 
       <li> <p><b>Nível de Acesso:</b> Selecione o nível de acesso a ser atribuído a este usuário.</p> 
       <p>Ao atribuir um nível de acesso a um usuário, você pode atribuir um nível igual ou inferior ao seu próprio nível de acesso.</p>
       <p>Por exemplo, se o seu nível de acesso for Plano, você não poderá atribuir o nível de acesso Administrador. No entanto, não é possível atribuir um nível de acesso que, por padrão, seja inferior ao seu próprio nível de acesso se o administrador do Workfront tiver ativado permissões não padrão no nível de acesso que também não estejam ativadas no seu próprio nível de acesso. </p>
       <p>Por exemplo, se você tiver uma licença de Plano sem acesso para excluir tarefas, não será possível atribuir uma licença de Trabalho a alguém com acesso para excluir tarefas, embora a licença de Trabalho seja inferior à licença de Plano. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> 
       <p>Para obter mais informações sobre níveis de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurar acesso ao Adobe Workfront</a>.</p>
       <p> <b>OBSERVAÇÃO:</b></p> 
       <p> Se sua organização usar o novo modelo de acesso (Padrão/Claro/Colaborador), você não poderá reatribuir um usuário Padrão ou Light a um nível de acesso de Colaborador se ele já tiver atingido o limite de decisão para o mês. </p><p>Para obter mais informações sobre o novo modelo de acesso, consulte <a href="../how-access-levels-work/access-level-overview.md" class="MCXref xref">Visão geral sobre novos níveis de acesso</a>. </p><p>Para obter informações sobre limites de decisão, consulte <a href="/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md" class="MCXref xref">Visão geral sobre documento limitado e decisão de prova para usuários não pagos</a>.</p></li> 
       <li> <p><b>Modelo de layout</b>: escolha um Modelo de layout para o usuário. Este modelo de layout tem prioridade sobre qualquer modelo de layout atribuído ao grupo padrão, à equipe padrão ou à função principal do usuário. Para obter mais informações sobre a prioridade de atribuição de Modelos de Layout, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> <p><b>NOTA</b>:  <p>A lista a seguir descreve como a lista de modelos disponíveis neste campo depende do seu acesso:</p> 
       <ul> 
       <li>Como administrador do Workfront, você pode ver todos os Modelos de layout no nível do sistema e no nível do grupo.</li> 
       <li>Como administrador de grupo, você pode ver o modelo de layout no nível do sistema, bem como aqueles associados aos grupos que gerencia.</li> 
       <li>Como um usuário com uma licença de Plano e acesso para editar usuários, você pode ver apenas Modelos de layout no nível do sistema.</li> 
       </ul> <p>Para obter mais informações sobre Modelos de Layout de nível de grupo, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organização </td> 
      <td> 
       <ul> 
      <li><b>Empresa</b>: a empresa do usuário. Os usuários podem ser associados a apenas uma empresa. Você deve criar uma empresa antes de associá-la a um usuário. Somente empresas ativas são exibidas na lista. Para obter informações sobre como criar empresas, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Criar e editar empresas</a>.</li> 
      <li><b>Relatórios para:</b> Se você especificou uma empresa para o usuário, você também pode especificar o gerente direto do usuário neste campo. Um usuário pode ter apenas um gerente. Esse campo não será exibido se o usuário não estiver associado a uma empresa primeiro. </li> 
      <li><b>Subordinados diretos:</b> Se você especificou uma empresa para o usuário, você também pode especificar os subordinados diretos do usuário. Um usuário pode ter vários subordinados diretos. Esse campo não será exibido se o usuário não estiver associado a uma empresa primeiro.</li> 
      <li><b>Equipe interna</b>: especifique a equipe interna do usuário. Os usuários só podem ter uma equipe inicial. A Equipe interna é importante ao atribuir um modelo de layout ou ao definir o botão Trabalhar na tarefa para as tarefas e problemas atribuídos ao usuário. </li> 
      <li><b>Outras equipes</b>: os usuários podem pertencer a várias equipes. Um usuário pode visualizar itens de trabalho atribuídos a qualquer uma de suas equipes na área Início. </li> 
      <li> <p><b>Grupo Padrão:</b> Selecione um grupo apropriado para atribuir ao usuário. Isso dá ao usuário a capacidade de acessar objetos que são compartilhados com o grupo. Você também pode compartilhar modelos de layout com o Grupo padrão do usuário.</p> <p>Este campo é obrigatório. Todos os usuários devem estar associados a um grupo padrão. Se você não selecionar um, seu grupo será atribuído como o grupo inicial do novo usuário.</p> <p><b>NOTA</b>:</p> 
      <p> Você pode atribuir um grupo a um usuário somente se um dos seguintes for verdadeiro:</p>
      <ul><li>você é um administrador do Workfront</li>
      <li>você é o administrador do grupo</li>
      <li>o grupo é público.</li></ul> 
      <li> <p><b>Outros grupos</b>: os usuários podem pertencer a vários grupos. Você pode atribuir um grupo a um usuário somente se for um administrador do Workfront, se for o administrador do grupo ou se o grupo for público.</p> <p><b>IMPORTANTE</b>:</p> 
      <p>Adicionar um usuário a mais de 100 grupos pode causar problemas de desempenho em qualquer área do Workfront que carrega a lista de grupos.</p> <p>Para obter mais informações sobre grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Criar um grupo</a>.</p> <p>Para obter mais informações sobre grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral sobre grupos</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planejamento de recursos </td> 
      <td> 
       <ul>
       <li>
       <b>Tempo de Trabalho</b>: representa a porcentagem de tempo FTE (equivalente a tempo completo) em que o usuário está disponível para o trabalho real, sem incluir a sobrecarga. A Hora Útil deve ser um número decimal até 1, e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.

   O campo padrão é 1, indicando que um usuário gasta todo o FTE em trabalho real relacionado ao projeto.

   O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho real relacionado ao projeto.

   Para obter mais informações sobre como criar agendas no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar uma agenda</a>.

   As exceções de agendamento e a folga também podem afetar a capacidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área Configuração. Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de Gerenciamento de Recursos</a>.

   <b>DICA</b>

   Defina o valor de Tempo de trabalho como 1 para indicar que o usuário está disponível para trabalho relacionado ao projeto em todo o equivalente de tempo integral.
   </li> 
      <li> <b>Desativação agendada</b>: marque esta caixa se desejar agendar a desativação deste usuário em uma determinada data e em um determinado horário. </li> 
       <li><b>Data de desativação agendada</b>: a data e a hora em que o usuário é desativado. Para obter informações sobre como agendar usuários para desativação, consulte os <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Agendar usuários para desativação</a> em <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</li> 
       <li> <p><b>Função principal</b>: esta é a função principal que o usuário pode desempenhar no Workfront. Todas as tarefas e problemas aos quais o usuário está atribuído também são atribuídos a essa função de trabalho. As funções de trabalho são essenciais no gerenciamento de recursos. Você só poderá atualizar esse campo se tiver uma licença de Plano com acesso de usuário administrativo ou se for um administrador do Workfront. Para obter mais informações sobre como configurar usuários com acesso administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> <p>Somente as funções de trabalho ativas são exibidas na lista. </p> </li> 
       <li>Se você selecionou uma <b>Função primária</b>, o campo <b>Porcentagem de disponibilidade de FTE</b> será exibido. Especifique o percentual de tempo do agendamento do usuário alocado para esta função de trabalho. O valor padrão para o Percentual de Disponibilidade de FTE para a Função Principal é 100%. </li> 
       <li> <p><b>Outras funções</b>: um usuário pode ter várias funções de trabalho no Workfront. As funções de trabalho são essenciais no gerenciamento de recursos. Não há limite para quantas funções de trabalho um usuário pode realizar. No entanto, recomendamos não atribuir um usuário a um número excessivamente grande de funções de trabalho, pois o gerenciamento de recursos pode se tornar muito complexo para esses usuários.<p>Somente as funções de trabalho ativas são exibidas na lista. Para obter mais informações sobre funções de trabalho, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> <p>Você só poderá atualizar esse campo se tiver uma licença de Plano com acesso de usuário administrativo ou se for um administrador do Workfront. <br>Para obter mais informações sobre como configurar usuários com acesso administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
       <li> <p>(Condicional) Se você selecionou uma ou várias <b>Outras funções</b>, o campo <b>Porcentagem de disponibilidade de FTE</b> será exibido para cada função. Especifique que porcentagem de tempo do cronograma do usuário está alocada para cada função de trabalho. O valor padrão para a Porcentagem de Disponibilidade FTE para as Outras Funções é 0%.</p> <p><b>OBSERVAÇÃO</b>: se outras funções tiverem 0% de disponibilidade de FTE, elas não serão exibidas no Planejador de recursos, a menos que os usuários sejam atribuídos a tarefas nessas funções.</p> <p> <img alt="user_settings_roles_and_date_boxes_rp_story.png" src="assets/user-settings-roles-and-dte-boxes-rp-story.png"> </p> <p><b>NOTA</b>: <p>A soma de todos os <b>Percentuais de Disponibilidade de FTE</b> para todas as funções deve ser igual a 100%. Cada Porcentagem de Disponibilidade de FTE calcula as Horas Disponíveis para cada função por usuário no Planejador de Recursos. As Horas Disponíveis para cada função por usuário dependem do tempo disponível para o usuário.</p> <p>O tempo disponível para o usuário é calculado pelo Workfront, dependendo do método selecionado pelo administrador do Workfront para calcular o FTE nas Preferências de gerenciamento de recursos.</p> <p>Para obter informações sobre como calcular a disponibilidade do usuário, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos</a>.</p> <p>Para obter informações sobre como configurar preferências de Gerenciamento de Recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências de Gerenciamento de Recursos</a>.</p> </p>
       <span class="preview"><p>(Opcional) As atribuições de função de trabalho de data de efetivação são usadas nos cálculos financeiros se a função de trabalho do usuário for alterada durante um projeto.</p><p>Clique em <b>Definir funções por data</b>, selecione a <b>Função Primária</b> e as <b>Outras Funções</b> e insira a porcentagem de alocação para cada função. As funções podem ser iguais às funções existentes (usando porcentagens diferentes) ou às novas funções. Selecione a <b>Data de início</b> quando essas funções se tornarem ativas. Esta pode ser uma data futura. Quando as funções mais recentes se tornarem ativas, você poderá clicar em <b>Mostrar funções anteriores</b> para ver as funções anteriores e inativas.</p> </li></span>
       <li> <p><b>Agendamento</b>: associe um agendamento ao usuário. O agendamento do usuário calcula a linha do tempo das tarefas às quais o usuário está atribuído.</p> <p>Você deve criar um agendamento antes de associá-lo a um usuário. Para obter mais informações sobre como criar agendas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar uma agenda</a>.</p> <p><b>OBSERVAÇÃO</b>: recomendamos que o agendamento associado ao usuário corresponda ao Fuso Horário do usuário.</p> </li> 
       <li> <p><b>Perfil de Planilha de Horas</b>: Associe um Perfil de Planilha de Horas ao usuário para garantir que as planilhas de horas sejam geradas automaticamente para o usuário.</p> <p><b>OBSERVAÇÃO</b>: a lista de perfis disponíveis neste campo depende do seu acesso:
       <ul>
       <li>Como administrador do Workfront, você pode ver todos os perfis de planilha de horas no nível do sistema e no nível do grupo.</li>
       <li>Como administrador de grupo, você pode ver os Perfis de planilha de horas no nível do sistema, bem como aqueles associados aos grupos que você gerencia.</li>
       <li>Como um usuário com uma licença de Plano e acesso para editar usuários, você pode ver somente Perfis de Planilha de Horas no nível do sistema. Para obter mais informações sobre Perfis de Planilha de Horas no nível do grupo, consulte <a href="../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md" class="MCXref xref">Criar, editar e atribuir perfis de planilha de horas</a>.</li>
      </ul></p> </li> 
       <li><b>Tipo de Hora Padrão</b>: Selecione o tipo de hora padrão para o usuário. Esse é o tipo de hora usado por padrão quando o usuário registra horas.</li> 
       <li><b>Tipos de Horas Disponíveis</b>: Selecione os tipos de horas que devem estar disponíveis para o usuário. Esses tipos de horas estão visíveis em qualquer lugar no Workfront, onde o usuário possa registrar horas. Um usuário só pode ver os tipos de horas que estão ativados no nível do projeto, bem como no nível do usuário. Para obter mais informações sobre quais tipos de horas estão disponíveis para os usuários, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir tipos de horas e disponibilidade</a>.</li> 
       <li><b>Registrar Tempo em:</b> Selecione se o usuário deve registrar horas em itens de trabalho em horas ou dias. Para obter mais informações, consulte <a href="../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md" class="MCXref xref">Configurar se a hora está conectada em horas ou dias</a>.</li>

   <li> <b>FTE</b>: este é o equivalente de tempo integral do usuário. O Workfront usa esse número para calcular a disponibilidade do usuário com base na Programação Padrão apenas quando as Preferências de Gerenciamento de Recursos no nível do sistema são definidas como A Programação Padrão.

   <p>O FTE indica a quantidade de tempo que o usuário pode gastar no trabalho. Isso inclui as despesas gerais e o tempo gasto no trabalho do projeto. Por exemplo, o tempo gasto em reuniões ou treinamento também é incluído no FTE.</p>

   O FTE deve ser um número decimal até 1 e não pode ser 0. Por exemplo, se o valor de FTE for 0,5 e o Agendamento padrão no Workfront for 40 horas, o usuário estará disponível 20 horas por semana.

   O padrão do campo é 1.

   Exceções de cronograma, tempo de folga pode e o valor de Tempo de trabalho pode afetar a disponibilidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área Configuração.

   Se as Preferências de Gerenciamento de Recursos no nível do sistema forem definidas como O Cronograma do Usuário, o valor especificado aqui será ignorado e o usuário será considerado disponível de acordo com o especificado em seu cronograma.

   Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de Gerenciamento de Recursos</a>.

   Para obter mais informações sobre como criar agendas no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar uma agenda</a>.
   </li>

   <li><b>Conjuntos de Recursos</b>: associe o usuário aos Conjuntos de Recursos. Para obter mais informações, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md" class="MCXref xref">Associar pools de recursos a usuários </a>.</li>

   <li><b>Taxa de Custo</b>: a quantidade de custo por hora para o usuário.
      <p>Para taxas de custo atuais, clique em <strong>Adicionar taxa</strong>. Informe o valor da taxa de custo para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A Taxa de Custo 1 não terá uma data inicial e a última taxa de custo não terá uma data final.</p><p>Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de Custo 1 não tiver uma data final e você adicionar a Taxa de Custo 2 com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de Custo 1 para que não haja lacunas.</p></li>

   <li><b>Taxa de Cobrança</b>: a quantidade de cobrança por hora para o usuário.
      <p>Para taxas de cobrança efetivas por data, clique em <strong>Adicionar taxa</strong>. Informe o valor da taxa de faturamento para o período e atribua uma Data Inicial e uma Data Final conforme necessário. A Taxa de Cobrança 1 não terá uma data inicial e a última taxa de cobrança não terá uma data final.</p> <p>Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de cobrança 1 não tiver uma data final e você adicionar um segundo com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de cobrança 1 para que não haja lacunas.</p><p> <img alt="Custo do usuário e taxas de faturamento" src="assets/edit-user-cost-billing-rate-2.png"> </p></li>

   </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulários personalizados</td> 
      <td><p>Associar um formulário personalizado de usuário existente a este usuário. Você deve criar um formulário personalizado antes de associá-lo a um usuário. Somente formulários personalizados ativos são exibidos na lista. Os campos que você não tem acesso para editar não são exibidos em um formulário personalizado individual.</p> <p><strong>Observação:</strong> recursos avançados de formulário personalizado, como campos de pesquisa Externos e campos nativos do Workfront, só estarão disponíveis quando você abrir o registro do usuário na página de detalhes, não na caixa de diálogo Editar Usuário. (Na lista de usuários, clique no nome do usuário para abrir os detalhes.)</p> <p>Para obter informações sobre como criar formulários personalizados, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md" class="MCXref xref">Criar um formulário com o designer de formulário</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Comentário</td> 
      <td>Digite o comentário que deseja enviar aos usuários e à área Atualizações dos perfis de usuários.</td> 
     </tr> 
    </tbody> 
   </table>
