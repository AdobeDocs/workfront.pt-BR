---
product-area: projects
navigation-topic: manage-issues
title: Atribuir problemas
description: Você pode atribuir problemas a usuários, funções e equipes para indicar quem é responsável por concluir os problemas. Para obter informações gerais sobre atribuição de problemas, consulte Modificar visão geral de atribuições de problemas.
author: Lisa
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: a18b70b20e37f9751fbae2d4aad76e4905f976b2
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 0%

---

# Atribuir problemas

<!--Audited: 10/2024-->

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> 
-->

Você pode atribuir problemas a usuários, funções e equipes para indicar quem é responsável por concluir os problemas. Para obter informações gerais sobre atribuição de problemas, consulte [Visão geral da modificação de atribuições de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
>
>Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
>
>* Reatribuir o item de trabalho aos recursos ativos.
>* Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.

Além deste artigo, recomendamos que você leia os seguintes artigos para obter mais informações sobre como atribuir problemas:

* [Visão geral da modificação das atribuições de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Modificar atribuições de usuário para vários problemas em uma lista](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Fazer atribuições inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Você pode atribuir uma ocorrência a um ou vários recursos no nível da ocorrência individual, ou pode atribuir vários recursos a várias ocorrências de uma vez.

A atribuição de problemas e tarefas é semelhante no Adobe Workfront. Para obter informações gerais sobre atribuição de tarefas, consulte [Visão geral da modificação de atribuições de tarefas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Colaborador ou superior</p>
   <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior aos Projetos e Tarefas para atribuir um problema</p> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p> Exibir permissões ou superiores para o projeto ou tarefa em que o problema está localizado, ao atribuir um problema</p><p>Ao atribuir vários problemas, contribua com permissões ou mais altas para o projeto ou tarefa em que o problema está localizado.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para várias atribuições para funções de trabalho, equipes e usuários

Considere o seguinte ao atribuir vários recursos a um item de trabalho:

* Os usuários podem ter mais de uma função de trabalho associada ao seu perfil. Para obter informações sobre como associar usuários a funções de trabalho, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Geralmente, tarefas ou problemas são atribuídos primeiro a uma ou várias funções de trabalho ou equipes. Quando os projetos estiverem prontos para serem iniciados, talvez também seja necessário atribuí-los aos usuários.

  Se uma tarefa ou um problema for atribuído a uma ou várias funções e você também atribuir um usuário, o Adobe Workfront decide qual função de trabalho deve ser associada ao usuário adicional (se houver) de acordo com as seguintes regras:

   * Se houver apenas uma função de trabalho atribuída e ela corresponder à função principal do usuário, a tarefa ou o problema será atribuído apenas ao usuário que desempenha sua função principal.
   * Se houver várias funções atribuídas e pelo menos uma das funções corresponder às funções secundárias do usuário, a tarefa ou o problema será atribuído ao usuário que desempenha uma de suas Outras funções — que o Workfront seleciona aleatoriamente se houver várias correspondências — bem como quaisquer funções adicionais atribuídas.
   * Se houver uma ou mais funções de trabalho atribuídas e não houver correspondência entre as funções do usuário, a tarefa ou o problema será atribuído à função ou às funções, bem como ao usuário.

* Se uma tarefa ou um problema for atribuído a uma equipe e você também atribuir um usuário, a tarefa ou o problema permanecerá atribuído à equipe e ao usuário.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2> </h2>
<h2>Considerations about removing assignments from issues</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and moved to Modify issue assignments overview article)</p>
<p>You can remove assignments from one issue at a time, or you can remove assignments from multiple issues in bulk.</p>
<p>For more information about removing assignments from issues in bulk, see <a href="../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md" class="MCXref xref">Modify user assignments for multiple issues in a list</a>. </p>
<p>Consider the following when removing assignments from issues: </p>
<ul>
<li>When you unassign a user from an issue, the issue remains assigned to the job role that the user fulfilled on the issue.</li>
<li>When you unassign a job role or a team from an issue, the issue remains unassigned if it is not assigned to any other resources. </li>
</ul>
</div>
-->

## Atribuir um único problema no cabeçalho do problema

1. Vá para um problema que deseja atribuir.
1. Clique em **Atribuir a** no canto superior direito do cabeçalho do problema, na área **Atribuições**

   Ou

   Clique no nome das atribuições atuais, se a ocorrência já tiver sido atribuída.

   ![Atribuir ao botão](assets/assign-to-button-in-header.png)

1. Siga um destes procedimentos:

   * Comece a digitar o nome de um usuário, função ou equipe que deseja atribuir e clique nele quando ele aparecer na lista.

     ![Pesquisa de atribuições](assets/smart-assignments-issue-header.png)

   * (Condicional) Clique em um dos nomes, funções ou equipes nas listas disponíveis
   * Clique em **Atribuir a mim** para atribuí-lo a si mesmo
   * Clique em **Avançado**.

     Criar atribuições avançadas é semelhante para tarefas e problemas. Para obter informações sobre como fazer atribuições avançadas, consulte [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos.
     >
     >Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
     >
     >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
     >

     <!-- this doesn't apply to issues; if it does, add this to the TIP above: 
      ><span class="preview">When adding a job role assignment, you can search for the job role or location. Select a role from the Job roles list to use the default billing rate for the assignment, or select a Rate card job role to use the billing rate from the rate card. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>-->


1. Clique em **Salvar** para concluir a atribuição do problema.
1. (Opcional) Clique no ícone **X** ao lado do nome das atribuições na área Atribuições no cabeçalho do problema para remover uma atribuição.

## Atribuir um problema ao editá-lo em linha em uma lista

Você pode atribuir problemas em uma lista ou em um relatório quando qualquer um dos campos de atribuição estiver visível na exibição da lista. Essa é uma maneira mais rápida de atribuir problemas.

Dependendo de qual campo estiver visível na visualização, você poderá atribuir as seguintes entidades à ocorrência:

| Opção | Entidades atribuídas |
|---|---|
| **Atribuir a** | Atribuir um usuário |
| **Atribuído** | Atribuir um usuário |
| **Atribuições** | Atribuir usuários, funções de trabalho ou equipes. |

Para atribuir ocorrências em uma lista:

1. Vá para uma lista de problemas que têm os campos Assigned To (Atribuído a), Assigned (Atribuído) ou Assignments (Atribuições) na exibição.
1. Para atribuir ocorrências, siga um destes procedimentos:

   * Clique dentro dos campos **Atribuído a** ou **Atribuído** e comece a digitar o nome de um usuário ativo que deseja atribuir ao problema, em seguida, clique nele quando ele for exibido na lista.

     ![Atribuído ao campo](assets/assigned-to-field-task-list-nwe.png)

   * Clique dentro do campo **Atribuições** e comece a digitar o nome de um usuário, função de trabalho ou equipe ativa que deseja atribuir ao problema, em seguida, clique nele quando ele for exibido na lista.

     ![Campo de atribuições](assets/assignments-field-0825.png)

   >[!TIP]
   >
   >Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos.
   >
   >Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
   >
   >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

1. (Condicional) No campo Atribuições, clique em **Avançadas** na parte inferior da lista, ou no **ícone Pessoas** ![ícone Pessoas](assets/teams.png) no canto superior direito da caixa Atribuições, para abrir a caixa Atribuições Avançadas e criar atribuições avançadas. Para obter mais informações, consulte [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Não é possível fazer atribuições avançadas nos campos Atribuído a ou Atribuído.

1. Depois de adicionar os atribuídos ao problema, pressione Enter ou clique em qualquer lugar na página para salvar as alterações.

## Atribuir um problema na caixa Editar problema

Você pode atribuir um problema ao editá-lo na caixa Editar problema.

Para obter informações, consulte a seção &quot;Atribuições&quot; no artigo [Editar problemas](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).

## Atribuir problemas em massa

<!--
Assigning issues in bulk is different depending on what environment you choose to do this. 

### Assign issues in bulk in the Production environment -->

1. Vá para uma lista de problemas que você deseja atribuir em massa.
1. Selecione vários problemas na lista.
1. Clique no **ícone Editar** ![ícone Editar](assets/qs-edit-icon.png).

   A caixa de diálogo **Editar Problemas** é aberta.

1. Na área **Atribuições**, marque a caixa **Destinatário** e comece a digitar o nome de um usuário, função de trabalho ou equipe que deseja atribuir a todos os problemas.

   >[!IMPORTANT]
   >
   >Se qualquer um dos problemas já estiver atribuído, os recursos que você indicar aqui serão adicionados aos problemas em vez de substituir os recursos existentes nos problemas.

1. (Opcional) Selecione o botão de opção na coluna **Proprietário do problema** para indicar qual recurso é o destinatário primário ou o Proprietário do problema, quando você atribui mais de um recurso ao problema. Isto não está disponível para equipes.
1. (Opcional) Selecione uma função que o usuário deve desempenhar no problema do menu suspenso **Escolha uma função** na coluna **Função do destinatário** ao atribuir usuários a problemas. Se você não selecionar uma função, o Workfront selecionará automaticamente a função principal do usuário.

1. (Opcional) Se quiser remover os atribuídos existentes de todas as ocorrências, execute um dos procedimentos a seguir:

   1. Comece digitando o nome de um usuário, função ou equipe que deseja remover do problema, selecione-o quando ele aparecer na lista e clique em **Remover responsável** para adicionar outros responsáveis a serem removidos.
   1. Clique em **Remover todos os atribuídos existentes** para remover todos os atribuídos de todas as questões selecionadas.

1. Clique em **Salvar alterações**.
1. (Opcional e condicional) Quando os campos Atribuído a ou Atribuições forem exibidos na lista de problemas, clique dentro de uma dessas colunas para um problema e, em seguida, clique no ícone **X** ao lado do nome de um destinatário para removê-lo do problema.

<!--
<div class="preview">

### Assign issues in bulk in the Preview environment

1. Go to a list of issues that you want to assign in bulk. 
1. Select several issues in the list. 
1. Click the **Edit icon** ![Edit icon](assets/qs-edit-icon.png).

   The **Edit Issues** dialog box opens.

1. Click **Assignments** in the left panel, and in the **Assignments** area, start typing the name of a user, role, or team in the **Search people, roles, or teams** field, then click it when it displays in the list

   Or

   Click **Assign to me** to assign the issues to yourself.

   >[!IMPORTANT]
   >
   >If any of the issues is already assigned, the resources you indicate here are added to the issues instead of replacing the existing resources on the issues. 
   
1. (Optional) If you want to remove existing assignees from all issues, click the **x** next to their name.

1. (Optional) Update the Planned Hours field. For more information, see [Edit issues](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md). 

1. Click **Save**.
1. (Optional and conditional) When the Assigned to or the Assignments fields display in your list of issues, click inside one of these columns for an issue, then click the **X icon** next to the name of an assignee to remove it from the issue.

</div>
-->
