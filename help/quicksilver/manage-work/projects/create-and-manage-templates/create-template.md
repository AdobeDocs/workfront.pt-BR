---
product-area: templates
navigation-topic: templates-navigation-topic
title: Criar um modelo de projeto
description: Você pode criar e excluir modelos da área Modelos. Ao criar um novo modelo, você pode inserir as informações para todas as tarefas e todas as informações para suas configurações futuras do projeto. Essas informações serão transferidas para o projeto, ao criá-las a partir do template.
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 0%

---

# Criar um modelo de projeto

Você pode criar e excluir modelos da área Modelos. Ao criar um novo modelo, você pode inserir as informações para todas as tarefas e todas as informações para suas configurações futuras do projeto. Essas informações serão transferidas para o projeto, ao criá-las a partir do template.

Você pode criar um novo template das seguintes maneiras:

* Do zero, conforme descrito neste artigo.
* A partir de projetos existentes, salvando um projeto como modelo.

   Para obter mais informações sobre como criar modelos a partir de projetos existentes, consulte [Salvar um projeto como modelo](../../../manage-work/projects/manage-projects/save-project-as-template.md).

* Copiando de outro modelo.

   Para obter mais informações sobre cópia de um modelo existente, consulte [Copiar um modelo de projeto](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Se você for um administrador do Workfront, poderá criar modelos importando Blueprints. Para obter mais informações, consulte [Configurar um blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Requisitos de acesso

Você deve ter o seguinte:

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
   <td> <p>Plano </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Administrador de sistema para importar modelos do Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a modelos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Por padrão, você tem permissões de gerenciamento para criar os modelos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um modelo

1. No **Menu principal** ![](assets/main-menu-icon.png) click **Modelos**.

1. Clique em **Novo modelo**.

   O modelo está sem título.

   ![Novo modelo](assets/create-template-nwe-2022-350x102.png)

1. Especifique um nome para o novo modelo no cabeçalho do modelo e pressione **Insira.**
1. Clique no botão **Tarefas do modelo** no painel esquerdo.
1. Clique em **Iniciar Adição de Tarefas de Modelo**.

   Ou

   Clique em **Nova Tarefa de Modelo** para começar a adicionar tarefas ao modelo.

   Adicionar tarefas de modelo a um modelo é idêntico à adição de tarefas a um projeto.

   Para obter mais informações sobre como adicionar tarefas a um projeto, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!NOTE]
   >
   >Não é possível adicionar tarefas recorrentes a um template.

1. (Opcional) Clique no botão **Gráfico de Gantt** no canto superior direito da Lista de tarefas para ver uma representação visual da lista de tarefas do modelo.

   >[!TIP]
   >
   >Não é possível editar tarefas diretamente deste gráfico de Gantt.

1. Para adicionar informações ao novo modelo, clique no botão **Mais** menu ![](assets/more-icon.png), depois clique em **Editar**.

   Para obter informações sobre como editar um modelo, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

1. Clique em **Salvar alterações**.
1. (Opcional) Se desejar adicionar itens ao modelo, consulte a seção [Adicionar itens adicionais a um modelo](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#adding-items-to-template) no artigo [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

## Configurações de modelo determinadas pela associação de grupo

A associação de um modelo de projeto a um grupo (ou sua falta) afeta como o projeto, a tarefa e as preferências de emissão determinam determinadas configurações no modelo. Para obter mais informações, consulte a seção [Criar e modificar modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md#template2) no artigo [Criar e modificar modelos de projeto de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).
