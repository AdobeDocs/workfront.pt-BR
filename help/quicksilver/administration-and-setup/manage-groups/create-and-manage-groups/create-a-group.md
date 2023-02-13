---
user-type: administrator
product-area: system-administration;user-management
keywords: criar,grupo,subgrupo,novo
navigation-topic: create-and-manage-groups
title: Criar um grupo
description: Como administrador do Adobe Workfront, você pode criar grupos para organizar usuários e projetos e atribuir direitos de acesso no Workfront.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 3%

---

# Criar um grupo

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Como administrador do Adobe Workfront, você pode criar grupos para organizar usuários e projetos e atribuir direitos de acesso no Workfront. Para obter mais informações, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Cada subgrupo precisa de pelo menos um administrador de grupo. Os administradores de grupo podem usar a página Grupos para gerenciar seus grupos em um único local.

Se você for um administrador de grupo ou um administrador do Workfront, também poderá criar subgrupos em um grupo. Para obter instruções, consulte [Criar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Criar um grupo de nível superior do zero

Essas etapas explicam como criar um novo grupo do zero. Para obter informações sobre como criar um grupo ou subgrupo copiando um existente, consulte [Criar um grupo de nível superior copiando um grupo ou subgrupo existente](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) neste artigo.

Você deve ser um administrador do Workfront para criar um grupo de nível superior.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Acima da lista de grupos, clique em **Novo grupo**.

   >[!TIP]
   >
   >Na parte inferior da lista de grupos, você também pode clicar em **Adicionar mais grupos** para adicionar um grupo em linha, clique em **Enter** quando terminar de adicionar as informações do grupo.

1. No **Novo grupo** que é exibida, digite um nome para o grupo.
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
      <td> <p>(Ativado por padrão) Torna o grupo ativo na instância do Workfront.</p> <p>Em campos do tipo forward como o mostrado abaixo, quando usuários regulares pesquisam um grupo para anexá-lo a um objeto ou para compartilhar um objeto com ele, somente grupos ativos são exibidos na lista.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para simplificar isso para seus usuários, você pode desativar a opção Está ativo para grupos que não estão em uso no momento.</p> <p>É possível exibir, filtrar e agrupar facilmente a lista de Grupos com base no status ativo ou inativo usando esse campo. Para obter informações sobre o uso de exibições, filtros e agrupamentos em listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatório: filtros, visualizações e agrupamentos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tornar este grupo e seus subgrupos públicos</td> 
      <td> <p>(Disponível somente se você estiver visualizando Detalhes de um grupo de nível superior, não de um subgrupo.) Ative essa opção para permitir que os usuários do grupo com acesso de usuário de edição (que não são administradores do grupo) adicionem esse grupo e seus subgrupos ao perfil de usuário de outros usuários.</p> <p>Para um grupo público, qualquer usuário (dentro ou fora do grupo) que tenha acesso de usuário de edição pode adicionar o grupo ao perfil de outros usuários. Eles não podem fazer isso por um grupo privado.</p> <p>Você pode editar essa opção somente no grupo principal superior em uma hierarquia de grupos que tenha mais de um nível. Todos os subgrupos do grupo pai herdam sua configuração.</p> <p><b>Nota</b>:  
        <ul> 
         <li>Você não pode tornar um subgrupo público por si só, mas pode torná-lo público, o que também torna públicos todos os subgrupos dos pais.</li> 
         <li>Um subgrupo que pertence a um grupo público é público por padrão, portanto, qualquer usuário com acesso de usuário de edição também pode adicionar o subgrupo a outros usuários.</li> 
        </ul> </p> <p>Se precisar de informações sobre o acesso necessário para editar usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>. Para obter informações sobre como editar usuários, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Líder de negócios </td> 
      <td> <p>Você pode atribuir um usuário como Líder de Negócios para um grupo que você gerencia. Um Líder de Negócios é alguém que toma decisões de negócios para o grupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Visão geral do líder empresarial</a><span>.</span></p> <p>Se a pessoa ainda não for membro do grupo, a adição do nome a esse campo também a adicionará ao grupo.</p> <p><b>Nota</b>:  
        <ul> 
         <li>Antes de remover o Líder de Negócios de um grupo, você deve remover o nome dele do campo Líder de Negócios.</li> 
         <li>Se você remover o nome do campo Líder de negócios , esse usuário permanecerá membro do grupo, a menos que você os remova dele. Para obter instruções sobre como remover alguém de um grupo, consulte a seção <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Gerenciar as associações de um grupo</a> no artigo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Gerenciar um grupo</a>.</li> 
        </ul> </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Visão geral do líder empresarial</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membros do Grupo e Administradores de Grupos</td> 
      <td> 
       <ul> 
        <p>Para adicionar membros do grupo, comece a digitar o nome de um usuário ou grupo existente que deseja adicionar e selecione o nome quando for exibido.</p> 
        <p>Os usuários e grupos adicionados têm acesso a todos os objetos compartilhados com o grupo.</p>
        <p>Um grupo de nível superior deve ter pelo menos um administrador de grupo. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Procurar pessoas e grupos na lista</td> 
      <td> Se você precisar localizar um usuário ou grupo já atribuído a esse grupo, digite o nome e selecione-o quando aparecer.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Criar grupo**.

## Criar um grupo de nível superior copiando um grupo ou subgrupo existente {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Como administrador do Workfront, você pode criar um novo grupo de nível superior copiando um grupo ou subgrupo existente.

Lembre-se do seguinte:

* Todos os membros e subgrupos pertencentes ao grupo existente são copiados para o novo grupo de nível superior.
* Os membros do grupo copiado mantêm as atribuições que tinham no grupo original. Portanto, os administradores de grupo do grupo original também são designados como administradores de grupo no grupo copiado.

Para criar um novo grupo de nível superior copiando um grupo ou subgrupo:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

   Na lista que é exibida, é possível ver os grupos gerenciados, juntamente com os subgrupos que eles possuem. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Selecione o grupo que deseja copiar e clique no ícone Copiar ![](assets/copy-icon.png).
1. No **Copiar grupo** que aparece, digite um **Nome do grupo** para o grupo copiado.

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
      <td> <p>(Ativado por padrão) Torna o grupo ativo na instância do Workfront.</p> <p>Em campos do tipo forward como o mostrado abaixo, quando usuários regulares pesquisam um grupo para anexá-lo a um objeto ou para compartilhar um objeto com ele, somente grupos ativos são exibidos na lista.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para simplificar isso para seus usuários, você pode desativar a opção Está ativo para grupos que não estão em uso no momento.</p> <p>É possível exibir, filtrar e agrupar facilmente a lista de Grupos com base no status ativo ou inativo usando esse campo. Para obter informações sobre o uso de exibições, filtros e agrupamentos em listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementos de relatório: filtros, visualizações e agrupamentos</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tornar este grupo e seus subgrupos públicos</td> 
      <td> <p>(Disponível somente se você estiver visualizando Detalhes de um grupo de nível superior, não de um subgrupo.) Ative essa opção para permitir que os usuários do grupo com acesso de usuário de edição (que não são administradores do grupo) adicionem esse grupo e seus subgrupos ao perfil de usuário de outros usuários.</p> <p>Para um grupo público, qualquer usuário (dentro ou fora do grupo) que tenha acesso de usuário de edição pode adicionar o grupo ao perfil de outros usuários. Eles não podem fazer isso por um grupo privado.</p> <p>Você pode editar essa opção somente no grupo principal superior em uma hierarquia de grupos que tenha mais de um nível. Todos os subgrupos do grupo pai herdam sua configuração.</p> <p><b>Nota</b>:  
        <ul> 
         <li>Você não pode tornar um subgrupo público por si só, mas pode torná-lo público, o que também torna públicos todos os subgrupos dos pais.</li> 
         <li>Um subgrupo que pertence a um grupo público é público por padrão, portanto, qualquer usuário com acesso de usuário de edição também pode adicionar o subgrupo a outros usuários.</li> 
        </ul> </p> <p>Se precisar de informações sobre o acesso necessário para editar usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Conceder acesso aos usuários</a>. Para obter informações sobre como editar usuários, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Editar o perfil de um usuário</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Líder de negócios </td> 
      <td> <p>Você pode atribuir um usuário como Líder de Negócios para um grupo que você gerencia. Um Líder de Negócios é alguém que toma decisões de negócios para o grupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral do líder empresarial</a><span>.</span></p> <p>Se a pessoa ainda não for membro do grupo, a adição do nome a esse campo também a adicionará ao grupo.</p> <p><b>Nota</b>:  
        <ul> 
         <li>Antes de remover o Líder de Negócios de um grupo, você deve remover o nome dele do campo Líder de Negócios.</li> 
         <li>Se você remover o nome do campo Líder de negócios , esse usuário permanecerá membro do grupo, a menos que você os remova dele. Para obter instruções sobre como remover alguém de um grupo, consulte a seção <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gerenciar as associações de um grupo</a> no artigo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gerenciar um grupo</a>.</li> 
        </ul> </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral do líder empresarial</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membros do Grupo e Administradores de Grupos</td> 
      <td> 
       <ul> 
        <li> <p>Membros do grupo: Para adicionar usuários e grupos ao grupo, comece a digitar o nome de um usuário ou grupo existente que deseja adicionar e selecione o nome quando for exibido.</p> <p>Os usuários e grupos adicionados têm acesso a todos os objetos compartilhados com o grupo.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.copied groups">Administradores de grupo: Todos os administradores de grupo do grupo original também são designados como administradores de grupo no grupo copiado. Você pode atribuir um membro do grupo como administrador para o grupo usando o menu suspenso à direita do nome do usuário.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Um grupo de nível superior deve ter pelo menos um administrador de grupo.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Procurar pessoas e grupos na lista</td> 
      <td> Se você precisar localizar um usuário ou grupo já atribuído a esse grupo, digite o nome e selecione-o quando aparecer.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Se o grupo original tiver subgrupos, os subgrupos serão adicionados ao novo grupo e seus nomes serão, por padrão, &quot;O nome do subgrupo original (Cópia)&quot;.
   >* É possível eliminar qualquer usuário ou subgrupo do grupo original clicando no X à direita do nome do usuário ou subgrupo.


1. Clique em **Criar grupo**.
