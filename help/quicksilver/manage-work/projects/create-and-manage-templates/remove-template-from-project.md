---
product-area: templates
navigation-topic: templates-navigation-topic
title: Remover informações do modelo de um projeto
description: Não é possível remover um modelo de um projeto. Você só pode remover manualmente as informações que foram adicionadas ao projeto depois que um modelo foi anexado ao projeto. Para obter informações sobre como anexar modelos, consulte Anexar um modelo a um projeto.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 1%

---

# Remover informações do modelo de um projeto

Não é possível remover um modelo de um projeto. Você só pode remover manualmente as informações que foram adicionadas ao projeto depois que um modelo foi anexado ao projeto. Para obter informações sobre como anexar modelos, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Padrão</p>
   <p>Atual: trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar o acesso a tarefas </p> <p>Contribute ou acesso superior ao projeto </p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Opções para remover informações de modelo de um projeto

Para remover as informações do modelo que foram adicionadas ao projeto, siga um destes procedimentos:

* Remova manualmente as informações do projeto após o modelo ter sido anexado.

  Para obter informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

* Exclua as tarefas no projeto que foram adicionadas com o modelo.

  Para obter informações, consulte a seção [Excluir tarefas criadas de um modelo](#delete-tasks-created-from-a-template) neste artigo.

* Exclua o modelo do Workfront. A exclusão do modelo do Workfront não exclui as tarefas adicionadas do modelo dos projetos.

  Para obter informações, consulte [Excluir modelos de projeto](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Excluir tarefas criadas a partir de um modelo {#delete-tasks-created-from-a-template}

1. Vá para a seção **Tarefas** do projeto.
1. Siga um destes procedimentos:

   * Crie um filtro para a lista de tarefas para exibir somente tarefas que foram criadas a partir de um modelo usando a seguinte instrução:

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Para obter informações sobre como criar um filtro, consulte [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     Quando você aplica o filtro, somente as tarefas associadas a uma ID de Tarefa de Modelo são exibidas na lista.

   * Crie um modo de exibição para a lista de tarefas para exibir os campos **ID da Tarefa de Modelo** ou **Nome da Tarefa de Modelo** em uma coluna.

     Quando você aplica a exibição, as tarefas que contêm informações na coluna ID da Tarefa de Modelo ou nome da Tarefa de Modelo são criadas usando um modelo.

     Para obter informações sobre como criar uma exibição, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Selecione todas as tarefas identificadas na Etapa 2 como criadas a partir de um modelo e clique em **o ícone Excluir**&#x200B;**> Sim, Excluir**. Para obter mais informações, consulte [Excluir tarefas](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
