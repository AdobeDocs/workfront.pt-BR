---
product-area: templates
navigation-topic: templates-navigation-topic
title: Remover informações de modelo de um projeto
description: Não é possível remover um modelo de um projeto. Você só pode remover manualmente as informações que foram adicionadas ao projeto depois que um modelo foi anexado ao projeto. Para obter informações sobre como anexar modelos, consulte Anexar um modelo a um projeto.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# Remover informações de modelo de um projeto

Não é possível remover um modelo de um projeto. Você só pode remover manualmente as informações que foram adicionadas ao projeto depois que um modelo foi anexado ao projeto. Para obter informações sobre como anexar modelos, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

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
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso às tarefas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso a tarefas </p> <p>Contribuir ou aumentar o acesso ao projeto </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Opções para remover informações do modelo de um projeto

Para remover as informações do modelo que foram adicionadas ao projeto, é possível fazer um dos seguintes procedimentos:

* Remova manualmente as informações do projeto depois que o modelo foi anexado.

   Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

* Exclua as tarefas no projeto que foram adicionadas com o modelo .

   Para obter informações, consulte o [Excluir tarefas criadas a partir de um modelo](#delete-tasks-created-from-a-template) neste artigo.

* Exclua o modelo do Workfront. A exclusão do modelo do Workfront não exclui as tarefas adicionadas do modelo dos projetos.

   Para obter mais informações, consulte [Excluir modelos de projeto](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Excluir tarefas criadas a partir de um modelo {#delete-tasks-created-from-a-template}

1. Vá para o **Tarefas** seção do projeto.
1. Siga um destes procedimentos:

   * Crie um filtro para a lista de tarefas para exibir somente as tarefas que foram criadas a partir de um modelo usando a seguinte instrução:

      ```
      Task >> Template Task ID >>Is Not Blank
      ```

      Para obter informações sobre como criar um filtro, consulte [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

      Ao aplicar o filtro, somente as tarefas associadas a uma ID de tarefa do modelo são exibidas na lista.

   * Crie uma exibição para a lista de tarefas para exibir a variável **ID da tarefa do modelo** ou **Nome da tarefa do modelo** em uma coluna.

      Ao aplicar a visualização, as tarefas que contêm informações na coluna ID da tarefa do modelo ou nome da tarefa do modelo eram criadas usando um modelo.

      Para obter informações sobre como criar uma exibição, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Selecione todas as tarefas identificadas na Etapa 2 como criadas a partir de um modelo e clique em **o ícone Excluir****> Sim, exclua**. Para obter mais informações, consulte [Excluir tarefas](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
