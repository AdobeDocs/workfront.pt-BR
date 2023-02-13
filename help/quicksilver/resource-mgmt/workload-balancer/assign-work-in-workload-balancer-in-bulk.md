---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Atribua trabalho em massa usando o Balanceador de Carga de Trabalho
description: Você pode atribuir itens de trabalho manualmente a usuários usando o Balanceador de Carga de Trabalho do Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: 10b905c8a66f2507cbfac7c15a01f38d40ab3e00
workflow-type: tm+mt
source-wordcount: '1545'
ht-degree: 2%

---

# Atribua trabalho em massa usando o Balanceador de Carga de Trabalho

<!--drafted
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 
-->

Você pode atribuir itens de trabalho manualmente a usuários usando o Balanceador de Carga de Trabalho do Adobe Workfront.

Para obter informações gerais sobre como atribuir trabalho a usuários usando o Balanceador de Carga de Trabalho, consulte [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

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
   <td> <p>Planejar, ao usar o Balanceador de Carga de Trabalho para uma equipe ou na área Recursos </p>
   <p>Trabalhe, ao usar o Balanceador de Carga de Trabalho de um projeto </p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Edite o acesso ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Tarefas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribua com permissões ou superior para projetos, tarefas e problemas que incluem Fazer atribuições</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações para fazer atribuições em massa no Balanceador de Carga de Trabalho

* Você pode gerenciar rapidamente as atribuições de usuários de várias tarefas e problemas em um ou mais projetos. As alterações nas atribuições são visíveis no Balanceador de Carga de Trabalho imediatamente.
* Não é possível atribuir recursos a itens de trabalho concluídos ou a itens que estejam em um projeto concluído.
* Você pode fazer o seguinte ao atribuir usuários em massa:

   * Atribua um usuário a todos os itens de trabalho atribuídos a uma função de trabalho no momento.
   * Substituir atribuições de usuário entre usuários.
   * Cancele a atribuição de um usuário de todos os seus itens de trabalho.

**EXEMPLOS**

* Você é responsável por fazer atribuições de usuários em vários novos projetos. Os projetos foram originalmente criados a partir de modelos e as funções de trabalho já estão atribuídas às várias tarefas dentro dos projetos. Você deseja atribuir um usuário específico, Jackie Simms, a todas as tarefas atribuídas a uma função de trabalho no momento. Você pode usar a função Atribuir para atribuir essas tarefas a Jackie Simms.
* 45 tarefas em 3 projetos diferentes são atribuídas a Jackie Simms. Jackie deixa a organização e agora você precisa reatribuir suas tarefas a outro usuário. Você pode usar a função Replace para atribuir essas tarefas à nova pessoa.
* 10 tarefas em 2 projetos diferentes são atribuídas a outro usuário, Rick Kuvec. Você percebe que o Rick foi atribuído a essas tarefas com erro, mas não tem certeza de quem elas precisam ser atribuídas no momento. Você precisa cancelar a atribuição do Rick a todas as tarefas ao mesmo tempo. Você pode usar a função Cancelar atribuição para remover o Rick dessas tarefas.

## Atribuir trabalho em massa no Balanceador de Carga de Trabalho

1. Vá para o Balanceador de Carga de Trabalho onde deseja atribuir trabalho.

   Você pode atribuir trabalhos a usuários usando o Balanceador de Carga de Trabalho na área Recursos, no projeto ou no nível da equipe. Para obter mais informações sobre onde o Balanceador de Carga de Trabalho está localizado no Workfront, consulte [Localizar o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Clique em **Atribuições em massa** ![](assets/bulk-assignments-wb.png) na parte superior do Balanceador de Carga de Trabalho.

   O painel Atribuições em massa é aberto à direita do Balanceador de Carga de Trabalho.

1. (Condicional) Se você estiver acessando o Balanceador de Carga de Trabalho na área Recursos ou para uma equipe, expanda a **Projeto: Nome** menu suspenso e use os modificadores de filtro para selecionar o projeto ou projetos para os quais deseja fazer atribuições. Você pode selecionar projetos por Nome (essa é a opção padrão) ou por Status.

Para obter informações sobre modificadores de filtro Workfront, consulte [Filtros e modificadores de condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>O Nome do projeto é selecionado por padrão quando você acessa o Balanceador de carga de trabalho de um projeto.

![](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. (Opcional) Clique em **Selecionar tarefas do projeto** para selecionar a tarefa ou tarefas para as quais deseja fazer atribuições e, em seguida, no **Tarefa: Nome** no menu suspenso, selecione tarefas por Nome (essa é a opção padrão) ou Status e use os modificadores de filtro para pesquisar tarefas específicas.

Para obter informações sobre modificadores de filtro Workfront, consulte [Filtros e modificadores de condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

>[!NOTE]
>
>Não é possível selecionar tarefas em um status Concluído.

![](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

>[!TIP]
>
>Deixe essa seleção em branco se desejar fazer atribuições em massa para problemas, bem como tarefas.

1. (Opcional) Clique no botão **Excluir** ícone ![](assets/delete.png) ao lado de um dos critérios selecionados

   Ou

   Clique em **Limpar tudo** no canto superior direito do painel Atribuições em massa para remover todas as seleções.

1. Selecione uma das opções a seguir e continue com as etapas descritas abaixo:

   * [Atribuir usuário](#assign-user)
   * [Substituir usuário](#replace-user)
   * [Retirar atribuição de usuário](#unassign-user)

   >[!TIP]
   >
   >Se nenhum item corresponder aos filtros selecionados, essas opções estarão esmaecidas.

### Atribuir usuário {#assign-user}

Quando você atribui um usuário usando Atribuições em massa no Balanceador de Carga de Trabalho, as seguintes coisas ocorrem:

* Um usuário é atribuído a todos os itens de trabalho atualmente atribuídos a uma função especificada nos projetos selecionados.
* O usuário não é atribuído aos seguintes tipos de itens de trabalho:

   * Itens já atribuídos a um usuário.
   * Itens concluídos.

* Se o usuário selecionado não estiver associado à função especificada, a função será substituída pelo usuário na Função primária do usuário.

Para atribuir um usuário a itens de trabalho atribuídos anteriormente a funções de trabalho:

1. Comece a atribuir itens de trabalho usando Atribuições em massa no Balanceador de Carga de Trabalho conforme descrito acima e selecione **Atribuir**.

1. No **Atribuição de função** , clique na seta suspensa para escolher em uma lista de funções. Somente as funções atribuídas atualmente nos projetos especificados são exibidas. Este campo é obrigatório.

   ![](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. No **Usuário a ser atribuído** , clique na seta suspensa para escolher em uma lista de usuários sugeridos ou para digitar o nome de outro usuário.

   Selecione usuários nas seguintes áreas:

   * **Atribuições sugeridas**: Usuários que podem cumprir a função selecionada e que correspondem aos critérios de Atribuições inteligentes. Para obter mais informações, consulte [Visão geral de atribuições inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Outras Atribuições**: Todos os usuários do sistema que podem atender à função selecionada.

      >[!TIP]
      >
      >Somente os primeiros 50 usuários são listados na área Outras Atribuições.
   Depois de selecionar um usuário, o Workfront exibe uma observação sobre o número de itens aos quais o usuário especificado será atribuído e qual função de trabalho ele substituirá.

   >[!TIP]
   >
   >Todas as funções do usuário são exibidas na lista, sob o nome do usuário.


1. Clique em **Atribuir**.

   As funções especificadas são substituídas pelos usuários selecionados.

   Você recebe uma confirmação de quantos itens de trabalho tiveram a função selecionada substituída pelo usuário selecionado.

   ![](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### Substituir usuário {#replace-user}

Você pode substituir um usuário que já esteja atribuído aos itens de trabalho por outro usuário nos projetos selecionados.

Quando você substitui um usuário por outro usando Atribuições em massa no Balanceador de Carga de Trabalho, as seguintes coisas ocorrem:

* O usuário substituto é atribuído a todos os itens de trabalho atribuídos a um usuário original nos projetos selecionados.

* O novo usuário não é atribuído a nenhum item de trabalho que já esteja marcado como Concluído.
* Se a função associada ao primeiro usuário não corresponder a nenhuma das funções do segundo usuário, o segundo usuário será atribuído em sua Função primária.

Para substituir um usuário por outro usuário:

1. Comece a atribuir itens de trabalho no Balanceador de Carga de Trabalho conforme descrito acima e selecione **Substituir**.
1. No **Usuário atribuído no momento** , clique na seta suspensa para escolher em uma lista de usuários. Somente os usuários atualmente atribuídos a itens de trabalho incompletos nos projetos especificados são exibidos. Este campo é obrigatório.

   ![](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. No **Usuário a ser atribuído** , clique na seta suspensa para escolher em uma lista de usuários sugeridos ou para digitar outro nome de usuário. Os usuários listados na lista por padrão correspondem aos critérios de Atribuições inteligentes. Para obter mais informações, consulte [Visão geral de atribuições inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   O Workfront exibe uma observação sobre o número de itens em que o usuário atribuído no momento substituirá o segundo usuário e quais funções ele substituirá.

   ![](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. Clique em **Substituir**.

   O primeiro usuário selecionado é substituído pelo segundo usuário em todos os itens de trabalho do projeto selecionado.

   Você recebe uma confirmação de quantos itens de trabalho tiveram a atribuição original do usuário substituída pelo segundo usuário selecionado.

### Retirar atribuição de usuário {#unassign-user}

Você pode cancelar a atribuição de um usuário de todos os itens de trabalho aos quais o usuário está atribuído nos projetos selecionados.

Quando você cancela a atribuição de um usuário de todas as suas atribuições usando Atribuições em massa no Balanceador de Carga de Trabalho, as seguintes coisas ocorrem:

* O usuário especificado é removido de todos os itens de trabalho aos quais está atribuído.
* Se o usuário não atribuído estiver associado a funções de trabalho, as funções de trabalho permanecerão atribuídas aos itens de trabalho quando o usuário for removido.

* Se o usuário especificado for atribuído a itens de trabalho concluídos, ele permanecerá atribuído a esses itens de trabalho.

Para obter mais informações sobre atribuições de usuário e função de trabalho, consulte [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para cancelar a atribuição de um usuário a partir de itens de trabalho nos projetos selecionados ou para as tarefas ou problemas selecionados onde eles são atribuídos:

1. Comece a atribuir itens de trabalho no Balanceador de Carga de Trabalho conforme descrito acima e selecione **Cancelar atribuição**.

1. No **Usuário para cancelar atribuição** , clique na seta suspensa para escolher em uma lista de usuários. Somente os usuários atualmente atribuídos a itens de trabalho incompletos nos projetos especificados são exibidos. Este campo é obrigatório.

   ![](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   O Workfront exibe uma observação sobre o número de itens em que o usuário atribuído no momento não será atribuído.

   ![](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. Clique em **Cancelar atribuição**.\
   Você recebe uma confirmação sobre o número de itens de trabalho onde o usuário especificado foi removido.

 
