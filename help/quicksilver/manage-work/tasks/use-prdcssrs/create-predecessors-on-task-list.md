---
product-area: projects
navigation-topic: use-predecessors
title: Criar uma relação de predecessora na lista de tarefas
description: É possível usar tarefas predecessoras (ou apenas predecessoras) para vincular tarefas que dependem de outras tarefas para serem iniciadas ou concluídas. Por exemplo, você não gostaria de hospedar um participante (tarefa dependente) antes de enviar os convites (tarefa predecessora).
author: Alina
feature: Work Management
exl-id: a84d88ac-8dd4-4952-b83f-02fafa61e68b
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# Criar uma relação de predecessora na lista de tarefas

É possível usar tarefas predecessoras (ou apenas predecessoras) para vincular tarefas que dependem de outras tarefas para serem iniciadas ou concluídas. Por exemplo, você não gostaria de hospedar um participante (tarefa dependente) antes de enviar os convites (tarefa predecessora).

Este artigo mostra como criar predecessores na lista de tarefas.

É possível exibir os predecessores das tarefas nas seguintes áreas do Adobe Workfront:

* Na lista de tarefas da coluna Predecessores.
* No gráfico de Gantt
* Na seção Predecessoras de uma tarefa dependente

Para obter mais informações, consulte [Visão geral dos predecessores da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Requisitos de acesso

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
   <td> <p>Novo: Padrão </p><p>Atual: Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront. Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Criar um predecessor

1. Ir para um projeto.
1. Clique em **Tarefas** no painel esquerdo.
1. Certifique-se de que o modo de exibição atual exiba a coluna **Predecessor**.

   Se a exibição não mostrar a coluna Predecessores, altere para uma exibição que sim ou adicione a coluna à exibição.

1. Selecione a tarefa que deseja designar como a tarefa dependente.
1. Clique dentro da coluna **Predecessores**.
1. Digite o número da tarefa que você deseja designar como predecessora da tarefa selecionada e pressione **Enter**.

   >[!TIP]
   >
   >Para adicionar uma predecessora entre projetos, faça o seguinte:
   >
   >1. Clique no ícone **Modo de Plano** e escolha **Salvamento Automático**.
   >
   >1. Digite o Número de Referência do projeto do antecessor seguido por dois pontos e o número da tarefa. Por exemplo, digite: 765021:12. Isso indica que o número de referência do projeto do antecessor é 765021 e o antecessor é a tarefa número 12 no projeto.
   >
   >1. Adicione o tipo de dependência para este predecessor. Para obter mais informações, consulte [Criar predecessores entre projetos](/help/quicksilver/manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
   >
   >Pressione **Enter**.
   >
   >**IMPORTANTE**
   >
   >Não é possível adicionar predecessoras entre projetos quando a lista de tarefas é exibida no modo de salvamento Manual.

   O ícone predecessor fica verde quando a tarefa predecessora é marcada como concluída. Isso indica que a tarefa dependente está pronta para o trabalho.

   Para obter mais informações sobre os tipos de relação disponíveis na coluna Predecessores, consulte [Visão geral dos predecessores da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md) em [Visão geral dos predecessores da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Exibir detalhes da predecessora

Você pode visualizar rapidamente os detalhes sobre o predecessor na lista de tarefas.

1. Na lista de tarefas, passe o mouse sobre o número do predecessor na coluna **Predecessores**.

   Uma caixa com os detalhes do antecessor é exibida.

   ![Detalhes do predecessor](assets/predecessor-details-in-task-list.png)

   Os seguintes detalhes são exibidos:

   **Nome do predecessor:** O nome do predecessor que está sendo referenciado. O número da tarefa do antecessor é incluído. Clique no nome da tarefa para abri-la. No exemplo acima, o antecessor é Produção/Execução/Entrega.

   **Nome do projeto:** O nome do projeto no qual o antecessor reside. O projeto é identificado como o projeto atual se o predecessor pertencer aos mesmos projetos que a tarefa, ou como um projeto cruzado, se o predecessor pertencer a um projeto diferente. No exemplo acima, o nome do projeto é Produção de ativos digitais (integrada) - Projeto. Para obter mais informações sobre predecessores entre projetos, consulte [Criar predecessores entre projetos](../../tasks/use-prdcssrs/cross-project-predecessors.md).

   Você pode expandir os detalhes do projeto para ver as datas de início e término planejadas do projeto, a condição, o status, o percentual concluído e o proprietário. Para um projeto cruzado, você pode clicar em **Ver Projeto** para abrir o projeto.

   **ID:** O número de referência do projeto onde a predecessora está localizada.

   **Início Planejado:** A Data de Início Planejada da tarefa predecessora.

   **Fim Planejado:** A Data de Término Planejada da tarefa predecessora.

   **Número de predecessores:** O número de predecessores do predecessor que está sendo referenciado. No exemplo acima, o predecessor que está sendo referenciado tem 1 predecessor.

   **Número de sucessores:** o número de tarefas sucessoras (ou dependentes) para a predecessora que está sendo referenciada. No exemplo acima, o antecessor que está sendo referenciado tem 1 sucessor.
