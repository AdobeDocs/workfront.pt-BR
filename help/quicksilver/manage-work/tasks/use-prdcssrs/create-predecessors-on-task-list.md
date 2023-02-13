---
product-area: projects
navigation-topic: use-predecessors
title: Criar uma relação de antecessor na lista de tarefas
description: Você pode usar tarefas antecessoras (ou apenas antecessores) para vincular tarefas que dependem de outras tarefas para iniciar ou concluir. Por exemplo, você não gostaria de hospedar uma parte (tarefa dependente) antes de enviar os convites (tarefa antecessora).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 420ba180dd0bfd53514c58f77ca9897ba9797320
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Criar uma relação de antecessor na lista de tarefas

Você pode usar tarefas antecessoras (ou apenas antecessores) para vincular tarefas que dependem de outras tarefas para iniciar ou concluir. Por exemplo, você não gostaria de hospedar uma parte (tarefa dependente) antes de enviar os convites (tarefa antecessora).

Este artigo mostra como criar antecessores na lista de tarefas.

Você pode visualizar os antecessores de tarefas nas seguintes áreas do Adobe Workfront:

* Na lista de tarefas na coluna Predecessors .
* No gráfico de Gantt
* Na seção Predecessores de uma tarefa dependente

Para obter mais informações, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um antecessor

1. Vá para um projeto.
1. Clique em **Tarefas** no painel esquerdo.
1. Certifique-se de que sua exibição atual exiba a variável **Predecessor** coluna.

   Se a exibição não exibir a coluna Predecessores , altere para uma exibição que o faz ou adicione a coluna à sua exibição.

1. Selecione a tarefa que deseja designar como a tarefa dependente.
1. Clique dentro do **Predecessores** coluna.
1. Digite o número da tarefa que deseja designar como o antecessor da tarefa selecionada e pressione **Enter**.

   O ícone antecessor fica verde quando a tarefa antecessora é marcada como concluída. Isso indica que a tarefa dependente está pronta para o trabalho.

   Para obter mais informações sobre os tipos de relacionamento disponíveis na coluna Predecessors , consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) em [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Exibir detalhes do antecessor

Você pode visualizar rapidamente os detalhes sobre o antecessor na lista de tarefas.

1. Na lista de tarefas, passe o mouse sobre o número do antecessor no **Predecessores** coluna.

   Uma caixa com os detalhes do antecessor é exibida.

   ![Detalhes do antecessor](assets/predecessor-details-in-task-list.png)

   Os seguintes detalhes são exibidos:

   **Nome do antecessor:** O nome do antecessor que está sendo referenciado. O número da tarefa do antecessor é incluído. Clique no nome da tarefa para abri-la. No exemplo acima, o antecessor é Produção/Execução/Delivery.

   **Nome do projeto:** O nome do projeto em que o antecessor reside. O projeto é identificado como o projeto atual se o antecessor pertencer aos mesmos projetos que a tarefa, ou como um projeto cruzado, se o antecessor pertencer a um projeto diferente. No exemplo acima, o nome do projeto é Digital Asset Production (Integrated) - Project. Para obter mais informações sobre predecessores entre projetos, consulte [Criar antecessores entre projetos](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Você pode expandir os detalhes do projeto para ver as datas de início e término planejadas do projeto, condição, status, porcentagem concluída e proprietário. Para um projeto cruzado, você pode clicar em **Consulte Projeto** para abrir o projeto.

   **ID:** Número de referência do projeto em que o antecessor está localizado.

   **Início planejado:** A Data Inicial Planejada da tarefa predecessora.

   **Fim planejado:** A Data de Conclusão Planejada da tarefa do antecessor.

   **Número de antecessores:** O número de antecessores para o antecessor que está sendo referenciado. No exemplo acima, o antecessor que está sendo referenciado tem 1 antecessor.

   **Número de sucessores:** O número de tarefas sucessoras (ou dependentes) do antecessor que está sendo referenciado. No exemplo acima, o antecessor que está sendo referenciado tem 1 sucessor.
