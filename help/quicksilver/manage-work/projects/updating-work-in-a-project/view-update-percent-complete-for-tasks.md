---
product-area: projects
navigation-topic: update-work-in-a-project
title: Exibir e atualizar o Percentual Concluído das tarefas
description: Você pode atualizar o percentual concluído de uma tarefa para indicar o progresso feito na tarefa em sua conclusão.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Exibir e atualizar o Percentual Concluído das tarefas

Você pode atualizar o percentual concluído de uma tarefa para indicar o progresso feito na tarefa em sua conclusão.

## Requisitos de acesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para atualizar tarefas manualmente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para a tarefa</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.


## Áreas em que é possível atualizar o percentual concluído de uma tarefa

Você pode atualizar o percentual concluído de uma tarefa em qualquer uma das seguintes áreas:

* **Em uma lista de tarefas**: É possível atualizar o percentual concluído de uma tarefa quando a coluna Percentual concluído é exibida.\
  Para obter mais informações sobre edição em linha, consulte [Itens de edição em linha em uma lista no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **Na visualização Marco**: é possível atualizar o percentual concluído de uma tarefa ao usar a visualização Marco em uma lista de projetos ou em um relatório de projeto. Para obter mais informações, consulte [Usar a visualização de Etapas](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Conforme você atualiza a tarefa**: é possível atualizar a opção de percentual concluído de uma tarefa ao adicionar uma atualização à tarefa.

  >[!IMPORTANT]
  >
  >Essa opção é exibida somente após a ativação da opção Mostrar porcentagem concluída.\
  >Para ativar a barra de atualização percentual concluído para tarefas, faça o seguinte:
  >
  >1. Vá para a **Principal** menu>seu nome>**Mais** ícone ao lado do seu nome >**Editar** > selecionar **Mostrar o percentual concluído em atualização de status**.\
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >

* **No cabeçalho da tarefa**: é possível atualizar o percentual concluído de uma tarefa no cabeçalho da tarefa. Para obter informações, consulte [Editar tarefas](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## Considerações sobre a atualização do percentual concluído de uma tarefa

* Quando você marca uma tarefa como 100% concluída, o Status da tarefa é atualizado para Concluído.
* Existem os seguintes cenários para tarefas pai:
   * Não é possível atualizar o percentual concluído de uma tarefa pai para 100% quando o Modo de Conclusão em Resumo do projeto está definido como Automático e as subtarefas não estão concluídas.
   * Você pode atualizar o percentual concluído de uma tarefa pai para 100% quando o Modo de Conclusão em Resumo do projeto estiver definido como Manual e as subtarefas estiverem concluídas ou incompletas.

  Para obter mais informações, consulte [Editar projetos](../manage-projects/edit-projects.md).

## Atualizar o percentual concluído de uma tarefa

1. Vá para qualquer uma das seguintes áreas no Workfront:

   * Uma lista de tarefas
   * Uma lista de projetos e aplicar a visualização Marco
   * Uma tarefa, acessando a página de tarefas
1. Localize o **Percentual Completo** campo da tarefa cuja porcentagem concluída você deseja atualizar.
1. Clique dentro do campo Percentual concluído e digite um número entre 0 e 100

   Ou

   Clique e arraste o **Percentual Completo** barra para o número necessário para indicar quanto da tarefa você concluiu.

   >[!NOTE]
   >
   >Quando você indica que 100% da tarefa está concluída, o status da tarefa também é atualizado para Concluído.


1. Pressione Enter no teclado para salvar a porcentagem concluída.

