---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Atribuir trabalho manualmente usando o Balanceador de carga de trabalho
description: Você pode atribuir itens de trabalho manualmente aos usuários usando o Balanceador de carga de trabalho do Adobe Workfront.
author: Lisa
feature: Resource Management
role: User
exl-id: 445cb250-53a4-488b-911d-3afca3a02c23
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 1%

---

# Atribuir trabalho manualmente usando o Balanceador de carga de trabalho

{{preview-fast-release-general}}

Você pode atribuir itens de trabalho manualmente aos usuários usando o Balanceador de carga de trabalho do Adobe Workfront.

Para obter informações gerais sobre como atribuir trabalho a usuários usando o Balanceador de carga de trabalho, consulte [Visão geral da atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td>
  </tr>
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Planejar, ao usar o Balanceador de carga de trabalho na área Recursos; Trabalhar, ao usar o Balanceador de carga de trabalho de uma equipe ou projeto</p></td>
  </tr>
  <tr> 
   <td>Configurações de nível de acesso</td> 
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
   <td>Permissões de objeto</td> 
   <td>Contribuir com permissões ou mais altas para projetos, tarefas e problemas que incluem Fazer atribuições</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Atribuir trabalho manualmente no Balanceador de carga de trabalho

Você pode atribuir itens de trabalho que ainda não foram atribuídos a um usuário ou reatribuir itens que foram atribuídos a usuários no Balanceador de carga de trabalho.

1. Vá para o Balanceador de carga de trabalho onde deseja atribuir trabalho.

   Você pode atribuir trabalho aos usuários usando o Balanceador de carga de trabalho na área Recursos, no projeto ou no nível da equipe. Para obter mais informações sobre onde o Balanceador de carga de trabalho está localizado na Workfront, consulte [Localizar o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

1. (Opcional) Vá para a área **Trabalho não atribuído** e aplique um filtro para exibir tarefas, problemas, <span class="preview">ou atribuições de função</span>.

   Ou

   Vá para a área **Trabalho atribuído** e expanda o nome de um usuário para ver os itens de trabalho atribuídos a ele, caso queira reatribuir seus itens.

   >[!NOTE]
   >
   ><span class="preview">As atribuições de função são exibidas em itens de trabalho na área Trabalho não atribuído quando a configuração Mostrar atribuições de função está habilitada. Para obter mais informações, consulte [Personalizar a exibição](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md#customize-the-view) em [Navegar pelo Balanceador de Carga de Trabalho](/help/quicksilver/resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).</span>

1. Clique no **Mais menu** ![Mais menu](assets/qs-more-menu.png) à esquerda de um nome de item de trabalho <span class="preview">ou de uma atribuição de função</span> e clique em **Atribuir a este(a)**.

   ![Atribuir esta a](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   >[!TIP]
   >
   >Você também pode usar os seguintes atalhos para atribuir tarefas ou problemas:
   >
   >* No Windows: CTRL+clique na barra de tarefas ou problemas.
   >* No Mac: CMD+clique na barra de tarefas ou problemas.

1. Siga um destes procedimentos:

   * Comece a digitar o nome de um usuário, função de trabalho ou equipe que deseja atribuir ao item no campo **Pesquisar pessoas, função ou equipes**, selecione-o quando ele for exibido na lista e clique em **Salvar**.

   >[!TIP]
   >
   >Ao adicionar um usuário, observe o avatar, a função principal do usuário e seu endereço de email para distinguir entre usuários com nomes idênticos.
   >
   >Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
   >
   > Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


   ![Atribuições avançadas](assets/assignments-box-with-advanced-assignments-delegations-wb.png)

   >[!TIP]
   >
   > Se a Workfront ou o administrador de grupo tiver ativado delegações no seu ambiente, use a guia Atribuições para atribuir usuários à tarefa ou problema. Use a guia Delegações para exibir os usuários delegados ao item de trabalho. Para obter informações sobre como delegar trabalho, consulte [Delegar tarefas e problemas](../../manage-work/delegate-work/how-to-delegate-work.md).


   Isso atribui ou reatribui o item de trabalho aos atribuídos especificados.

   Se você atribuir um item apenas a uma equipe ou função de trabalho, o item será exibido somente na área Trabalho não atribuído. Você deve atribuir itens de trabalho aos usuários para exibi-los na área Trabalho atribuído do Balanceador de carga de trabalho.

   >[!TIP]
   >
   >Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
   >
   >
   >Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
   >
   >   
   >   
   >   * Reatribuir o item de trabalho aos recursos ativos.
   >   * Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.
   >   
   >

   * Clique em **Avançado** para acessar as Atribuições avançadas.

     Para obter mais informações sobre como fazer atribuições avançadas, consulte [Criar atribuições avançadas](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. (Opcional) Clique no **ícone Mostrar alocações** ![ícone Mostrar alocações](assets/show-allocations-icon-small.png) e no **menu Mais** ![menu Mais](assets/qs-more-menu.png) > **Editar alocações**.

   Ou

   Clique duas vezes em uma alocação diária ou semanal para modificar a quantidade de tempo que o usuário está alocado para o item de trabalho.

   Para obter informações sobre como modificar alocações de usuários no Balanceador de carga de trabalho, consulte a seção &quot;Modificar alocações de usuários&quot; no artigo [Gerenciar alocações de usuários no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

   Para obter informações sobre como remover atribuições de um item de trabalho usando o Balanceador de carga de trabalho, consulte [Cancelar atribuição de trabalho no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/unassign-work-in-workload-balancer.md).

    
