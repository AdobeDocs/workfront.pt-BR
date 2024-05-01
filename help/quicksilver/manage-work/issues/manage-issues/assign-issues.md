---
product-area: projects
navigation-topic: manage-issues
title: Atribuir problemas
description: Você pode atribuir problemas a usuários, funções e equipes para indicar quem é responsável por concluir os problemas. Para obter informações gerais sobre atribuição de problemas, consulte Modificar visão geral de atribuições de problemas.
author: Alina
feature: Work Management
role: User
exl-id: e2dce29e-7370-4580-8326-99c4437998bf
source-git-commit: abe6d1dbd256506fd733fa626ac5907fb9c24d65
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 0%

---

# Atribuir problemas

{{highlighted-preview}}

Você pode atribuir problemas a usuários, funções e equipes para indicar quem é responsável por concluir os problemas. Para obter informações gerais sobre atribuição de problemas, consulte [Visão geral da modificação de atribuições de emissão](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!TIP]
>
>Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
>
>Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
>
>* Reatribuir o item de trabalho aos recursos ativos.
>* Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.

Além deste artigo, recomendamos que você leia os seguintes artigos para obter mais informações sobre como atribuir problemas:

* [Visão geral da modificação de atribuições de emissão](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)
* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Modificar atribuições de usuário para vários problemas em uma lista](../../../manage-work/issues/manage-issues/edit-assignments-for-multiple-issues.md)
* [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md)
* [Fazer atribuições inteligentes](../../../manage-work/tasks/assign-tasks/make-smart-assignments.md)
* [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md)
* [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)

Você pode atribuir uma ocorrência a um ou vários recursos no nível da ocorrência individual, ou pode atribuir vários recursos a várias ocorrências de uma vez.

A atribuição de problemas e tarefas é semelhante no Adobe Workfront. Para obter informações gerais sobre atribuição de tarefas, consulte [Visão geral da modificação de atribuições de tarefas](../../../manage-work/tasks/assign-tasks/modify-task-assignments-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior a projetos e tarefas</p> <p>Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a problemas em seu Nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p>Contribua com permissões para o item em que você está copiando o problema com a capacidade de Adicionar problemas.</p> <p> Para obter informações sobre a concessão de permissões para problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a></p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Conceder acesso aos usuários</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Considerações para várias atribuições para funções de trabalho, equipes e usuários

Considere o seguinte ao atribuir vários recursos a um item de trabalho:

* Os usuários podem ter mais de uma função de trabalho associada ao seu perfil. Para obter informações sobre como associar usuários a funções de trabalho, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

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

## Atribuir um único problema

1. Vá para um problema que deseja atribuir.
1. Clique em **Atribuir a** no canto superior direito do cabeçalho do problema, na caixa **Atribuições** área

   Ou

   Clique no nome das atribuições atuais, se a ocorrência já tiver sido atribuída.

   ![Botão Atribuir a](assets/assign-to-button-in-header.png)

1. Siga um destes procedimentos:

   * Comece a digitar o nome de um usuário, função ou equipe que deseja atribuir e clique nele quando ele aparecer na lista.

     Imagem de amostra no ambiente de produção:
     ![](assets/nwe-assignments-expanded-in-task-header-350x259.png)

     <span class="preview">Imagem de exemplo no ambiente de Pré-visualização:</span>
     ![Pesquisa de atribuições](assets/assignments-expanded-in-task-issue-header.png)

   * (Condicional) Clique em um dos nomes na caixa **Atribuições sugeridas** lista
   * Clique em **Atribuir a mim** para atribuir a si mesmo
   * Clique em **Avançado**.

     Criar atribuições avançadas é semelhante para tarefas e problemas. Para obter informações sobre como fazer atribuições avançadas, consulte [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     >[!TIP]
     >
     >Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos.
     >
     >Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
     >
     >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)


1. Clique em **Salvar** para concluir a atribuição da ocorrência.
1. (Opcional) Clique no link **Ícone X** ao lado do nome das atribuições na área Atribuições no cabeçalho do problema para remover uma atribuição.

## Atribuir um problema em uma lista

Você pode atribuir problemas em uma lista ou em um relatório quando qualquer um dos campos de atribuição estiver visível na exibição da lista. Essa é a maneira mais rápida de atribuir problemas.

Dependendo de qual campo estiver visível na visualização, você poderá atribuir as seguintes entidades à ocorrência:

| Opção | Entidades atribuídas |
|---|---|
| **Atribuir a** | Atribuir um usuário |
| **Atribuído** | Atribuir um usuário |
| **Atribuições** | Atribuir usuários, funções de trabalho ou equipes. |

Para atribuir ocorrências em uma lista:

1. Vá para uma lista de problemas que têm os campos Assigned To (Atribuído a), Assigned (Atribuído) ou Assignments (Atribuições) na exibição.
1. Para atribuir ocorrências, siga um destes procedimentos:

   * Clique dentro do **Atribuído a** ou **Atribuído** e comece a digitar o nome de um usuário ativo que você deseja atribuir ao problema, em seguida, clique nele quando ele for exibido na lista.

     ![](assets/assigned-to-field-task-list-nwe.png)

   * Clique dentro do **Atribuições** e comece digitando o nome de um usuário, função de trabalho ou equipe ativa que deseja atribuir ao problema e clique nele quando ele for exibido na lista.

     Imagem de amostra no ambiente de produção:
     ![](assets/assignments-field-task-list-nwe.png)

     <span class="preview">Imagem de exemplo no ambiente de Pré-visualização:</span>
     ![Campo Atribuições](assets/assignments-field-task-list-0424.png)

   >[!TIP]
   >
   >Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos.
   >
   >Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
   >
   >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


1. (Condicional) Quando visível no campo Atribuições, clique no botão **Ícone Pessoas** ![](assets/teams.png) no canto superior direito da caixa atribuições, para abrir a caixa atribuições avançadas e criar atribuições avançadas. Para obter mais informações, consulte [Criar atribuições avançadas](../../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

   >[!TIP]
   >
   >Não é possível fazer atribuições avançadas nos campos Atribuído a ou Atribuído.

1. Depois de adicionar os atribuídos ao problema, pressione Enter ou clique em qualquer lugar na página para salvar as alterações.

## Atribuir problemas em massa

1. Vá para uma lista de problemas que você deseja atribuir em massa.
1. Selecione vários problemas na lista.
1. Clique em **Ícone Editar** ![](assets/qs-edit-icon.png).

   A variável **Editar Problemas** é aberta.

1. No **Atribuições** , selecione a **Destinatário** e comece a digitar o nome de um usuário, função de trabalho ou equipe que deseja atribuir a todas as questões.

   >[!IMPORTANT]
   >
   >Se qualquer um dos problemas já estiver atribuído, os recursos que você indicar aqui serão adicionados aos problemas em vez de substituir os recursos existentes nos problemas.

1. (Opcional) Selecione o botão de opção na caixa **Proprietário do problema** para indicar qual recurso é o principal designado ou o Proprietário da ocorrência, quando você atribui mais de um recurso à ocorrência. Isto não está disponível para equipes.
1. (Opcional) Selecione uma função que o usuário deve desempenhar no problema a partir da **Escolher uma função** menu suspenso no **Função do atribuidor** quando você atribui usuários a ocorrências. Se você não selecionar uma função, o Workfront selecionará automaticamente a função principal do usuário.

1. (Opcional) Se quiser remover os atribuídos existentes de todas as ocorrências, execute um dos procedimentos a seguir:

   1. Comece a digitar o nome de um usuário, função ou equipe que deseja remover do problema, selecione-o quando ele aparecer na lista e clique em **Remover atribuidor** para adicionar outros atribuídos a serem removidos.
   1. Clique em **Remover todos os atribuídos existentes** para remover todos os atribuídos de todas as questões selecionadas.

1. Clique em **Salvar alterações**.
1. (Opcional e condicional) Quando os campos Atribuído a ou Atribuições forem exibidos na lista de ocorrências, clique dentro de uma dessas colunas para uma ocorrência e, em seguida, clique na guia **Ícone X** ao lado do nome de um destinatário para removê-lo da ocorrência.
