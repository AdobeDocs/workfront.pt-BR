---
title: Conceder acesso aos usuários
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a outros usuários no Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 1%

---


# Conceder acesso aos usuários

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a outros usuários no Workfront, conforme explicado na [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configuração do acesso aos usuários

Você pode gerenciar quais informações os usuários podem visualizar e editar para outros usuários usando um nível de acesso padrão ou um nível de acesso personalizado que você cria. Usuários com as licenças padrão de Plano e Trabalho podem exibir as informações de contato de outros usuários. Qualquer um dos usuários a seguir pode criar e editar outros usuários:

* Um administrador do Workfront.

  Para obter mais informações, consulte [Conceder a um usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Um usuário com uma licença de Plano padrão que também tem acesso aos usuários, conforme explicado neste artigo.

  Os usuários restritos a visualizar apenas os usuários de sua empresa ou da empresa primária têm acesso para editar apenas os usuários que eles podem ver. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Um usuário com uma licença de Plano padrão que também é especificado como gerente de outro usuário.

  Os usuários que recebem acesso de Edição aos usuários em seus níveis de acesso podem gerenciar os usuários subordinados a eles. Para obter informações sobre como gerenciar um usuário, consulte [Exibir o organograma](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Um usuário com uma licença de Plano padrão que criou um usuário pode desativar, excluir ou editar o usuário que ele criou. Para obter informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, conforme explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Para alterar a capacidade de usuários com uma licença de Plano ou Trabalho exibirem os perfis de outros usuários:

   1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no botão **Exibir** à direita de **Usuários**.

   1. Desabilite **Exibir informações de contato** e clique no X para fechar a caixa **Ajustar suas configurações**.

      ![ajustar configurações do usuário](assets/fine-tune-users.png)

1. Para modificar a capacidade de usuários com acesso a licença de Plano de editar outros usuários, clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no botão **Editar** à direita de **Usuários** e selecione as capacidades que deseja conceder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Criar</strong> </td> 
      <td> <p>Permite aos usuários criar usuários.<br>Esta opção está habilitada por padrão.</p> 
     <p><b>OBSERVAÇÃO</b>: não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte o administrador de rede ou de TI se precisar de mais informações.</p>
        </td>  
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Excluir</strong> </td> 
      <td> <p> Permite que os usuários excluam os usuários que eles próprios criaram.<br>Esta opção está habilitada por padrão.</p> <p><b>OBSERVAÇÃO</b>: não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte o administrador de rede ou de TI se precisar de mais informações.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador de Usuários (Todos os Usuários)</strong> </td> 
      <td> <p>Permite que os usuários façam o seguinte para qualquer usuário no Workfront:</p> 
       <ul> 
        <li>Editar, excluir ou desativar o usuário</li> 
        <li>Fazer logon como usuário<p><b>OBSERVAÇÃO</b>: você não pode fazer logon como qualquer usuário administrador do sistema.</p></li> 
        <li>Redefinir a senha do usuário</li> 
       </ul> <p>Essa opção está desabilitada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador de Usuários (Usuários de Grupo)</strong> </td> 
      <td> <p>Permite que os usuários façam o seguinte para qualquer usuário em um grupo que administram: 
        <ul>
         <li><p>Editar, excluir ou desativar o usuário</p></li>
         <li>Fazer logon como usuário</li>
         <li><p>Redefinir a senha do usuário</p><p><b>OBSERVAÇÃO</b>: um administrador de grupo não pode fazer logon como ou redefinir a senha de um administrador do Workfront.</p></li>
        </ul><p>Essa opção está desabilitada por padrão.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se você não quiser conceder aos administradores de grupos acesso a todos os membros dos grupos que eles administram, desative ambas as opções de Administrador de usuários acima. Os administradores de grupo ainda poderão acessar membros de grupo que adicionam à Workfront ou que se reportam a eles no Workfront.

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

## Acesso a usuários por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com os usuários, consulte a seção [Usuários](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
