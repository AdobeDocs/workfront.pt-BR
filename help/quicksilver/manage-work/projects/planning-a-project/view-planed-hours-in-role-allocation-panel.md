---
product-area: projects
navigation-topic: plan-a-project
title: Exibir horas planejadas do projeto no painel Alocação de função
description: Você pode visualizar a alocação de funções para todas as funções de trabalho atribuídas a itens de trabalho em um projeto no painel Alocação de funções do projeto.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 1%

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
>  Você deve ter uma licença do Planejador de cenários para ver as horas de iniciativa no painel Alocação de função. Para obter informações sobre o Planejador de cenários, consulte [Introdução ao Planejador de cenários](../../../scenario-planner/get-started-with-scenario-planning.md).
>

## Requisitos de acesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
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
</table>

-->

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso de visualização ou superior aos Projetos</p> <p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões do projeto ou superiores</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Pré-requisitos

Você deve ter o seguinte:

* Tarefas ou problemas atribuídos a funções de trabalho ou a usuários associados a uma função de trabalho.

  >[!TIP]
  >
  >Se as tarefas ou problemas tiverem atribuição cancelada, forem atribuídos a equipes ou forem atribuídos a usuários sem função de trabalho, as Horas planejadas do projeto serão zero no painel Alocação de função.

* Tarefas e problemas com uma Duração maior que zero.

## Exibir horas planejadas do projeto no painel Alocação de função

1. Clique no ícone **Menu principal** ![Ícone do Menu principal](assets/main-menu-icon.png), no canto superior direito do Adobe Workfront, e clique em **Projetos**.
1. Clique no nome de um projeto para acessá-lo. Isso abre a página Projeto.
1. Clique em uma das opções a seguir no painel esquerdo:

   * **Tarefas**
   * **Balanceador de carga de trabalho**

1. Clique no ícone ![](assets/show-role-allocation-icon.png) **Mostrar alocação de função**.

   O painel Alocação de função é exibido.

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Revise as seguintes informações no painel **Alocação de função**:

   | Campo | Descrição |
   |---|---|
   | **Função** | Funções de trabalho atribuídas a tarefas e problemas no projeto. Podem ser funções de trabalho atribuídas diretamente a tarefas e problemas ou funções de trabalho associadas a usuários atribuídos a tarefas e problemas no projeto. |
   | **Horas planejadas** | O número total de Horas Planejadas de tarefas e problemas atribuídas a funções de trabalho ou usuários associados a uma função de trabalho no projeto. |

