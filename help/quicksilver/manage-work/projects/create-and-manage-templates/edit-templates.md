---
product-area: templates
navigation-topic: templates-navigation-topic
title: Editar modelos de projeto
description: Você pode editar modelos de projeto para refletir as alterações nos processos e configurações de projetos futuros. É possível editar um modelo por vez ou vários modelos em massa.
author: Alina
feature: Work Management
exl-id: da0fca31-6a50-4862-ad9a-a453ef968773
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '5655'
ht-degree: 2%

---

# Editar modelos de projeto

<!-- Audited: 7/2025 -->

<!--The Resource Pools part also duplicates in the "Working with Resource Pools" article-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 

-->


Você pode editar modelos de projeto para refletir as alterações nos processos e configurações de projetos futuros.

Depois de atualizar e salvar as alterações em um modelo, as novas alterações ficam visíveis em novos projetos quando os projetos são criados usando o modelo.

As alterações feitas no modelo não refletem nos projetos que estão usando esse modelo no momento.

É possível editar um modelo por vez ou em massa.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças da Adobe Workfront*</td> 
   <td>
      <p>Novo: Padrão</p>
      <p>Ou</p>
      <p>Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso</td> 
   <td> <p>Editar acesso a modelos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> 
    <ul> 
     <li> <p>Contribuir com permissões para um modelo para editá-lo na guia Detalhes do modelo</p> </li> 
     <li> <p>Gerenciar permissões de um modelo para editá-lo na caixa Editar modelo</p> </li> 
   </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação da Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar um modelo {#edit-a-template}

1. Vá para o template que deseja editar.
1. (Condicional) Para editar informações limitadas sobre o modelo, clique em **Detalhes do modelo** no painel esquerdo e vá para as áreas listadas no painel esquerdo para editar as informações de cada área.
1. Para editar informações na seção Detalhes, clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) e selecione uma das áreas abaixo ou clique em **Editar tudo** para editar informações em todas as áreas:

   * Visão geral
   * Formulários personalizados

   Os nomes dos formulários de alfândega são exibidos somente se houver formulários personalizados anexados ao objeto.

   * Finanças

   >[!TIP]
   >
   >Para obter informações sobre todos os campos exibidos na área Detalhes, continue editando todos os campos usando a caixa Editar modelo abaixo.

1. (Condicional) Para editar todas as informações sobre o modelo, clique no ícone **Mais** do menu ![Mais](assets/qs-more-icon-on-an-object.png) ao lado do nome do modelo e clique em **Editar**.

   A caixa **Editar Modelo** é aberta. As seções nesta caixa contêm os campos disponíveis na seção Detalhes do Modelo, bem como campos adicionais.

1. Considere a edição de informações em qualquer uma das seguintes seções:

   * [Nome do Modelo](#template-name)
   * [Visão geral](#overview-preview)
   * [Finanças](#finance-preview)
   * [Formulários personalizados](#custom-forms-preview)
   * [Configurações do modelo](#template-settings)
   * [Configurações de tarefas](#task-settings)
   * [Configurações de Problema](#issue-settings)
   * [Access](#access-preview)
   * [Comentário](#comment)
   <!--* [Linked folders](#linked-folders-conditional-availability) -->

### Nome do Modelo{#template-name}

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Nome do Modelo**.
1. Atualize ou substitua o nome do template.
1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar

   Ou

   Clique em **Salvar**.

### Visão geral {#overview-preview}

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Visão Geral**.

   ![Editar seção de Visão Geral da caixa de modelo](assets/edit-template-box-overview-section.png)

1. Atualize os seguintes campos:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
         <tr> 
         <td role="rowheader"><strong>Descrição</strong></td> 
         <td>Adicione mais informações sobre o template.</td> 
       </tr> 
         <tr> 
         <td role="rowheader"><strong>Prioridade</strong></td> 
         <td><p>Este é apenas um sinalizador visual para você, que permite priorizar seus projetos futuros. Selecione entre as seguintes opções:</p> 
         <ul> 
         <li><p><strong>Nenhum(a)</strong></p></li> 
         <li><p><strong>Baixa</strong></p></li> 
         <li><p><strong>Normal</strong></p></li> 
         <li><p><strong>Alta</strong></p></li> 
         <li><p><strong>Urgente</strong></p></li> 
         </ul><p><p>Dependendo das Preferências do projeto selecionadas pelo administrador do Workfront, os nomes das prioridades podem ser diferentes para você. Para obter mais informações sobre como editar prioridades, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Criar e personalizar prioridades</a>.</p></p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>URL</strong></td> 
         <td>Especifique um link da Web relacionado às informações sobre este modelo.</td> 
       </tr>
   <tr> 
      <td role="rowheader"><strong>Está ativo</strong></td> 
      <td><p>Ative essa opção se desejar que o template esteja ativo. Outros usuários podem encontrar esse modelo e anexá-lo a projetos ao criar projetos. Desative a opção se desejar desativar modelos que não são mais usados. Modelos desativados não podem ser anexados a projetos. Isso é ativado por padrão. </p><p><b>DICA</b></p>

   <p>Você pode desativar um modelo no cabeçalho do modelo conforme descrito na seção "Ativar ou desativar um modelo" neste artigo.</p></td> 
     </tr>

<tr> 
<td role="rowheader"><strong>Tipo de condição</strong></td> 
   <td><p>Selecione entre os seguintes Tipos de Condição:</p> 
   <ul> 
   <li><strong>Manual:</strong> o proprietário do projeto define a Condição do projeto manualmente. <strong></strong></li> 
   <li><strong>Status do Progresso:</strong> o Workfront define automaticamente a Condição do projeto futuro com base no Status do Progresso das tarefas no Caminho Crítico. Para obter mais informações sobre como entender o Status de Progresso, consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do Status de Progresso da Tarefa</a>.</li> 
   </ul>
   </td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Modo de cronograma</strong></td> 
   <td><p>Especifique se o projeto usando este modelo está agendado a partir da <strong>Data de Início</strong> ou da <strong>Data de Conclusão</strong>. Esta seleção determina as datas planejadas das tarefas futuras no projeto usando este modelo. </p><p>Selecione entre as seguintes opções: </p> 
   <ul> 
   <li><p><strong>Agendar a partir da data de início</strong>: a data de início do modelo é, na verdade, o dia de início. Ao agendar um modelo a partir da Data inicial, o Adobe Workfront calcula o Dia de conclusão do modelo com base na Duração de todas as tarefas do modelo. O dia de início do modelo se torna a Data de início planejada do projeto futuro.</p></li> 
   <li><p><strong>Agendamento a partir da data de conclusão</strong>: a data de conclusão do modelo é, na verdade, o dia de conclusão. Ao programar um modelo a partir da Data de conclusão, o Workfront calcula o Dia de início do modelo com base na Duração de todas as tarefas do modelo. O Dia de conclusão do modelo se torna a Data de conclusão planejada do projeto futuro. </p></li> 
   </ul><p>Para obter mais informações sobre os Dias de Início e Término das tarefas do modelo, consulte <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Visão Geral dos Dias de Início e Término em um modelo</a>. </p><p>A configuração Agendar de dos modelos é semelhante à dos projetos. O administrador do Workfront seleciona a configuração padrão Agendar de para os projetos do seu sistema. Para obter informações sobre como definir padrões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto do sistema</a>.</p></td> 
   </tr>

<tr> 
   <td role="rowheader"><strong>Portfólio</strong></td> 
   <td><p>Especifique uma Portfolio para os projetos criados a partir deste modelo. Você deve criar um Portfolio primeiro, antes que ele apareça na lista suspensa. </p><p>Somente portfólios ativos são exibidos na lista. Para obter mais informações sobre como criar portfólios, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Criar um portfólio </a>.</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Programa</strong></td> 
   <td><p>Se você selecionou um Portfolio para o modelo, especifique um <strong>Programa</strong> para o projeto futuro. Alguns portfólios podem não ter programas. Você deve criar um Programa primeiro, antes que ele apareça nesta lista suspensa. Somente programas ativos são exibidos na lista.</p><p>Para obter mais informações sobre como criar programas, consulte <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Criar um programa</a>.</p></td> 
   </tr>  
   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader"><strong>Grupo</strong></td> 
   <td><p>Na lista suspensa, selecione o grupo que deseja associar aos projetos criados a partir do modelo. Pode ser um grupo de qualquer nível. </p><p>Você pode verificar se está selecionando o grupo correto passando o cursor do mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> <p><b>NOTAS</b>

<ul> 
   <li><p>Na área Projetos da página de um grupo, quando alguém cria um projeto usando um modelo que não tem um grupo selecionado, o sistema associa o grupo aberto no momento ao projeto.</p><p>Isso é diferente de outras áreas onde o sistema associa o Grupo inicial de um usuário ao projeto quando o usuário cria o projeto usando um modelo que não tem um grupo selecionado.</p></li> 
   <li><p>Se um usuário selecionar um modelo que tenha um grupo selecionado ao criar um projeto ou ao converter uma tarefa ou problema em um projeto, ele poderá escolher um grupo diferente para o projeto.</p></li> 
   <li>Embora esse campo esteja disponível em modelos somente na nova experiência do Adobe Workfront, você pode vê-lo em listas e relatórios lá e no Adobe Workfront Classic. </li> 
   </ul> </p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Empresa</strong></td> 
   <td><p>Especifique a Empresa que deseja associar ao modelo. Somente empresas ativas são exibidas na lista.</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Proprietário do modelo</strong></td> 
   <td><p>O usuário designado como Proprietário do Modelo deve ser um usuário ativo do Workfront. </p><p>Considere o seguinte sobre o usuário designado como o Proprietário do modelo: </p> 
   <ul> 
   <li>Eles recebem automaticamente permissões Gerenciar para o modelo. </li> 
   <li>Eles são adicionados à equipe do projeto e recebem automaticamente permissões de gerenciamento para o projeto criado a partir do modelo. </li> 
   <li>Eles se tornam o Proprietário do projeto quando o projeto é criado a partir desse modelo. </li> 
   <li> Se o usuário designado como Proprietário do modelo tiver acesso limitado aos modelos ou projetos por meio de seu nível de acesso, as permissões de Gerenciamento no modelo e nos projetos serão limitadas. Por exemplo, se eles tiverem somente o acesso de Visualização para modelos ou projetos em seu nível de acesso, eles receberão automaticamente permissões de Visualização no modelo e no projeto quando forem designados como o Proprietário do modelo.</li>
   </ul></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Patrocinador do modelo</strong></td> 
   <td><p>O usuário especificado nesse campo se torna o Patrocinador do projeto quando o modelo é adicionado ao projeto. Este usuário é adicionado à equipe do projeto e recebe automaticamente permissões de exibição para o projeto. O usuário designado como Patrocinador do modelo deve ser um usuário ativo do Workfront. </p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Gerenciador de Recursos</strong></td> 
   <td><p>Os usuários especificados recebem automaticamente permissões de gerenciamento para os projetos futuros e podem atribuir recursos às tarefas e problemas dos projetos. Você pode especificar mais de um Gerenciador de recursos. </p></td> 
   </tr> 
</table>

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Finanças {#finance-preview}

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Finanças**.

   ![Editar seção Financeira da caixa de modelo](assets/edit-template-box-finance-section.png)

1. Atualize os seguintes campos:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
         <tr> 
         <td role="rowheader"><strong>Descrição</strong></td> 
         <td>Adicione mais informações sobre o template.</td> 
       </tr> 
         <tr> 
         <td role="rowheader"><strong>Prioridade</strong></td> 
         <td><p>Este é apenas um sinalizador visual para você, que permite priorizar seus projetos futuros. Selecione entre as seguintes opções:</p> 
         <ul> 
         <li><p><strong>Nenhum(a)</strong></p></li> 
         <li><p><strong>Baixa</strong></p></li> 
         <li><p><strong>Normal</strong></p></li> 
         <li><p><strong>Alta</strong></p></li> 
         <li><p><strong>Urgente</strong></p></li> 
         </ul><p><p>Dependendo das Preferências do projeto selecionadas pelo administrador do Workfront, os nomes das prioridades podem ser diferentes para você. Para obter mais informações sobre como editar prioridades, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Criar e personalizar prioridades</a>.</p></p></td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>URL</strong></td> 
         <td>Especifique um link da Web relacionado às informações sobre este modelo.</td> 
       </tr>
   <tr> 
      <td role="rowheader"><strong>Está ativo</strong></td> 
      <td><p>Ative essa opção se desejar que o template esteja ativo. Outros usuários podem encontrar esse modelo e anexá-lo a projetos ao criar projetos. Desative a opção se desejar desativar modelos que não são mais usados. Modelos desativados não podem ser anexados a projetos. Isso é ativado por padrão. </p><p><b>DICA</b></p>

   <p>Você pode desativar um modelo no cabeçalho do modelo conforme descrito na seção "Ativar ou desativar um modelo" neste artigo.</p></td> 
     </tr>

<tr> 
<td role="rowheader"><strong>Tipo de condição</strong></td> 
   <td><p>Selecione entre os seguintes Tipos de Condição:</p> 
   <ul> 
   <li><strong>Manual:</strong> o proprietário do projeto define a Condição do projeto manualmente. <strong></strong></li> 
   <li><strong>Status do Progresso:</strong> o Workfront define automaticamente a Condição do projeto futuro com base no Status do Progresso das tarefas no Caminho Crítico. Para obter mais informações sobre como entender o Status de Progresso, consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do Status de Progresso da Tarefa</a>.</li> 
   </ul>
   </td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Modo de cronograma</strong></td> 
   <td><p>Especifique se o projeto usando este modelo está agendado a partir da <strong>Data de Início</strong> ou da <strong>Data de Conclusão</strong>. Esta seleção determina as datas planejadas das tarefas futuras no projeto usando este modelo. </p><p>Selecione entre as seguintes opções: </p> 
   <ul> 
   <li><p><strong>Agendar a partir da data de início</strong>: a data de início do modelo é, na verdade, o dia de início. Ao agendar um modelo a partir da Data inicial, o Adobe Workfront calcula o Dia de conclusão do modelo com base na Duração de todas as tarefas do modelo. O dia de início do modelo se torna a Data de início planejada do projeto futuro.</p></li> 
   <li><p><strong>Agendamento a partir da data de conclusão</strong>: a data de conclusão do modelo é, na verdade, o dia de conclusão. Ao programar um modelo a partir da Data de conclusão, o Workfront calcula o Dia de início do modelo com base na Duração de todas as tarefas do modelo. O Dia de conclusão do modelo se torna a Data de conclusão planejada do projeto futuro. </p></li> 
   </ul><p>Para obter mais informações sobre os Dias de Início e Término das tarefas do modelo, consulte <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Visão Geral dos Dias de Início e Término em um modelo</a>. </p><p>A configuração Agendar de dos modelos é semelhante à dos projetos. O administrador do Workfront seleciona a configuração padrão Agendar de para os projetos do seu sistema. Para obter informações sobre como definir padrões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto do sistema</a>.</p></td> 
   </tr>

<tr> 
   <td role="rowheader"><strong>Portfólio</strong></td> 
   <td><p>Especifique uma Portfolio para os projetos criados a partir deste modelo. Você deve criar um Portfolio primeiro, antes que ele apareça na lista suspensa. </p><p>Somente portfólios ativos são exibidos na lista. Para obter mais informações sobre como criar portfólios, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Criar um portfólio </a>.</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Programa</strong></td> 
   <td><p>Se você selecionou um Portfolio para o modelo, especifique um <strong>Programa</strong> para o projeto futuro. Alguns portfólios podem não ter programas. Você deve criar um Programa primeiro, antes que ele apareça nesta lista suspensa. Somente programas ativos são exibidos na lista.</p><p>Para obter mais informações sobre como criar programas, consulte <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Criar um programa</a>.</p></td> 
   </tr>  
   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader"><strong>Grupo</strong></td> 
   <td><p>Na lista suspensa, selecione o grupo que deseja associar aos projetos criados a partir do modelo. Pode ser um grupo de qualquer nível. </p><p>Você pode verificar se está selecionando o grupo correto passando o cursor do mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> <p><b>NOTAS</b>

<ul> 
   <li><p>Na área Projetos da página de um grupo, quando alguém cria um projeto usando um modelo que não tem um grupo selecionado, o sistema associa o grupo aberto no momento ao projeto.</p><p>Isso é diferente de outras áreas onde o sistema associa o Grupo inicial de um usuário ao projeto quando o usuário cria o projeto usando um modelo que não tem um grupo selecionado.</p></li> 
   <li><p>Se um usuário selecionar um modelo que tenha um grupo selecionado ao criar um projeto ou ao converter uma tarefa ou problema em um projeto, ele poderá escolher um grupo diferente para o projeto.</p></li> 
   <li>Embora esse campo esteja disponível em modelos somente na nova experiência do Adobe Workfront, você pode vê-lo em listas e relatórios lá e no Adobe Workfront Classic. </li> 
   </ul> </p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Empresa</strong></td> 
   <td><p>Especifique a Empresa que deseja associar ao modelo. Somente empresas ativas são exibidas na lista.</p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Proprietário do modelo</strong></td> 
   <td><p>O usuário designado como Proprietário do Modelo deve ser um usuário ativo do Workfront. </p><p>Considere o seguinte sobre o usuário designado como o Proprietário do modelo: </p> 
   <ul> 
   <li>Eles recebem automaticamente permissões Gerenciar para o modelo. </li> 
   <li>Eles são adicionados à equipe do projeto e recebem automaticamente permissões de gerenciamento para o projeto criado a partir do modelo. </li> 
   <li>Eles se tornam o Proprietário do projeto quando o projeto é criado a partir desse modelo. </li> 
   <li> Se o usuário designado como Proprietário do modelo tiver acesso limitado aos modelos ou projetos por meio de seu nível de acesso, as permissões de Gerenciamento no modelo e nos projetos serão limitadas. Por exemplo, se eles tiverem somente o acesso de Visualização para modelos ou projetos em seu nível de acesso, eles receberão automaticamente permissões de Visualização no modelo e no projeto quando forem designados como o Proprietário do modelo.</li>
   </ul></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Patrocinador do modelo</strong></td> 
   <td><p>O usuário especificado nesse campo se torna o Patrocinador do projeto quando o modelo é adicionado ao projeto. Este usuário é adicionado à equipe do projeto e recebe automaticamente permissões de exibição para o projeto. O usuário designado como Patrocinador do modelo deve ser um usuário ativo do Workfront. </p></td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Gerenciador de Recursos</strong></td> 
   <td><p>Os usuários especificados recebem automaticamente permissões de gerenciamento para os projetos futuros e podem atribuir recursos às tarefas e problemas dos projetos. Você pode especificar mais de um Gerenciador de recursos. </p></td> 
   </tr> 
</table>

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Formulários personalizados {#custom-forms-preview}

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Forms Personalizado**.

   ![Editar seção Forms Personalizada da caixa de modelo](assets/edit-template-box-custom-forms-section.png)

   Os nomes dos formulários personalizados já anexados ao modelo são exibidos no painel esquerdo.

1. Clique dentro do campo **Adicionar formulário personalizado** e selecione o(s) formulário(s) personalizado(s) que deseja associar ao modelo. Você deve criar os formulários personalizados antes que eles estejam disponíveis para seleção neste campo.

   Somente formulários personalizados ativos são exibidos na lista. Para obter mais informações sobre a criação de formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   Você pode adicionar até dez formulários personalizados a um modelo.

   Os formulários serão adicionados ao projeto criado a partir deste modelo.

1. (Opcional) Atualize as informações em qualquer um dos campos nos formulários personalizados. As informações serão transferidas para os projetos que serão criados a partir do modelo.

1. (Opcional) Clique no ícone **x** à direita de um nome de formulário personalizado e clique em **Remover** para removê-lo do modelo.

1. (Opcional) Continue editando a seção a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Configurações de modelo {#template-settings}

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Configurações do Projeto**.

   ![Editar seção de Configurações de Modelo da caixa de modelo](assets/edit-template-box-project-settings-section.png)

1. Atualize os seguintes campos:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
       <td role="rowheader"><strong>Caminho de Etapas</strong> </td> 
       <td> <p>Selecione um Caminho de Etapas para o modelo. Somente os caminhos de etapas ativos são exibidos na lista.<br>Para obter mais informações sobre Caminhos de Etapas, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Criar um caminho de etapas</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Modo de conclusão</strong> </td> 
       <td> <p>Controla como o projeto futuro será marcado como Concluído. <br>Selecione entre as seguintes opções:</p> 
       <ul> 
       <li> <p><strong>Automático</strong>: o projeto é marcado como Concluído quando todas as tarefas e problemas são concluídos.</p> </li> 
       <li> <p><strong>Manual</strong>: você precisa selecionar manualmente o status Concluído para o projeto quando todas as tarefas e problemas forem concluídos. </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Modo de conclusão do resumo</strong> </td> 
       <td> <p>Controla como as tarefas pai no projeto futuro são marcadas como Concluídas. <br>Selecione entre as seguintes opções:</p> 
       <ul> 
       <li> <p><strong>Automático</strong>: as tarefas pai estão marcadas como Concluídas e atualizam sua porcentagem concluída automaticamente, à medida que as tarefas filho são concluídas e a porcentagem concluída dos filhos é atualizada. </p> </li> 
       <li> <p><strong>Manual</strong>: você precisa atualizar manualmente a porcentagem concluída e o status das tarefas pai, independentemente de quais alterações são feitas nas tarefas filho. </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Tipo de Atualização</strong> </td> 
       <td> <p>Controla quando as alterações feitas na linha do tempo do projeto futuro são salvas no projeto. </p> 
       <b>EXEMPLO </b> 
       <p>As seguintes alterações no projeto acionam uma atualização na linha do tempo do projeto:</p> 
       <ul> 
       <li> <p>atualizar as datas das tarefas</p> </li> 
       <li> <p>alterar relacionamentos de predecessores<br></p> </li> 
       <li> <p>alterar relações pai-filho</p> </li> 
       <li> <p>adicionar ou remover atribuições além de alterar a restrição ou o tipo de duração da tarefa.</p> </li> 
       </ul> 
       </div> <p>Selecione entre as seguintes opções:<br></p> 
       <ul> 
       <li> <p><strong>Automático e Mediante alteração</strong> (Configuração padrão): a linha de tempo do projeto futuro é atualizada sempre que ocorre uma alteração no projeto ou em outro projeto do qual a linha de tempo depende (Mediante alteração). A linha do tempo do projeto também é atualizada todas as noites (Automático).<br>Esta é a configuração recomendada para este campo porque ela garante que a linha de tempo do projeto esteja sempre atualizada.<br>Quando você executa uma ação em uma tarefa ou projeto que dispara um recálculo de linha de tempo, todas as datas disponíveis são exibidas imediatamente, permitindo que você continue trabalhando. Em projetos com mais de 100 tarefas, as datas que exigem recálculos mais longos são exibidas brevemente como um ponto de interrogação (entre 1 e 5 segundos ou até um minuto para projetos grandes). Isso indica que o recálculo ainda não foi concluído e as datas estão sujeitas a alterações.<br></p> </li> 
       </ul> 
       <ul> 
       <li> <p><strong>Somente Alteração</strong>: a linha de tempo do projeto é atualizada sempre que ocorre uma alteração no projeto ou em outro projeto do qual a linha de tempo depende. Você pode selecionar essa opção se alterações raramente ocorrerem no projeto ou em outros projetos dos quais a linha do tempo depende.<br></p> </li> 
       </ul> 
       <ul> 
       <li> <p><strong>Somente Automático</strong>: a linha do tempo do projeto é atualizada todas as noites; ela não é atualizada imediatamente após as alterações serem feitas.<br>Talvez você queira selecionar esta opção se muitas alterações ocorrerem todos os dias no projeto ou em outros projetos dos quais a linha do tempo depende. No entanto, lembre-se de que você escolheu essa configuração, pois o projeto não será atualizado ao mesmo tempo em que as alterações são feitas.<br></p> </li> 
       </ul> 
       <ul> 
       <li> <p><strong>Somente Manual</strong>: a linha de tempo do projeto é atualizada apenas quando você seleciona a opção para Recalcular Linhas de Tempo, conforme descrito em <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalcular linhas de tempo do projeto</a>.<br></p> </li> 
       </ul> <p>Você pode selecionar essa opção se estiver fazendo muitas alterações ao projeto de uma vez e quiser que o recálculo da linha do tempo ocorra após todas as alterações terem sido feitas (em vez de após cada alteração individual).</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Agendar</strong> </td> 
       <td> <p>Selecione um agendamento para o seu modelo. Isso se tornará o agendamento do projeto criado a partir desse modelo. Deve ser o mesmo agendamento atribuído à maioria das pessoas que estão trabalhando no projeto. Você deve criar um agendamento antes de atribuí-lo a um modelo.<br>Para obter mais informações sobre como criar agendas, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar uma agenda</a>. <br>Se você não tiver criado agendamentos personalizados em seu sistema, o Agendamento padrão será selecionado. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Tempo de folga do usuário</strong> </td> 
       <td> <p>Determina se o tempo de folga do Destinatário principal de uma tarefa ajusta as datas planejadas da tarefa. Quando você anexa o modelo a um projeto existente e o modelo tem uma configuração para esse campo diferente do projeto, a configuração no projeto permanece inalterada. A opção padrão para essa configuração para um novo modelo é a mesma que a preferência de projeto no nível do sistema. </p> <p>Para obter informações sobre as preferências do projeto no nível do Sistema, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências do projeto do sistema</a>. </p> <p>Para obter informações sobre como essa configuração afeta as datas da tarefa em um projeto, consulte <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar projetos</a>.<br>Selecione entre as seguintes opções:<br></p> 
       <ul> 
       <li> <p><strong>Considere o tempo de folga do usuário nas durações da tarefa</strong>: ao selecionar essa opção, as datas planejadas das tarefas no projeto criado a partir desse modelo se ajustam de acordo com o tempo de folga do Atribuidor principal da tarefa, se o tempo de folga ocorrer durante a duração da tarefa. </p> </li> 
       <li> <p><strong>Ignorar o tempo de folga do usuário nas durações da tarefa</strong>: ao selecionar esta opção, as datas planejadas das tarefas no projeto criado a partir deste modelo permanecem como planejadas originalmente, mesmo que o Principal Responsável da tarefa tenha um tempo de folga durante a duração da tarefa. </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Modo de Nivelamento de Recursos</strong> </td> 
       <td> <p>Selecione entre as seguintes opções:<br></p> 
       <ul> 
       <li> <p><strong>Manual</strong>: você deve nivelar manualmente seus recursos no projeto criado a partir deste modelo (esta é a configuração padrão)</p> </li> 
       <li> <p><strong>Automático:</strong> o Workfront nivela os recursos no projeto futuro. <br>Para obter mais informações sobre o Nivelamento de Recursos, consulte <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Nivelar Recursos no Gráfico de Gantt </a>. </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Risco</strong> </td> 
       <td> <p>Defina o nível de risco dos projetos criados a partir deste modelo. O risco é apenas um indicador do quão arriscado um projeto pode ser. Você pode priorizar a execução de seus projetos com base no nível de risco.<br>Considere selecionar entre os seguintes níveis de risco:<br></p> 
       <ul> 
       <li> <p><strong>Muito Baixo</strong> </p> </li> 
       <li> <p><strong>Baixo</strong> </p> </li> 
       <li> <p><strong>Medium</strong> </p> </li> 
       <li> <p><strong>Alta</strong> </p> </li> 
       <li> <p><strong>Muito Alto</strong> </p> </li> 
       </ul> </td> 
       </tr> 
       <tr> 
       <td role="rowheader"><strong>Conjuntos de Recursos</strong> </td> 
       <td> <p>Especifique os conjuntos de recursos associados ao modelo. Conjuntos de recursos são coleções de usuários que são necessárias ao mesmo tempo para a conclusão de um projeto. Para obter mais informações sobre pools de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos pools de recursos </a>.</p> <p> <p><b>Nota</b>

       Quando você edita modelos em massa, somente os conjuntos de recursos que são comuns a todos os modelos selecionados aparecem neste campo. Se os modelos selecionados não tiverem conjuntos de recursos compartilhados, esse campo estará vazio. Os conjuntos de recursos especificados aqui substituirão os conjuntos de recursos individuais dos modelos.&lt;/p> &lt;/p> &lt;/td>
       &lt;/tr>
   
   <tr> 
      <td role="rowheader"><strong>Exigir que o tempo seja aprovado para este projeto</strong></td>

   <td><p>Selecione esta opção para exigir que o futuro Proprietário do projeto criado a partir deste modelo aprove o tempo registrado no projeto.</p> 
   <p>Se você estiver usando Registros de cobrança e selecionar essa opção, somente as horas aprovadas no projeto aparecerão como horas faturáveis disponíveis para os Registros de cobrança. </p>
   <p>A aprovação de horas no projeto é independente da aprovação de folhas de horas. Para obter mais informações sobre a exigência de tempo para aprovação em um projeto, consulte <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Exigir tempo para aprovação em um projeto</a>.</p>
   </td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Filtrar tipo de horas</strong> </td> 
   <td> <p>Considere o seguinte:</p> <p>Selecione <strong>Não</strong> para disponibilizar todos os tipos de horas específicos do projeto no projeto futuro. (Esta é a seleção padrão)</p> <p>Ou</p> <p>Selecione <strong>Sim</strong> para disponibilizar no futuro projeto apenas um subconjunto dos tipos de horas específicos do projeto e, em seguida, selecione os tipos de horas que deseja disponibilizar. (Mantenha pressionada a tecla Shift para selecionar vários tipos de horas.)</p> <p>Se você selecionar essa opção, somente os tipos de horas selecionados serão disponibilizados para seleção ao registrar horas no projeto (ou em tarefas e problemas no projeto). Você deve selecionar pelo menos um tipo de hora; se você selecionar essa opção e não selecionar nenhum tipo de hora, todos os tipos de hora serão disponibilizados no projeto.</p> <p>As mesmas seleções de tipo de hora devem ser feitas no nível do usuário individual para que o usuário veja essas opções de tipo de hora no projeto. </p> <p>Para obter mais informações sobre como definir tipos de horas no nível do usuário, consulte a seção <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Tempo do log</a> em <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Tempo do log</a>.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader"><strong>Notificação de Lembrete</strong> </td> 
   <td>Selecione a Notificação de lembrete que deve ser associada ao projeto futuro. Você deve configurar Notificações de lembrete para que os projetos deste campo apareçam durante a edição de um modelo. <br>Para obter mais informações sobre como configurar Notificações de Lembrete, consulte <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Configurar notificações de lembrete</a>.</td> 
   </tr>
   <tr> 
   <td role="rowheader"><strong>Processo de aprovação</strong> </td> 
   <td> <p>Selecione o processo de aprovação que deseja associar ao modelo. O administrador do Workfront ou um usuário com acesso administrativo aos Processos de aprovação deve definir processos de aprovação de projeto no nível do sistema ou no nível do grupo antes de ser associado a um modelo. Para obter mais informações sobre como criar processos de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Criar um processo de aprovação para itens de trabalho</a>.</p> <p>Considere o seguinte ao adicionar processos de aprovação: </p> 
   <ul> 
   <li>Somente os processos de aprovação ativos são exibidos na lista. </li> 
   <li> <p>Os processos de aprovação específicos do grupo e de todo o sistema são exibidos na lista. Um processo de aprovação associado a um grupo diferente daquele do modelo não é exibido na lista.</p> <p><b>IMPORTANTE</b>

   Se o grupo associado ao modelo for alterado, o processo de aprovação específico do grupo se tornará um processo de aprovação de uso único. Para obter mais informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos</a>. </p> </li>
   <li> <p>Se você adicionou um processo de aprovação de uso único, ele é exibido como "Personalizado" neste campo. Para obter informações, consulte <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associar um processo de aprovação novo ou existente ao trabalho</a>. </p> 
      </li> 
      <li> <p>Quando você edita modelos em massa, os seguintes cenários existem:</p> 
      <ul> 
         <li> <p>Quando você seleciona modelos do mesmo grupo, os processos de aprovação de nível de sistema e de grupo são exibidos nesse campo.</p> </li> 
         <li> <p>Ao selecionar modelos de grupos diferentes, somente os processos de aprovação no nível do sistema são exibidos nesse campo.</p> </li> 
         <li> <p>Quando qualquer um dos modelos tiver um processo de aprovação de uso único anexado, ele será substituído pelo nível do sistema selecionado. </p> </li> 
      </ul> </li> 
      </ul> </td> 
       </tr>  
       </tbody> 
      </table>

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.\
   Ou
1. Clique em **Salvar**.

### Configurações da tarefa {#task-settings}

Você pode definir os padrões que serão associados a todas as novas tarefas quando adicioná-los a um projeto criado a partir do modelo.

Para obter informações sobre como essas configurações afetam a criação de novas tarefas, consulte [Visão geral da criação de tarefas](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Configurações de Tarefa**.

   ![Editar seção de Configurações de Tarefa da caixa de modelo](assets/edit-template-box-task-settings-section.png)

1. Na caixa **Processo de Aprovação Padrão de Tarefa**, selecione o Processo de Aprovação que deseja associar a todas as novas tarefas ao adicioná-las a um projeto criado a partir deste modelo. Você deve criar um Processo de Aprovação para tarefas antes de associá-lo a tarefas. Somente os processos de aprovação ativos são exibidos na lista. Para obter mais informações sobre como criar Processos de Aprovação, consulte [Criando Processos de Aprovação](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. Na caixa **Forms Personalizado Padrão de Tarefa**, selecione o(s) formulário(s) personalizado(s) que deseja associar a todas as novas tarefas quando adicioná-las a um projeto criado a partir deste modelo. Você deve criar os formulários personalizados antes que eles estejam disponíveis para seleção neste campo. Somente formulários personalizados ativos são exibidos na lista. Para obter mais informações sobre a criação de formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Você pode associar até dez formulários personalizados a uma tarefa.
1. (Opcional) Selecione **Usar Esforço de trabalho para calcular automaticamente as Horas planejadas da tarefa** se desejar habilitar o gerenciamento do esforço da tarefa usando o Esforço de trabalho em vez das Horas planejadas no projeto criado a partir do modelo.
1. (Condicional e opcional) Se você selecionou Usar esforço do trabalho para calcular automaticamente as Horas planejadas das tarefas, clique no menu suspenso para atualizar a porcentagem para cada nível de esforço do trabalho. Os seguintes valores percentuais são os padrões:

   | Nível de esforço de trabalho | Valor percentual |
   |---|---|
   | Pequena | 25% |
   | Médio | 50% |
   | Grande | 75% |

   Para obter informações sobre como usar o Esforço de trabalho para gerenciar o esforço em tarefas em projetos, consulte [Visão geral do Esforço de trabalho](../../../manage-work/tasks/task-information/work-effort.md).

1. (Opcional) Continue editando a seção a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Configurações do problema {#issue-settings}

Ao editar configurações de problemas, você pode impedir que os usuários adicionem problemas em linha no projeto futuro criado a partir do modelo.

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Configurações de Problema**.

   ![Editar seção Configurações de Problema da caixa de modelo](assets/edit-template-box-issue-settings-section.png)

1. (Opcional) Desmarque a opção **Permitir que os usuários adicionem problemas em linha**. Esta opção está habilitada por padrão.

   Ao desabilitar essa opção, os usuários não podem adicionar problemas em linha ao projeto ou às tarefas na seção Problemas, quando o projeto é criado a partir do modelo.

   >[!TIP]
   >
   >Desative essa opção se quiser forçar os usuários a preencherem os Campos de novo problema ou os formulários personalizados associados a novos problemas.

   Ao desabilitar essa opção, os usuários com permissões para adicionar problemas ao projeto criado a partir do modelo podem fazer isso usando o botão Novo problema ou uma fila de solicitações associada ao projeto.

   Para obter mais informações sobre como definir configurações de problemas em projetos, consulte a seção [Configurações de Problemas](../../../manage-work/projects/manage-projects/edit-projects.md#issue) no artigo [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

   Para obter informações sobre como criar problemas em projetos, consulte [Criar problemas](../../../manage-work/issues/manage-issues/create-issues.md).

1. (Opcional) Continue editando a seção a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

### Acesso {#access-preview}

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Acesso**.

   ![Editar seção de Acesso à caixa de modelo](assets/edit-template-box-access-section.png)

   O Acesso especificado para seu modelo se tornará o Acesso de usuários associados ao projeto quando o modelo for usado para criar um projeto.

   Especifique as seguintes informações de **Acesso** para o modelo:

   <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
       <tr> 
         <td role="rowheader"><strong>Quando alguém é atribuído a uma tarefa</strong> </td> 
         <td> <p>Selecione o acesso de <strong>Exibir</strong>, <strong>Contribute</strong> ou <strong>Gerenciar</strong> a uma tarefa. O usuário atribuído a uma tarefa recebe automaticamente esse acesso à tarefa. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Também conceder acesso ao projeto</strong> </td> 
         <td> <p> Selecione o acesso do <strong>View</strong>, <strong>Contribute</strong> ou <strong>Manage</strong> ao projeto. O usuário atribuído a uma tarefa também recebe automaticamente esse acesso ao projeto. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Quando alguém é atribuído a um problema</strong> </td> 
         <td> <p>Selecione o acesso de <strong>Visualização</strong>, <strong>Contribute,</strong> ou <strong>Gerenciar</strong> a um problema. O usuário atribuído a um problema recebe automaticamente esse acesso ao problema. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Também conceder acesso ao projeto</strong> </td> 
         <td> <p> Selecione o acesso do <strong>View</strong>, <strong>Contribute</strong> ou <strong>Manage</strong> ao projeto. O usuário atribuído a um problema também recebe automaticamente esse acesso ao projeto. </p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Quando alguém enviar uma solicitação: Conceda a ele acesso</strong> </td> 
         <td> <p> Selecione o acesso de <strong>Visualização</strong>, <strong>Contribute</strong> ou <strong>Gerenciar</strong> à solicitação. Quando enviam uma solicitação para o projeto, eles recebem esse acesso à solicitação enviada. Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a>.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>As pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações</strong> </td> 
         <td> <p>Selecione este campo se desejar que as pessoas da mesma empresa tenham o mesmo acesso a todas as solicitações do projeto, sejam elas enviadas ou não.</p> </td> 
       </tr> 
       <tr> 
         <td role="rowheader"><strong>Quando alguém tiver acesso a este projeto: conceda a ele acesso a...</strong> </td> 
         <td> <p>Selecione as opções de acesso que você deseja que os usuários tenham no projeto, se o projeto for compartilhado com eles. Selecione as opções específicas para seu acesso, se elas forem designadas como <strong>Visualizadores</strong>, <strong>Colaboradores</strong> ou <strong>Gerentes</strong> ao compartilhar o projeto com eles. </p> </td> 
       </tr> 
       </tbody> 
      </table>

1. (Opcional) Continue editando as seções a seguir, dependendo das informações que você deseja modificar.

   Ou

   Clique em **Salvar**.

   Suas alterações serão enviadas para este modelo.

   Agora, quando você usa esse modelo para criar um projeto, todas essas configurações serão transferidas para o novo projeto.

<!--I don't think this note is valid anymore - this note was on Edit project when the section below was in that article, by mistake: 
>[!NOTE]
>
>Because linked folders are created when the project is created, editing the linked folder workflow on an existing project is ineffective. Editing these values when creating a project functions as expected.-->

<!-- This section is here by mistake - it should be maybe in layout templates?? 

### Linked folders (conditional availability) {#linked-folders}

Linked folder functionality automatically creates folders in Adobe Experience Manager Assets, and connects these folders to Workfront. 

This section appears only if all of the following apply:

* Your organization has been migrated to the Adobe Admin Console
* Your organization has enabled and configured an integration with Adobe Experience Manager
* The template has enabled and configured linked folders.

For instructions on editing Linked folders, see [Edit workflow values in a project](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md#edit-workflow-values-in-a-project) in the article [Use workflows in the Experience Manager Assets integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

-->

### Comentário

1. Comece a editar o template conforme descrito acima.
1. Na caixa **Editar Modelo**, clique em **Comentário**.

   ![Editar seção de comentário da caixa de modelo](assets/edit-template-box-comment-section.png)
1. Adicione um comentário sobre a atualização que você está fazendo, marque usuários adicionais ou selecione a caixa **Privado para minha empresa** para manter a atualização privada para os usuários de sua empresa e clique em **Salvar**.

## Editar modelos em massa

É possível editar modelos em massa e atualizar todas as informações ao mesmo tempo.

<!--
Editing templates in bulk differs depending on which environment you are using. 

### Edit templates in bulk in the Production environment 

*****************and hide the first line below************ -->

{{step1-to-templates}}

1. Selecione vários modelos na lista.
1. Clique no ícone **Editar** ![Ícone Editar](assets/edit-icon.png).

   A caixa de diálogo **Editar Modelos** é aberta.

   ![Editar modelos](assets/bulk-edit-templates-0925.png)

1. Clique nas seções à esquerda para editar todos os modelos selecionados.

   Para obter mais informações sobre como editar informações sobre modelos, consulte a seção [Editar um modelo](#edit-a-template) neste artigo.

1. Atualize as seguintes seções dos modelos selecionados:

   * Visão geral
   * Finanças
   * Formulários personalizados
   * Configurações de modelo
   * Configurações da tarefa
   * Configurações do problema
   * Acesso
   * Comentário

1. Clique em **Salvar**.

   Todas as alterações feitas agora estão visíveis em todos os modelos selecionados.

<!--
<div class="preview">

### Edit templates in bulk in the Preview environment 

*****************and hide/delete the first line below************

To edit templates in bulk:

{{step1-to-templates}}

1. Select several templates in the list.
1. Click the **Edit** icon ![Edit icon](assets/edit-icon.png).

   The **Edit Templates** dialog box opens.

   ![Edit templates in bulk box](assets/edit-templates-in-bulk-box.png)

1. Click the sections on the left to edit all selected templates.

   For more information about editing information on templates, see the [Edit a template](#edit-a-template) section in this article.

1. Update the following sections of the selected templates:

   * Overview
   * Custom Forms
   * Finance
   * Template Settings
   * Task Settings
   * Issue Settings
   * Access
   * Comment

1. Click **Save**.

   All changes you made are now visible on all the selected templates.

</div>

-->

## Adicionar tarefas a um modelo

Depois de criar seu modelo e editar as informações dele, você pode adicionar tarefas a ele.

Adicionar tarefas a um modelo é semelhante a adicionar tarefas a um projeto.

Para obter mais informações sobre como adicionar tarefas a um projeto, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

Quando você adiciona tarefas a um modelo, a Duração do modelo e os Dias de Início e Término do modelo são alterados de acordo. Para obter informações sobre os Dias de Início e Conclusão do modelo e das tarefas do modelo, consulte [Visão Geral dos Dias de Início e Conclusão em um modelo](../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md).

## Adicionar mais itens a um modelo

Depois de criar seu modelo e editar as informações dele, você pode adicionar mais itens a ele. Os itens adicionados estarão disponíveis para o projeto quando você o criar a partir do modelo.

Adicionar os seguintes itens a um modelo é idêntico a adicioná-los a um projeto:

* Documentos
* Riscos

  Para obter mais informações sobre como criar riscos, consulte [Criar e editar riscos em projetos](/help/quicksilver/manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

* Processos de aprovação

  Para obter informações sobre como associar processos de aprovação a trabalho, consulte [Associar um processo de aprovação novo ou existente a trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

* Taxas de cobrança

  Adicionar taxas de faturamento para um modelo é semelhante a adicionar taxas de faturamento a um projeto. Para obter mais informações, consulte [Substituir taxas de cobrança de função de trabalho no nível do projeto](/help/quicksilver/manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

* Despesas

  Para obter mais informações sobre como adicionar despesas, consulte [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Detalhes da fila

  Para obter informações sobre como adicionar Detalhes da Fila a um projeto ou modelo, consulte [Criar uma Fila de Solicitação](/help/quicksilver/manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Grupos de Tópicos e Tópicos de Fila

  Para obter informações sobre como adicionar Grupos de tópicos e Tópicos da fila a um projeto ou modelo, consulte os seguintes artigos:

   * [Criar Grupos de Tópicos](/help/quicksilver/manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Criar Tópicos de Fila](/help/quicksilver/manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)

É possível adicionar os seguintes itens às tarefas no modelo:

* Documentos
* Despesas

  Para obter mais informações sobre como adicionar despesas, consulte [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* Aprovações

  Para obter mais informações sobre como associar aprovações a trabalho, consulte [Associar um processo de aprovação novo ou existente a trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).


## Ativar ou desativar um modelo

Você pode desativar um modelo se quiser que os usuários não possam encontrá-lo e criar projetos com base nele. Não é possível anexar um modelo desativado aos projetos nem usá-lo para criar um projeto.

Os modelos desativados não afetam os projetos existentes que foram criados usando-os.

Para desativar um modelo:

1. Vá para um modelo ativo e clique no menu **Mais** ![Mais ícone](assets/qs-more-icon-on-an-object.png) ao lado do nome do modelo e clique em **Desativar**.

   ![Desativar modelo](assets/deactivate-template-link-in-more-menu.png)

   O modelo não está mais ativo e os usuários não podem mais encontrá-lo para criar projetos a partir dele.
1. (Opcional) Para ativar o modelo, clique no menu **Mais** ![Mais ícone](assets/qs-more-icon-on-an-object.png) ao lado do nome do modelo e clique em **Ativar**.

   O modelo agora está ativo e pode ser anexado a projetos ou usado para criar projetos.


<!--
Editing a template differs depending on what environment you choose. 

### Edit a template in the Production environment {#edit-a-template-in-the-production-environment} 

1. Go to the template you want to edit.
1. (Conditional) To edit limited information about the template,  click **Template Details** in the left panel, then go to the areas listed in the left panel to edit information for each area. 
1. To edit information in the Details section, click the **Edit** icon ![Edit icon](assets/edit-icon.png), then select from any of the areas below, or click **Edit all** to edit information in all areas:

   * Overview
   * Custom Forms

     Names of customs forms display only if there are custom forms attached to the object.
   
   * Finance

   >[!TIP]
   >
   >For information about all fields that display in the Details area, continue with editing all fields using the Edit Template box below.

1. (Conditional) To edit all information about the template, click the **More** menu ![More icon](assets/qs-more-icon-on-an-object.png) next to the name of the template, then click **Edit**.

   The **Edit Template** box opens. The sections in this box contain the same fields available in  the Template Details section .

1. Consider editing information in any of the following sections:

   * [Overview](#overview) 
   * [Finance](#finance) 
   * [Portfolio](#portfolio) 
   * [Settings](#settings) 
   * [Access](#access) 
   * [Custom Forms](#custom-forms) 
   * [Tasks](#tasks) 
   * [Issues](#issues) 
   * [Comment](#comment)

### Overview {#overview}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Overview**.

   ![Edit template overview](assets/edit-template-overview-with-tasks-and-issues-350x210.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong></td> 
      <td>Specify a name for the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong></td> 
      <td>Add additional information about the template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Is Active</strong></td> 
      <td><p>Select this checkbox if you want the template to be active. Other users can find this template and attach it to projects when creating projects. Deselect this checkbox if you want to deactivate templates that are no longer used. Deactivated templates cannot be attached to projects. This is enabled by default. </p><p><b>TIP</b>
      
      You can deactivate a template from the template header as described in the [Activate or deactivate a template](#activate-or-deactivate-a-template) section in this article.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong></td> 
      <td>Specify a web link that relates to information about this template.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule From</strong></td> 
      <td><p>Specify whether the project using this template is scheduled from the <strong>Start Date</strong>, or from the <strong>Completion Date</strong>. This selection determines the planned dates of the future tasks on the project using this template. </p><p>Select from the following: </p> 
       <ul> 
        <li><p><strong>Schedule From Start Date</strong>: The Start Date of the template is actually the Start Day. When you schedule a template from Start Date, Adobe Workfront calculates the Completion Day of the template based on the Duration of all the template tasks. The Start Day of the template becomes the Planned Start Date of the future project.</p></li> 
        <li><p><strong>Schedule from Completion Date</strong>: The Completion Date of the template is actually the Completion Day. When you schedule a template from Completion Date, Workfront calculates the Start Day of the template based on the Duration of all the template tasks. The Completion Day of the template becomes the Planned Completion Date of the future project. </p></li> 
       </ul><p>For more information about the Start and Completion Days of template tasks, see <a href="../../../manage-work/projects/create-and-manage-templates/overview-of-start-completion-day-on-template.md" class="MCXref xref">Overview of Start and Completion Days in a template</a>. </p><p>The Schedule From setting for templates is similar to that of projects. Your Workfront administrator selects the default Schedule From setting for the projects in your system. For information about setting project defaults, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Condition Type</strong></td> 
      <td><p>Select between the following Condition Types:</p> 
       <ul> 
        <li><strong>Manual:</strong> The project owner sets the Condition of the project on the project manually. <strong></strong></li> 
        <li><strong>Progress Status:</strong> Workfront automatically sets the Condition of the future project based on the Progress Status of tasks on the Critical Path. For more information about understanding Progress Status, see <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Task Progress Status overview</a>.</li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority</strong></td> 
      <td><p>This is just a visual flag for you which allows you to prioritize your future projects. Select from the following options:</p> 
       <ul> 
        <li><p><strong>None</strong></p></li> 
        <li><p><strong>Low</strong></p></li> 
        <li><p><strong>Normal</strong></p></li> 
        <li><p><strong>High</strong></p></li> 
        <li><p><strong>Urgent</strong></p></li> 
       </ul><p><p>Depending on the Project Preferences selected by your Workfront administrator, the names of priorities might be different for you. For more information about editing priorities, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Create and customize priorities</a>.</p></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Owner</strong></td> 
      <td><p>The user who is designated as the Template Owner must be a Workfront active user. </p><p>Consider the following about the user designated as the Template Owner: </p> 
       <ul> 
        <li>They are automatically given Manage permissions to the template. </li> 
        <li>They are added to the project team and are automatically given Manage permissions to the project created from the template. </li> 
        <li>They become the Project Owner, when the project is created from this template. </li> 
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Sponsor</strong></td> 
      <td><p>The user specified in this field becomes the Project Sponsor, when the template is added to the project. This user is added to the project team and is automatically given view permissions to the project. The user who is designated as the Template Sponsor must be a Workfront active user. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Manager</strong></td> 
      <td><p>The specified users are automatically given manage permissions to the future projects and can assign resources to the tasks and issues of the projects. You can specify more than one Resource Manager. </p></td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Group</strong></td> 
      <td><p>In the drop-down list, select the group that you want to be associated with projects created from the template. It can be a group of any level. </p><p>You can make sure you are selecting the right group by hovering over it and clicking the information icon <img src="assets/info-icon.png"> that displays next to it. This displays a tooltip listing information about the group, such as the hierarchy of groups above it and its administrators.</p> <p><b>NOTES</b>
      
    <ul> 
    <li><p>In the Projects area on a group's page, when someone creates a project using a template that doesn't have a group selected, the system associates the currently open group with the project.</p><p>This is different from other areas where the system associates a user's Home Group with the project when the user creates the project using a template that doesn't have a group selected.</p>
    </li> 
      <li><p>If a user selects a template that has a group selected while creating a project—or while converting a task or issue to a project—the user can choose a different group for the project.</p></li> 
      <li>Though this field is available in templates only in the new Adobe Workfront experience, you can see it in lists and reports both there and in Adobe Workfront Classic. </li> 
      </ul> </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Company</strong></td> 
      <td><p>Specify the Company that you want to associate with the template. Only active companies display in the list.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Finance {#finance}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Finance**.

   ![Edit template finance](assets/edit-template-finance-with-tasks-and-issues-350x259.png)

1. Update the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Performance Index Method</strong></td> 
      <td><p>Specify whether the Earned Value metrics of the future project are calculated using hours or costs. For more information about the Performance Index Method, see <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Set the Performance Index Method (PIM)</a>. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Budget</strong></td> 
      <td><p>Specify a Budget for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Cost</strong></td> 
      <td><p>Specify the Fixed Cost for the projects that are created from this template. This is different than the Labor Cost which comes from the hours on the project and the Expense Cost which comes from the amount of expenses on the project. The Fixed Cost of a project is taken into account when calculating the Net Value of a project and it is part of the Budgeted Cost.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Fixed Revenue</strong></td> 
      <td><p>Specify the Fixed Revenue for the projects that are created from this template.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Template Currency</strong></td> 
      <td><p>Specify the currency for the future project, if it is different than the default currency of your system. This field is not visible if you have only the default currency in the system.<br>For more information about currency, see <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Require time to be approved for this project</strong></td> 
      <td><p>Select this option to require the Project Owner of the future project created from this template to approve time logged on the project. If you are using Billing Records and you select this option, only the approved hours on the project appear as available billable hours for the Billing Records. Approving time on the project is independent of approving timesheets. For more information about requiring time to be approved on a project, see <a href="../../../manage-work/projects/manage-projects/require-time-approval-for-projects.md" class="MCXref xref">Require time to be approved for a project</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Portfolio {#portfolio}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Portfolio**.

   ![Edit template portfolio](assets/edit-template-portfolio-with-tasks-and-issues-350x228.png)

1. Update the following fields:

   <table style="table-layout:auto">
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Portfolio</strong></td> 
      <td><p>Specify a Portfolio for the projects that are created from this template. You must create a Portfolio first, before it appears in the drop-down list. </p><p>Only active portfolios display in the list. For more information about creating portfolios, see <a href="../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md" class="MCXref xref">Create a portfolio </a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Program</strong></td> 
      <td><p>If you selected a Portfolio for the template, specify a <strong>Program</strong> for the future project. Some Portfolios might not have Programs. You must create a Program first, before it appears in this drop-down list. Only active programs display in the list.</p><p>For more information about creating programs, see <a href="../../../manage-work/portfolios/create-and-manage-programs/create-program.md" class="MCXref xref">Create a program</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Planned Benefit</strong></td> 
      <td><p>Specify the Planned Benefit of the projects that are created from this template. The Planned Benefit is used in the Business Case of the project and the Portfolio Optimizer. </p><p>For more information about the Planned Benefit of a project, see <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Overview of project Planned Benefit</a>. The Planned Benefit of a project is taken into account when the Net Value of a project is calculated. </p><p>For more information about using the Portfolio Optimizer, see <a href="../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md" class="MCXref xref">Manage projects in the Portfolio Optimizer</a> </p></td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Settings {#settings}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Settings**.

   ![Edit template settings](assets/edit-template-settings-with-tasks-and-issues-350x336.png)

1. Update the following fields: 

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Milestone Path</strong> </td> 
      <td> <p>Select a Milestone Path for the template. Only active milestone paths display in the list.<br>For more information about Milestone Paths, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Create a milestone path</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Completion Mode</strong> </td> 
      <td> <p>Controls how the future project will be marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The project is marked Complete when all the tasks and issues are completed.</p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually select the Complete status for the project, when all the tasks and issues are completed. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Summary Completion Mode</strong> </td> 
      <td> <p>Controls how the parent tasks on the future project are marked as Complete. <br>Select from the following options:</p> 
       <ul> 
        <li> <p><strong>Automatic</strong>: The parent tasks are marked Complete and they update their percent complete automatically, as the children tasks are completed and the percent complete of the children is updated. </p> </li> 
        <li> <p><strong>Manual</strong>: You have to manually update the percent complete and the status of the parent tasks, independently of what changes are made to the children tasks. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Update Type</strong> </td> 
      <td> <p>Controls when the changes you make to the timeline of the future project are saved on the project. </p> 
       <b>EXAMPLE </b> 
        <p>The following changes to the project trigger an update to the timeline of the project:</p> 
        <ul> 
         <li> <p>update the dates of tasks</p> </li> 
         <li> <p>change predecessor relationships<br></p> </li> 
         <li> <p>change parent-child relationships</p> </li> 
         <li> <p>add or remove assignments in addition to changing the task constraint or duration type.</p> </li> 
        </ul> 
       </div> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Automatic and On Change</strong> (Default setting): The future project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on (On Change). The project timeline is also updated each night (Automatic).<br>This is the recommended setting for this field because it ensures that the project timeline is always up to date.<br>When you perform an action on a task or project that triggers a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer recalculations display briefly as a question mark (between 1 and 5 seconds, or up to a minute for large projects). This indicates that the recalculation is not yet finished, and the dates are subject to change.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Change Only</strong>: The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on. You might want to select this option if changes rarely occur in the project or in other projects that the timeline is dependent on.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Automatic Only</strong>: The project timeline is updated each night; it is not updated immediately after changes are made.<br>You might want to select this option if many changes occur each day in the project or in other projects that the timeline is dependent on. However, be aware that you chose this setting, as the project will not update at the same time that the changes are made.<br></p> </li> 
       </ul> 
       <ul> 
        <li> <p><strong>Manual Only</strong>: The project timeline is updated only when you select the option to Recalculate Timelines, as described in <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Recalculate project timelines</a>.<br></p> </li> 
       </ul> <p>You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schedule</strong> </td> 
      <td> <p>Select a schedule for your template. This will become the schedule of the project that is created from this template. This should be the same schedule assigned to most people that are working on the project. You must create a schedule before you can assign it to a template.<br>For more information about creating schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>. <br>If you have not created custom schedules in your system, the Default Schedule is selected. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>User Time Off</strong> </td> 
      <td> <p>Determines whether the time off of the Primary Assignee of a task adjusts the task planned dates. When you attach the template to an existing project, and the template has a different setting for this field than the project, the setting on the project remains unchanged. The default option for this setting for a new template is the same as the system-level project preference. </p> <p>For information about the project preferences at the System level, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> <p>For information about how this setting affects the task dates on a project, see <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.<br>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Consider user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template adjust according to the time off of the Primary Assignee of the task, if the time off occurs during the duration of the task. </p> </li> 
        <li> <p><strong>Ignore user time off in task durations</strong>: When selecting this option, the planned dates of the tasks on the project created from this template remain as originally planned, even if the Primary Assignee of the task has time off during the duration of the task. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Leveling Mode</strong> </td> 
      <td> <p>Select from the following options:<br></p> 
       <ul> 
        <li> <p><strong>Manual</strong>: you must manually level your resources on the project created from this template (this is the default setting)</p> </li> 
        <li> <p><strong>Automatic:</strong> Workfront levels the resources on the future project. <br>For more information about Resource Leveling, see <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md" class="MCXref xref">Level Resources in the Gantt Chart </a>. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Risk</strong> </td> 
      <td> <p>Define the level of risk of the projects created from this template. The risk is just an indicator of how risky a project can be. You can prioritize the execution of your projects based on the level of risk.<br>Consider selecting from the following levels of risk:<br></p> 
       <ul> 
        <li> <p><strong>Very Low</strong> </p> </li> 
        <li> <p><strong>Low</strong> </p> </li> 
        <li> <p><strong>Medium</strong> </p> </li> 
        <li> <p><strong>High</strong> </p> </li> 
        <li> <p><strong>Very High</strong> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Resource Pools</strong> </td> 
      <td> <p>Specify the resource pools associated with the template. Resource pools are collections of users that are needed at the same time for the completion of a project. For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> <p> <p><b>NOTE</b> 
      
      When you edit templates in bulk, only the resource pools that are common to all the templates selected appear in this field. If the templates selected have no shared resource pools, this field will be empty. The resource pools you specify here will overwrite the templates' individual resource pools.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Approval Process</strong> </td> 
      <td> <p>Select the approval process you want to associate with the template. Your Workfront administrator or a user with administrative access to Approval Processes must define system-level or group-level project approval processes before you can associate them with a template. For more information about creating approval processes, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Create an approval process for work items</a>.</p> <p>Consider the following when adding approval processes: </p> 
      <ul> 
      <li>Only active approval processes display in the list. </li> 
      <li> <p>System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the template does not display in the list.</p> <p><b>IMPORTANT</b> 
      
      If the group associated with the template changes, the group-specific approval process becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md">How group and approval process changes affect assigned approval processes</a>. </p> </li> 
      <li> <p>If you added a single-use approval process, it displays as "Custom" in this field. For information, see <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associate a new or existing approval process with work</a>. </p> 
      </li> 
      <li> <p>When bulk-editing templates, the following scenarios exist:</p> 
      <ul> 
         <li> <p>When you select templates from the same group, both system-level and group-level approval processes display in this field.</p> </li> 
         <li> <p>When you select templates from different groups, only system-level approval processes display in this field.</p> </li> 
         <li> <p>When any of the templates has a single-use approval process attached, it is replaced by the system-level you select. </p> </li> 
      </ul> </li> 
      </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Filter Hour Types</strong> </td> 
      <td> <p>Consider the following:</p> <p>Select <strong>No</strong> to make all project-specific hour types available on the future project. (This is the default selection)</p> <p>Or</p> <p>Select <strong>Yes</strong> to make only a subset of the project-specific hour types available on the future project, then select the hour types you want to make available. (Hold the Shift key to select multiple hour types.)</p> <p>If you select this option, only the hour types you select are made available to select when logging hours on the project (or on tasks and issues within the project). You must select at least one hour type; if you select this option and you do not select any hour types, all hour types are made available on the project.</p> <p>The same hour type selections must be made at the individual user level in order for the user to see these hour type options on the project. </p> <p>For more information about defining hour types at the user level, see the section <a href="../../../timesheets/create-and-manage-timesheets/log-time.md#understa" class="MCXref xref">Log time</a> in <a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">Log time</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Reminder Notification</strong> </td> 
      <td>Select the Reminder Notification that should be associated with the future project. You must configure Reminder Notifications for projects for this field to appear during editing a template. <br>For more information about configuring Reminder Notifications, see <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Set up reminder notifications</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.  
   Or
1. Click **Save Changes**.

### Access {#access}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Access**.

   ![Edit template access](assets/edit-template-access-with-tasks-and-issues-350x241.png)

   The Access you specify for your template will become the Access of users associated with the project when the template is used to create a project.

   Specify the following **Access** information for the template:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to a task</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to a task. The user assigned to a task is automatically granted this access to the task. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to a task is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is assigned to an issue</strong> </td> 
      <td> <p>Select from <strong>View</strong>, <strong>Contribute,</strong> or <strong>Manage</strong> access to an issue. The user assigned to an issue is automatically granted this access to the issue. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Also grant access to the project</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the project. The user assigned to an issue is automatically granted this access to the project, as well. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone submits a request: Give them access</strong> </td> 
      <td> <p> Select from <strong>View</strong>, <strong>Contribute</strong>, or <strong>Manage</strong> access to the request. When they submit a request to the project, they are granted this access to the request they submitted. For more information, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>People from the same company will inherit the same permissions for all requests</strong> </td> 
      <td> <p>Select this field if you want people from the same company to have the same access to all the requests on the project, whether they submitted them or not.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>When someone is given access to this project: Give them access to ...</strong> </td> 
      <td> <p>Select the access options that you want users to have on the project, if the project is shared with them. Select the specific options for their access, if they are designated as <strong>Viewers</strong>, <strong>Contributors</strong>, or <strong>Managers</strong> when sharing the project with them. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Continue editing the following sections, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Custom Forms {#custom-forms}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Custom Forms**.

   ![edit_tempate_custom_forms.png](assets/edit-tempate-custom-forms-tasks-with-issues-sections-350x136.png)

1. Select the custom form or forms that you want to associate with the template. You must build the custom forms before they are available to select in this field.

   Only active custom forms display in the list. s

   You can add up to ten custom forms to a template.

   The forms will be added to the project that is created from this template. 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Tasks {#tasks}

You can define the defaults that will be associated with all the new tasks when you add them to a project that is created from the template.

For information about how these settings affect creating new tasks, see [Create tasks overview](../../../manage-work/tasks/create-tasks/create-tasks-overview.md).

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Tasks**.

   ![Edit template tasks](assets/edit-template-with-tasks-and-issue-sections-350x144.png)

1. In the **Task Default Approval Process** box, select the Approval Process you want to associate with all new tasks when you add them to a project created from this template. You must create an Approval Process for tasks before you can associate it with tasks. Only active approval processes display in the list. For more information about creating Approval Processes, see [Creating Approval Processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
1. In the **Task Default Custom Forms** box, select the custom form or forms that you want to associate with all new tasks when you add them to a project created from this template. You must build the custom forms before they are available to select in this field. Only active custom forms display in the list. You can associate up to ten custom forms with a task.
1. (Optional) **Select Use Work Effort to automatically calculate task Planned Hours** if you want to enable managing task effort by using&nbsp;Work Effort instead of Planned Hours in the project created from the template.
1. (Conditional and optional) If you selected Use Work Effort to automatically calculate task Planned Hours, click the drop-down menu to update the percentage for each level of Work Effort. The following percentage values are the defaults:
 
   | Work Effort level |Percentage value|
   |---|---|
   | Small |25% |
   | Medium |50% |
   | Large |75% |

  For information about using Work Effort to manage the effort on tasks on projects, see [Work Effort overview](../../../manage-work/tasks/task-information/work-effort.md).

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Issues {#issues}

By editing issue settings, you can prevent users from adding issues inline in the future project created from the template.

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Issues**.

   ![Edit template issues](assets/edit-template-box-with-issues-nwe-350x171.png)

1. (Optional) Deselect the **Allow users to add issues inline** option. It is enabled by default.

   When disabling this option users cannot add issues inline to the project or the tasks in the Issues section, when the project is created from the template.

   >[!TIP]
   >
   >Disable this option if you want to enforce users to complete the New Issue Fields or the custom forms associated with new issues.

   When disabling this option, users with permissions to add issues to the project created from the template can do so by using the New Issue button or a request queue associated with the project.

   For more information about configuring issue settings on projects, see the [Issue Settings](../../../manage-work/projects/manage-projects/edit-projects.md#issue) section in the article [Edit projects](../../../manage-work/projects/manage-projects/edit-projects.md).

   For information about creating issues on projects, see [Create issues](../../../manage-work/issues/manage-issues/create-issues.md). 

1. (Optional) Continue editing the following section, depending on the information you want to modify.

   Or

   Click **Save Changes**.

### Comment {#comment}

1. Begin editing your template as described above.
1. In the **Edit Template** box, click **Comment**.

   ![edit_templates_comment.png](assets/edit-templates-comment-with-tasks-and-issues-350x177.png)

1. Specify a comment that you want to display in the updates stream of the template in the available field.

   This comment is visible for everyone with View access to the template and with access to view Notes.

1. Click **Save Changes**.

   Your changes will be submitted for this template.

   Now, when you use this template to create a project all these settings will transfer to the new project.


   <!--drafted section below for the edit template story: 
   remove this tag and add the Preview blurb at the top of this article in yellow, if it's not already there. Keep the "div class" tags below until 23.1 production: 


### Edit a template in the Preview environment {#edit-a-template-in-the-preview-environment}
-->