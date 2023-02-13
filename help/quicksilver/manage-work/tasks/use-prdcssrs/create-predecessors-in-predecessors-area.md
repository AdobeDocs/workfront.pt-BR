---
product-area: projects
navigation-topic: use-predecessors
title: Criar uma relação de antecessor usando a área Predecessores
description: Você pode usar tarefas antecessoras (ou apenas antecessores) para vincular tarefas que dependem de outras tarefas para iniciar ou concluir. Por exemplo, você não gostaria de hospedar uma parte (tarefa dependente) antes de enviar os convites (tarefa antecessora).
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Criar uma relação de antecessor usando a área Predecessores

Você pode usar tarefas antecessoras (ou apenas antecessores) para vincular tarefas que dependem de outras tarefas para iniciar ou concluir. Por exemplo, você não gostaria de hospedar uma parte (tarefa dependente) antes de enviar os convites (tarefa antecessora).

Este artigo mostra como você pode definir predecessores usando a guia Predecessores em uma tarefa.

Para obter informações sobre como configurar predecessores em uma lista de tarefas, consulte [Criar uma relação de antecessor na lista de tarefas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

Você pode visualizar os antecessores de tarefas nas seguintes áreas do Adobe Workfront:

* Na seção Predecessores das tarefas dependentes
* No Gráfico de Gantt
* Na lista de tarefas na coluna Predecessors

Para obter informações sobre predecessores, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um antecessor para uma tarefa

1. Vá para uma tarefa que deseja designar como uma tarefa dependente e clique em **Predecessores** no painel esquerdo.

   Talvez seja necessário clicar em **Mostrar mais**, em seguida **Predecessores**.

1. Clique em **+Adicionar antecessor**.
1. (Opcional) Para adicionar um antecessor entre projetos, substitua o nome do projeto no **Projeto pai** com outro projeto, digite o nome da tarefa ou tarefas que deseja como antecessores.

   Para obter informações sobre como adicionar predecessores entre projetos, consulte [Criar antecessores entre projetos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

1. Digite o nome da tarefa ou tarefas que deseja designar como antecessores.

   ![](assets/add-predecessor-box-nwe-350x465.png)

1. Selecione um **Tipo de dependência**.

   Para obter informações sobre tipos de dependência de tarefa, consulte um [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Especifique um **Atraso** em dias.

   Para obter informações sobre tipos de atraso, consulte &#x200B; [Visão geral dos tipos de atraso](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

1. Selecionar **Forçado** se quiser impor a relação do antecessor entre as duas tarefas.

   Para obter informações sobre como impor predecessores, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

1. Clique em **Salvar**.
