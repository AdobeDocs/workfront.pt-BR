---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Cancelar atribuição de trabalho no Balanceador de carga de trabalho
description: Você pode desatribuir usuários de itens de trabalho na área Trabalho atribuído do Balanceador de carga de trabalho do Adobe Workfront ou reatribuí-los a outros usuários, funções ou equipes.
author: Lisa
feature: Resource Management
exl-id: e4293d4a-afb8-48ef-8a8e-6fad2ef82a25
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 2%

---

# Cancelar atribuição de trabalho no Balanceador de carga de trabalho

Você pode desatribuir usuários de itens de trabalho na área Trabalho atribuído do Balanceador de carga de trabalho do Adobe Workfront ou reatribuí-los a outros usuários, funções ou equipes.

Você pode cancelar a atribuição de itens de trabalho manualmente, arrastando e soltando ou em massa. Este artigo descreve como cancelar a atribuição de usuários manualmente.

Para obter informações sobre como desatribuir usuários arrastando e soltando, consulte [Atribuir trabalho no Balanceador de carga de trabalho arrastando e soltando](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md)

Para obter informações sobre como desatribuir usuários em massa, consulte [Atribuir trabalho em massa usando o Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

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
    </ul></td>
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Contribuir com permissões ou mais altas para projetos, tarefas e problemas que incluem Fazer atribuições</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cancelar atribuição de itens de trabalho no Balanceador de carga de trabalho

Você pode cancelar a atribuição de itens de usuários e movê-los para a área Trabalho não atribuído ou reatribuí-los a outros usuários.

Para desatribuir itens de trabalho dos usuários:

1. No Balanceador de carga de trabalho, vá para a área **Trabalho atribuído** e expanda um usuário.
1. Siga um destes procedimentos:

   * Localize o item que deseja cancelar a atribuição na área de um usuário, clique nele e arraste e solte-o na área Não atribuído ou na área de outro usuário.
   * Clique no ícone **Mais** ícone ![Mais ícone](assets/more-icon-task-list.png) à direita do nome de um item de trabalho, clique em **Atribuir a este item**, remova o nome das entidades atribuídas ao item de trabalho ou insira outro nome e clique em **Salvar**.

     ![Atribuir esta a](assets/assign-this-to-link-from-task-wb-nwe-350x104.png)

   O item é exibido na área Trabalho não atribuído se corresponder aos critérios de filtragem para essa área e não estiver atribuído a outros usuários, ou é exibido na área do usuário se estiver atribuído a outro usuário.

   Para obter informações sobre como filtrar informações no Balanceador de carga de trabalho, consulte [Informações de filtro no Balanceador de carga de trabalho](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
