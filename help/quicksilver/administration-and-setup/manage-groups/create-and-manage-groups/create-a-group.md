---
user-type: administrator
product-area: system-administration;user-management
keywords: criar,grupo,subgrupo,novo
navigation-topic: create-and-manage-groups
title: Criar um grupo
description: Como administrador do Adobe Workfront, você pode criar grupos para organizar usuários e projetos e atribuir direitos de acesso no Workfront.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1652'
ht-degree: 3%

---

# Criar um grupo

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Como administrador do Adobe Workfront, você pode criar grupos para organizar usuários e projetos e atribuir direitos de acesso no Workfront. Para obter mais informações, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Todo subgrupo precisa de pelo menos um administrador de grupo. Os administradores de grupo podem usar a página Grupos para gerenciar seus grupos em um único local.

Se você for um administrador de grupo ou um administrador do Workfront, também poderá criar subgrupos em um grupo. Para obter instruções, consulte [Criar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

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
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um grupo de nível superior do zero

Essas etapas explicam como criar um novo grupo do zero. Para obter informações sobre como criar um grupo ou subgrupo copiando um existente, consulte [Criar um grupo de nível superior copiando um grupo ou subgrupo existente](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) neste artigo.

Você precisa ser um administrador do Workfront para criar um grupo de nível superior.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Acima da lista de grupos, clique em **Novo Grupo**.

   >[!TIP]
   >
   >Na parte inferior da lista de grupos, você também pode clicar em **Adicionar mais grupos** para adicionar um grupo incorporado e, em seguida, clicar em **Inserir** quando terminar de adicionar as informações do grupo.

1. Na caixa **Novo Grupo** que é exibida, digite um nome para o grupo.
1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do grupo</td> 
      <td>Altere o nome do grupo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição para o grupo. É possível digitar até 512 caracteres.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Está ativo</td> 
      <td> <p>(Ativado por padrão) Torna o grupo ativo na instância do Workfront.</p> <p>Em campos de digitação antecipada como o mostrado abaixo, quando os usuários regulares procuram um grupo para anexá-lo a um objeto ou compartilhar um objeto com ele, somente os grupos ativos são exibidos na lista.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para simplificar isso para seus usuários, você pode desativar a opção Está ativo para grupos que não estão em uso no momento.</p> <p>Você pode visualizar, filtrar e agrupar facilmente a lista Grupos com base no status ativo ou inativo usando esse campo. Para obter informações sobre como usar modos de exibição, filtros e agrupamentos em listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatório: filtros, modos de exibição e agrupamentos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tornar este grupo e seus subgrupos públicos</td> 
      <td> <p>(Disponível somente se você estiver exibindo Detalhes para um grupo de nível superior, não para um subgrupo.) Ative esta opção para permitir que os usuários no grupo com acesso de edição de usuário (que não são administradores do grupo) adicionem este grupo e seus subgrupos ao perfil de usuário de outros usuários.</p> <p>Para um grupo público, qualquer usuário (dentro ou fora do grupo) que tenha acesso de usuário de edição pode adicionar o grupo ao perfil de outros usuários. Eles não podem fazer isso para um grupo privado.</p> <p>Você pode editar essa opção somente no grupo pai superior em uma hierarquia de grupos que tenha mais de um nível. Todos os subgrupos do grupo pai herdam sua configuração.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Você não pode tornar um subgrupo público por si só, mas pode tornar público o grupo pai de nível superior, o que também torna públicos todos os subgrupos do pai.</li> 
         <li>Um subgrupo que pertence a um grupo público é público por padrão, portanto, qualquer usuário com acesso de usuário de edição também pode adicionar o subgrupo a outros usuários.</li> 
        </ul> </p> <p>Se precisar de informações sobre o acesso necessário para editar usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>. Para obter informações sobre como editar usuários, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de usuário</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Líder de negócios </td> 
      <td> <p>Você pode atribuir um usuário como Líder de negócios para um grupo que gerencia. Um Líder de negócios é alguém que toma decisões de negócios para o grupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Visão geral do Líder de negócios</a><span>.</span></p> <p>Se a pessoa ainda não for membro do grupo, adicionar seu nome a esse campo também a adicionará ao grupo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Antes de remover o Líder de negócios de um grupo, é necessário remover o nome dele do campo Líder de negócios.</li> 
         <li>Se você remover o nome do campo Líder de negócios, esse usuário permanecerá membro do grupo, a menos que você o remova dele. Para obter instruções sobre como remover alguém de um grupo, consulte a seção <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Gerenciar associações de um grupo</a> no artigo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Gerenciar um grupo</a>.</li> 
        </ul> </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Visão geral do Líder de negócios</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membros do Grupo e Administradores de Grupos</td> 
      <td>
        <p>Para adicionar membros do grupo, comece digitando o nome de um usuário ou grupo existente que deseja adicionar e, em seguida, selecione o nome quando ele for exibido.</p> 
        <p>Os usuários e grupos adicionados têm acesso a todos os objetos compartilhados com o grupo.</p>
        <p>Um grupo de nível superior deve ter pelo menos um administrador de grupo. </p>
     </tr> 
     <tr> 
      <td role="rowheader">Procurar pessoas e grupos na lista</td> 
      <td> Se você precisar encontrar um usuário ou grupo já atribuído a esse grupo, digite o nome dele aqui e selecione-o quando ele aparecer.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Criar Grupo**.

## Criar um grupo de nível superior copiando um grupo ou subgrupo existente {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Como administrador do Workfront, você pode criar um novo grupo de nível superior copiando um grupo ou subgrupo existente.

Lembre-se do seguinte quando quiser fazer isso:

* Todos os membros e quaisquer subgrupos pertencentes ao grupo existente são copiados para o novo grupo de nível superior.
* Os membros do grupo copiado retêm as atribuições que tinham no grupo original. Portanto, os administradores de grupo do grupo original também são designados como os administradores de grupo no grupo copiado.

Para criar um novo grupo de nível superior copiando um grupo ou subgrupo:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Selecione o grupo que deseja copiar e clique no ícone Copiar ![](assets/copy-icon.png).
1. Na caixa **Copiar Grupo** exibida, digite um **Nome de Grupo** para o grupo copiado.

1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do grupo</td> 
      <td>Altere o nome do grupo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição para o grupo. É possível digitar até 512 caracteres.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Está ativo</td> 
      <td> <p>(Ativado por padrão) Torna o grupo ativo na instância do Workfront.</p> <p>Em campos de digitação antecipada como o mostrado abaixo, quando os usuários regulares procuram um grupo para anexá-lo a um objeto ou compartilhar um objeto com ele, somente os grupos ativos são exibidos na lista.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para simplificar isso para seus usuários, você pode desativar a opção Está ativo para grupos que não estão em uso no momento.</p> <p>Você pode visualizar, filtrar e agrupar facilmente a lista Grupos com base no status ativo ou inativo usando esse campo. Para obter informações sobre como usar modos de exibição, filtros e agrupamentos em listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementos de relatório: filtros, modos de exibição e agrupamentos</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tornar este grupo e seus subgrupos públicos</td> 
      <td> <p>(Disponível somente se você estiver exibindo Detalhes para um grupo de nível superior, não para um subgrupo.) Ative esta opção para permitir que os usuários no grupo com acesso de edição de usuário (que não são administradores do grupo) adicionem este grupo e seus subgrupos ao perfil de usuário de outros usuários.</p> <p>Para um grupo público, qualquer usuário (dentro ou fora do grupo) que tenha acesso de usuário de edição pode adicionar o grupo ao perfil de outros usuários. Eles não podem fazer isso para um grupo privado.</p> <p>Você pode editar essa opção somente no grupo pai superior em uma hierarquia de grupos que tenha mais de um nível. Todos os subgrupos do grupo pai herdam sua configuração.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Você não pode tornar um subgrupo público por si só, mas pode torná-lo público, o que também torna públicos todos os subgrupos do pai.</li> 
         <li>Um subgrupo que pertence a um grupo público é público por padrão, portanto, qualquer usuário com acesso de usuário de edição também pode adicionar o subgrupo a outros usuários.</li> 
        </ul> </p> <p>Se precisar de informações sobre o acesso necessário para editar usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Conceder acesso aos usuários</a>. Para obter informações sobre como editar usuários, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Editar perfil de usuário</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Líder de negócios </td> 
      <td> <p>Você pode atribuir um usuário como Líder de negócios para um grupo que gerencia. Um Líder de negócios é alguém que toma decisões de negócios para o grupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral do Líder de negócios</a><span>.</span></p> <p>Se a pessoa ainda não for membro do grupo, adicionar seu nome a esse campo também a adicionará ao grupo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Antes de remover o Líder de negócios de um grupo, é necessário remover o nome dele do campo Líder de negócios.</li> 
         <li>Se você remover o nome do campo Líder de negócios, esse usuário permanecerá membro do grupo, a menos que você o remova dele. Para obter instruções sobre como remover alguém de um grupo, consulte a seção <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gerenciar associações de um grupo</a> no artigo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gerenciar um grupo</a>.</li> 
        </ul> </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral do Líder de negócios</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membros do Grupo e Administradores de Grupos</td> 
      <td> 
       <ul> 
        <li> <p>Membros do grupo: para adicionar usuários e grupos ao grupo, comece digitando o nome de um usuário ou grupo existente que deseja adicionar e, em seguida, selecione o nome quando ele for exibido.</p> <p>Os usuários e grupos adicionados têm acesso a todos os objetos compartilhados com o grupo.</p> </li> 
        <li> <p>Administradores de grupo: quaisquer administradores de grupo do grupo original também são designados como os administradores de grupo no grupo copiado. Você pode atribuir um membro do grupo como administrador do grupo usando o menu suspenso à direita do nome do usuário.</p> <p>Um grupo de nível superior deve ter pelo menos um administrador de grupo.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Procurar pessoas e grupos na lista</td> 
      <td> Se você precisar encontrar um usuário ou grupo já atribuído a esse grupo, digite o nome dele aqui e selecione-o quando ele aparecer.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Se o grupo original tiver subgrupos, eles serão adicionados ao novo grupo e seus nomes serão, por padrão, &quot;O nome do subgrupo original (Copiar)&quot;.
   >* Você pode eliminar qualquer usuário ou subgrupo do grupo original clicando no X à direita do nome do usuário ou subgrupo.

1. Clique em **Criar Grupo**.
