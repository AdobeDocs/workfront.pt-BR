---
product-area: projects
navigation-topic: manage-projects
title: Editar projetos
description: Você pode editar um projeto no Adobe Workfront sempre que necessário. Idealmente, você deve editar um projeto quando ele estiver no status Planejando.
author: Alina
feature: Work Management
exl-id: a6a1f178-189a-4c41-835b-7726081a2b49
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '7666'
ht-degree: 2%

---

# Editar projetos

<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização.</span>

<!--
<p>***Linked to many articles,</p>
<p>The Resource Pools part also duplicates in the "Working with Resource Pools" article </p>
<p>The Update Type section is also documented in Selecting the Project Update Type article</p>
<p>Keep the reference link to the other article that also documents the Update Type) </p>
<p>(NOTE 2: information described here also exists in these articles:</p>
<p>** Project Overview area</p>
<p>**Manage project Finance area</p>
<p>If you need to update just one field, check to see if that field is also listed there and update in both places.)</p>
</div>
-->

Você pode editar um projeto no Adobe Workfront sempre que necessário. Recomendamos que você edite os projetos minimamente depois que seu status for alterado para Atual, para evitar confusão enviando notificações sobre as alterações para toda a equipe de projeto. Idealmente, você deve editar um projeto quando ele estiver no status Planejando. Para obter informações sobre a equipe do projeto, consulte [Visão geral da equipe do projeto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisitos de acesso

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> 
    <ul> 
     <li> <p>Contribute permissions to a project to edit it in the Project Details area </p> </li> 
     <li> <p>Manage permissions to a project to edit it in the Edit Project box</p> </li> 
    </ul> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a projetos, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Conceder acesso aos projetos</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> 
    <ul> 
     <li> <p>Contribuir com permissões para um projeto para editá-lo na área Detalhes do projeto </p> </li> 
     <li> <p>Gerenciar permissões para um projeto para editá-lo na caixa Editar projeto</p> </li> 
    </ul> <p> Para obter informações sobre permissões de projeto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartilhar um projeto no Adobe Workfront</a>.</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Limitações para editar projetos

Existem algumas limitações que podem impedir a edição de projetos.

Considere o seguinte ao editar projetos:

* Não é possível editar projetos que estão em um Processo de aprovação, exceto pelo registro de tempo.
* Você pode anexar documentos ou modelos a um projeto com status Concluído, Inativo ou Pendente de Aprovação somente se o administrador do Workfront ou um administrador de grupo tiver ativado essa funcionalidade na área Preferências do projeto. Para obter informações sobre como configurar as preferências do projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Você só pode editar as seguintes informações em um projeto com status Desativado ou Concluído:

   * Modificar despesas existentes.
   * Adicionar, remover ou editar formulários personalizados.

## Editar um projeto

Ao editar um projeto, você pode modificar as informações e configurações do projeto, bem como as tarefas e problemas do projeto.

Algumas configurações mencionadas neste artigo podem ser modificadas do status padrão pelo seu estado no template do qual o projeto foi criado. Para obter informações sobre a edição de modelos, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Projetos**.
1. (Opcional) Clique em **Projetos em que estou trabalhando** ou **Projetos dos quais sou proprietário** no canto superior direito para exibir projetos dos quais você é o proprietário ou projetos dos quais faz parte da equipe do projeto.

   ![](assets/projects-on-my-own-buttons-350x302.png)

1. Clique no nome do projeto que deseja editar para abrir a página do projeto.

   >[!NOTE]
   >
   >Se você for um administrador de grupo, poderá ver e editar os projetos do seu grupo na área Grupos e na área Projetos. Para obter mais informações, consulte [Criar e modificar os projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. (Opcional) Para editar informações limitadas sobre um projeto, clique em **Detalhes do projeto** no painel esquerdo.

   ![](assets/nwe-project-details-expanded-350x298.png)

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront ou o administrador de Grupo modificou o Modelo de layout, os campos na área Detalhes do projeto podem ser reorganizados ou não ser exibidos. Para obter informações, consulte [Personalizar a exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Para editar informações na seção Detalhes, faça o seguinte:

   1. (Opcional) Clique no link **Recolher Tudo** no canto superior direito para recolher todas as áreas.
   1. (Opcional e condicional) Quando uma área for recolhida, clique no botão **seta para a direita** ![](assets/right-pointing-arrow.png) ao lado de cada área para expandir a área que você deseja editar.
   1. Para obter mais informações sobre como editar informações na guia Detalhes do projeto, consulte os seguintes artigos:

      * [Gerenciar informações na área Visão geral do projeto](../../../manage-work/projects/manage-projects/understand-project-overview-area.md)
      * [Gerenciar informações na área de finanças do projeto](../../../manage-work/projects/project-finances/manage-project-finance-area.md)
   1. (Opcional) Para anexar um formulário personalizado, comece digitando o nome de um formulário na **Adicionar formulário personalizado** , selecione-o quando ele for exibido na lista e clique em **Salvar alterações**.
   1. (Opcional) Clique no link **Exportar** ícone ![](assets/export.png) para exportar as informações de Visão geral e formulários personalizados para um arquivo PDF, em seguida, clique em **Exportar**. Selecione entre as seguintes opções:

      * Selecionar tudo (é exibido somente quando há pelo menos um formulário personalizado anexado)
      * Visão geral
      * O nome de um ou vários formulários personalizados

      O arquivo PDF é baixado no computador.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Para obter mais informações, consulte [Exportar formulários personalizados e detalhes do objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   Para obter informações sobre os campos visíveis na seção Detalhes do projeto, continue editando o projeto na caixa Editar projeto, conforme descrito abaixo.
1. Para editar todas as informações sobre o projeto, clique no link **Mais** menu ![](assets/qs-more-menu.png) ao lado do nome do projeto, clique em **Editar**.

   Ou

   Em uma lista de projetos, selecione um projeto e clique no botão **Editar** ícone ![](assets/edit-icon.png) no topo da lista.

   A variável **Editar Projeto** é aberta.

   >[!IMPORTANT]
   >
   >Você deve ter Permissões de gerenciamento no projeto para ver a opção Editar.

   Todos os campos de projeto estão disponíveis na caixa Editar projeto e são agrupados pelas áreas listadas no painel esquerdo.

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront ou do Administrador de grupo modificou o Modelo de layout, as áreas no painel esquerdo da caixa Editar projeto ou quaisquer campos listados nessas áreas podem ser reorganizados ou não serão exibidos. Para obter informações, consulte [Personalizar a exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. (Condicional) Se você clicou na variável **Mais** e depois **Editar**, considere atualizar as informações em qualquer uma das seguintes áreas listadas no painel esquerdo:

   * [Nome do Projeto](#project-name)
   * [Visão geral](#overview)
   * [Formulários personalizados](#custom-forms)
   * [Finanças](#finance)
   * [Parâmetros do projeto](#project-settings)
   * [Configurações da tarefa](#task-settings)
   * [Configurações do problema](#issue-settings)
   * [Acesso](#access)

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront configura nosso Modelo de layout para a área Detalhes do projeto, as seções e os campos na caixa Editar projeto podem ser diferentes em seu ambiente. Para obter informações, consulte [Personalizar a exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### Nome do Projeto {#project-name}

1. Comece a editar seu projeto conforme descrito acima.
1. Clique em **Nome do projeto** no painel esquerdo.

   ![](assets/nwe-project-name-in-edit-project-box-350x125.png)

1. Atualize o nome do projeto.

   Não é possível editar o nome do projeto ao editar projetos em massa.

### Visão geral {#overview}

1. Comece a editar seu projeto conforme descrito acima.
1. Clique em **Visão geral** no painel esquerdo.

   ![](assets/nwe-overview-in-edit-project-box-350x172.png)

1. Atualize as seguintes informações sobre o projeto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td> <p>Inclua informações adicionais sobre o projeto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td> <p>Selecione o status do projeto. Não é possível marcar um projeto como Concluído antes que todas as tarefas e problemas sejam concluídos. Para obter informações sobre status de projetos, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md" class="MCXref xref">Acessar a lista de status de projeto do sistema</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridade</strong> </td> 
      <td> <p> <p>Este é apenas um sinalizador visual para você que permite priorizar seus projetos.</p> <p>Dependendo das Preferências do projeto selecionadas pelo administrador do Workfront, os nomes das prioridades podem ser diferentes para você. Para obter mais informações sobre edição de prioridades, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Criar e personalizar prioridades</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Especifique um link da Web relacionado às informações sobre este projeto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipo de Condição</strong> </td> 
      <td> <p>Selecione entre os seguintes Tipos de Condição: 
       <ul> 
       <li><strong>Manual:</strong> O proprietário do projeto define a condição no projeto manualmente.</li> 
       <li><strong>Status do progresso:</strong> O Workfront define automaticamente a condição com base no Status de Progresso das tarefas no Caminho Crítico. Para obter mais informações sobre como entender o Status do Progresso, consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do status de progresso da tarefa</a>.</li> 
       </ul><p>Seu administrador do Workfront<span> ou um administrador de grupo</span> seleciona o padrão de como a condição dos projetos é calculada para o seu sistema <span>ou seu grupo</span>. Para obter informações sobre como configurar os padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>. </p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condição</strong> </td> 
      <td> <p> <p>(É exibido somente após selecionar <strong>Manual</strong> para o <strong>Tipo de condição</strong>): Selecione uma Condição para indicar como o projeto está indo. </p> <p>Para obter informações sobre como as condições do projeto podem ser definidas automática ou manualmente, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Visão geral da condição do projeto e do tipo de condição</a></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Modo de Cronograma</strong> </td> 
      <td> <p>Especifique se o projeto está agendado a partir da Data inicial ou da Data de conclusão. Essa seleção determina as datas planejadas das tarefas no projeto. 
       <ul> 
       <li><strong>Data de início</strong>: por padrão, a primeira tarefa do projeto tem a mesma Data de início planejada do projeto. Para obter informações sobre a Data de Início Planejada da tarefa, consulte <a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Visão geral da Data de Início Planejada da tarefa</a>. O cronograma do projeto é calculado a partir da Data inicial e a Data de conclusão do projeto é calculada pelo sistema, com base na duração de todas as tarefas. </li> 
       <li><strong>Data de Término</strong>: A última tarefa do projeto tem a mesma Data de conclusão planejada que o projeto. A linha do tempo do projeto é calculada a partir da Data de conclusão e a Data inicial do projeto é calculada pelo sistema, subtraindo a duração de todas as tarefas da Data de conclusão do projeto. </li> 
       </ul><p>Seu administrador do Workfront<span> ou um administrador de grupo</span> seleciona a configuração padrão Modo de programação para seu sistema ou grupo. Para obter informações sobre como configurar os padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data e hora de início planejadas</strong> </td> 
      <td> <p> <p>Especifique a data ao selecionar <strong>Agendar a Partir da Data de Início</strong>. <br></p> <p>Este campo é somente leitura ao selecionar <strong>Programação a partir da data de conclusão</strong>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data e hora de conclusão planejadas</strong> </td> 
      <td> <p>Especifique a data ao selecionar <strong>Programação a partir da data de conclusão</strong>. </p> <p>Este campo é somente leitura ao selecionar <strong>Agendar a partir da Data de Início</strong>.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Portfólio</strong></td> 
      <td>Indique um Portfolio ao qual o projeto pertence. Você deve criar um Portfolio primeiro, antes que ele apareça na lista suspensa. Somente portfólios ativos podem ser associados a um projeto. Para obter mais informações sobre como criar portfólios, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Criar um portfólio </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Programa</strong></td> 
      <td> <p>Se você selecionou um Portfolio para o projeto, especifique um Programa para o projeto. Alguns Portfolio podem não ter programas. Você deve criar um Programa primeiro, antes que ele apareça nesta lista suspensa. Somente programas ativos podem ser associados a um projeto. </p> <p>Para obter mais informações sobre a criação de programas, consulte <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Criar um programa</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Grupo</strong></td> 
      <td> <p> <p>Especifique o nome do grupo associado ao projeto. </p>Este campo é obrigatório. Você não pode ter um projeto que não esteja associado a um grupo. </p> <p>Você pode verificar se está selecionando o grupo correto ao passar o mouse sobre ele e clicar no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> Por padrão, um dos grupos a seguir é associado automaticamente a um projeto quando ele é criado, a menos que você especifique um grupo diferente:</p> 
       <ul> 
       <li> <p><span>Quando o projeto é criado na área Projetos, o Grupo inicial do criador do projeto é associado ao projeto.</span> </p> <p>Isso também ocorre quando o projeto é criado a partir da seção Projetos em um portfólio ou programa.</p> </li> 
       <li> <p>Quando o projeto é criado a partir da página principal de um grupo na área Configuração, esse grupo é associado ao projeto.</p> </li> 
       </ul> </p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> <p>Se o projeto, suas tarefas ou problemas já estiverem associados a um processo de aprovação em nível de grupo usando status personalizados em nível de grupo, alterar o grupo pode criar um conflito entre os status de aprovação do grupo anterior e os existentes no nível do sistema. Considere remover os processos de aprovação em nível de grupo no projeto, ou suas tarefas ou problemas, antes de atualizar o grupo. Para obter informações sobre como criar processos de aprovação de nível de grupo, consulte <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processos de aprovação de nível de grupo</a>. Para obter informações sobre como criar um status personalizado em nível de grupo, consulte <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md" class="MCXref xref">Criar ou editar um status de grupo</a></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Empresa</strong> </td> 
      <td> <p>Especifique uma empresa associada ao projeto. Você deve criar uma empresa antes de associá-la a um projeto. Somente empresas ativas podem ser associadas a um projeto. Para obter informações sobre como criar empresas, consulte <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md" class="MCXref xref">Criar e editar empresas</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Proprietário do projeto</strong> </td> 
      <td> <p>Comece digitando o nome de um usuário para adicioná-lo ao projeto e, em seguida, selecione-o quando ele for exibido na lista. O usuário é adicionado à equipe do projeto e recebe automaticamente permissões de gerenciamento para o projeto. O usuário designado como Proprietário do projeto deve ser um usuário ativo do Workfront.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Patrocinador do projeto</strong> </td> 
      <td> <p>Comece digitando o nome de um usuário para adicioná-lo ao projeto e, em seguida, selecione-o quando ele for exibido na lista. O usuário é adicionado à equipe do projeto e recebe automaticamente permissões de Exibição para o projeto. O usuário designado como Patrocinador do projeto deve ser um usuário ativo do Workfront.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gerenciador de Recursos</strong> </td> 
      <td> <p> Comece digitando os nomes dos usuários para adicioná-los ao projeto e, em seguida, selecione-os quando eles forem exibidos na lista. Os usuários são adicionados à equipe do projeto e recebem automaticamente permissões de Gerenciamento para o projeto e podem atribuir recursos às tarefas e problemas no projeto. Os usuários mantêm permissões de Gerenciamento no projeto mesmo quando são removidos do campo Gerenciador de recursos. Você pode especificar mais de um Gerenciador de recursos.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Ao atualizar os campos Proprietário do projeto, Patrocinador do projeto e Gerente de recursos, observe o avatar, a Função principal do usuário ou o endereço de email dele para distinguir entre usuários com nomes idênticos. Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Formulários personalizados {#custom-forms}

Dependendo do seu nível de acesso e da sua permissão no projeto, os seguintes cenários existem:

* Se você não tiver permissões Editar formulário personalizado no projeto, não poderá editar os campos em nenhum dos formulários personalizados anexados. Você só pode exibir os campos nos formulários personalizados anexados ao projeto.
* Se você tiver acesso de Visualização (e não de Edição) a uma seção em um formulário personalizado, não poderá editar os campos nessa seção.
* Se você não tiver acesso a uma seção em um dos formulários personalizados anexados ao projeto, a seção não será exibida na caixa Editar projeto.

Ao selecionar mais de um projeto para editá-los em massa, os seguintes cenários existem:

* Se você não tiver permissões Editar formulário personalizado em pelo menos um dos projetos selecionados, não poderá editar os campos em nenhum dos formulários personalizados anexados. Você só pode exibir os campos nos formulários personalizados anexados
* Se você tiver acesso de Visualização (e não de Edição) a uma seção em um formulário personalizado, não poderá editar os campos nessa seção. Você só pode exibir os campos nessa seção.
* Se você não tiver acesso a uma seção em um dos formulários personalizados anexados a pelo menos um dos projetos, a seção não será exibida na caixa Editar projetos.

Para obter informações sobre o acesso a formulários personalizados, consulte os seguintes artigos:

* [Compartilhar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
* [Adicionar uma quebra de seção a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)

Para editar informações sobre formulários personalizados:


1. Comece a editar seu projeto conforme descrito acima.
1. Clique em **Forms personalizado** no painel esquerdo.

   ![](assets/nwe-custom-forms-in-edit-project-box-350x170.png)

1. Clique em **Adicionar formulário personalizado** e selecione um formulário na lista para anexá-lo ao projeto. Por padrão, os primeiros 40 formulários são exibidos em ordem alfabética. Se você não vir o formulário na lista, comece digitando o nome dele, em seguida, selecione-o quando ele aparecer na lista.

   >[!NOTE]
   >
   >Você deve criar os formulários personalizados antes que eles estejam disponíveis para seleção neste campo. Somente formulários personalizados ativos são exibidos na lista. Para obter mais informações sobre a criação de formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Você pode adicionar até dez formulários personalizados a um projeto.


1. (Condicional) Se você anexou um formulário personalizado ao projeto, edite os campos no formulário. Você deve especificar todos os campos obrigatórios antes de salvar o projeto.
1. (Opcional) Clique no link **Ícone X** à direita do nome de um formulário personalizado para removê-lo, depois clique em **Remover**.
1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar

   Ou

   Clique em **Salvar**.

### Finanças {#finance}

Dependendo do seu nível de acesso e da sua permissão no projeto, os seguintes cenários existem:

* Se você tiver o acesso de Visualização de Dados Financeiros e permissões de Visualização de Finanças no projeto, poderá apenas visualizar os campos na seção de Finanças. Não é possível editar os campos nesta seção.
* Se você tiver acesso para Editar aos Dados Financeiros e Gerenciar Finanças no projeto, poderá atualizar os campos desta seção.

Ao selecionar mais de um projeto para editá-los em massa e no, os seguintes cenários existem:

* Se você selecionar pelo menos um projeto no qual tenha permissões de Exibir finanças (em vez de Gerenciar finanças), poderá exibir somente os campos desta seção para todos os projetos selecionados. Não é possível editar os campos em massa na seção Finanças.
* Se você selecionar pelo menos um projeto sem permissões financeiras, esta seção não será exibida.

Para editar campos na área Finanças:


1. Comece a editar seu projeto conforme descrito acima.
1. Clique em **Finanças** no painel esquerdo.

   ![](assets/nwe-finance-in-edit-project-box-350x183.png)

1. Atualize as seguintes informações financeiras do projeto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Moeda</strong> </td> 
      <td> <p> <p>Especifique a moeda do projeto, se for diferente da moeda padrão do sistema. Não é possível alterar a moeda de um projeto se já houver informações financeiras sobre o projeto. Esse campo não estará visível se você só tiver a moeda padrão no sistema. </p> <p>Para obter mais informações sobre moeda, consulte <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.<br></p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Orçamento</strong> </td> 
      <td> <p>Especifique um Orçamento para o projeto.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Método Índice de desempenho</strong> </td> 
      <td> <p>Selecionar <b>Baseado em Hora</b>ou <b>Baseado em Custo</b> para indicar se as métricas de Valor Agregado do projeto (como Índice de Desempenho de Custo ou Custo Efetivo Estimado) são calculadas usando horas ou custos. </p> <p>Para obter mais informações sobre o Método Índice de desempenho, consulte <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Definir o PIM (Método de Índice de Desempenho)</a>. </p> <p>Seu administrador do Workfront<span> ou um administrador de grupo</span> seleciona a configuração padrão Método de indexação de desempenho para o seu sistema ou grupo. Para obter informações sobre como configurar os padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Calcular ao concluir</strong> </td> 
      <td> <p> <p>Especifique como o Workfront deve calcular a EAC (Estimativa no Término). </p>
      Selecione entre as seguintes opções: 
      <ul><li><b>Calcular no nível do projeto</b></li>
      <li><b>Extrair de tarefas/subtarefas</b></li> </ul>
      <p>Para obter mais informações sobre como é calculada a Estimativa no término, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular Estimativa no Término (EAC)</a>.</p> <p>O administrador do Workfront ou do grupo seleciona a configuração padrão Estimar na conclusão para o seu sistema ou grupo. Para obter informações sobre como configurar os padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benefício Planejado</strong> </td> 
      <td> <p>Estime qual é o benefício planejado do projeto. Isso é usado no Business Case do projeto e no Portfolio Otimizer. Para obter mais informações sobre o Benefício Planejado de um projeto, consulte <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Visão Geral do Benefício Planejado do projeto</a>. O Benefício Planejado de um projeto é considerado quando o Valor Líquido de um projeto é calculado. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Gerenciar projetos no Portfolio Otimizer</a> .<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benefício Efetivo</strong> </td> 
      <td> <p>Estimativa do Benefício Efetivo do projeto. Esse é um valor na moeda que representa o benefício que sua empresa ou departamento ganharia após a conclusão desse projeto. </p> </td> 
     </tr> 
      <tr> 
      <td role="rowheader"><strong>Custo Fixo</strong> </td> 
      <td> <p>Especifique o Custo Fixo do projeto. Isso é diferente do Custo de mão de obra que vem das horas no projeto e do Custo de despesa que vem da quantidade de despesas no projeto. O Custo Fixo de um projeto é considerado ao calcular o Valor Líquido de um projeto e faz parte do Custo Orçado.<br></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Receita com Valor Fixo</strong> </td> 
      <td> <p>Especifique a Receita Fixa do projeto.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Parâmetros do projeto {#project-settings}

1. Comece a editar seu projeto conforme descrito acima.
1. Clique em **Configurações do projeto** no painel esquerdo.

   ![](assets/nwe-project-settings-in-edit-project-box-350x380.png)

1. Atualize as seguintes informações:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
      <td role="rowheader"><strong>Caminho de Etapas</strong> </td> 
       <td> <p>Selecione um Caminho de Etapas para o projeto. Somente os caminhos de etapas ativos são exibidos na lista.</p> <p>Para obter mais informações sobre Caminhos de Etapas, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Criar um caminho de etapas</a>.</p> </td> 
      </tr> 
      <tr> 
      <td role="rowheader"><strong>Modelo de Término</strong> </td> 
      <td> <p>Controla como o projeto é marcado como Concluído. Selecione entre as seguintes opções: 
       <ul> 
       <li><p><strong>Automático</strong>: o projeto é marcado como Concluído quando todas as tarefas e problemas são concluídos.</p><p>O status do projeto é alterado automaticamente para Concluído somente quando o status do projeto é Atual quando as tarefas são concluídas. </p></li> 
       <li><strong>Manual</strong>: é necessário selecionar manualmente o status Concluído para o projeto quando todas as tarefas e problemas estiverem concluídos.</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Modo de conclusão em resumo</strong></td> 
       <td> <p>Controla como as tarefas pai são marcadas como Concluídas. Selecione entre as seguintes opções: 
       <ul> 
       <li><strong>Automático</strong>: as tarefas pai são marcadas como Concluídas e atualizam seu percentual concluído automaticamente, à medida que as tarefas filho são concluídas e o percentual concluído dos filhos é atualizado. </li> 
       <li><strong>Manual</strong>: é necessário atualizar manualmente o percentual concluído e o status das tarefas pai, independentemente de quais alterações são feitas nas tarefas filho.</li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Tipo de Atualização</strong></td> 
       <td> <p>Controla quando as alterações feitas na linha do tempo do projeto são salvas no projeto ou nas tarefas pai. Por exemplo, as seguintes alterações no projeto acionam uma atualização na linha do tempo do projeto: 
       <ul> 
       <li>Atualizar as datas das tarefas</li> 
       <li>Alterar relações predecessoras de tarefas</li> 
       <li><p>Alterar relações pai-filho, adicionando ou removendo atribuições, além de alterar a restrição ou o tipo de duração da tarefa.</p><p>Quando as tarefas são atualizadas, seus objetos principais (tarefas principais ou o projeto) são atualizados no momento indicado pelo Tipo de Atualização. </p><p>Se os objetos pai não forem atualizados imediatamente após a alteração ao selecionar "Automático e Ao Alterar" ou "Alterar Somente" Tipo de Atualização, atualize a página</p><p>Selecione entre as seguintes opções: </p><p>- <strong>Automático e Mediante alteração</strong> (Configuração padrão): a linha do tempo do projeto é atualizada sempre que uma alteração ocorre no projeto ou em outro projeto do qual o projeto depende (Na alteração). A linha do tempo do projeto também é atualizada todas as noites (Automático).</p><p>Essa é a configuração recomendada para esse campo porque garante que o projeto esteja sempre atualizado.</p><p>Quando você executa uma ação em uma tarefa ou projeto que aciona um recálculo de linha do tempo, todas as datas disponíveis são exibidas imediatamente, permitindo que você continue trabalhando. Em projetos com mais de 100 tarefas, as datas que exigem recálculos mais longos são exibidas brevemente como um ponto de interrogação (entre 1 e 5 segundos ou até um minuto para projetos grandes). Isso indica que o recálculo ainda não foi concluído e as datas estão sujeitas a alterações.</p><p>- <strong>Somente Alteração</strong>: a linha do tempo do projeto é atualizada sempre que uma alteração ocorre no projeto ou em outro projeto do qual o projeto depende. Você pode selecionar essa opção se alterações raramente ocorrerem no projeto ou em outros projetos dos quais a linha do tempo depende.</p><p>- <strong>Somente automática</strong>: a linha do tempo do projeto é atualizada todas as noites; a linha do tempo não é atualizada imediatamente após as alterações serem feitas.</p><p>Você pode selecionar essa opção se muitas alterações ocorrerem todos os dias no projeto ou em outros projetos dos quais a linha do tempo depende. No entanto, lembre-se de que você escolheu essa configuração, pois o projeto não será atualizado ao mesmo tempo em que as alterações são feitas.</p><p>- <strong>Somente manual</strong>: a linha do tempo do projeto é atualizada somente quando você seleciona a opção Recalcular linha do tempo. Para obter mais informações sobre o recálculo manual da linha de tempo do projeto, consulte <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular linhas do tempo do projeto</a>. </p><p>Você pode selecionar essa opção se estiver fazendo muitas alterações ao projeto de uma vez e quiser que o recálculo da linha do tempo ocorra após todas as alterações terem sido feitas (em vez de após cada alteração individual).</p></li> 
       </ul></p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Cronograma</strong> </td> 
       <td> <p>Selecione um cronograma para o seu projeto. Deve ser o mesmo agendamento atribuído à maioria das pessoas que estão trabalhando no projeto. Você deve criar um cronograma antes de atribuí-lo a um projeto ou usuário. Se você não tiver criado agendamentos personalizados em seu sistema, o Agendamento padrão será selecionado.</p> <p>Para obter mais informações sobre a criação de cronogramas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Tempo de folga do usuário</strong> </td> 
       <td> <p>Determina se o tempo de folga do Destinatário principal de uma tarefa ajusta as datas planejadas da tarefa no projeto. </p><p>Seu administrador do Workfront<span> ou um administrador de grupo</span> seleciona o padrão para esta configuração para seu sistema <span>ou seu grupo</span>. Para obter informações sobre como configurar os padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>. </p><p>Selecione entre as seguintes opções:<br>- <strong>Considerar o tempo de folga do usuário nas durações de tarefas</strong>: ao selecionar essa opção, as datas planejadas das tarefas são ajustadas de acordo com o tempo de folga do Principal responsável pela tarefa, se o tempo de folga ocorrer durante a duração da tarefa. </p><p>Por exemplo, se uma tarefa com uma restrição O Mais Breve Possível estiver programada para iniciar em 1º de junho e terminar em 3 de junho, e o Destinatário principal tiver 2 de junho marcado para Folga, quando essa seleção estiver ativada, as datas planejadas da tarefa serão de 1º de junho a 4 de junho. Dependendo da Restrição da Tarefa, existem os seguintes cenários: </p> 
       <ul> 
       <li>Para restrições de tarefa relacionadas ao planejamento a partir de uma data inicial (Assim que Possível, Primeiro Horário Disponível, Não Iniciar Antes De, Não Iniciar Depois De, Deve Iniciar Em), a Data Inicial Planejada não é alterada, mas a Data de Conclusão Planejada é alterada.</li> 
       <li>Para restrições de tarefa relacionadas ao planejamento a partir de uma data de conclusão (O Mais Tarde Possível, Último Tempo Disponível, Não Terminar Antes De, Não Terminar Depois De, Deve Terminar Em), a Data de Conclusão Planejada não é alterada, mas a Data Inicial Planejada é alterada.</li> 
       <li>Para tarefas com uma restrição de Datas Fixas, nem a Data de Início Planejada nem a Data de Conclusão são alteradas. </li> 
       </ul><p>A duração da tarefa não é alterada ao selecionar essa configuração. Somente as datas planejadas mudam, dependendo da Restrição da Tarefa. Para obter informações sobre a restrição da tarefa, consulte <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Visão geral de Restrição de Tarefa</a>. </p><p>- <strong>Ignorar o tempo de folga do usuário nas durações de tarefas</strong>: ao selecionar essa opção, as datas planejadas das tarefas no projeto permanecem como planejadas originalmente, mesmo que o Principal responsável da tarefa tenha uma folga durante a duração da tarefa. </p><p>Considere o seguinte ao selecionar opções para essa configuração:</p> 
       <ul> 
       <li><p>A opção padrão para essa configuração para um novo projeto é a mesma que a preferência de projeto no nível do sistema. </p><p>Para obter informações sobre as preferências do projeto no nível do Sistema, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>. </p></li> 
       <li>Ao anexar um modelo a um projeto existente, a configuração no projeto é atualizada para corresponder à do modelo. </li> 
       <li><p>O Workfront decide quais datas da tarefa planejada ajustar de acordo com o valor de Restrição da Tarefa da tarefa. Dependendo do que for, o Início planejado ou a Data de conclusão planejada, ou ambos, podem ser afetados ou podem até permanecer os mesmos. Por exemplo, se uma tarefa tiver uma Restrição de datas fixas, as datas não serão ajustadas quando o Principal responsável tiver folga, mesmo quando <strong>Considerar o tempo de folga do usuário nas durações de tarefas</strong> está selecionada. </p></li> 
       </ul></td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Modo de Nivelamento de Recursos</strong> </td> 
       <td> <p> <p>Selecione entre as seguintes opções:</p> <p>- <strong>Manual</strong>: você deve nivelar os recursos manualmente (essa é a configuração padrão)</p> <p>- <strong>Automático</strong>: o Workfront nivela seus recursos.</p> <p>Para obter mais informações sobre o Nivelamento de Recursos, consulte <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Nivelar Recursos no Gráfico de Gantt </a>.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Risco</strong> </td> 
       <td> <p> <p>Defina o nível de risco do seu projeto. O risco é apenas um indicador do quão arriscado um projeto pode ser. Você pode priorizar a execução de seus projetos com base no nível de risco.</p> <p> <p>Considere selecionar entre os seguintes níveis de risco:</p> <p>- Muito Baixo</p> <p>- Baixa</p> <p>- Média</p> <p>- Alta</p> <p>- Muito Alto</p> <p>Os níveis de riscos que você indicar aqui não podem ser personalizados.</p> <p>Eles não estão relacionados aos riscos potenciais que podem ocorrer durante a vida de um projeto e que você deve registrar na guia Riscos do projeto ou no Business Case. Para obter informações sobre riscos potenciais do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md" class="MCXref xref">Editar e criar tipos de risco</a>. </p> </p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Conjuntos de Recursos</strong> </td> 
       <td> <p> <p>Especifique os Conjuntos de recursos associados ao projeto. Conjuntos de recursos são coleções de usuários que são necessárias ao mesmo tempo para a conclusão de um projeto e permitem o orçamento do projeto no Planejador de recursos. Para obter mais informações sobre Conjuntos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos conjuntos de recursos </a>. </p> <p>Ao editar projetos em massa, somente os Conjuntos de recursos comuns a todos os projetos selecionados aparecem nesse campo. Se os projetos selecionados não tiverem Conjuntos de recursos compartilhados, esse campo estará vazio. Os Conjuntos de recursos que você especificar aqui substituirão os Conjuntos de recursos individuais dos projetos.</p> </p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <strong>Permitir que taxas de cobrança no nível de empresa substituam taxas de cobrança no nível do projeto</strong></td> 
       <td>Selecione esta opção para permitir que taxas de cobrança no nível da empresa substituam taxas de função de trabalho históricas, a menos que essas taxas estejam marcadas como faturadas. Ativar essa opção substitui taxas de funções de trabalho históricas, a menos que estejam marcadas como faturadas. <br>Para obter mais informações, consulte <a href="../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md" class="MCXref xref">Sobrepor Taxas de Cobrança no Nível do Projeto com Taxas de Cobrança no Nível da Empresa</a>.</td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Exigir que o tempo seja aprovado para este projeto</strong></td> 
       <td> <p> Selecione esta opção para exigir que o Proprietário do projeto aprove as horas registradas no projeto. Se você estiver usando Registros de cobrança e selecionar essa opção, somente as horas aprovadas no projeto aparecerão como horas faturáveis disponíveis para os Registros de cobrança. A aprovação de horas no projeto é independente da aprovação de folhas de horas. </p> <p>Para obter mais informações sobre a exigência de tempo para aprovação em um projeto, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Exigir que o tempo seja aprovado para um projeto</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"><strong>Filtrar Tipos de Hora</strong> e</span> <strong>Tipos de Hora</strong></td> 
       <td> <p> <p>Selecione entre as seguintes opções:</p> 
       <ul> 
       <li> <p>Selecionar <strong>Não</strong> para disponibilizar todos os tipos de horas específicos do projeto. (Esta é a seleção padrão)</p> <p>Ou</p> </li> 
       <li>Selecionar <strong>Sim</strong> para disponibilizar no projeto apenas um subconjunto dos tipos de horas específicos do projeto, selecione os tipos de horas que deseja disponibilizar. (Mantenha pressionada a tecla Shift para selecionar vários tipos de horas.)</li> 
       <p>Se você selecionar essa opção, somente os tipos de horas selecionados serão disponibilizados para seleção ao registrar horas no projeto (ou em tarefas e problemas no projeto). Você deve selecionar pelo menos um tipo de hora; se você selecionar essa opção e não selecionar nenhum tipo de hora, todos os tipos de hora serão disponibilizados no projeto.</p> </ul>

   <p>As mesmas seleções de tipo de hora devem ser feitas no nível do usuário individual para que o usuário veja essas opções de tipo de hora no projeto. Para obter mais informações sobre como definir tipos de horas no nível do usuário, consulte <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Registrar tempo</a>. </p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>Lembrete de Notificação</strong> </td> 
       <td> <p> <p>Selecione a Notificação de lembrete que deve ser associada ao projeto. Você deve configurar Notificações de lembrete para que os projetos sejam exibidos durante a edição de um projeto. Para obter mais informações sobre como configurar Notificações de lembrete, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md"><a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurar notificações de lembrete</a> .</a></p> </p> </td> 
      </tr> 
      <tr data-mc-conditions=""> 
       <td role="rowheader"><strong>Processo de aprovação</strong></td> 
       <td> <p>Selecione o processo de aprovação que deseja associar ao projeto. O administrador do Workfront deve definir Processos de aprovação no nível do sistema antes que você possa associá-los a projetos. <span>Um usuário com acesso administrativo aos processos de Aprovação também pode criar processos de aprovação específicos do grupo.</span> Para obter mais informações sobre como criar processos de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Criar um processo de aprovação para itens de trabalho</a>.</p> <p>Considere o seguinte ao adicionar processos de aprovação: </p> 
       <ul> 
       <li>Somente os processos de aprovação ativos são exibidos na lista. </li> 
       <li> <p>Os processos de aprovação específicos do grupo e de todo o sistema são exibidos na lista. Um processo de aprovação associado a um grupo diferente daquele do projeto não é exibido na lista.</p> <p>Se o grupo associado ao projeto mudar, o processo de aprovação específico do grupo se tornará um processo de aprovação de uso único. Para obter mais informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos</a>. </p> </li> <!--(NOTE: this bullet stays here although the sections it might appear in are QS only, so we can use the snippet for both Qs and classic)-->
       <p>Quando você edita projetos em massa, os seguintes cenários existem:</p> 
       <ul> 
       <li> <p>Quando você seleciona projetos do mesmo grupo, os processos de aprovação de nível de sistema e de grupo são exibidos nesse campo.</p> </li> 
       <li> <p>Ao selecionar projetos de grupos diferentes, somente os processos de aprovação no nível do sistema são exibidos nesse campo.</p> </li> 
       <li> <p>Quando qualquer um dos projetos tiver um processo de aprovação de uso único anexado, ele será substituído pelo processo de aprovação no nível do sistema ou do grupo selecionado. </p> </li> 
      </ul> </td> 
      </tr> 
      <tr> 
      </tr> 
      </tbody> 
      </table>

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Configurações da tarefa {#task-settings}

Você pode definir os padrões que serão associados a todas as novas tarefas ao adicioná-los ao projeto.

Para obter informações sobre como essas configurações afetam a criação de novas tarefas, consulte a seção [Padrões de tarefa ao adicionar tarefas a um projeto](../../../manage-work/tasks/create-tasks/create-tasks-overview.md#understa) no artigo [Visão geral da criação de tarefas](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Comece a editar seu projeto conforme descrito acima.
1. Clique em **Configurações da tarefa** no painel esquerdo.

   ![](assets/nwe-task-settings-in-edit-project-box-350x211.png)

1. No **Processo padrão de aprovação de tarefas** , selecione a tarefa Processo de Aprovação que deseja associar a todas as novas tarefas quando adicioná-las ao projeto.

   O administrador do Workfront (ou um usuário com acesso administrativo aos processos de Aprovação) deve criar um processo de aprovação no nível do sistema para uma tarefa antes de você associá-la a um projeto. Somente os processos de aprovação ativos são exibidos na lista. Para obter informações sobre como criar Processos de Aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md). Para obter informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte [Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

   Quando você edita projetos em massa, os seguintes cenários existem:

   * Quando você seleciona vários projetos do mesmo grupo, os processos de aprovação de tarefas específicos do sistema e do grupo são exibidos nesse campo.
   * Quando você seleciona vários projetos de grupos diferentes, somente os processos de aprovação de tarefa no nível do sistema são exibidos nesse campo.

1. No **Forms Personalizado Padrão de Tarefa** , selecione o(s) formulário(s) personalizado(s) que deseja associar a todas as novas tarefas quando adicioná-los ao projeto. Você deve criar os formulários personalizados antes que eles estejam disponíveis para seleção neste campo. Somente formulários personalizados ativos são exibidos na lista. Para obter mais informações sobre a criação de formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). Você pode associar até dez formulários personalizados a uma tarefa.
1. (Opcional) Selecione **Use o esforço do trabalho para calcular automaticamente as Horas Planejadas das tarefas** se quiser ativar o gerenciamento do esforço da tarefa usando o Esforço de trabalho em vez das Horas planejadas.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

1. (Condicional e opcional) Se você selecionou Usar esforço do trabalho para calcular automaticamente as Horas planejadas da tarefa, clique no menu suspenso de cada nível de esforço e selecione uma porcentagem para cada nível. Os seguintes valores percentuais são padrões:

   | Tamanho | Percentagem |
   |---|---|
   | Pequena | 25% |
   | Média | 50% |
   | Grande | 75% |

   >[!TIP]
   >
   >Quando o Tipo de atualização do projeto é definido como Automático e você seleciona essa configuração, as Horas planejadas das tarefas são atualizadas de acordo com a Duração da tarefa e a porcentagem do Esforço de trabalho, se forem definidas como zero. Para obter mais informações sobre como usar o Esforço de trabalho para planejar o esforço para uma tarefa, consulte [Visão geral do esforço de trabalho](../../../manage-work/tasks/task-information/work-effort.md).

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Configurações do problema {#issue-settings}

1. Comece a editar seu projeto conforme descrito acima.
1. Clique em **Configurações do problema** no painel esquerdo.

   ![](assets/nwe-issue-settings-in-edit-project-box-350x306.png)

1. (Opcional) Desmarque a opção **Permitir que os usuários adicionem problemas em linha** opção. Ela é selecionada por padrão.

   Ao desmarcar essa opção, os usuários não podem adicionar problemas em linha ao projeto ou às tarefas na seção Problemas.

   >[!TIP]
   >
   >Desmarque essa opção se quiser forçar os usuários a preencherem os Campos de novo problema ou os formulários personalizados associados a novos problemas. Permitir que os usuários insiram problemas em linha permite que eles ignorem os campos Novo problema e formulários personalizados ao criar problemas. Para obter informações sobre como configurar campos e formulários personalizados para novos problemas, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Ao desmarcar essa opção, os usuários com permissões para adicionar problemas ao projeto ou às tarefas podem fazer isso das seguintes maneiras:

   * Clique em Novo problema na parte superior da lista de problemas na seção Problemas do projeto ou das tarefas.
   * Quando o projeto é configurado como uma fila de solicitações, eles podem inserir uma nova solicitação na área Solicitações.

   >[!NOTE]
   >
   >Ao editar projetos em massa, essa configuração será ativada se pelo menos um projeto tiver essa opção ativada e estiver desativada se todos os projetos selecionados tiverem essa opção desativada.

   <!--drafted for bulk edit projects: the statement above needs to be corrected when the new UI for bulk edit projects is updated; not sure if we'll need to describe this at all or we can cover this in  a "Considerations" mini section inside the Editing in bulk section below- ??? -->

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Acesso {#access}

1. Comece a editar seu projeto conforme descrito acima.
1. Clique em **Access** no painel esquerdo.

   ![](assets/nwe-access-in-edit-project-box-350x262.png)

1. Especifique o seguinte **Access** informações do projeto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Quando alguém é designado a uma tarefa</strong></td> 
      <td><p>Selecionar de <strong>Exibir</strong>, <strong>Contribuir,</strong> ou <strong>Gerenciar</strong> acesso a uma tarefa. O usuário atribuído a uma tarefa recebe automaticamente esse acesso à tarefa.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Conceder acesso ao projeto também</strong></td> 
      <td><p>Selecionar de <strong>Exibir</strong>, <strong>Contribute</strong>ou <strong>Gerenciar</strong> acesso ao projeto. O usuário atribuído a uma tarefa também recebe automaticamente esse acesso ao projeto.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Quando alguém é designado a um problema</strong></td> 
      <td><p>Selecionar de <strong>Exibir</strong>, <strong>Contribuir,</strong> ou <strong>Gerenciar</strong> acesso a um problema. O usuário atribuído a um problema recebe automaticamente esse acesso ao problema. Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Conceder acesso ao projeto também</strong></td> 
      <td><p>Selecionar de <strong>Exibir</strong>, <strong>Contribute</strong>ou <strong>Gerenciar</strong> acesso ao projeto. O usuário atribuído a um problema também recebe automaticamente esse acesso ao projeto.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>Quando alguém enviar uma solicitação: conceda acesso a ela</strong></td> 
      <td><p>Selecionar de <strong>Exibir</strong>, <strong>Contribute</strong>ou <strong>Gerenciar</strong> acesso à solicitação. Quando o projeto também está em uma fila de solicitações e um usuário envia uma solicitação para o projeto, ele recebe esse acesso à solicitação que enviou. Para obter informações sobre como configurar um projeto como uma fila de solicitações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>.<br></p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><strong>As pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações</strong></td> 
      <td><p>Selecione este campo se desejar que as pessoas da mesma empresa tenham o mesmo acesso a todas as solicitações do projeto, sejam elas enviadas ou não.<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Quando é concedido acesso a alguém a este projeto: conceda-lhe acesso a ...</strong></td> 
      <td><p>Selecione as opções de acesso que você deseja que os usuários tenham no projeto, se o projeto for compartilhado com eles. Selecione as opções específicas para seu acesso se forem designadas como <strong>Visualizadores</strong>, <strong>Colaboradores</strong>ou <strong>Gerentes</strong> ao compartilhar o projeto com eles. </p><p>A variável <strong>Excluir</strong> acesso no <strong>Gerenciar</strong> o nível de permissão determina se os usuários podem excluir o próprio projeto. Usuários com <strong>Gerenciar</strong> o acesso ao projeto pode excluir tarefas e problemas dentro do projeto independentemente de essa opção estar selecionada, se eles tiverem <strong>Gerenciar</strong> permissões para as tarefas e problemas. </p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

## Editar um projeto no cabeçalho do projeto (limitado)

É possível editar uma quantidade limitada de informações no cabeçalho do projeto.

O administrador do sistema ou do grupo pode personalizar os campos exibidos no cabeçalho do projeto.

![](assets/project-header-350x18.png)

Os campos a seguir são incluídos no cabeçalho do projeto, por padrão.

* Nome do projeto
* Proprietário do projeto
* Data e hora de conclusão planejadas

   >[!NOTE]
   >
   >Você pode editar esse campo somente quando o projeto é agendado a partir da Data de conclusão. Quando o projeto é agendado a partir da Data inicial, a Workfront calcula a Data e a hora de conclusão planejadas com base na duração das tarefas.

* Condição

   >[!NOTE]
   >
   >Você pode editar esse campo somente quando o Tipo de condição do projeto é Manual. Quando o Tipo de condição é definido como Status de progresso, o Workfront calcula a condição com base no progresso das tarefas. Para obter informações, consulte [Visão geral da condição do projeto e do tipo de condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

* Status
* Tome decisões de aprovação se você estiver definido como aprovador em um processo de aprovação atual

## Editar projetos em massa

É possível editar projetos em massa e atualizar informações de todos os projetos selecionados ao mesmo tempo.


As informações que você está alterando em todos os projetos selecionados substituem as informações existentes sobre projetos individuais, exceto para o campo Gerenciador de recursos.

Adicionar um novo gerenciador de recursos ao editar projetos em massa adiciona esse gerenciador a todos os projetos selecionados. Se outros gerentes de recursos estiverem associados aos projetos selecionados, eles permanecerão nos projetos, além do adicionado por meio da edição em massa.

A edição de projetos em massa difere de acordo com o ambiente em que você escolhe atualizá-los.

### Editar projetos em massa no ambiente de produção

Para editar projetos em massa:

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Projetos**.
1. Selecione vários projetos na lista.
1. Clique em **Editar**.

   A variável **Editar Projetos** é aberta.

   ![](assets/edit-projects-in-bulk-nwe-350x303.png)

1. Especifique as informações sobre todos os projetos selecionados nas seguintes seções:

   * **Visão geral**

      Para obter informações, consulte a [Visão geral](#overview) neste artigo.

   * **Finanças**

      Para obter informações, consulte a [Finanças](#finance) neste artigo.

   * **Portfólio**

      Para obter informações, consulte a seção &quot;Associação de projeto&quot; no [Visão geral](#overview) neste artigo.

   * **Configurações**

      Para obter informações, consulte a [Configurações do projeto](#project-settings) neste artigo.

   * **Acesso**

      Para obter informações, consulte a [Access](#access) neste artigo.

   * **Formulários personalizados**

      Para obter informações, continue com a etapa 7 abaixo.

      <!--   
     <p>(NOTE:&nbsp;make sure this stays accurate)</p>   
     -->

   * **Tarefas**

      Para obter informações, consulte a [Configurações da tarefa](#task-settings) neste artigo.

   * **Problemas**

      Para obter informações, consulte a   [Configurações do problema](#issue-settings) neste artigo.

   * **Comentário**

      Para obter informações, continue com a etapa 9 abaixo.

      <!--   
     <p>(NOTE: ensure this step stays accurate)</p>   
     -->


1. (Opcional) Na área Configurações, selecione qualquer uma das seguintes opções:

   * **Recalcular Custos e Receitas**: selecione esta opção para recalcular custos e receitas em todos os projetos selecionados.
   * **Recalcular Linhas de Tempo**: selecione esta opção para recalcular as Linhas de Tempo de todos os projetos selecionados.
   * **Recalcular Scorecards**: selecione esta opção para recalcular os valores do Scorecard para todos os projetos selecionados.

   ![recalculate_cost_scorecards_etc_in_bulk_edit_for_projects.PNG](assets/recalculate-costs--scorecards--etc-in-bulk-edit-for-projects-350x225.png)

1. Clique em **Forms personalizado** para editar os formulários personalizados anexados a todos os projetos selecionados.

   Se os projetos selecionados não tiverem formulários personalizados comuns, nenhum formulário será listado nesta seção.

   É possível editar apenas os campos nos formulários anexados a todos os projetos selecionados e que você tem permissão para editar.

1. (Opcional) Na seção Forms personalizado, selecione a **Recalcular expressões personalizadas** opção para garantir que todos os Campos personalizados calculados que estão no Forms personalizado anexado aos projetos selecionados estejam atualizados.

   >[!IMPORTANT]
   >
   >Recomendamos não selecionar mais de 500 projetos de uma vez ao recalcular expressões personalizadas.

1. (Opcional) Clique em **Comentário**, em seguida, selecione a caixa Publicar uma atualização em cada projeto e especifique um comentário que deseja exibir no fluxo de atualizações do projeto no campo disponível e siga um destes procedimentos:

   * Clique em **Pessoas** ícone ![](assets/people-icon-updates-classic.png) para marcar um usuário que será notificado sobre seu comentário.
   * Clique em **Bloquear** ícone ![](assets/lock-icon-open-updates-classic.png) para restringir seu comentário somente às pessoas da sua empresa.

   Este comentário está visível para todos com acesso de Visualização ao projeto e com acesso para visualizar Notas.

1. Clique em **Salvar alterações**.

   Todas as alterações feitas agora estão visíveis em todos os projetos selecionados.

<div class="preview">

### Editar projetos em massa no ambiente de Pré-visualização

Considere o seguinte ao editar projetos em massa no ambiente de Pré-visualização:

* Quando você seleciona projetos com valores diferentes para o mesmo campo, o campo exibe um indicador &quot;Vários valores&quot; na caixa Editar projetos. Os campos que são caixas de seleção, botões de opção e alternadores têm um indicador de &quot;Vários valores&quot; ao lado deles.

   ![](assets/multiple-values-indicator-dates-bulk-edit-projects.png)

* Além do indicador &quot;Valores múltiplos&quot;, quando as opções escolhidas são diferentes em pelo menos um dos projetos selecionados, os campos com várias opções são exibidos de uma das seguintes maneiras:

   * Os campos de caixa de seleção têm uma linha em vez de uma caixa de seleção para a opção marcada para alguns, mas não para todos os projetos selecionados.

      ![](assets/multiple-values-indicator-check-boxes-bulk-edit-projects.png)

   * Os campos do tipo alternância são exibidos esmaecidos, com a opção no meio ativada para alguns projetos selecionados, mas não para todos.

   ![](assets/multiple-values-highlighted-bulk-edit-projects.png)

   * Os campos do tipo botão de opção que têm algumas opções selecionadas, mas não todas, exibem todos os botões de opção como vazios.

      ![](assets/multiple-values-indicator-radio-buttons-bulk-edit-projects.png)


* Ao atualizar uma opção em um campo de várias opções (como um campo exibido como um conjunto de alternâncias ou caixas de seleção), todas as outras opções devem corresponder entre os projetos selecionados.

   >[!IMPORTANT]
   >
   >Por exemplo, você pode ter um campo de caixa de seleção com três caixas de seleção (Opção 1, Opção 2 e Opção 3) e a Opção 1 está desmarcada para todos os projetos, e as Opções 2 e 3 estão marcadas para alguns e desmarcadas para outros projetos selecionados. Se quiser marcar a Opção 1 para todos os projetos, você também deverá fazer com que as Opções 2 e 3 correspondam a todos os projetos selecionados antes de salvar suas alterações. Portanto, você deve selecioná-las ou desmarcá-las para que possam corresponder a todos os projetos selecionados. Se não alterar nenhuma das opções, você poderá salvar o campo como está e os projetos manterão sua seleção atual para todas as opções.

* Quando você seleciona vários projetos que pertencem a grupos diferentes, os status exibidos no campo Status são status de nível do sistema e não de nível de grupo.

Para editar projetos no ambiente de Pré-visualização:

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique em **Projetos**.
1. Selecione vários projetos na lista.
1. Clique em **Editar** ícone ![](assets/edit-icon.png) no topo da lista.
A variável **Editar Projetos** é aberta.

   ![](assets/edit-projects-in-bulk-modal-unshimmed.png)

Dependendo de como o administrador do Workfront ou do Administrador de grupo modificou o Modelo de layout, as áreas no painel esquerdo da caixa Editar projeto ou quaisquer campos listados nessas áreas podem ser reorganizados ou não serão exibidos. Para obter informações, consulte [Personalizar a exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Clique em **Visão geral** para editar informações gerais sobre os projetos selecionados.  Para obter mais informações sobre a edição da área Visão geral, consulte a seção [Visão geral](#overview) neste artigo.

   >[!TIP]
   >
   >Os campos editados são exibidos com um plano de fundo roxo-claro.

1. Clique em **Forms personalizado** para editar, adicionar ou substituir formulários personalizados associados aos projetos selecionados.

   Os formulários personalizados anexados a todos os projetos selecionados são exibidos no **Formulários personalizados em comum** subseção no **Forms personalizado** área.

   ![](assets/custom-forms-in-common-unshimmed.png)

   >[!TIP]
   >
   >   Os nomes dos formulários comuns a todos os projetos selecionados são exibidos no painel esquerdo da caixa Editar projetos.

1. Comece digitando o nome de um formulário personalizado no **Adicionar formulário personalizado** campo.


   ![](assets/forms-already-attached-indication-in-bulk-editing-projects-unshimmed.png)

   Os formulários personalizados já anexados aos projetos selecionados são exibidos no **Formulários anexados** subseção no **Adicionar formulário personalizado** campo.

   Outros formulários personalizados que podem ser associados a projetos, mas não estão anexados a nenhum dos projetos selecionados, são exibidos no **Forms a adicionar** subseção no **Adicionar formulário personalizado** campo.

1. Clique para selecionar o formulário personalizado adicional na **Adicionar formulário personalizado** ou **Forms a adicionar** subseções quando ele é exibido na lista.

   Quando um formulário personalizado já estiver anexado a alguns dos projetos selecionados, há uma indicação ao lado do nome do formulário de quantos projetos já têm o formulário selecionado, ao adicionar um formulário.

1. (Opcional) Clique no link **x** ícone à direita do nome de um formulário personalizado e clique em **Remover** para removê-lo de todos os projetos selecionados.

   >[!CAUTION]
   >
   >A remoção de formulários personalizados faz com que todas as informações de campo personalizado existentes nos formulários sejam perdidas. Isso não pode ser recuperado.

   Para obter mais informações sobre edição de formulários personalizados, consulte a seção [Forms personalizado](#custom-forms) neste artigo.

1. Clique em **Finanças** para editar informações financeiras de todos os projetos selecionados.
Para obter mais informações sobre a edição da área Finanças, consulte a seção [Finanças](#finance) neste artigo.
1. Clique em **Configurações do projeto** para editar as configurações de todos os projetos selecionados.
Para obter mais informações sobre a edição da área Configurações do projeto, consulte a seção [Configurações do projeto](#project-settings) neste artigo.
1. Clique em **Configurações da tarefa** para editar as configurações da tarefa de todos os projetos selecionados.
Para obter mais informações sobre a edição da área Configurações da tarefa, consulte a seção [Configurações da tarefa](#task-settings) neste artigo.
1. Clique em **Configurações do problema** para editar as configurações de problema de todos os projetos selecionados.
Para obter mais informações sobre como editar a área Configurações de problema, consulte a seção [Configurações do problema](#issue-settings) neste artigo.
1. Clique em **Access** para editar as configurações de acesso de todos os projetos selecionados.
Para obter mais informações sobre como editar a área de Acesso, consulte a seção [Access](#access) neste artigo.
1. (Opcional) Para remover qualquer informação adicionada na caixa Editar projetos, passe o mouse sobre um campo editado, em seguida, clique no **x** ícone de descartar no canto superior direito do campo.

   ![](assets/discard-icon-for-field-edit-projects-in-bulk-unshimmed.png)

1. (Opcional) Clique em **Cancelar** na parte inferior do **Editar projetos** para remover todas as alterações feitas em todos os projetos.
1. Clique em **Salvar**.

</div>

