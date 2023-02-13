---
title: Conceder acesso aos usuários
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a outros usuários no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: d1fe7165932fb6f2aff3c8488bdb8e1dfae3b6d3
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# Conceder acesso aos usuários

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a outros usuários no Workfront, como explicado em [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuração do acesso dos usuários

Você pode gerenciar quais informações os usuários podem visualizar e editar para outros usuários usando um nível de acesso padrão ou um nível de acesso personalizado criado por você. Os usuários com as licenças de Plano e Trabalho padrão podem exibir as informações de contato de outros usuários. Qualquer um dos usuários a seguir pode criar e editar outros usuários:

* Um administrador do Workfront.

   Para obter mais informações, consulte [Conceder ao usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* Um usuário com uma licença padrão do Plan que também tem acesso a usuários, conforme explicado neste artigo.

   Os usuários restritos para ver apenas usuários de sua empresa ou da empresa primária têm acesso para editar apenas os usuários que podem ver. Para obter mais informações, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Um usuário com uma licença padrão de Plano, que também é especificada como gerente de outro usuário.

   Os usuários que recebem o acesso Editar para os usuários em seu nível de acesso podem gerenciar usuários que relatam para eles. Para obter informações sobre como gerenciar um usuário, consulte [Exibir o gráfico organizacional](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* Um usuário com uma licença padrão do Plan que criou um usuário pode desativar, excluir ou editar o usuário que ele criou. Para obter informações sobre como criar novos usuários, consulte [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, como explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Para alterar a capacidade dos usuários com uma licença de Plano ou Trabalho de visualizar os perfis de outros usuários:

   1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no **Exibir** à direita de **Usuários**.

   1. Desativar **Exibir informações de contato** e clique no X para fechar o **Ajustar as configurações** caixa.

1. Para modificar a capacidade dos usuários com acesso a uma licença do Plano para editar outros usuários, clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no **Editar** à direita de **Usuários** e selecione as capacidades que deseja conceder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Criar</strong> </td> 
      <td> <p>Permite que usuários criem usuários.<br>Essa opção é ativada por padrão.</p> 
      &lt;!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Certifique-se de que essa alteração esteja sendo feita antes de desfazer a redação dessas duas notas. Em 29/3, o req doc diz que isso depende dos resultados da investigação.</p>

       &lt;p>&lt;b>OBSERVAÇÃO&lt;/b>: Isso não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte seu administrador de rede ou de TI se precisar de mais informações.&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Excluir</strong> </td> 
      <td> <p> Permite que os usuários excluam os usuários que eles próprios criaram.<br>Essa opção é ativada por padrão.</p> <p><b>OBSERVAÇÃO</b>: Isso não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte seu administrador de rede ou de TI se precisar de mais informações.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador de Usuários (Todos os usuários)</strong> </td> 
      <td> <p>Permite que os usuários façam o seguinte para qualquer usuário no Workfront:</p> 
       <ul> 
        <li>Editar, excluir ou desativar o usuário</li> 
        <li>Fazer logon como o usuário</li> 
        <li>Redefinir a senha do usuário</li> 
       </ul> <p>Essa opção é desativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador de Usuários (Usuários de Grupo)</strong> </td> 
      <td> <p>Permite que os usuários façam o seguinte para qualquer usuário em um grupo que eles administram: 
        <ul>
         <li><p>Editar, excluir ou desativar o usuário</p></li>
         <li>Fazer logon como o usuário</li>
         <li><p>Redefinir a senha do usuário</p><p><b>OBSERVAÇÃO</b>: Um administrador de grupo não pode fazer logon como ou redefinir a senha de um administrador do Workfront.</p></li>
        </ul><p>Essa opção é desativada por padrão.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Se você não quiser conceder acesso aos administradores de grupo a todos os membros dos grupos que eles administram, desative as duas opções de Administrador de usuário acima. Os administradores de grupo ainda poderão acessar membros de grupo adicionados ao Workfront ou que se reportam a eles no Workfront.

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configuração do acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

## Acesso dos utilizadores por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com os usuários, consulte a seção [Usuários](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
