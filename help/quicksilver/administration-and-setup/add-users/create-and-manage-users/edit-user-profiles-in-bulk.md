---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Editar perfis de usuário em massa
description: Como administrador do Adobe Workfront, você pode editar contas de usuário em massa.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: 95c999a72020ce825f3a8377662c71e35a194d80
workflow-type: tm+mt
source-wordcount: '2384'
ht-degree: 0%

---

# Editar perfis de usuário em massa

<span class="preview">As informações destacadas nesta página se referem à funcionalidade ainda não disponível no geral. Está disponível somente no ambiente de Visualização.</span>

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter instruções sobre como editar o perfil de um usuário no Adobe Admin Console, consulte a seção &quot;Editar detalhes do usuário&quot; no artigo [Usuários de upload em massa](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) ou entre em contato com o administrador do Adobe Admin Console.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Você pode editar contas de usuário em massa. Ao editar usuários em massa, somente os campos que você selecionar especificamente são atualizados com as mesmas informações para todos os usuários selecionados. Todos os outros campos deixados não selecionados permanecem os mesmos para cada usuário individual, mesmo que sejam diferentes para cada usuário.

>[!NOTE]
>
>* Não é possível editar em massa a seção Informações pessoais dos perfis dos usuários, pois essas informações devem ser exclusivas para cada usuário.
>* Para garantir a precisão dos dados e o desempenho ideal, recomendamos que você selecione no máximo 2000 usuários ao mesmo tempo para uma edição em massa.
>


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

## Editar contas de usuário em massa

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Selecione mais de um usuário e clique no ícone Editar ![](assets/edit-icon.png).

1. No **Editar usuário** for exibida, altere qualquer uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferências</td> 
      <td> 
       <ul> 
        <li><b>Fuso Horário:</b> O fuso horário dos usuários.</li> 
        <li><b>Localidade</b>: A localidade preferencial dos usuários. Isso afeta o formato de números e datas nos emails provenientes do Workfront.</li> 
        <li><b>Mostrar porcentagem concluída no status de atualização</b>: Marque essa opção se desejar exibir uma barra de porcentagem completa dentro do fluxo de atualizações de tarefas para todos os usuários.</li> 
        <li><b>Enviar trabalho que atribuo a mim mesmo para a guia Trabalhar</b>: Marque essa opção se desejar que tudo o que os usuários atribuírem a eles mesmos apareça diretamente na guia Trabalhar em . O padrão é listar tudo o que é atribuído a um usuário na guia Solicitação de trabalho.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações</td> 
      <td>Selecione as notificações por email que devem ser ativadas para o novo usuário.<p>Você pode selecionar notificações instantâneas e diárias de resumo. Todas as notificações de resumo diário são entregues em algum momento após o mesmo tempo para todos os usuários selecionados. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configurar notificações de evento para todos no sistema</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acesso</td> 
      <td> 
       <ul> 
        <li><b>Está ativo:</b> Selecione esse campo para indicar se os usuários estão ativos. Usuários ativos usam uma licença do Workfront. Desmarcar o campo desativa os usuários.</li> 
        <li> 
        <p><b>Nível de acesso:</b> Selecione o nível de acesso a ser atribuído a esses usuários. Todos os usuários selecionados terão o mesmo nível de acesso.
        </p> 
        <p>Ao atribuir um nível de acesso a usuários, é possível atribuir um nível igual ou inferior ao seu próprio nível de acesso. (Por exemplo, se o nível de acesso for Planejador, você não poderá atribuir o nível de acesso Administrador.) </p>
        <p>No entanto, você não poderá atribuir um nível de acesso menor que o seu se o administrador do Workfront tiver ativado permissões no nível de acesso que também não estão ativadas por si mesmo (por meio das configurações de Ajuste Otimizado, conforme descrito em <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>).</p> 
        <p>Para obter mais informações sobre níveis de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configuração do acesso ao Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Modelo de layout</b>: Escolha um modelo de layout para os usuários. O modelo de layout atribuído aos usuários terá prioridade sobre qualquer modelo de layout atribuído ao Grupo doméstico, Equipe inicial ou função de trabalho principal. Para obter mais informações sobre a prioridade de atribuição do modelo de layout, consulte <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Criar e gerenciar modelos de layout</a>.</p> 
        <p><b>OBSERVAÇÃO</b>: A lista de modelos de layout disponíveis neste campo depende do seu acesso:
          <ul>
           <li>Como administrador do Workfront, você pode ver todos os modelos de layout de nível de sistema e de grupo.</li>
           <li>Como administrador de grupo, você pode ver modelos de layout de nível de sistema, bem como os associados aos grupos que você gerencia.</li>
           <li><p>Como usuário com uma licença do Planejador e acesso para editar usuários, você pode ver apenas modelos de layout no nível do sistema. </p>
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
        <li><b>Empresa</b>: A empresa dos usuários. Os usuários podem ser associados somente a uma empresa. Você deve criar uma empresa antes de associá-la a um usuário. Somente empresas ativas são exibidas na lista. Para obter informações sobre como criar empresas, consulte Entendendo e Gerenciando Empresas.</li> 
        <li><b>Equipe inicial</b>: Especifique a equipe inicial dos usuários. Os usuários só podem ter uma equipe inicial. </li> 
        <li><b>Outras equipes</b>: Os usuários podem pertencer a várias equipes. </li> 
        <li> <p><b>Grupo Doméstico:</b> Selecione um grupo apropriado para atribuir os usuários como seu Grupo Doméstico. Isso dá ao usuário a capacidade de acessar objetos que são compartilhados com o grupo.</p> <p><b>OBSERVAÇÃO</b>: Este é um campo obrigatório. Você não pode ter usuários associados a um Grupo doméstico.</p> <p>Você pode atribuir um grupo a usuários somente nas seguintes situações:</p> 
         <ul> 
          <li>Você é um administrador do Workfront.</li> 
          <li>Você é o administrador desse grupo.</li> 
          <li>O grupo é público.</li> 
         </ul> </li> 
        <li> <p><b>Outros grupos</b>: Os usuários podem pertencer a vários grupos. Você pode atribuir um grupo a um usuário somente nas seguintes situações:</p> 
         <ul> 
          <li>Você é um administrador do Workfront.</li> 
          <li>Você é o administrador desse grupo.</li> 
          <li> <p>O grupo é público. </p> 
          <p>Para obter mais informações sobre grupos públicos, consulte <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Criar um grupo</a>.</p> 
          <p>Para obter mais informações sobre grupos, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Visão geral dos grupos</a>.</p> 
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
       <b><span class="preview">Tempo de trabalho</span></b>: <span class="preview">Representa a porcentagem do tempo FTE (Equivalente de Tempo Total) que o usuário está disponível para o trabalho real, não incluindo a sobrecarga. O Tempo de Trabalho deve ser um número decimal de até 1 e não pode ser 0. Por exemplo, uma disponibilidade de 20% para o trabalho real seria de 0,2.</span>

   <span class="preview">O padrão do campo é 1, indicando que um usuário gasta o FTE inteiro no trabalho real relacionado ao projeto.</span>

   <span class="preview">O sistema usa esse número para calcular a disponibilidade do usuário para o trabalho real relacionado ao projeto. </span>

   <span class="preview">Para obter mais informações sobre como criar programações no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um agendamento</a>.</span>

   <span class="preview">As exceções de agendamento e o tempo limite também podem afetar a capacidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências do Gerenciamento de Recursos na área Configurar . Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências do Gerenciamento de recursos</a>.

   <b>DICA</b>

   <span class="preview">Defina o valor Tempo de trabalho como 1 para indicar que o usuário está disponível para trabalho relacionado ao projeto e todo o seu equivalente em tempo integral.</span>
   </li>

   <li><b>Agendar desativação</b>: Marque essa caixa se desejar agendar a desativação dos usuários após um período de tempo.</li> 
       <li><b>Data de desativação programada</b>: A data após a qual os usuários se tornam desativados. Para obter mais informações sobre como programar usuários para desativação, consulte a seção <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Agendar usuários para desativação</a> em <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</li> 
       <li> <p><b>Função principal</b>: Esta é a função de trabalho principal que um usuário tem no Workfront. Todas as tarefas e problemas aos quais os usuários estão atribuídos também são atribuídos a essa função de trabalho, por padrão. As funções de trabalho são essenciais no gerenciamento de recursos. Para obter mais informações sobre funções do job, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a></p> <p>Você pode atualizar este campo somente se tiver uma licença do Plan com acesso administrativo de usuário ou se for um administrador do Workfront. Para obter mais informações sobre como configurar usuários com acesso administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
       <li>(Condicional) Se você selecionou um <b>Função principal</b>, o <b>Porcentagem de disponibilidade de FTE</b> é exibido. Especifique qual porcentagem de tempo dos agendamentos dos usuários está alocada para esta função de trabalho. O valor padrão da Porcentagem de Disponibilidade de FTE para a Função Principal é 100%.</li> 
       <li> <p><b>Outras funções</b>: Os usuários podem ter várias funções de trabalho no Workfront. As funções de trabalho são essenciais no gerenciamento de recursos. Não há limite para quantas funções de trabalho um usuário pode atender. No entanto, recomendamos não atribuir um usuário a um número excessivamente grande de funções de trabalho, pois o gerenciamento de recursos pode se tornar muito complexo para esses usuários.</p> <p>Para obter mais informações sobre funções do job, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Criar e gerenciar funções de trabalho</a>.</p> <p>Você pode atualizar este campo somente se tiver uma licença do Plan com acesso administrativo de usuário ou se for um administrador do Workfront. Para obter mais informações sobre como configurar usuários com acesso administrativo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
       <li> <p>(Condicional) Se você selecionou um ou vários <b>Outras funções</b>, o <b>Porcentagem de disponibilidade de FTE</b> é exibido para cada função. Especifique qual porcentagem de tempo dos agendamentos dos usuários é alocada para cada função de cargo. O valor padrão da Porcentagem de Disponibilidade de FTE para outras Funções é 0%.</p> <p><b>Nota</b>:  
       <ul> 
       <li>Se Outras Funções tiverem uma Disponibilidade de FTE de 0%, elas não serão exibidas no Planejador de Recursos, a menos que os usuários sejam atribuídos a tarefas nessas funções.</li> 
       <li> <p>A soma de todas as Porcentagens da Disponibilidade de FTE para todas as funções deve ser igual a 100%. Cada Porcentagem da Disponibilidade de FTE calcula as Horas Disponíveis para cada função por usuário no Planejador de Recursos. As Horas Disponíveis para cada função por usuário dependem do tempo disponível para o usuário.</p> <p>O tempo disponível para o usuário é calculado pela Workfront, dependendo do método que foi selecionado pelo administrador do Workfront para calcular o FTE nas Preferências de gerenciamento de recursos.</p> <p>Para obter mais informações sobre como calcular a disponibilidade para o usuário, consulte <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos</a>.</p> <p>Para obter mais informações sobre como configurar preferências de Gerenciamento de Recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências do Gerenciamento de recursos</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Agendar</b>: Associe um agendamento aos usuários. O agendamento dos usuários calcula a linha do tempo das tarefas às quais os usuários estão atribuídos.</p> <p>Um administrador do Workfront ou um administrador de grupo deve criar um agendamento antes que possa ser associado aos usuários.</p> <p>Selecione um agendamento de nível de sistema ou de grupo para atribuí-lo aos usuários selecionados.</p> <p>Para obter mais informações sobre programações de grupo e de nível de sistema, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>.</p> <p><b>IMPORTANTE</b>: O Workfront usa a programação de um usuário somente quando a configuração Calcular disponibilidade de recurso usando está definida como A programação do usuário. Para obter informações sobre como a configuração Calcular disponibilidade de recurso usando afeta qual programação é usada para o Gerenciamento de recursos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configurar preferências do Gerenciamento de recursos</a>.</p> </li> 
       <li> <p><b>Perfil da folha de horas</b>: Associe um Perfil de Folha de Horas aos usuários. Isso garante que as folhas de horas sejam geradas automaticamente para os usuários.</p> 
       <p><b>Nota</b>:  
       <ul> 
       <li>A lista de perfis da folha de ponto disponíveis neste campo depende do seu acesso:
       <ul>
       <li>Como administrador do Workfront, você pode ver todos os perfis de folha de ponto no nível do sistema e do grupo.</li>
       <li><p>Como administrador de grupo, você pode ver perfis de folha de ponto no nível do sistema, bem como aqueles associados aos grupos que você gerencia.</p></li>
       <li><p>Como usuário com uma licença do Planejador e acesso para editar usuários, você pode ver somente perfis de folha de ponto no nível do sistema.</p></li>
       </ul></li> 
       <li>Se você for um administrador de grupo, todos os usuários que você estiver editando deverão ser membros de um grupo que você administra.</li> 
       </ul> </p> </li> 
       <li><b>Tipo de hora padrão</b>: Selecione o tipo de hora padrão para os usuários. Esse é o tipo de hora usado por padrão quando os usuários registram a hora.</li> 
       <li> <p><b>Tipos de hora disponíveis</b>: Selecione os tipos de hora que devem estar disponíveis para o usuário. Esses tipos de hora estão visíveis em qualquer lugar no Workfront, onde os usuários podem registrar o tempo. Um usuário só pode ver os tipos de hora que estão ativados no nível do projeto, bem como o nível do usuário.</p> 
       <p>Para obter mais informações sobre quais tipos de hora estão disponíveis para os usuários, consulte <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Definir os tipos de hora e a disponibilidade das folhas de horas</a>.</p> 
       </li> 
       <li> <b>FTE</b>: Este é o Equivalente de Tempo Total do usuário. A Workfront usa esse número para calcular a disponibilidade do usuário com base na Programação Padrão somente quando as Preferências de Gerenciamento de Recursos no nível do sistema estão definidas como A Programação Padrão.

   <p>O FTE indica o tempo que o usuário pode gastar no trabalho. Isso inclui despesas gerais, bem como tempo gasto no trabalho do projeto. Por exemplo, o tempo gasto em reuniões ou treinamento também é incluído no ETI.</p>

   O FTE deve ser um número decimal até 1 e não pode ser 0. Por exemplo, se o valor FTE for 0,5 e o Horário padrão no Workfront for de 40 horas, o usuário estará disponível por 20 horas por semana.

   O padrão do campo é 1.

   Exceções de agendamento, o tempo limite pode, <span class="preview">e o valor do Tempo de Trabalho</span> pode afetar a disponibilidade do usuário.

   O Workfront calcula a disponibilidade de um usuário dependendo das preferências do Gerenciamento de Recursos na área Configurar .

   Se as Preferências do Gerenciamento de Recursos no nível do sistema estiverem definidas como O Agendamento do Usuário, o valor especificado aqui será ignorado e o usuário será considerado como disponível de acordo com o que é especificado em seu agendamento.

   Para obter mais informações, consulte <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências do Gerenciamento de recursos</a>.

   Para obter mais informações sobre como criar programações no Workfront, consulte <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Criar um agendamento</a>.
   </li> 
       <li> <p><b>Pools de Recursos</b>: Associe os usuários a pools de recursos.</p> <p><b>OBSERVAÇÃO</b>: Apenas os pools de recursos comuns a todos os usuários selecionados aparecem neste campo. Se os usuários selecionados não tiverem pools de recursos compartilhados, esse campo estará vazio. Se este campo estiver vazio, os pools de recursos especificados aqui substituirão os pools de recursos individuais.</p> 
       <p>Para obter mais informações sobre pools de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos pools de recursos </a>.</p> </li> 
       <li><b>Custo por hora</b>: A quantidade de custo por hora para o usuário. </li> 
       <li><b>Faturamento por hora</b>: A quantidade de faturamento por hora para o usuário.</li> 
       <li><b>Forms personalizada</b>: Associe um formulário personalizado do usuário existente aos usuários. É necessário criar um formulário personalizado antes de associá-lo a um usuário. Somente os formulários personalizados ativos são exibidos na lista. Para obter informações sobre como criar formulários personalizados, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a>.</li> 
       <li><b>Comentário</b>: Insira um comentário no campo fornecido. Todos os usuários selecionados receberão uma notificação no aplicativo, bem como uma notificação por email com seu comentário. O comentário é exibido na guia Atualizações do perfil do usuário.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Na seção **Forms personalizada** selecione a **Recalcular expressões personalizadas** para garantir que todos os campos personalizados calculados em formulários personalizados anexados aos usuários selecionados estejam atualizados.

1. Clique em **Salvar alterações**.
