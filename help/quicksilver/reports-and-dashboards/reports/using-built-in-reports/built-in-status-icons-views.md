---
product-area: reporting
navigation-topic: using-built-in-reports
title: Ícones de status integrados nas visualizações
description: Você pode adicionar o campo Ícones de status internos como uma coluna nas exibições para melhorar a visibilidade dos pontos principais sobre os objetos.
author: Courtney
feature: Reports and Dashboards
exl-id: 7831d5c1-e982-4780-a5a8-54dc6decb3a1
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 11%

---

# Ícones de status integrados nas visualizações

<!-- Audited: 11/2024 -->

<!--(NOTE: ALina: ***Link this from the Understanding Fields in Lists and Reports.)-->

Você pode adicionar o campo Ícones de status internos como uma coluna nas exibições para melhorar a visibilidade dos pontos principais sobre os objetos. Usando os Ícones de status, você pode ver rapidamente quando as seguintes condições existem:

* Um objeto tem documentos em anexo
* Um objeto está associado a um processo de aprovação
* Um objeto tem notas adicionais associadas a ele
* Uma despesa é faturável ou reembolsável
* Uma tarefa está em um caminho crítico
* Um usuário pertence a uma empresa, equipe ou está localizado pessoalmente em um fuso horário diferente

Considere o seguinte:

* A maioria dos indicadores no campo Ícones de status são links rápidos para o objeto ou a área real do objeto que eles representam.

* Se algum item representado pelos ícones estiver ausente do objeto, o ícone que representa o item ausente aparecerá esmaecido na coluna Ícones de status em vez de uma imagem colorida.

  ![task_status_icons.png](assets/task-status-icons.png)

  Para obter mais informações, consulte a seção [Visão Geral de Ícones e Sinalizadores de Status](#overview-of-status-icons-and-flags) neste artigo.

* Em algumas exibições, o campo **Ícones de Status** é chamado de **Sinalizadores** ou **Ícones de Exibição**.\
  Não é possível personalizar a aparência dos ícones incluídos no campo Ícones de status.

* Não é possível editar o número de ícones no campo Ícones de status.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
      <p>Colaborador ou posterior</p>
      <p>Solicitação ou posterior</p>
   </td>
  </tr>
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a relatórios, painéis, calendários para adicionar colunas a um relatório</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para uma exibição existente</p> <p>Gerenciar permissões de um relatório para adicionar colunas a ele</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar o campo Ícones de status a uma exibição

Algumas exibições e relatórios internos já têm o campo Ícones de status incluído.

Não é possível adicionar o campo Ícones de status a todas as exibições.

Para adicionar o campo Ícones de status a uma exibição personalizada criada do zero:

1. Vá para uma lista de qualquer um dos seguintes objetos:

   * Tarefas
   * Problemas
   * Projetos
   * Modelo de Tarefa
   * Modelos
   * Despesas
   * Documentos
   * Usuários\
     Apenas esses objetos têm o campo **Ícones de Status** disponível.\
     Para obter informações sobre listas de objetos, consulte [Introdução às listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. No menu suspenso **Exibição**, selecione **Nova Exibição**.

1. Clique em **Adicionar coluna**.
1. Na caixa **Mostrar nesta coluna**, comece a digitar qualquer um dos seguintes nomes de campo e selecione-o quando ele aparecer na lista:

   * *Ícones de Status*
   * *Sinalizadores*
   * *Exibir Ícones* (somente em exibições de Documento).

   Os ícones internos são listados sob qualquer um desses nomes.\
   O modo de exibição Modelo contém os **Ícones de Status** e os **Sinalizadores** campos. Nesse caso, as duas colunas contêm ícones idênticos.\
   Os modos de exibição de documento contêm um campo **Exibir Ícones**.

1. Clique em **Salvar visualização**.
1. (Opcional) Especifique um novo nome para o modo de exibição e clique em **Salvar Modo de Exibição**.\
   Isso adiciona a coluna **Ícones de Status** ao Modo de Exibição.
1. (Opcional) Passe o mouse sobre um ícone para entender o que ele representa.
1. (Opcional) Clique em um ícone para ir até a área do objeto representado por ele.\
   Nem todos os ícones são vínculos a objetos.\
   Para obter uma lista completa de atributos para cada ícone, consulte a seção [Visão Geral de Ícones e Sinalizadores de Status](#overview-of-status-icons-and-flags).

## Visão Geral de Ícones e Sinalizadores de Status {#overview-of-status-icons-and-flags}

A tabela a seguir lista todos os Ícones de status disponíveis no Workfront, os tipos de objetos que podem ser associados a eles e o que acontece quando você clica neles.

Você deve ter permissões para pelo menos Exibir os objetos para poder clicar em alguns dos ícones a seguir e acessar esses objetos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Ícone ou Sinalizador de Status</strong> </th> 
   <th><strong>Descrição</strong> </th> 
   <th><strong>Objeto</strong> </th> 
   <th>Ao clicar</th> 
   <th> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <img src="assets/condition-update-icon-on-target-29x34.png" alt="condition_update_icon_on_target.png" style="width: 29;height: 34;">ou <img src="assets/screen-shot-2018-08-17-at-9.49.36-am-29x37.png" alt="Screen_Shot_2018-08-17_at_9.49.36_AM.png" style="width: 29;height: 37;"><br><img src="assets/condition-update-icon--in-trouble-29x26.png" alt="condition_update_icon__in_trouble.png" style="width: 29;height: 26;"> ou <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-29x26.png" style="width: 29;height: 26;"><br><img src="assets/condition-update-at-risk-27x28.png" alt="condition_update_at_risk.png" style="width: 27;height: 28;"> ou <img src="assets/screen-shot-2018-08-17-at-9.49.23-am-33x34.png" alt="Screen_Shot_2018-08-17_at_9.49.23_AM.png" style="width: 33;height: 34;"></td> 
   <td>Indica que a condição do projeto é No destino (verde), Em problema (vermelho) ou Em risco (amarelo).<br>Para obter informações sobre a Condição do projeto, consulte <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Visão Geral da Condição do Projeto e do Tipo de Condição</a>.</td> 
   <td>Projetos</td> 
   <td>Clique para abrir a lista de tarefas do projeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/notes-icon-44x34.png" alt="notes_icon.png" style="width: 44;height: 34;"> </td> 
   <td>Indica que o objeto tem observações (atualizações) na guia Atualizações.</td> 
   <td> <p>Projetos<br>Tarefas<br>Problemas<br>Modelos<br>Tarefas de Modelo</p> </td> 
   <td> <p>Clique em para abrir a guia Atualizações do objeto. </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/document-icon-35x42.png" alt="document_icon.png" style="width: 35;height: 42;">ou <img src="assets/new-documents-icon-36x43.png" alt="new_documents_icon.png" style="width: 36;height: 43;"></td> 
   <td>Indica que o objeto tem documentos anexados. </td> 
   <td> Projetos<br>Tarefas<br>Problemas<br>Modelos<br>Tarefas de Modelo </td> 
   <td>Clique em para abrir a guia Documentos do objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/open-issu-icon-34x36.png" alt="open_issu_icon.png" style="width: 34;height: 36;">ou <img src="assets/new-open-issues-25x30.png" alt="new_open_issues.png" style="width: 25;height: 30;"></td> 
   <td>Indica que há ocorrências abertas no projeto ou na tarefa.</td> 
   <td> Projetos<br>Tarefas </td> 
   <td>Clique para abrir o objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/approval-icon-42x38.png" alt="Approval_icon.png" style="width: 42;height: 38;"> ou <img src="assets/new-approval-icon-33x35.png" alt="new_Approval_icon.png" style="width: 33;height: 35;"></td> 
   <td>Indica que há uma aprovação no objeto.</td> 
   <td> Projetos<br>Tarefas<br>Problemas<br>Modelos<br>Tarefas de Modelo </td> 
   <td>Clique para abrir o objeto. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/expenses-icon-52x40.png" alt="costs_icon.png" style="width: 52;height: 40;"> </td> 
   <td> <p>Você pode adicionar uma coluna Ícone de Despesas em sua exibição para exibir esse ícone. Isso indica que o projeto ou a tarefa tem despesas associadas a eles.</p> </td> 
   <td> <p>Projetos</p> <p>Tarefas</p> </td> 
   <td>Clique para abrir a guia Despesas do projeto ou da tarefa. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-progress-status-icon-on-time-44x39.png" alt="task_progress_status_icon_on_time.png" style="width: 44;height: 39;"> <br> <img src="assets/task-progress-status-late-44x43.png" alt="task_progress_status_late.png" style="width: 44;height: 43;"> <br> <img src="assets/task-progress-status-at-risk-44x35.png" alt="task_progress_status_at_risk.png" style="width: 44;height: 35;"> <br> <img src="assets/task-progress-status-icon-behind-44x35.png" style="width: 44;height: 35;"> </td> 
   <td> <p>Indica que o Status do Andamento de uma tarefa é um dos seguintes:</p> 
    <ul> 
     <li>No prazo (quadrado verde)</li> 
     <li>Atrasado (círculo vermelho)</li> 
     <li>Em risco (diamante azul)</li> 
     <li>Atrás (triângulo amarelo)</li> 
    </ul> <p>Para obter informações sobre o Status do Progresso das tarefas, consulte <a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">Visão geral do Status do Progresso da Tarefa</a>.</p> </td> 
   <td>Tarefas</td> 
   <td>Clique em para abrir a tarefa. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/task-critical-path-icon-36x35.png" alt="task_critical_path_icon.png" style="width: 36;height: 35;"> ou <img src="assets/new-critical-path-icon-34x34.png" alt="new_critical_path_icon.png" style="width: 34;height: 34;"></td> 
   <td>Indica que a tarefa está atualmente no Caminho Crítico. <br>Para obter informações sobre tarefas em um Caminho Crítico do projeto, consulte <a href="../../../manage-work/tasks/manage-tasks/critical-path.md" class="MCXref xref">Visão geral do Caminho Crítico do projeto</a>.</td> 
   <td>Tarefas</td> 
   <td>Clique em para abrir a tarefa.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/milestone-icon-50x43.png" alt="milestone_icon.png" style="width: 50;height: 43;"> </td> 
   <td>Indica que a tarefa está associada a uma etapa. O administrador do sistema pode personalizar a cor do diamante do ambiente.<br>Para obter informações sobre etapas, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">Criar um caminho de etapa do projeto</a>.</td> 
   <td>Tarefas</td> 
   <td>Clique em para abrir a tarefa. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/issue-source-link-icon-44x41.png" alt="issue_source_link_icon.png" style="width: 44;height: 41;"> </td> 
   <td>Vincule ao objeto de origem de uma ocorrência. O objeto de origem de uma ocorrência é o objeto em que a ocorrência foi registrada. Uma tarefa ou um projeto pode ser objetos de origem para ocorrências. </td> 
   <td>Problemas</td> 
   <td>Clique para abrir o objeto de origem (tarefa ou projeto) de uma ocorrência. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resolving-object-icon-43x45.png" alt="resolving_object_icon.png" style="width: 43;height: 45;"> </td> 
   <td>Indica que há um objeto de resolução que finalmente resolve o problema. Nesse caso, você não pode concluir o problema. É concluído quando o objeto de resolução é concluído. <br>Para obter informações sobre como resolver objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral de Resolvendo e Resolvendo Objetos </a>.</td> 
   <td>Problemas</td> 
   <td>Clique em para abrir o objeto de resolução do problema. </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/view-doc-icon-45x48.png" alt="view_doc_icon.png" style="width: 45;height: 48;"> </td> 
   <td>Visualizar um documento.</td> 
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
   <td> <img src="assets/user-belongs-to-company-icon-44x44.png" alt="user_owners_to_company_icon.png" style="width: 44;height: 44;"> </td> 
   <td>Indica que o usuário está associado a uma Empresa. </td> 
   <td>Usuários</td> 
   <td>Indisponível</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/user-with-team-icon-40x48.png" alt="user_with_team_icon.png" style="width: 40;height: 48;"> </td> 
   <td>Indica que o usuário está associado a uma Equipe.</td> 
   <td>Usuários</td> 
   <td>Clique em para abrir o perfil do usuário.</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/resource-grid-icon-44x46.png" alt="resource_grid_icon.png" style="width: 44;height: 46;"> </td> 
   <td>Atalho para a guia Alocação do usuário. </td> 
   <td>Usuários</td> 
   <td>Clique para abrir a guia Alocação do usuário e saber a quais itens de trabalho o usuário está atribuído.</td> 
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
   <td> <img src="assets/billable-expense-icon-44x45.png" alt="billable_cost_icon.png" style="width: 44;height: 45;"> </td> 
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
   <td> <img src="assets/reimbursed-expense-icon-44x43.png" alt="refund_cost_icon.png" style="width: 44;height: 43;"></td> 
   <td> Indica que uma despesa foi reembolsada.<br>Para obter informações sobre despesas, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gerenciar despesas do projeto </a>.</td> 
   <td>Despesas</td> 
   <td>Indisponível</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>
