---
title: Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos
user-type: administrator
content-type: reference
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Este artigo explica o que acontece quando um processo de aprovação já está em uso quando um administrador do Workfront (ou um usuário com acesso administrativo aos processos de aprovação) altera sua associação com um grupo.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 77b2dce2-1523-4262-a659-0d301059a54c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 1%

---

# Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos

Este artigo explica o que acontece quando um processo de aprovação já está associado a tarefas, problemas, projetos, modelos ou tarefas de modelo e um administrador do Workfront (ou um usuário com acesso administrativo aos processos de aprovação) realiza uma das seguintes ações:

* Altera o processo de aprovação (nível de grupo) de um grupo para outro
* Altera o grupo associado ao projeto
* Altera o processo de aprovação de nível de grupo para nível de sistema
* Altera o processo de aprovação do nível do sistema para o nível do grupo

O artigo também descreve o que acontece ao mover ou copiar tarefas ou problemas associados a um processo de aprovação em nível de grupo entre dois projetos de grupos diferentes.

Para obter informações sobre os três tipos de processos de aprovação que podem ser usados no Workfront, consulte [Visão geral do processo de aprovação](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

>[!NOTE]
>
>Se o projeto, suas tarefas ou problemas já estiverem associados a um processo de aprovação em nível de grupo usando status personalizados em nível de grupo, alterar o grupo pode criar um conflito entre os status de aprovação do grupo anterior e os existentes no nível do sistema.
>
>Por exemplo, se um processo de aprovação contiver dois caminhos, um para um status de nível de sistema e um segundo para um status de nível de grupo que equivale ao mesmo status de nível de sistema, alterar o grupo do projeto original resultará em problemas da Workfront para entender o status específico do grupo que pode não existir no segundo grupo. Nesse caso, você encontrará um erro.
>
>Considere remover os processos de aprovação em nível de grupo no projeto, ou suas tarefas ou problemas, antes de atualizar o grupo do projeto.
>
>Para obter informações sobre como criar processos de aprovação de nível de grupo, consulte [Processos de aprovação de nível de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).
>
>Para obter informações sobre como criar um status personalizado em nível de grupo, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)

## Alterar um processo de aprovação específico de grupo de um grupo para outro

Os cenários a seguir ocorrem quando um processo de aprovação específico do grupo já está sendo usado em um objeto e alguém o reatribui a um grupo diferente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área ou objeto ao qual o processo de aprovação foi anexado</th> 
   <th>Objeto de aprovação</th> 
   <th>Alteração no processo de aprovação do objeto ou da área</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aprovação de projeto ou modelo </td> 
   <td>Projeto</td> 
   <td>Torna-se um processo de aprovação de uso único</td> 
  </tr> 
  <tr> 
   <td>Aprovação de tarefa ou de tarefa de modelo </td> 
   <td>Tarefa</td> 
   <td>Torna-se um processo de aprovação de uso único </td> 
  </tr> 
  <tr> 
   <td>Aprovação de problema</td> 
   <td>Problema</td> 
   <td>Torna-se um processo de aprovação de uso único</td> 
  </tr> 
  <tr> 
   <td>Área Tarefas na caixa Editar projeto ou Editar modelo</td> 
   <td>Tarefa</td> 
   <td> <p>O campo Processo de Aprovação Padrão de Tarefa é redefinido como N/D.</p> <p>Por padrão, nenhum processo de aprovação é associado às novas tarefas no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td>Seção Detalhes da fila de um projeto ou modelo</td> 
   <td>Problema</td> 
   <td> <p>O campo Aprovação padrão é redefinido para N/D.</p> <p>Por padrão, nenhum processo de aprovação é associado a novos problemas ou solicitações no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td>Seção de Tópico de Fila de um projeto ou modelo</td> 
   <td>Problema</td> 
   <td> <p>O campo Aprovação padrão é redefinido para N/D.</p> <p>Nenhum processo de aprovação está associado a novos problemas ou solicitações no projeto por padrão.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Alteração do grupo associado a um projeto

Quando alguém altera o grupo associado a um projeto para um grupo diferente, ocorre o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área ou objeto que tem o processo de aprovação já anexado</th> 
   <th>Objeto de aprovação</th> 
   <th>Alteração no processo de aprovação do objeto ou da área</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aprovação de projeto ou modelo </td> 
   <td>Projeto</td> 
   <td>Torna-se um processo de aprovação de uso único e o status associado a ele é atualizado para corresponder a um status semelhante para o novo grupo.</td> 
  </tr> 
  <tr> 
   <td>Aprovação de tarefa ou de tarefa de modelo </td> 
   <td>Tarefa</td> 
   <td>Torna-se um processo de aprovação de uso único e o status associado a ele é atualizado para corresponder a um status semelhante para o novo grupo.</td> 
  </tr> 
  <tr> 
   <td>Aprovação de problema</td> 
   <td>Problema</td> 
   <td>Torna-se um processo de aprovação de uso único e o status associado a ele é atualizado para corresponder a um status semelhante para o novo grupo.</td> 
  </tr> 
  <tr> 
   <td>Área Tarefas na caixa Editar projeto ou Editar modelo</td> 
   <td>Tarefa</td> 
   <td> <p>O campo Processo de Aprovação Padrão de Tarefa é redefinido como N/D</p> <p>Por padrão, nenhum processo de aprovação está associado às novas tarefas no projeto</p> </td> 
  </tr> 
  <tr> 
   <td>Seção Detalhes da fila de um projeto ou modelo</td> 
   <td>Problema</td> 
   <td> <p>O campo Processo de Aprovação Padrão é redefinido para N/D</p> <p>Por padrão, nenhum processo de aprovação é associado a novos problemas ou solicitações no projeto</p> </td> 
  </tr> 
  <tr> 
   <td>Seção de Tópico de Fila de um projeto ou modelo</td> 
   <td>Problema</td> 
   <td> <p>O campo Processo de Aprovação Padrão é redefinido para N/D</p> <p>Por padrão, nenhum processo de aprovação é associado a novos problemas ou solicitações no projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

## Alterando um processo de aprovação de nível de grupo para nível de sistema

Quando alguém altera a opção Grupo em um processo de aprovação específico do grupo para &quot;Todos os grupos&quot;, o processo de aprovação se torna geral do sistema e ocorre o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área ou objeto ao qual o processo de aprovação foi anexado</th> 
   <th>Objeto de aprovação</th> 
   <th>Alteração no processo de aprovação do objeto ou da área</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Aprovação de projeto ou modelo </td> 
   <td>Projeto</td> 
   <td>Sem alterações</td> 
  </tr> 
  <tr> 
   <td>Aprovação de tarefa ou de tarefa de modelo </td> 
   <td>Tarefa</td> 
   <td>Sem alterações</td> 
  </tr> 
  <tr> 
   <td>Aprovação de problema</td> 
   <td>Problema</td> 
   <td>Sem alterações</td> 
  </tr> 
  <tr> 
   <td>Área Tarefas na caixa Editar projeto ou Editar modelo</td> 
   <td>Tarefa</td> 
   <td> <p>Nenhuma alteração no processo de aprovação, mas, por padrão, ele está associado às novas tarefas no projeto</p> </td> 
  </tr> 
  <tr> 
   <td>Seção Detalhes da fila de um projeto ou modelo</td> 
   <td>Problema</td> 
   <td> <p>Nenhuma alteração no processo de aprovação, mas, por padrão, está associada a novos problemas ou solicitações no projeto</p> </td> 
  </tr> 
  <tr> 
   <td>Seção de Tópico de Fila de um projeto ou modelo</td> 
   <td>Problema</td> 
   <td> <p>Nenhuma alteração no processo de aprovação, mas, por padrão, está associada a novos problemas ou solicitações no projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

## Alterando um processo de aprovação do nível do sistema para o nível do grupo

Quando alguém altera a disponibilidade de um processo de aprovação em todo o sistema de &quot;Todos os grupos&quot; para um grupo específico, o processo de aprovação se torna específico do grupo e ocorre o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Área ou objeto ao qual o processo de aprovação foi anexado</th> 
   <th>Objeto de aprovação</th> 
   <th>Alteração no processo de aprovação do objeto ou da área</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projeto, tarefa, problema, modelo ou tarefa de modelo que pertence ao grupo do processo de aprovação</td> 
   <td> <p>Projeto, tarefa ou problema</p> </td> 
   <td>Sem alterações</td> 
  </tr> 
  <tr> 
   <td>Área Tarefas na caixa Editar projeto ou Editar modelo para um projeto ou modelo que pertence ao grupo do processo de aprovação</td> 
   <td>Tarefa</td> 
   <td> <p>Nenhuma alteração no processo de aprovação, mas, por padrão, ele está associado às novas tarefas no projeto</p> </td> 
  </tr> 
  <tr> 
   <td>Seção Detalhes da fila para um projeto ou modelo que pertence ao grupo do processo de aprovação</td> 
   <td>Problema</td> 
   <td> <p>Nenhuma alteração no processo de aprovação, mas, por padrão, está associada a novos problemas ou solicitações no projeto</p> </td> 
  </tr> 
  <tr> 
   <td>Seção de Tópico de Fila para um projeto ou modelo que pertence ao grupo do processo de aprovação</td> 
   <td>Problema</td> 
   <td> <p>Nenhuma alteração no processo de aprovação, mas, por padrão, está associada a novos problemas ou solicitações no projeto</p> </td> 
  </tr> 
  <tr> 
   <td>Projeto, tarefa, problema, modelo ou tarefa de modelo que pertence a um grupo diferente do grupo do processo de aprovação</td> 
   <td> <p>Projetos</p> <p>Tarefas</p> <p>Problemas</p> </td> 
   <td>Torna-se um processo de aprovação de uso único</td> 
  </tr> 
  <tr> 
   <td>Área Tarefas na caixa Editar projeto ou Editar modelo para um projeto ou modelo que pertence a um grupo diferente do grupo do processo de aprovação</td> 
   <td>Tarefas</td> 
   <td> <p>O campo Processo de Aprovação Padrão de Tarefa é redefinido como N/D.</p> <p>Por padrão, nenhum processo de aprovação é associado às novas tarefas no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td>Seção Detalhes da Fila para um projeto ou modelo que pertence a um grupo diferente do grupo do processo de aprovação</td> 
   <td>Problemas</td> 
   <td> <p>O campo Aprovação padrão é redefinido para N/D.</p> <p>Por padrão, nenhum processo de aprovação é associado a novos problemas ou solicitações no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td>Seção de Tópico de Fila para um projeto ou modelo que pertence a um grupo diferente do grupo do processo de aprovação</td> 
   <td>Problemas</td> 
   <td> <p>O campo Aprovação padrão é redefinido para N/D.</p> <p>Por padrão, nenhum processo de aprovação é associado a novos problemas ou solicitações no projeto.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Mover ou copiar uma tarefa ou um problema para um projeto com um grupo diferente daquele do processo de aprovação

Mover ou copiar uma tarefa ou um problema de um projeto para outro pode afetar os processos de aprovação existentes na tarefa ou no problema, dependendo dos grupos dos dois projetos. A tabela a seguir ilustra os cenários que podem existir:

| Processo original de aprovação de tarefas ou problemas | Grupos dos dois projetos | Alterações no processo de aprovação depois que a tarefa ou o problema é movido para outro projeto |
|---|---|---|
| Processo de aprovação de uso único associado a um status em todo o sistema | Os projetos estão no mesmo grupo ou em grupos diferentes | Sem alterações |
| Processo de aprovação de uso único associado a um status específico de grupo | Os projetos estão em grupos diferentes | A aprovação permanece como um processo de aprovação de uso único e o status associado às atualizações de aprovação para corresponder a um status semelhante para o novo grupo. |
| Processo de aprovação do sistema inteiro | Os projetos estão no mesmo grupo ou em grupos diferentes | Sem alterações |
| Processo de aprovação específico do grupo | Os projetos estão no mesmo grupo | Sem alterações |
| Processo de aprovação específico do grupo | Os projetos estão em grupos diferentes e os grupos têm status diferentes para grupos específicos | A aprovação se torna um processo de aprovação de uso único e o status associado às atualizações de aprovação para corresponder a um status semelhante para o novo grupo. |
| Processo de aprovação específico do grupo | Os projetos estão em grupos diferentes e há um status com a mesma chave no novo grupo que o status associado ao processo de aprovação do primeiro grupo | Sem alterações |
