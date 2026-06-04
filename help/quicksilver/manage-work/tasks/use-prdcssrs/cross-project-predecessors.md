---
product-area: projects
navigation-topic: use-predecessors
title: Criar projetos cruzados predecessores
description: Uma Predecessora entre projetos é uma tarefa da qual outra tarefa (chamada tarefa sucessora) em outro projeto depende. O predecessor é a tarefa que tem prioridade sobre a tarefa dependente (sucessora). Por exemplo, você pode criar uma dependência que exija que a tarefa predecessora seja marcada como Concluída antes que a tarefa dependente possa ser iniciada.
author: Alina
feature: Work Management
exl-id: 7e29e589-e0a5-437e-935d-d5bc1b268594
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/zIOMy7FbFVgc700F0WyhfzazwS5ocbCgz5-9F0ohLak
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 755
ht-degree: 4%

---

# Criar predecessores entre diferentes projetos

<!--Audited: 12/2024-->

Uma predecessora entre projetos é uma tarefa da qual outra tarefa (chamada tarefa sucessora) em outro projeto depende. O predecessor é a tarefa que tem prioridade sobre a tarefa dependente (sucessora). Por exemplo, você pode criar uma dependência que exija que a tarefa predecessora seja marcada como Concluída antes que a tarefa dependente possa ser iniciada.

O Adobe Workfront permite que as tarefas sejam dependentes de tarefas em outros projetos, da mesma forma que permite predecessores em um único projeto.

>[!INFO]
>
>Por exemplo, uma empresa de escavação tem apenas uma retroescavadeira e dois projetos têm tarefas que exigem o uso da retroescavadeira. O gerente de projeto pode tornar a tarefa no primeiro projeto uma predecessora da tarefa no segundo projeto. Isso mostra que o segundo projeto pode começar a usar a retroescavadeira quando o primeiro projeto for concluído com ela.

Ao vincular projetos por meio de predecessores entre projetos, as datas do projeto principal (aquele que tem a tarefa predecessora) afetarão o projeto secundário (aquele que tem a tarefa sucessora).

>[!TIP]
>
>Você deve recalcular as linhas do tempo dos projetos para ver as datas atualizadas do projeto secundário. Para obter mais informações sobre como recalcular linhas do tempo, consulte [Configurar recálculos de linha do tempo para projetos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para obter mais informações sobre relações de predecessoras, consulte [Visão geral das predecessoras da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

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

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Standard </p> 
  
   <p>Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the projects</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Criar uma predecessora entre projetos

>[!TIP]
>
>Embora a criação de predecessores de tarefas de modelo seja semelhante à criação de predecessores de tarefas de projeto, não é possível criar predecessores entre modelos para tarefas de modelo.


1. Vá para a tarefa que será sua sucessora (tarefa dependente).
1. Clique em **Predecessores** no painel esquerdo.

   >[!TIP]
   >
   >   O administrador do Workfront ou de grupo pode remover a seção **Predecessores** ou outras seções do painel esquerdo.

1. Clique em **Adicionar Predecessora.**
1. No campo **Projeto principal**, comece digitando o nome do projeto que contém a tarefa que você deseja que seja a predecessora da tarefa atual.
1. Clique no nome quando ele aparecer na lista suspensa.
1. No campo **Tarefas**, comece digitando o nome da tarefa que você deseja que seja a predecessora da tarefa atual.
1. Especifique as seguintes informações para definir a relação entre a tarefa predecessora e a tarefa dependente:


   * **Tipo de Dependência:** Selecione a relação que você deseja que a tarefa predecessora tenha com a tarefa dependente. A relação padrão é &quot;Término-Início&quot;, o que significa que a tarefa predecessora deve terminar antes que a tarefa dependente possa iniciar. Para obter mais informações sobre os vários tipos de dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * **Atraso:** especifique a quantidade de tempo que deve decorrer após a conclusão de uma predecessora imposta até que a tarefa dependente possa começar. Para obter mais informações sobre os vários tipos de atraso, consulte [Visão geral dos Tipos de Atraso](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

   * **Imposto:** quando esta opção é selecionada, a relação de dependência entre as duas tarefas não pode ser contornada pelos usuários que iniciam as tarefas antecipadamente. Por exemplo, se você impor uma relação entre a Tarefa A e a Tarefa B, a Tarefa B não poderá ser iniciada até que a Tarefa A seja concluída. Para obter mais informações sobre como impor predecessores, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

     Quando essa opção não está selecionada, a dependência é tratada como uma sugestão para os usuários. Por exemplo, os usuários podem iniciar a Tarefa B antes que a Tarefa A seja concluída.

1. Clique em **Salvar**.

   As tarefas com predecessoras entre projetos exibem o número de referência do projeto ao qual a predecessora pertence e o número da tarefa, separado por dois pontos, na coluna Predecessoras em uma lista de tarefas.

   ![Predecessora entre projetos](assets/cross-project-predecessor-in-list-view.png)

   O ícone predecessor fica verde quando a tarefa predecessora é marcada como concluída. Isso indica que a tarefa dependente está pronta para o trabalho.

   Passe o mouse sobre esse valor para obter mais informações sobre o predecessor, o projeto e as datas. Clique no predecessor entre projetos na caixa de detalhes para abrir a tarefa.

   Clique próximo à parte superior da janela de flutuação para ver mais informações sobre o projeto do predecessor.

   Clique em **Ver projeto** para abrir o projeto do antecessor.

   ![Detalhes de predecessoras entre projetos](assets/cross-project-predecessor-details.png)

   >[!TIP]
   >
   >   A opção **Ver Projeto** é exibida somente durante a exibição de um predecessor entre projetos.

