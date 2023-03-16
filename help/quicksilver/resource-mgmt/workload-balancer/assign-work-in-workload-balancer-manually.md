---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Atribuir trabalho manualmente usando o Balanceador de Carga de Trabalho
description: Você pode atribuir itens de trabalho manualmente a usuários usando o Balanceador de Carga de Trabalho do Adobe Workfront.
author: Alina
feature: Resource Management
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 2%

---

# Atribuir trabalho manualmente usando o Balanceador de Carga de Trabalho

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
   <td> <p>Planejar, ao usar o Balanceador de Carga de Trabalho na área Recursos</p>
   <p>Trabalhe, ao usar o Balanceador de Carga de Trabalho de uma equipe ou projeto</p>
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

## Atribuir trabalhos manualmente no Balanceador de Carga de Trabalho

Você pode atribuir itens de trabalho que ainda não foram atribuídos a um usuário ou reatribuir itens que foram atribuídos a usuários no Balanceador de Carga de Trabalho.

1. Vá para o Balanceador de Carga de Trabalho onde deseja atribuir trabalho.

   Você pode atribuir trabalhos a usuários usando o Balanceador de Carga de Trabalho na área Recursos, no projeto ou no nível da equipe. Para obter mais informações sobre onde o Balanceador de Carga de Trabalho está localizado no Workfront, consulte [Localizar o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Opcional) Vá para o **Trabalho Não Atribuído** e aplicar um filtro para exibir tarefas ou problemas

   Ou

   Vá para o **Trabalho Atribuído** e expanda o nome de um usuário para exibir os itens de trabalho atribuídos a ele, caso deseje reatribuir seus itens.

1. Clique no botão **Menu Mais** ![](assets/qs-more-menu.png) à esquerda de um nome de item de trabalho, em seguida, clique em **Atribua isso a**.

   ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Você também pode usar os seguintes atalhos para atribuir tarefas ou problemas:
   >
   >* No Windows: Clique com a tecla CTRL pressionada na barra de tarefas ou problemas.
   >* No Mac: Clique com a tecla CMD na barra de tarefas ou problemas.


1. Siga um destes procedimentos:

   * Comece a digitar o nome de um usuário, função de trabalho ou equipe que você deseja atribuir ao item na **Pesquisar pessoas, funções ou equipes** , selecione-o quando for exibido na lista e clique em **Salvar**.
   >[!TIP]
   >
   >Ao adicionar um usuário, observe o avatar, a função primária do usuário e seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os adiciona.

   ![](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Se o administrador do Workfront ou do grupo ativou delegações em seu ambiente, use a guia Atribuições para atribuir usuários à tarefa ou problema. Use a guia Delegações para exibir os usuários que são delegados ao item de trabalho. Para obter informações sobre delegação de trabalho, consulte [Gerenciar delegação de tarefa e emissão](../../manage-work/delegate-work/how-to-delegate-work.md).


   Isso atribui ou reatribui o item de trabalho aos destinatários especificados.

   Se você atribuir um item somente a uma equipe ou a uma função de trabalho, o item será exibido somente na área de Trabalho Não Atribuído. Você deve atribuir itens de trabalho aos usuários para exibi-los na área de Trabalho Atribuído do Balanceador de Carga de Trabalho.

   >[!TIP]
   >
   >Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários ativos, funções de trabalho e equipes.
   >
   >
   >Se um usuário, uma função de trabalho ou uma equipe tiver sido atribuída antes de ser desativada, ela permanecerá atribuída ao item de trabalho. Nesse caso, recomendamos o seguinte:
   >
   >   
   >   
   >   * Atribua novamente o item de trabalho aos recursos ativos.
   >   * Associe os usuários em uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.


   * Clique em **Avançado** para acessar Atribuições avançadas.

      Para obter mais informações sobre como fazer Atribuições avançadas, consulte [Criar atribuições avançadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).


1. (Opcional) Clique no botão **Ícone Mostrar alocações** ![](assets/show-allocations-icon-small.png), em seguida, clique no botão **Menu Mais** ![](assets/qs-more-menu.png) > **Editar alocações**.

   Ou

   Clique duas vezes em uma alocação diária ou semanal para modificar a quantidade de tempo que o usuário está alocado para o item de trabalho.

   Para obter informações sobre como modificar alocações de usuários no Balanceador de Carga de Trabalho, consulte a seção &quot;Modificar alocações de usuários&quot; no artigo [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Para obter informações sobre como remover atribuições de um item de trabalho usando o Balanceador de Carga de Trabalho, consulte [Cancelar atribuição de trabalho no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
