---
product-area: projects
navigation-topic: use-predecessors
title: Forçar Predecessoras
description: Predecessoras são tarefas das quais outras tarefas dependem para serem concluídas. As relações predecessoras afetam as datas de início e conclusão das tarefas e afetam a linha do tempo do projeto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/GRkH39mvpwOvxVqlDdiB9vgz5tMfhv5nTlsEK4iY6jM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 479
ht-degree: 6%

---

# Forçar predecessores

<!-- Audited: 11/2025 -->

Predecessoras são tarefas das quais outras tarefas dependem para serem concluídas. As relações predecessoras afetam as datas de início e conclusão das tarefas e afetam a linha do tempo do projeto.

Para obter informações sobre predecessores, consulte [Visão geral dos predecessores da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Ao definir as relações de predecessoras entre tarefas, você define como o início ou o término de uma tarefa dependente depende do início ou do término de suas tarefas predecessoras. Isso é feito usando diferentes Tipos de dependência.

Para obter informações sobre Tipos de Dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Visão geral de predecessores aplicados

>[!IMPORTANT]
>
>Você deve impor predecessores para exigir que as relações predecessoras sejam respeitadas. Sem impor as predecessoras, as tarefas dependentes podem iniciar e terminar independentemente do início e do fim de suas predecessoras, independentemente de seus Tipos de Dependência.

Você pode impor a relação da predecessora ao definir predecessores em um projeto.

Se uma predecessora for imposta, a tarefa sucessora não poderá ser iniciada antes que a predecessora seja concluída. Por exemplo, impor uma relação Término-Início entre a Tarefa A e a Tarefa B significa que a Tarefa B não pode iniciar (o Status deve permanecer Novo e a Porcentagem Concluída deve permanecer 0%) até que a Tarefa A seja marcada como concluída. A imposição de relacionamentos se aplica a todos os tipos de predecessores.

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
      <p>New: Standard</p> 
      <p>OR</p>
      <p>Current: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td><p>Manage permissions to the tasks and the project</p></td> 
  </tr> 
 </tbody> 
</table>
-->

## Forçar um predecessor no nível da tarefa

1. Vá para a tarefa sucessora cujo antecessor você deseja impor.
1. Clique em **Predecessoras** no painel esquerdo e em **Adicionar Predecessora**.
1. (Condicional) Se quiser adicionar uma predecessora entre projetos, remova o nome do projeto no campo **Projeto principal** e substitua-o por outro projeto.
1. Especifique o nome da(s) tarefa(s) predecessora(s) no campo **Tarefas**.
1. Especifique o **Tipo de Dependência** entre essas duas tarefas.

   O **Tipo de dependência** padrão é **Término-Início**.

1. Selecione o campo **Imposto** para impor o predecessor.
1. Clique em **Salvar**.

## Forçar um predecessor em uma lista de tarefas

1. Ir para uma lista de tarefas em um projeto.
1. No menu suspenso **Exibir**, selecione a **Exibição Padrão**.

1. Tome nota mental do número de tarefas que você vai designar como o antecessor.
1. Localize a tarefa sucessora cujo antecessor você deseja impor.
1. Na coluna **Predecessores**, comece inserindo o número da tarefa predecessora seguido por &quot;e&quot;. Por exemplo, digite &quot;1e&quot; para adicionar a tarefa número 1 como predecessora da tarefa selecionada.
1. Clique em Enter para salvar as informações de sua predecessora da tarefa.

   ![Lista imposta por predecessora](assets/predecessor-enforced-in-list-350x308.png)

   As informações sobre o predecessor que está sendo aplicado são salvas imediatamente.
