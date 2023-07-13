---
product-area: templates
navigation-topic: templates-navigation-topic
title: Criar um modelo de projeto
description: É possível criar e excluir modelos na área Modelos. Ao criar um novo modelo, você pode inserir as informações de todas as tarefas e todas as informações para suas configurações de projeto futuras. Essas informações serão transferidas para o projeto quando você criá-las a partir do modelo.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 79822d258642675331e1998dd3552e3078db41f8
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Criar um modelo de projeto

É possível criar e excluir modelos na área Modelos. Ao criar um novo modelo, você pode inserir as informações de todas as tarefas e todas as informações para suas configurações de projeto futuras. Essas informações serão transferidas para o projeto quando você criá-las a partir do modelo.

>[!NOTE]
>
>Um modelo e suas tarefas não têm datas reais, mas uma indicação de qual dia (de quando o projeto futuro pode começar) uma tarefa pode começar e em qual dia a tarefa pode precisar ser concluída. Ao usar modelos para criar os projetos futuros, os projetos receberão datas reais. Para obter informações, consulte [Criar um projeto](../create-projects/create-project.md).


Você pode criar um novo modelo das seguintes maneiras:

* Do zero, conforme descrito neste artigo.
* Em projetos existentes, salvando um projeto como modelo.

  Para obter mais informações sobre como criar modelos a partir de projetos existentes, consulte [Salvar um projeto como modelo](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiando-o de outro modelo.

  Para obter mais informações sobre como copiar um modelo existente, consulte [Copiar um modelo de projeto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Se você for um administrador do Workfront, poderá criar modelos importando Blueprints. Para obter informações, consulte [Configurar um blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisitos de acesso

Você deve ter o seguinte:

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
   <td> <p>Plano </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Administrador do sistema para importar modelos de blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a modelos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Por padrão, você tem permissões de gerenciamento para os modelos que criar</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Criar um modelo

1. No **Menu principal** ![](assets/main-menu-icon.png) click **Modelos**.

1. Clique em **Novo modelo**.

   O modelo não tem título.

   ![Novo modelo](assets/create-template-nwe-2022-350x102.png)

1. Especifique um nome para o novo modelo no cabeçalho do modelo e pressione **Digite.**
1. Clique em **Modelos de Tarefa** no painel esquerdo.
1. Clique em **Comece a Adicionar Tarefas de Modelo**.

   Ou

   Clique em **Novo Modelo de Tarefa** para começar a adicionar tarefas ao seu modelo.

   Adicionar tarefas de modelo a um modelo é idêntico a adicionar tarefas a um projeto.

   Para obter mais informações sobre como adicionar tarefas a um projeto, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Não é possível adicionar tarefas recorrentes a um modelo.

1. (Opcional) Clique no link **Gráfico de Gantt** no canto superior direito da Lista de Tarefas para ver uma representação visual da lista de tarefas do modelo.

   >[!TIP]
   >
   >Não é possível editar tarefas diretamente neste Gráfico de Gantt.

1. Para adicionar informações ao novo modelo, clique no link **Mais** menu ![](assets/more-icon.png)e, em seguida, clique em **Editar**.

   Para obter informações sobre como editar um modelo, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Clique em **Salvar alterações**.
1. (Opcional) Se quiser adicionar mais itens ao modelo, consulte a seção [Adicionar mais itens a um modelo](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) no artigo [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Configurações de modelo determinadas pela associação de grupo

A associação de um modelo de projeto a um grupo (ou a falta dele) afeta como as preferências de projeto, tarefa e problema determinam determinadas configurações no modelo. Para obter mais informações, consulte a seção [Criar e modificar os modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) no artigo [Criar e modificar os modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
