---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Permitir atribuições de usuários independentemente da função e associação de grupo nas áreas de Programação
description: No Agendamento de Recursos, as atribuições só podem ser feitas a usuários que tenham uma função definida em seu perfil de usuário que corresponda à atribuição de função da tarefa ou problema que está sendo atribuído a eles.
author: Alina
feature: Resource Management
exl-id: 0f90ffde-6f07-4c3c-b963-de28b1b55dc1
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---

# Permitir atribuições de usuários independentemente da função e associação de grupo nas áreas de Programação

>[!IMPORTANT]
>  
><span class="preview">A funcionalidade de Agendamento descrita neste artigo foi descontinuada e removida do Adobe Workfront a partir da versão 23.1 em janeiro de 2023.   </span>
>  
> <span class="preview"> Este artigo também será removido logo após a versão 23.1, no início de 2023. Nesse momento, recomendamos que você atualize todos os marcadores adequadamente. </span>
> 
><span class="preview"> Agora você pode usar o Balanceador de Carga de Trabalho para agendar o trabalho de seus recursos. </span>
>  
> <span class="preview">Para obter informações sobre como programar recursos usando o Balanceador de Carga de Trabalho, consulte a seção [O Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer.</span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE:&nbsp;***LINKED TO THE UI FROM Resource Scheduling (People> Teams>Working On>Settings>Limit Assignments to the Group Associated with the Project) - ALSO FROM THE WORKING ON TAB OF TEAMS and AT THE PROJECT STAFFING TAB TOO)</p>
<p>NOTE: Alina; broken off the original article; retitle, reformat, relink sections) </p>
</div>
-->

Por padrão, as atribuições só podem ser feitas a usuários que tenham uma função definida em seu perfil de usuário que corresponda à atribuição de função da tarefa ou problema que está sendo atribuído a eles ao usar as ferramentas de Agendamento de Recursos.

Você pode configurar o Adobe Workfront para permitir que tarefas e problemas sejam atribuídos a qualquer usuário, independentemente de esse usuário ter uma função definida em seu perfil de usuário que corresponda à atribuição de função da tarefa ou problema que está sendo atribuído a ele. Quando você atribui um usuário a uma tarefa ou ocorrência e esse usuário não tem uma função que corresponda à atribuição de função na tarefa ou ocorrência, a atribuição de função original é removida e a atribuição de função é alterada para a função do usuário que você está atribuindo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso a Projetos, Tarefas e Problemas</p> <p><strong>Nota</strong>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribua com permissões ou mais para projetos, tarefas e problemas para os quais você atualiza atribuições</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Permitir atribuições a usuários independentemente da função

1. Vá para a linha do tempo de agendamento para vários projetos, para um projeto individual ou para uma equipe:

   * **Para vários projetos**:  Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para um projeto individual**: Vá para um projeto e clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para uma equipe**: Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.

1. Clique no botão **Configurações** na linha do tempo de agendamento.
1. Desativar a opção **Limitar Atribuições a Usuários com Função Correspondente**.
1. Clique em **Retornar ao agendamento**.

## Permitir atribuições a usuários independentemente da associação a grupos

<!--
<p>(NOTE: Alina: **^ This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!!) </p>
-->

Por padrão, as atribuições só podem ser feitas a usuários que sejam membros do grupo associado ao projeto (esse é o grupo definido ao editar o projeto).

>[!IMPORTANT]
>
>Essa configuração considera somente os membros do grupo associado ao projeto, e não os membros de qualquer subgrupo desse grupo.

Você pode configurar o Workfront para permitir que tarefas e problemas sejam atribuídos a qualquer usuário, independentemente de esse usuário ser membro do grupo associado ao projeto em que a tarefa ou problema reside.

1. Vá para a linha do tempo de agendamento para vários projetos, para um projeto individual ou para uma equipe:

   * **Para vários projetos**:  Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para um projeto individual**: Vá para um projeto e clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para uma equipe**: Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.

1. Clique no botão **Configurações** na linha do tempo de agendamento.
1. Desativar a opção **Limitar Atribuições ao Grupo Associado ao Projeto**.
1. Clique em **Retornar ao agendamento**.

 
