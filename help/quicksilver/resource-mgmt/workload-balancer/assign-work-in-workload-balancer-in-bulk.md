---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Atribuir trabalho em massa usando o Balanceador de carga de trabalho
description: Você pode atribuir recursos a várias tarefas e problemas em massa usando o Balanceador de carga de trabalho do Adobe Workfront.
author: Lisa
feature: Resource Management
exl-id: fb0f80d3-7da4-4f5f-857d-3fb518ba12e2
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '1551'
ht-degree: 1%

---

# Atribuir trabalho em massa usando o Balanceador de carga de trabalho

<!--Audited: 07/2024-->

Você pode atribuir recursos a várias tarefas e problemas em massa usando o Balanceador de carga de trabalho do Adobe Workfront.

Para obter informações gerais sobre como atribuir trabalho a usuários usando o Balanceador de carga de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: plano, ao usar o Balanceador de Carga de Trabalho na área Recursos;</br>
       Trabalhar, ao usar o Balanceador de carga de trabalho de uma equipe ou projeto</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso ao seguinte:</p> 
    <ul> 
     <li>Gerenciamento de recursos</li> 
     <li>Projetos</li> 
     <li>Tarefas</li> 
     <li>Problemas</li> 
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Contribuir com permissões ou mais altas para projetos, tarefas e problemas que incluem Fazer atribuições</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para fazer atribuições em massa no Balanceador de carga de trabalho

* Você pode gerenciar rapidamente as atribuições de usuários para várias tarefas e problemas em um ou mais projetos. As alterações nas atribuições ficam visíveis no Balanceador de carga de trabalho imediatamente.
* Não é possível atribuir recursos a itens de trabalho que estão concluídos ou a itens que estão em um projeto concluído.
* Você pode fazer o seguinte ao atribuir usuários em massa:

   * Atribua um usuário a todos os itens de trabalho atualmente atribuídos a uma função de trabalho.
   * Substituir atribuições de usuário entre usuários.
   * Cancele a atribuição de um usuário de todos os seus itens de trabalho.

**EXEMPLOS**

* Você é responsável por fazer atribuições de usuários em vários projetos novos. Os projetos foram originalmente criados a partir de modelos e as funções de trabalho já estão atribuídas a várias tarefas nos projetos. Você deseja atribuir um usuário específico, Jackie Simms, a todas as tarefas atualmente atribuídas a uma função de trabalho. Você pode usar a função Atribuir para atribuir essas tarefas a Jackie Simms.
* 45 tarefas em 3 projetos diferentes são atribuídas a Jackie Simms. Jackie deixa a organização, e agora você precisa reatribuir suas tarefas para outro usuário. Você pode usar a função Substituir para atribuir essas tarefas à nova pessoa.
* Dez tarefas em dois projetos diferentes são atribuídas a outro usuário, Rick Kuvec. Você percebe que Rick foi designado para essas tarefas por engano, mas você não tem certeza de a quem eles precisam ser atribuídos neste momento. Você precisa desatribuir Rick para todas as tarefas ao mesmo tempo. Você pode usar a função Cancelar atribuição para remover Rick dessas tarefas.

## Atribuir trabalho em massa no Balanceador de carga de trabalho

1. Vá para o Balanceador de carga de trabalho onde deseja atribuir trabalho.

   Você pode atribuir trabalho aos usuários usando o Balanceador de carga de trabalho na área Recursos, no projeto ou no nível da equipe. Para obter mais informações sobre onde o Balanceador de carga de trabalho está localizado na Workfront, consulte [Localizar o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).


1. Clique em **Atribuições em massa** ![Atribuições em massa](assets/bulk-assignments-wb.png) na parte superior do Balanceador de carga de trabalho.

   O painel Atribuições em massa é aberto à direita do Balanceador de carga de trabalho.

1. (Condicional) Se você estiver acessando o Balanceador de carga de trabalho da área de Recursos ou de uma equipe, expanda o menu suspenso **Projeto: Nome** e use os modificadores de filtro para selecionar o projeto ou projetos para os quais deseja fazer atribuições. Você pode selecionar projetos por Nome (esta é a opção padrão) ou por Status.

   Para obter informações sobre modificadores de filtro Workfront, consulte [Filtros e modificadores de condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >O Nome do projeto é selecionado por padrão quando você acessa o Balanceador de carga de trabalho de um projeto.

   ![Nome do projeto em atribuições em massa](assets/project-name-status-dropdown-bulk-assignments-wb-nwe-350x133.png)

1. (Opcional) Clique em **Selecionar tarefas do projeto** para selecionar a(s) tarefa(s) para a(s) qual(is) você deseja fazer atribuições. Em seguida, no menu suspenso **Tarefa: Nome**, selecione as tarefas por Nome (esta é a opção padrão) ou Status e use os modificadores de filtro para procurar tarefas específicas.

   Para obter informações sobre modificadores de filtro Workfront, consulte [Filtros e modificadores de condição](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Não é possível selecionar tarefas com o status Concluído.

   ![Status da tarefa em atribuições em massa](assets/task-name-status-dropdown-bulk-assignments-wb-nwe-350x102.png)

   >[!TIP]
   >
   >Deixe essa seleção em branco se quiser fazer atribuições em massa para problemas e tarefas.

1. (Opcional) Clique no ícone **Excluir** ![Excluir ícone](assets/delete.png) ao lado de um dos critérios selecionados

   Ou

   Clique em **Limpar tudo** no canto superior direito do painel Atribuições em massa para remover todas as seleções.

1. Selecione uma das seguintes opções e continue com as etapas descritas abaixo:

   * [Atribuir usuário](#assign-user)
   * [Substituir usuário](#replace-user)
   * [Retirar atribuição de usuário](#unassign-user)

   >[!TIP]
   >
   >Se nenhum item corresponder aos filtros selecionados, essas opções estarão esmaecidas.

### Atribuir usuário {#assign-user}

Quando você atribui um usuário usando Atribuições em massa no Balanceador de carga de trabalho, as seguintes situações ocorrem:

* Um usuário é atribuído a todos os itens de trabalho atualmente atribuídos a uma função especificada nos projetos selecionados.
* O usuário não está atribuído aos seguintes tipos de itens de trabalho:

   * Itens já atribuídos a um usuário.
   * Itens concluídos.

* Se o usuário selecionado não estiver associado à função especificada, a função será substituída pelo usuário na função principal do usuário.

Para atribuir um usuário a itens de trabalho previamente atribuídos a funções de trabalho:

1. Comece a atribuir itens de trabalho usando Atribuições em massa no Balanceador de carga de trabalho conforme descrito acima e selecione **Atribuir**.

1. No campo **Atribuição de função**, clique na seta suspensa para escolher em uma lista de funções. Somente as funções atualmente atribuídas nos projetos especificados são exibidas. Este campo é obrigatório.

   ![Atribuição de função](assets/bulk-assignments-workload-balancer-assign-selected.png)

1. No campo **Usuário a ser atribuído**, clique na seta suspensa para escolher de uma lista de usuários sugeridos ou para digitar o nome de outro usuário.

   Selecione usuários nas seguintes áreas:

   * **Atribuições sugeridas**: usuários que podem atender à função selecionada e que correspondem aos critérios das Atribuições inteligentes. Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).
   * **Outras Atribuições**: Todos os usuários do sistema que podem desempenhar a função selecionada.

     >[!TIP]
     >
     >Somente os primeiros 50 usuários são listados na área Outras atribuições.


   Depois de selecionar um usuário, o Workfront exibe uma observação sobre o número de itens aos quais o usuário especificado será atribuído e qual função de trabalho será substituída.

   >[!TIP]
   >
   >Todas as funções do usuário são exibidas na lista, sob o nome do usuário.


1. Clique em **Atribuir**.

   As funções especificadas são substituídas pelos usuários selecionados.

   Você receberá uma confirmação sobre quantos itens de trabalho tiveram a função selecionada substituída pelo usuário selecionado.

   ![Confirmação de atribuição em massa](assets/bulk-assign-user-confirmation-before-assigning-nwe-350x83.png)

### Substituir usuário {#replace-user}

Você pode substituir um usuário que já está atribuído a itens de trabalho por outro usuário nos projetos selecionados.

Quando você substitui um usuário por outro usando Atribuições em massa no Balanceador de carga de trabalho, as seguintes situações ocorrem:

* O usuário substituto é atribuído a todos os itens de trabalho atualmente atribuídos a um usuário original dentro dos projetos selecionados.

* O novo usuário não está atribuído a nenhum item de trabalho já marcado como Concluído.
* Se a função associada ao primeiro usuário não corresponder a nenhuma função do segundo usuário, o segundo usuário será atribuído em sua Função principal.

Para substituir um usuário por outro usuário:

1. Comece a atribuir itens de trabalho no Balanceador de carga de trabalho conforme descrito acima e selecione **Substituir**.
1. No campo **Usuário atribuído no momento**, clique na seta suspensa para escolher em uma lista de usuários. Somente os usuários atualmente atribuídos a itens de trabalho incompletos dentro dos projetos especificados são exibidos. Este campo é obrigatório.

   ![Substituir usuário](assets/bulk-assignments-workload-balancer-replace-selected-350x345.png)

1. No campo **Usuário a ser atribuído**, clique na seta suspensa para escolher de uma lista de usuários sugeridos ou para digitar outro nome de usuário. Os usuários listados na lista por padrão correspondem aos critérios das Atribuições inteligentes. Para obter mais informações, consulte [Visão geral das atribuições inteligentes](../../manage-work/tasks/assign-tasks/smart-assignments.md).

   O Workfront exibe uma observação sobre o número de itens em que o usuário atribuído no momento substituirá o segundo usuário e quais funções ele substituirá.

   ![Confirmação de substituição de usuário em massa](assets/bulk-replace-user-confirmation-before-replacing-nwe-350x49.png)

1. Clique em **Substituir**.

   O primeiro usuário selecionado é substituído pelo segundo em todos os itens de trabalho do projeto selecionado.

   Você receberá uma confirmação sobre quantos itens de trabalho tiveram a atribuição de usuário original substituída pelo segundo usuário selecionado.

### Retirar atribuição de usuário {#unassign-user}

Você pode desatribuir um usuário de todos os itens de trabalho aos quais ele está atribuído nos projetos selecionados.

Quando você cancela a atribuição de um usuário de todas as atribuições usando Atribuições em massa no Balanceador de carga de trabalho, as seguintes situações ocorrem:

* O usuário especificado é removido de todos os itens de trabalho aos quais está atribuído.
* Se o usuário não atribuído estiver associado a funções de trabalho, as funções de trabalho permanecerão atribuídas aos itens de trabalho quando o usuário for removido.

* Se o usuário especificado for atribuído a itens de trabalho concluídos, o usuário permanecerá atribuído a esses itens de trabalho.

Para obter mais informações sobre atribuições de usuários e funções de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

Para desatribuir um usuário dos itens de trabalho nos projetos selecionados ou para as tarefas ou problemas selecionados nas quais ele está atribuído:

1. Comece a atribuir itens de trabalho no Balanceador de carga de trabalho conforme descrito acima e selecione **Cancelar atribuição**.

1. No campo **Usuário a ser desatribuído**, clique na seta suspensa para escolher em uma lista de usuários. Somente os usuários atualmente atribuídos a itens de trabalho incompleto nos projetos especificados são exibidos. Este campo é obrigatório.

   ![Cancelar atribuição de usuário](assets/bulk-assignments-workload-balancer-unassign-selected-350x318.png)

   O Workfront exibe uma observação sobre o número de itens para os quais o usuário atribuído no momento terá a atribuição cancelada.

   ![Confirmação de cancelamento de atribuição em massa](assets/bulk-unassign-user-confirmation-before-assigning-nwe-350x45.png)

1. Clique em **Cancelar atribuição**.\
   Você recebe uma confirmação sobre o número de itens de trabalho dos quais o usuário especificado foi removido.


