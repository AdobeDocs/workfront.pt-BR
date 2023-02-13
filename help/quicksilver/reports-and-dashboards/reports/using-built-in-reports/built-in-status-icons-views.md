---
product-area: reporting
navigation-topic: using-built-in-reports
title: Ícones de status incorporados nas exibições
description: Ícones de status incorporados nas exibições
author: Nolan
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1291'
ht-degree: 2%

---

# Ícones de status incorporados nas exibições

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.) </p>
-->

É possível adicionar o campo Ícones de status integrado como uma coluna em suas visualizações para melhorar a visibilidade em pontos-chave sobre seus objetos. Usando ícones de status, você pode ver rapidamente quando as seguintes condições existem:

* Um objeto tem documentos anexados
* Um objeto está associado a um processo de aprovação
* Um objeto tem observações adicionais associadas a ele
* Uma despesa é faturável ou reembolsável
* Uma tarefa está em um caminho crítico
* Um usuário pertence a uma empresa, uma equipe ou está localizado em um fuso horário diferente

A maioria dos indicadores no campo Ícones de status são links rápidos para o objeto ou área real do objeto que eles representam.

Se algum dos itens representados pelos ícones estiver ausente no objeto, o ícone que representa o item ausente aparecerá como um outline na coluna Ícones de status em vez de uma imagem completa.\
![task_status_icons.png](assets/task-status-icons.png)\
Para obter mais informações, consulte o [Visão geral de ícones e sinalizadores de status](#overview-of-status-icons-and-flags) neste artigo.\
Em algumas exibições, a variável **Ícones de status** campo é nomeado **Sinalizadores** ou **Exibir ícones**.\
Não é possível personalizar a aparência dos ícones incluídos no campo Ícones de status .

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para adicionar colunas a um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para uma exibição existente</p> <p>Gerenciar permissões de um relatório para adicionar colunas a ele</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Adicionar o campo Ícones de status a uma visualização

Algumas exibições e relatórios internos já têm o campo Ícones de status incluído.

Não é possível adicionar o campo Ícones de status a todas as exibições.

Para adicionar o campo Ícones de status a uma visualização personalizada que você cria do zero:

1. Vá para uma lista de qualquer um dos seguintes objetos:

   * Tarefas
   * Problemas
   * Projetos
   * Modelo de Tarefa
   * Modelos
   * Despesas
   * Documentos
   * Usuários\
      Somente esses objetos têm a variável **Ícones de status** campo disponível.\
      Para obter informações sobre listas de objetos, consulte [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. No **Exibir** , selecione **Nova exibição**.

1. Clique em **Adicionar coluna**.
1. No **Mostrar nesta coluna** , comece a digitar qualquer um dos seguintes nomes de campo e, em seguida, selecione-o quando aparecer na lista:

   * *Ícones de Status*
   * *Marcações*
   * *Ícones de Exibição * (somente em Visualizações de Documento).

   Os ícones integrados são listados em qualquer um desses nomes.\
   Uma exibição Modelo contém ambos os **Ícones de status** e **Sinalizadores** campos. Nesse caso, as duas colunas contêm ícones idênticos.\
   As exibições de documento contêm um **Exibir ícones** campo.

1. Clique em **Salvar exibição**.
1. (Opcional) Especifique um novo nome para sua exibição e clique em **Salvar exibição**.\
   Isso adiciona a variável **Ícones de status** para sua Exibição.
1. (Opcional) Passe o mouse sobre um ícone para entender o que ele representa.
1. (Opcional) Clique em um ícone para ir até a área do objeto representado por ele.\
   Nem todos os ícones são links para objetos.\
   Para obter uma lista completa dos atributos para cada ícone, consulte o [Visão geral de ícones e sinalizadores de status](#overview-of-status-icons-and-flags) seção.

## Visão geral de ícones e sinalizadores de status {#overview-of-status-icons-and-flags}

A tabela a seguir lista todos os Ícones de status disponíveis no Workfront, o tipo de objetos que podem ser associados a eles, bem como o que acontece quando você clica neles.

Você deve ter permissões para, pelo menos, Exibir os objetos para poder clicar em alguns dos ícones a seguir e acessar esses objetos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Ícone de status ou sinalizador</strong> </th> 
   <th><strong>Descrição</strong> </th> 
   <th><strong>Objeto</strong> </th> 
   <th>Ao clicar</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">ou <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon_in_trouh.png" style="width: 29;height: 26;"> ou <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> ou <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>Indica que a condição do projeto é No destino (verde), Em problema (vermelho) ou Em risco (amarelo).<br>Para obter informações sobre a condição do projeto, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Visão geral da condição do projeto e do tipo de condição</a>.</td> 
   <td>Projetos</td> 
   <td>Clique em para abrir a lista de tarefas do projeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>Indica que o objeto tem notas (atualizações) na guia Atualizações .</td> 
   <td> <p>Projetos<br>Tarefas<br>Problemas<br>Modelos<br>Tarefas do modelo</p> </td> 
   <td> <p>Clique em para abrir a guia Atualizações do objeto. </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">ou <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>Indica que o objeto tem documentos anexados. </td> 
   <td> Projetos<br>Tarefas<br>Problemas<br>Modelos<br>Tarefas do modelo </td> 
   <td>Clique em para abrir a guia Documents do objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issue_icon.png" style="width: 34;height: 36;">ou <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>Indica que há problemas em aberto no projeto ou na tarefa.</td> 
   <td> Projetos<br>Tarefas </td> 
   <td>Clique em para abrir o objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="approval_icon.png" style="width: 42;height: 38;"> ou <img src="assets/new-approval-icon-33x35.png" alt="new_approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>Indica que existe uma aprovação no objeto.</td> 
   <td> Projetos<br>Tarefas<br>Problemas<br>Modelos<br>Tarefas do modelo </td> 
   <td>Clique em para abrir o objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="people_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>É possível adicionar uma coluna de Ícone de Despesas na visualização para exibir esse ícone. Isso indica que o projeto ou a tarefa tem despesas associadas a elas.</p> </td> 
   <td> <p>Projetos</p> <p>Tarefas</p> </td> 
   <td>Clique em para abrir a guia Expenses do projeto ou da tarefa. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>Indica que o Status de Andamento de uma tarefa é um dos seguintes:</p> 
    <ul> 
     <li>No horário (quadrado verde)</li> 
     <li>Atraso (círculo vermelho)</li> 
     <li>Em risco (diamante azul)</li> 
     <li>Atrás (triângulo amarelo)</li> 
    </ul> <p>Para obter informações sobre o Status de Andamento de tarefas, consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do status de progresso da tarefa</a>.</p> </td> 
   <td>Tarefas</td> 
   <td>Clique em para abrir a tarefa. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_primary_path_icon.png" style="width: 36;height: 35;"> ou <img src="assets/new-critical-path-icon-34x34.png" alt="new_primary_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>Indica que a tarefa está atualmente no Caminho Crítico. <br>Para obter informações sobre tarefas em um Caminho Crítico do projeto, consulte <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">Visão geral do caminho crítico do projeto</a>.</td> 
   <td>Tarefas</td> 
   <td>Clique em para abrir a tarefa.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>Indica que a tarefa está associada a um marco. O administrador do sistema pode personalizar a cor do diamante em seu ambiente.<br>Para obter informações sobre marcos, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Criar um caminho de marco</a>.</td> 
   <td>Tarefas</td> 
   <td>Clique em para abrir a tarefa. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>Link para o objeto de origem de um problema. O objeto de origem de um problema é o objeto no qual o problema foi registrado. Uma tarefa ou um projeto pode ser objeto de origem para problemas. </td> 
   <td>Problemas</td> 
   <td>Clique em para abrir o objeto de origem (tarefa ou projeto) de um problema. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolvendo_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>Indica que existe um objeto de resolução que resolve o problema. Nesse caso, não é possível concluir o problema. Ele é concluído quando o objeto de resolução é concluído. <br>Para obter informações sobre como resolver objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</td> 
   <td>Problemas</td> 
   <td>Clique em para abrir o objeto de resolução do problema. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>Exibir um documento.</td> 
   <td>Documentos</td> 
   <td>Clique em para baixar o documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/download-doc-icon.png"> </td> 
   <td>Baixe um documento.</td> 
   <td>Documentos</td> 
   <td>Clique em para baixar o documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-type-icon.png"> </td> 
   <td>Indica o tipo de documento.</td> 
   <td>Documentos</td> 
   <td>Clique em para baixar o documento.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_Pertenços_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>Indica que o usuário está associado a uma Empresa. </td> 
   <td>Usuários</td> 
   <td>Indisponível</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_Team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>Indica que o usuário está associado a uma Equipe.</td> 
   <td>Usuários</td> 
   <td>Clique em para abrir o perfil do usuário.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>Atalho para a guia Alocação do usuário. </td> 
   <td>Usuários</td> 
   <td>Clique em para abrir a guia Alocação do usuário e saber quais itens de trabalho o usuário está atribuído.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/screen-shot-2018-07-26-at-2.31.40-pm-44x40.png" alt="Screen_Shot_2018-07-26_at_2.31.40_PM.png" style="width: 44;height: 40;"> </td> 
   <td>Indica que o usuário está em um fuso horário diferente do do sistema.</td> 
   <td>Usuários</td> 
   <td>Indisponível</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="bilable_cost_icon.png" style="width: 44;height: 45;"> </td> 
   <td>Indica que uma despesa é faturável.<br>Para obter informações sobre despesas, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gerenciar despesas do projeto </a>.</td> 
   <td>Despesas</td> 
   <td>Indisponível</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expense-reimbursable-icon-44x45.png" alt="cost_reembolsable_icon.png" style="width: 44;height: 45;"> </td> 
   <td> Indica que uma despesa é reembolsável.<br>Para obter informações sobre despesas, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gerenciar despesas do projeto </a>.</td> 
   <td>Despesas</td> 
   <td>Indisponível</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="reembolsar_despesas_ícone.png" style="width: 44;height: 43;"></td> 
   <td> Indica que uma despesa foi reembolsada.<br>Para obter informações sobre despesas, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gerenciar despesas do projeto </a>.</td> 
   <td>Despesas</td> 
   <td>Indisponível</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
