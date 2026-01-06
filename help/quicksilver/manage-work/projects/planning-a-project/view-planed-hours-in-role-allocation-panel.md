---
product-area: projects
navigation-topic: plan-a-project
title: Exibir horas planejadas do projeto no painel Alocação de função
description: Você pode visualizar a alocação de funções para todas as funções de trabalho atribuídas a itens de trabalho em um projeto no painel Alocação de funções do projeto.
author: Alina, Lisa
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 5%

---

# Exibir horas planejadas do projeto no painel Alocação de função

Você pode visualizar a alocação de funções para todas as funções de trabalho atribuídas a itens de trabalho em um projeto no painel Alocação de funções do projeto.

>[!NOTE]
>
>Este artigo se refere à exibição das funções de trabalho associadas a tarefas e problemas em um projeto e suas Horas planejadas alocadas no painel Alocação de função de um projeto. Para obter informações sobre como reconciliar Horas planejadas com horas de iniciativas usando o Painel Alocação de função ao usar o Planejador de cenários do Adobe Workfront, consulte o seguinte:
>
>* [Mostrar alocação de funções para projetos e iniciativas na lista de tarefas](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Mostrar alocação de funções para projetos e iniciativas no Balanceador de Carga de Trabalho](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Você deve ter uma licença do Planejador de cenários para ver as horas de iniciativa no painel Alocação de função. Para obter informações sobre o Planejador de cenários, consulte [Introdução ao Planejador de cenários](../../../scenario-planner/get-started-with-scenario-planning.md).
>
>Se sua empresa comprou o Planejador de cenários da Adobe no passado, ele não tem mais direitos. O Planejador de cenários não está mais disponível para compra.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Adobe Workfront Ultimate</p>
   <p>Ultimate de fluxo de trabalho do Adobe</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Leve ou superior</p>
   <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de visualização ou superior aos Projetos</p>
   <p>Editar acesso ao Planejador de cenários para atualizar horas nas iniciativas</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões do projeto ou superiores</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

able style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Pré-requisitos

Você deve ter o seguinte:

* Tarefas ou problemas atribuídos a funções de trabalho ou a usuários associados a uma função de trabalho.

  >[!TIP]
  >
  >Se as tarefas ou problemas tiverem atribuição cancelada, forem atribuídos a equipes ou forem atribuídos a usuários sem função de trabalho, as Horas planejadas do projeto serão zero no painel Alocação de função.

* Tarefas e problemas com uma Duração maior que zero.

## Exibir horas planejadas do projeto no painel Alocação de função

{{step1-to-projects}}

1. Clique no nome de um projeto para acessá-lo. Isso abre a página Projeto.
1. Clique em uma das opções a seguir no painel esquerdo:

   * **Tarefas**
   * **Balanceador de carga de trabalho**

1. Clique no ícone **Mostrar alocação de função** ![Mostrar ícone de alocação de função](assets/show-role-allocation-icon.png).

   O painel Alocação de função é exibido.

   ![Painel de alocação de funções somente com horas planejadas](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Revise as seguintes informações no painel **Alocação de função**:

   | Campo | Descrição |
   |---|---|
   | **Função** | Funções de trabalho atribuídas a tarefas e problemas no projeto. Podem ser funções de trabalho atribuídas diretamente a tarefas e problemas ou funções de trabalho associadas a usuários atribuídos a tarefas e problemas no projeto. |
   | **Horas planejadas** | O número total de Horas Planejadas de tarefas e problemas atribuídas a funções de trabalho ou usuários associados a uma função de trabalho no projeto. |

