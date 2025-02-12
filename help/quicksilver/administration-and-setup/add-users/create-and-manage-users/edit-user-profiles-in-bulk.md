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
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 0%

---

# Editar perfis de usuário em massa

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

Para obter mais detalhes sobre as informações nesta tabela, consulte [Os requisitos de acesso na documentação](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) da Workfront.

+++

## contas Editar usuário em massa

{{step-1-to-users}}

1. Selecione mais de uma usuário e clique no ícone ![Editar Editar ícone](assets/edit-icon.png).

1. **Na caixa Editar Usuário** exibida, altere qualquer uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferências</td> 
      <td> 
       <ul> 
        <li><b>Fuso horário:</b> o fuso horário dos usuários.</li> 
        <li><b></b>Localidade: a localidade preferida dos usuários. Isso afeta o formato dos números e datas nos emails provenientes do Workfront.</li> 
        <li><b>Envie o trabalho que atribuo a mim mesmo para a minha guia</b> de trabalho: esta configuração se refere a um recurso obsoleto que foi removido do Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações</td> 
      <td>Selecione as notificações por email que devem ser ativadas para o novo usuário.<p>Você pode selecionar notificações instantâneas e diárias de resumo. Todas as notificações diárias de resumo são entregues algum tempo depois do mesmo tempo para todos os usuários selecionados. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurar evento notificações para todos no sistema</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acesso</td> 
      <td> 
       <ul> 
        <li><b>Está Ativo:</b> selecione este campo para indicar se os usuários estão ativos. Usuários ativos usam uma licença Workfront. Desmarcar o campo desativa os usuários.</li> 
        <li> 
        <p><b>Nível de Acesso:</b> Selecione o nível de acesso a ser atribuído a esses usuários. Todos os usuários selecionados terão o mesmo nível de acesso.
        </p> 
        <p>Ao atribuir um nível de acesso aos usuários, você pode atribuir um nível igual ou inferior ao seu próprio nível de acesso. (Por exemplo, se o nível de acesso for Planejador, não será possível atribuir o nível de acesso do Administrador.) </p>
        <p>No entanto, você não pode atribuir um nível de acesso menor que o seu se o administrador da Workfront tiver ativado permissões no nível de acesso que também não são habilitadas por conta própria (por meio das configurações de Ajuste fino, conforme descrito em <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis</a> de acesso personalizados).</p> 
        <p>Para obter mais informações sobre níveis de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configurar acesso ao Adobe Systems Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Modelo</b>: escolha um modelo de layout para os usuários. O layout modelo atribuído aos usuários terá precedência em relação a qualquer layout modelo atribuído ao Grupo inicial, à Equipe inicial ou aos função de trabalho principal. Para obter mais informações sobre a prioridade de atribuição dos modelo de layout, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos</a> de layout.</p> 
        <p><b>OBSERVAÇÃO</b>: a lista de modelos de layout disponíveis neste campo depende do seu acesso:
          <ul>
           <li>Como administrador do Workfront, você pode ver todos os modelos de layout de nível de sistema e de grupo.</li>
           <li>Como administrador de grupo, você pode ver modelos de layout no nível do sistema, bem como aqueles associados aos grupos que gerencia.</li>
           <li><p>Como um usuário com uma licença de Planejador e acesso para editar usuários, você pode ver apenas modelos de layout no nível do sistema. </p>
           <p>Para obter informações sobre modelos de layout em nível de grupo, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organização</td> 
      <td> 
       <ul> 
        <li><b>Empresa</b>: o empresa dos usuários. Os usuários podem ser associados somente a uma empresa. Você deve criar uma empresa para associá-la a uma usuário. Somente empresas ativas são exibidas no lista. Para obter informações sobre como criar empresas, consulte Entender e gerenciar empresas.</li> 
        <li><b>Home Team</b>: especifique a equipe inicial para os usuários. Os usuários só podem ter uma equipe inicial. </li> 
        <li><b>Outras equipes</b>: os usuários podem pertencer a várias equipes. </li> 
        <li> <p><b>Grupo inicial:</b> selecione uma grupo apropriada para atribuir os usuários como seu grupo inicial. Isso dá ao usuário a capacidade de acessar objetos compartilhados com o grupo.</p> <p><b>OBSERVAÇÃO</b>: este é um campo obrigatório. Você não pode ter usuários não associados a um Grupo inicial.</p> <p>Você pode atribuir uma grupo a usuários somente nas seguintes situações:</p> 
         <ul> 
          <li>Você é um administrador da Workfront.</li> 
          <li>Você é o administrador desse grupo.</li> 
          <li>O grupo é público.</li> 
         </ul> </li> 
        <li> <p><b>Outros grupos</b>: os usuários podem pertencer a vários grupos. Você pode atribuir um grupo a um usuário somente nas seguintes situações:</p> 
         <ul> 
          <li>Você é um administrador do Workfront.</li> 
          <li>Você é o administrador desse grupo.</li> 
          <li> <p>O grupo é público. </p> 
          <p>Para obter mais informações sobre grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Criar um grupo</a>.</p> 
          <p>Para obter mais informações sobre grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral sobre grupos</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Planejamento de recursos</td> 
      <td> 
       <ul>

   <li>
       <b>Tempo de Trabalho</b>: representa a porcentagem de tempo FTE (equivalente a tempo completo) em que o usuário está disponível para o trabalho real, sem incluir a sobrecarga. A Hora Útil deve ser um número decimal até 1, e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.

   O campo padrão é 1, indicando que um usuário gasta todo o FTE em trabalho real relacionado ao projeto.

   O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho real relacionado ao projeto.

   Para obter mais informações sobre como criar agendas no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar uma agenda</a>.

   Exceções de agendamento e folga também podem afetar a capacidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área Configuração. Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de Gerenciamento de Recursos</a>.

   <b>DICA</b>

   Defina o valor de Tempo de trabalho como 1 para indicar que o usuário está disponível para trabalho relacionado ao projeto em todo o equivalente de tempo integral.
   </li>

   <li><b>Desativação agendada</b>: marque esta caixa se desejar agendar usuários para desativação após um período.</li> 
       <li><b>Data de desativação agendada</b>: a data após a qual os usuários serão desativados. Para obter mais informações sobre o agendamento de usuários para desativação, consulte a seção <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Agendar usuários para desativação</a> em <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</li> 
       <li> <p><b>Função</b> primária: esta é a principal tarefa função que um usuário tem na Workfront. Todas as tarefa e problemas aos quais os usuários são atribuídos também são atribuídos a essa tarefa função, por padrão. As funções de trabalho são essenciais na gestão de recursos. Para obter mais informações sobre funções de trabalho, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a></p> <p>Você pode atualizar esse campo somente se tiver uma licença de plano com acesso administrativo usuário ou se for um administrador do Workfront. Para obter mais informações sobre como configurar usuários com acesso administrativo usuário, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
       <li>(Condicional) Se você selecionou uma <b>Função</b> primária, o <b>campo Porcentagem de FTE Disponibilidade</b> é exibido. Especifique qual a porcentagem de tempo dos horários dos usuários alocados para esse trabalho função. O valor padrão da Porcentagem de FTE Disponibilidade para a Função primária é 100%.</li> 
       <li> <p><b>Outras funções</b>: os usuários podem ter várias funções de trabalho no Workfront. As funções de trabalho são essenciais na gestão de recursos. Não há limite para quantas funções de trabalho um usuário pode cumprir. No entanto, recomendamos não atribuir uma usuário a um número excessivamente grande de funções de trabalho, porque o gerenciamento de recursos pode se tornar muito complexo para esses usuários.</p> <p>Para obter mais informações sobre funções de trabalho, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções</a> de trabalho.</p> <p>Você pode atualizar esse campo somente se tiver uma licença de plano com acesso administrativo usuário ou se for um administrador do Workfront. Para obter mais informações sobre como configurar usuários com acesso administrativo usuário, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
       <li> <p>(Condicional) Se você selecionou uma ou várias Outras <b>funções</b>, a <b>Porcentagem do campo Disponibilidade</b> FTE será exibida para cada função. Especifique qual a porcentagem de tempo dos horários dos usuários está alocada para cada tarefa função. O valor padrão da Porcentagem de FTE Disponibilidade para as outras funções é 0%.</p> <p><b>NOTA</b>:  
       <ul> 
       <li>Se Outras Funções tiverem 0% de Disponibilidade FTE, elas não serão exibidas no Planejador de Recursos, a menos que os usuários sejam atribuídos a tarefas nessas funções.</li> 
       <li> <p>A soma de todas as Porcentagens de Disponibilidade de FTE para todas as funções deve ser igual a 100%. Cada Porcentagem de Disponibilidade de FTE calcula as Horas Disponíveis para cada função por usuário no Planejador de Recursos. As Horas Disponíveis para cada função por usuário dependem do tempo disponível para o usuário.</p> <p>O tempo disponível para o usuário é calculado pela Workfront dependendo do método selecionado pelo administrador da Workfront para calcular as FTE na Preferências de Gerenciamento de recursos.</p> <p>Para obter mais informações sobre como calcular a disponibilidade para o usuário, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador</a> de recursos.</p> <p>Para obter mais informações sobre como configurar preferências de Gerenciamento de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências de Gerenciamento de recursos</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Agendamento</b>: associe um agendamento com os usuários. A agenda dos usuários calcula a linha do tempo das tarefas às quais os usuários são atribuídos.</p> <p>Um administrador da Workfront ou um grupo administrador deve criar um agendamento antes de poder ser associado aos usuários.</p> <p>Selecione um cronograma de nível de sistema ou grupo para atribuí-lo aos usuários selecionados.</p> <p>Para obter mais informações sobre agendamentos no nível do sistema e no grupo, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>.</p> <p><b>IMPORTANTE</b>: a workfront usa o agendamento de uma usuário somente quando a configuração Calcular disponibilidade de recursos Usando está definida como Agendamento do usuário. Para obter informações sobre como a disponibilidade do recurso Calcular usando a configuração afeta qual agendamento é usado para o Gerenciamento de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências</a> de Gerenciamento de recursos.</p> </li> 
       <li> <p><b>Perfil de</b> folha de tempo: associe um perfil de folha de tempo aos usuários. Isso garante que as planilhas de tempo gerem automaticamente para os usuários.</p> 
       <p><b>OBSERVAÇÃO</b>:  
       <ul> 
       <li>A lista de perfis de folha de tempo disponíveis neste campo depende do seu acesso:
       <ul>
       <li>Como administrador da Workfront, você pode ver todos os perfis de folha de tempo de nível de sistema e grupo nível.</li>
       <li><p>Como um administrador grupo, você pode ver perfis de folha de tempo no nível do sistema, bem como aqueles associados aos grupos que você gerenciar.</p></li>
       <li><p>Como um usuário com uma licença de Planejador e acesso para editar usuários, você pode ver apenas perfis de planilha de horas no nível do sistema.</p></li>
       </ul></li> 
       <li>Se você for um administrador de grupo, todos os usuários que estiver editando deverão ser membros de um grupo que você administra.</li> 
       </ul> </p> </li> 
       <li><b>Tipo</b> de hora padrão: selecione o tipo de hora padrão para os usuários. Esse é o tipo de hora que é usado por padrão quando o usuário registra o tempo.</li> 
       <li> <p><b>Tipos</b> de hora disponíveis: selecione os tipos de hora que devem estar disponíveis para o usuário. Esses tipos de hora são visíveis em todos os lugares da Workfront, onde os usuários podem registrar o tempo. Um usuário pode ver apenas os tipos de hora ativados no nível do projeto, bem como o nível usuário.</p> 
       <p>Para obter mais informações sobre quais tipos de hora estão disponíveis para os usuários, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir tipos de hora e disponibilidade</a>.</p> 
       </li> 
       <li> <b></b>FTE: isso é o equivalente em tempo integral do usuário. O Workfront usa esse número para calcular a disponibilidade do usuário com base na Programação Padrão apenas quando as Preferências de Gerenciamento de Recursos no nível do sistema são definidas como A Programação Padrão.

   <p>O FTE indica a quantidade de tempo que o usuário pode gastar no trabalho. Isso inclui as despesas gerais e o tempo gasto no trabalho do projeto. Por exemplo, o tempo gasto em reuniões ou treinamento também é incluído no FTE.</p>

   O FTE deve ser um número decimal até 1 e não pode ser 0. Por exemplo, se o valor de FTE for 0,5 e o Agendamento padrão no Workfront for 40 horas, o usuário estará disponível 20 horas por semana.

   O padrão do campo é 1.

   Exceções de cronograma, tempo de folga pode e o valor de Tempo de trabalho pode afetar a disponibilidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências de Gerenciamento de recursos na área Configuração.

   Se as Preferências de Gerenciamento de Recursos no nível do sistema forem definidas como O Cronograma do Usuário, o valor especificado aqui será ignorado e o usuário será considerado disponível de acordo com o especificado em seu cronograma.

   Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de Gerenciamento de Recursos</a>.

   Para obter mais informações sobre como criar agendas no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar uma agenda</a>.
   </li> 
       <li> <p><b>Pools de Recursos</b>: associe os usuários aos pools de recursos.</p> <p><b>OBSERVAÇÃO</b>: somente os pools de recursos comuns a todos os usuários selecionados aparecem neste campo. Se os usuários selecionados não tiverem conjuntos de recursos compartilhados, esse campo estará vazio. Se esse campo estiver vazio, os conjuntos de recursos especificados aqui substituirão seus conjuntos de recursos individuais.</p> 
       <p>Para obter mais informações sobre pools de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos pools de recursos </a>.</p> </li> 
       <li><b>Custo por hora</b>: a quantidade de custo por hora para o usuário. </li> 
       <li><b>Cobrança por hora</b>: a quantidade de cobrança por hora para o usuário.</li> 
       <li><b>Forms personalizado</b>: associe um formulário personalizado de usuário existente aos usuários. Você deve criar um formulário personalizado antes de associá-lo a um usuário. Somente formulários personalizados ativos são exibidos na lista. Para obter informações sobre como criar formulários personalizados, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Criar um formulário personalizado</a>.</li> 
       <li><b>Comentário</b>: insira um comentário no campo fornecido. Todos os usuários selecionados receberão uma notificação no aplicativo, bem como uma notificação por email com seu comentário. O comentário é exibido na guia Atualizações do perfil do usuário.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Na seção **Forms Personalizado**, selecione a opção **Recalcular Expressões Personalizadas** para garantir que todos os campos personalizados calculados em formulários personalizados anexados aos usuários selecionados estejam atualizados.

1. Clique em **Salvar alterações**.
