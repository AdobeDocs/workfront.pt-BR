---
product-area: projects
navigation-topic: use-predecessors
title: Criar um relacionamento predecessor usando a área Predecessores
description: É possível usar tarefas predecessoras (ou apenas predecessoras) para vincular tarefas que dependem de outras tarefas para serem iniciadas ou concluídas.
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Criar um relacionamento predecessor usando a área Predecessores

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Novo: Padrão </p>
   <p>Ou </p>
   <p>Atual: Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um predecessor para uma tarefa

1. Navegue até a tarefa que deseja designar como uma tarefa dependente.

1. No painel esquerdo, clique em **Predecessores**.

1. Na seção **Predecessoras**, clique em **+Adicionar Predecessora**. A caixa de diálogo **Adicionar Predecessora** é aberta.

1. (Opcional) Para adicionar um predecessor entre projetos, substitua o nome do projeto no campo **Projeto principal** por outro projeto.

   Para obter informações, consulte [Criar predecessores entre projetos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. No campo **Tarefas**, digite o nome da(s) tarefa(s) que deseja designar como predecessoras e, em seguida, selecione-as quando elas aparecerem no menu suspenso.

1. Selecione um **Tipo de dependência**.

   Para obter informações, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Insira um valor de **Defasagem**.

   Para obter informações, consulte &#x200B;[visão geral sobre Tipos de Defasagem](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   ![Caixa de diálogo Adicionar Predecessora](assets/add-predecessor-dialog-box.png)

1. Marque a caixa de seleção **Enforced** se desejar impor a relação de predecessora entre as duas tarefas.

   Para obter informações, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Clique em **Salvar**.
