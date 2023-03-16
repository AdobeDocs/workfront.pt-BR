---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Cancelar atribuição de trabalho no Balanceador de Carga de Trabalho
description: Você pode cancelar a atribuição de usuários a partir de itens de trabalho na área de Trabalho Atribuído do Balanceador de Carga de Trabalho da Adobe Workfront ou reatribuí-los a outros usuários, funções ou equipes.
author: Alina
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 2%

---

# Cancelar atribuição de trabalho no Balanceador de Carga de Trabalho

Você pode cancelar a atribuição de usuários a partir de itens de trabalho na área de Trabalho Atribuído do Balanceador de Carga de Trabalho da Adobe Workfront ou reatribuí-los a outros usuários, funções ou equipes.

Você pode cancelar a atribuição de usuários de itens de trabalho manualmente, arrastando e soltando ou em massa. Este artigo descreve como cancelar a atribuição de usuários manualmente.

Para obter informações sobre como cancelar a atribuição de usuários arrastando e soltando, consulte [Atribua trabalho ao Balanceador de Carga de Trabalho arrastando e soltando](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Para obter informações sobre como cancelar a atribuição de usuários em massa, consulte [Atribua trabalho em massa usando o Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Edite o acesso ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Tarefas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribua com permissões ou superior para projetos, tarefas e problemas que incluem Fazer atribuições</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

 

## Cancelar atribuição de itens de trabalho no Balanceador de Carga de Trabalho

Você pode cancelar a atribuição de itens de usuários e movê-los para a Área de trabalho não atribuída ou reatribuí-los a outros usuários.

Para cancelar a atribuição de itens de trabalho dos usuários:

1. No Balanceador de Carga de Trabalho, acesse **Trabalho Atribuído** e expandir um usuário.
1. Siga um destes procedimentos:

   * Localize o item que deseja cancelar a atribuição na área de um usuário, clique nele e arraste-o e solte-o na área Não atribuído ou em outra área de usuário.
   * Clique no botão **Mais** ícone ![](assets/more-icon-task-list.png) à direita do nome de um item de trabalho, clique em **Atribua isso a**, remova o nome das entidades atribuídas ao item de trabalho ou insira outro nome e clique em **Salvar**.

      ![](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)
   O item é exibido na área de trabalho não atribuído se corresponder aos critérios de filtragem dessa área e não estiver atribuído a nenhum outro usuário, ou será exibido na área de usuário se estiver atribuído a outro usuário.

   Para obter informações sobre filtragem no Balanceador de Carga de Trabalho, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
