---
product-area: resource-management
navigation-topic: resource-pools
title: Criar pools de recursos
description: Os pools de recursos são coleções de usuários que ajudam a gerenciar os recursos de forma mais fácil no Adobe Workfront. Para obter mais informações sobre pools de recursos, consulte Visão geral dos pools de recursos .
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---

# Criar pools de recursos

Os pools de recursos são coleções de usuários que ajudam a gerenciar os recursos de forma mais fácil no Adobe Workfront. Para obter mais informações sobre pools de recursos, consulte [Visão geral dos pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Gerenciar conjuntos de recursos</p> <p>Editar acesso a usuários, projetos e modelos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões dos projetos e modelos aos quais deseja associar os Pools de Recursos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar um Pool de Recursos {#create-a-resource-pool}

1. Faça logon como um usuário que tem acesso para editar os Pools de Recursos.\
   Para obter mais informações, consulte [Criar um Pool de Recursos](#create-a-resource-pool).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Recursos**.
1. Clique em **Pools de Recursos** no painel esquerdo.\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. Clique em **Novo Pool de Recursos**.
1. Especifique o seguinte:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td>Este é o nome do Pool de Recursos.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrição</strong></td>
      <td>Esta é uma breve descrição sobre este Pool de Recursos. Por exemplo, você pode especificar para qual finalidade ela deve ser usada.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Membros do conjunto</strong></td>
      <td><p> Adicione usuários ao Pool de Recursos individualmente.<br>Ou <br>Para adicionar uma grande quantidade de usuários ao Pool de Recursos de uma só vez. Você pode adicionar uma das seguintes entidades associadas aos usuários ou à coleção de usuários:
        <ul>
         <li><strong>Equipes</strong>: todos os membros da equipe são adicionados ao Pool de Recursos.</li>
         <li><strong>Grupos</strong>: todos os membros do grupo são adicionados ao Pool de Recursos.</li>
         <li><strong>Funções</strong>: todos os usuários associados a essa função são adicionados ao Pool de Recursos.</li>
         <li><strong>Empresas</strong>: todos os usuários da empresa são adicionados ao Pool de Recursos.</li>
        </ul><p>Dica: Você só pode adicionar usuários ativos, equipes, <span>funções,</span> ou empresas.</p><p>Observação: Se um usuário se tornar membro de um grupo, equipe, empresa ou estiver associado a uma função de trabalho depois que o grupo, a equipe, a empresa ou a função de trabalho tiverem sido adicionados ao Pool de Recursos, o novo membro não será automaticamente adicionado ao Pool de Recursos. <br>Se um usuário pertencer à equipe, grupo, empresa e função de trabalho que você está adicionando, ao mesmo tempo, o usuário será adicionado apenas uma vez ao Pool de Recursos.<br>Os usuários que são desativados depois de terem sido adicionados ao Pool de Recursos aparecem esmaecidos na lista de usuários e são marcados como desativados.</p></p></td>
     </tr>
    </tbody>
   </table>

1. (Opcional) Use o **Desfazer** link para remover os usuários adicionados por meio de um grupo, equipe, empresa ou função de trabalho.

   >[!NOTE]
   >
   >Não há limite para quantos usuários você pode ter em um Pool de Recursos. No entanto, recomendamos não adicionar muitos usuários a um pool de recursos, pois caso contrário, o gerenciamento de recursos poderá se tornar um desafio. A lista de usuários mostra apenas os primeiros 2.000 usuários no Pool de Recursos, e eles estão listados em ordem alfabética.

   ![Resource_pools_NEW__UNDO_button_for_times_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. (Opcional) Clique no ícone X à direita do nome de um usuário para remover um usuário. Para obter mais informações sobre como remover usuários de um pool de recursos, consulte [Remover usuários de pools de recursos](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. (Opcional) Use o **Pesquisar** para localizar um usuário no Pool de Recursos.
1. Clique em **Criar**.
