---
product-area: projects
navigation-topic: use-predecessors
title: Criar um relacionamento predecessor usando a área Predecessores
description: É possível usar tarefas predecessoras (ou apenas predecessoras) para vincular tarefas que dependem de outras tarefas para serem iniciadas ou concluídas. Por exemplo, você não gostaria de hospedar um participante (tarefa dependente) antes de enviar os convites (tarefa predecessora).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: d5f4e83badd4d011816551f06b056ffe886d3b17
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Criar um relacionamento predecessor usando a área Predecessores

É possível usar tarefas predecessoras (ou apenas predecessoras) para vincular tarefas que dependem de outras tarefas para serem iniciadas ou concluídas. Por exemplo, você não gostaria de hospedar um participante (tarefa dependente) antes de enviar os convites (tarefa predecessora).

Este artigo mostra como definir predecessores usando a guia Predecessores em uma tarefa.

Para obter informações sobre como configurar predecessores em uma lista de tarefas, consulte [Criar uma relação de predecessora na lista de tarefas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

É possível exibir os predecessores das tarefas nas seguintes áreas do Adobe Workfront:

* Na seção Predecessoras das tarefas dependentes
* No Gráfico de Gantt
* Na lista de tarefas da coluna Predecessores

Para obter informações sobre predecessores, consulte [Visão geral das predecessoras da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Criar um predecessor para uma tarefa

1. Vá para uma tarefa que você deseja designar como uma tarefa dependente e clique em **Predecessores** no painel esquerdo.

   Talvez seja necessário clicar em **Mostrar mais**, depois **Predecessores**.

1. Clique em **+Adicionar predecessor**.
1. (Opcional) Para adicionar uma predecessora entre projetos, substitua o nome do projeto na **Projeto pai** com outro projeto e digite o nome da tarefa ou tarefas que deseja como predecessoras.

   Para obter informações sobre a adição de predecessores entre projetos, consulte [Criar predecessores entre projetos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Digite o nome da tarefa ou tarefas que você deseja designar como predecessoras.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Selecione um **Tipo de Dependência**.

   Para obter informações sobre Tipos de Dependência da tarefa, consulte uma [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Especificar um **Defasagem** valor em dias.

   Para obter informações sobre Tipos de Defasagem, consulte &#x200B; [Visão geral dos Tipos de Defasagem](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Selecionar **Reforçado** se quiser impor a relação de predecessora entre as duas tarefas.

   Para obter informações sobre a imposição de predecessores, consulte [Forçar predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Clique em **Salvar**.
