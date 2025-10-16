---
product-area: templates
navigation-topic: templates-navigation-topic
title: Criar um modelo de projeto
description: É possível criar e excluir modelos na área Modelos. Ao criar um novo modelo, você pode inserir as informações de todas as tarefas e das configurações futuras do projeto. Essas informações serão transferidas para qualquer projeto criado a partir do modelo.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 3%

---

# Criar um modelo de projeto

<!-- Audited: 1/2024 -->

É possível criar e excluir modelos na área Modelos. Ao criar um novo modelo, você pode inserir as informações de todas as tarefas e das configurações futuras do projeto. Essas informações serão transferidas para qualquer projeto criado a partir do modelo.

>[!NOTE]
>
>Um modelo e suas tarefas não têm datas reais, mas uma indicação de qual dia (de quando o projeto futuro pode começar) uma tarefa pode começar e em qual dia a tarefa pode precisar ser concluída. Ao usar modelos para criar os projetos futuros, os projetos receberão datas reais. Para obter informações, consulte [Criar um projeto](../create-projects/create-project.md).


Você pode criar um novo modelo das seguintes maneiras:

* Do zero, conforme descrito neste artigo.
* Em projetos existentes, salvando um projeto como modelo.

  Para obter mais informações sobre como criar modelos a partir de projetos existentes, consulte [Salvar um projeto como um modelo](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiando-o de outro modelo.

  Para obter mais informações sobre como copiar um modelo existente, consulte [Copiar um modelo de projeto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Importando blueprints. Você precisa ser um administrador do Workfront para importar Blueprints. Para obter informações, consulte [Configurar um blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Standard </p><p>Plano</p> <p>Você precisa ser um administrador do sistema para importar modelos de blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a modelos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Por padrão, você tem permissões de gerenciamento para os modelos que criar</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Criar um modelo

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Modelos**.

1. Clique em **Novo Modelo**.

   O modelo não tem título.

   ![Novo modelo](assets/create-template-nwe-2022-350x102.png)

1. Especifique um nome para o novo modelo no cabeçalho do modelo e pressione **Enter.**
1. Clique na seção **Tarefas de modelo** no painel esquerdo.
1. Clique Em **Começar A Adicionar Tarefas De Modelo**.

   Ou

   Clique em **Nova Tarefa de Modelo** para começar a adicionar tarefas ao seu modelo.

   Adicionar tarefas de modelo a um modelo é idêntico a adicionar tarefas a um projeto.

   Para obter mais informações sobre como adicionar tarefas a um projeto, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Não é possível adicionar tarefas recorrentes a um modelo.

1. (Opcional) Clique no ícone do **Gráfico de Gantt** no canto superior direito da Lista de Tarefas para ver uma representação visual da lista de tarefas do modelo.

   >[!TIP]
   >
   >Não é possível editar tarefas diretamente neste Gráfico de Gantt.

1. Para adicionar informações ao novo modelo, clique no ícone **Mais** do menu ![Mais](assets/more-icon.png) e clique em **Editar**.

   Para obter informações sobre como editar um modelo, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Clique em **Salvar alterações**.
1. (Opcional) Se quiser adicionar mais itens ao modelo, consulte a seção [Adicionar mais itens a um modelo](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#add-additional-items-to-a-template) no artigo [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Configurações de modelo determinadas pela associação de grupo

A associação de um modelo de projeto a um grupo (ou a falta de um grupo) afeta como as preferências do projeto, da tarefa e do problema determinam determinadas configurações no modelo. Para obter mais informações, consulte a seção [Criar e modificar modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#create-and-modify-a-groups-project-templates) no artigo [Criar e modificar modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
