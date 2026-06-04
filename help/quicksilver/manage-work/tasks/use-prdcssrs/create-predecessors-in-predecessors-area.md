---
product-area: projects
navigation-topic: use-predecessors
title: Criar uma relação de predecessora usando a área predecessoras
description: É possível usar tarefas predecessoras (ou apenas predecessoras) para vincular tarefas que dependem de outras tarefas para serem iniciadas ou concluídas.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
TQID: https://experienceleague.adobe.com/BOZkyUl3TKCzpbjbLnUcMQZjM-1laW-TSsVptvBP-0U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 422
ht-degree: 8%

---

# Criar uma relação de predecessor usando a área Predecessores

<!-- Audited: 5/2025 -->

É possível usar tarefas predecessoras (ou apenas predecessoras) para vincular tarefas que dependem de outras tarefas para serem iniciadas ou concluídas. Por exemplo, você não gostaria de hospedar um participante (tarefa dependente) antes de enviar os convites (tarefa predecessora).

Este artigo mostra como definir predecessores usando a guia Predecessores em uma tarefa.

Para obter informações sobre como definir predecessores em uma lista de tarefas, consulte [Criar uma relação de predecessora na lista de tarefas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

É possível exibir os predecessores das tarefas nas seguintes áreas do Adobe Workfront:

* Na seção Predecessoras das tarefas dependentes
* No Gráfico de Gantt
* Na lista de tarefas da coluna Predecessores

Para obter informações sobre predecessores, consulte [Visão geral dos predecessores da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td><p>Padrão</p> 
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um predecessor para uma tarefa

Criar um predecessor para uma tarefa do projeto usando a área Predecessores é semelhante a criar predecessores para uma tarefa de modelo em um modelo.

Para criar uma tarefa predecessora para uma tarefa do projeto:

1. Navegue até a tarefa que deseja designar como uma tarefa dependente.

1. No painel esquerdo, clique em **Predecessores**.

1. Na seção **Predecessoras**, clique em **Adicionar Predecessora**. A caixa de diálogo **Adicionar Predecessora** é aberta.

1. (Opcional) Para adicionar um predecessor entre projetos, substitua o nome do projeto no campo **Projeto principal** por outro projeto.

   Para obter informações, consulte [Criar predecessores entre projetos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

   >[!TIP]
   >
   >Não é possível criar predecessores entre modelos para tarefas de modelo.


1. No campo **Tarefas**, digite o nome da(s) tarefa(s) que deseja designar como predecessoras e, em seguida, selecione-as quando elas aparecerem no menu suspenso.

1. Selecione um **Tipo de dependência**.

   Para obter informações, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Insira um valor de **Defasagem**.

   Para obter informações, consulte &#x200B;[visão geral sobre Tipos de Defasagem](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Caixa de diálogo Adicionar Predecessora](assets/add-predecessor-dialog-box.png)

1. Marque a caixa de seleção **Enforced** se desejar impor a relação de predecessora entre as duas tarefas.

   Para obter informações, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Clique em **Salvar**.

1. (Opcional) Para remover um predecessor, selecione-o na lista de predecessores, em seguida, clique no ícone **Remover** ícone ![Remover](assets/remove-or-delete-icon.png).

   O antecessor é removido da lista. A tarefa predecessora não é excluída de seu projeto.
