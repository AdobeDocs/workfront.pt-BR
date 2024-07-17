---
product-area: resource-management
navigation-topic: resource-pools
title: Criar conjuntos de recursos
description: Conjuntos de recursos são coleções de usuários que ajudam a gerenciar recursos com mais facilidade no Adobe Workfront. Para obter mais informações sobre conjuntos de recursos, consulte Visão geral dos conjuntos de recursos.
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 1%

---

# Criar conjuntos de recursos

Conjuntos de recursos são coleções de usuários que ajudam a gerenciar recursos com mais facilidade no Adobe Workfront. Para obter mais informações sobre pools de recursos, consulte [Visão geral dos pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Gerenciar conjuntos de recursos</p> <p>Editar acesso a usuários, projetos e modelos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões dos projetos e modelos aos quais você deseja associar os Conjuntos de Recursos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Criar um conjunto de recursos {#create-a-resource-pool}

1. Faça logon como um usuário com acesso para editar Conjuntos de recursos.\
   Para obter mais informações, consulte [Criar um Pool de Recursos](#create-a-resource-pool).

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal**, no canto superior direito do Adobe Workfront.

1. Clique em **Recursos**.
1. Clique em **Conjuntos de Recursos** no painel esquerdo.\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. Clique em **Novo Conjunto de Recursos**.
1. Especifique o seguinte:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td>Este é o nome do Conjunto de Recursos.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrição</strong></td>
      <td>Esta é uma breve descrição sobre este Conjunto de Recursos. Por exemplo, é possível especificar com que finalidade ele deve ser usado.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Membros do conjunto</strong></td>
      <td><p> Adicione usuários ao Conjunto de recursos individualmente.<br>Ou <br>Para adicionar uma grande quantidade de usuários ao Pool de Recursos de uma só vez. Você pode adicionar uma das seguintes entidades associadas a usuários ou a uma coleção de usuários:
        <ul>
         <li><strong>Equipes</strong>: todos os membros da equipe são adicionados ao Conjunto de Recursos.</li>
         <li><strong>Grupos</strong>: todos os membros do grupo são adicionados ao Conjunto de Recursos.</li>
         <li><strong>Funções</strong>: todos os usuários associados a essa função são adicionados ao Pool de Recursos.</li>
         <li><strong>Empresas</strong>: todos os usuários da empresa são adicionados ao Conjunto de Recursos.</li>
        </ul><p>Dica: você só pode adicionar usuários, equipes, <span>funções,</span> ou empresas ativos.</p><p>Observação: se um usuário se tornar membro de um grupo, equipe, empresa ou estiver associado a uma função de trabalho depois que o grupo, a equipe, a empresa ou a função de trabalho forem adicionados ao Conjunto de Recursos, o novo membro não será adicionado automaticamente ao Conjunto de Recursos. <br>Se um usuário pertencer à equipe, grupo, empresa e função de trabalho que você está adicionando, ao mesmo tempo, o usuário será adicionado apenas uma vez ao Pool de Recursos.<br>Os usuários desativados após serem adicionados ao Pool de Recursos aparecem esmaecidos na lista de usuários e marcados como desativados.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Opcional) Use o link **Desfazer** para remover os usuários adicionados por meio de um grupo, equipe, empresa ou função de trabalho.

   >[!NOTE]
   >
   >Não há limite para o número de usuários que você pode ter em um Conjunto de Recursos. No entanto, recomendamos não adicionar muitos usuários a um Conjunto de recursos, pois o Gerenciamento de recursos pode se tornar um desafio caso contrário. A lista de usuários mostra apenas os primeiros 2.000 usuários no Conjunto de recursos e eles são listados em ordem alfabética.

   ![Resource_pools_NEW__UNDO_button_for_team_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Opcional) Clique no ícone X à direita do nome de um usuário para remover um usuário. Para obter mais informações sobre como remover usuários de um pool de recursos, consulte [Remover usuários dos pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Opcional) Use a opção **Pesquisar** para localizar um usuário no Pool de Recursos.
1. Clique em **Criar**.
