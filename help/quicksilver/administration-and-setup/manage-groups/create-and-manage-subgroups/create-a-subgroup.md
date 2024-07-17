---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Criar um subgrupo
description: É possível criar um subgrupo em um grupo que você gerencia para organizar usuários e projetos e atribuir direitos de acesso no Adobe Workfront. Normalmente, os administradores de grupos gerenciam grupos e subgrupos. Eles podem usar a página Grupos para gerenciar seus grupos e subgrupos em um único local.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 3%

---

# Criar um subgrupo

É possível criar um subgrupo em um grupo que você gerencia para organizar usuários e projetos e atribuir direitos de acesso no Adobe Workfront.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Normalmente, no entanto, os administradores de grupos gerenciam grupos e subgrupos. Eles podem usar a página Grupos para gerenciar seus grupos e subgrupos em um único local. Para obter informações sobre como grupos e subgrupos funcionam na Workfront, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md) e [Visão geral dos subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença, contate o administrador do Workfront.

## Adicionar um subgrupo

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Grupos**.

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Selecione o grupo ou subgrupo existente ao qual deseja adicionar um novo subgrupo.
1. Clique em **Novo Subgrupo**.
1. Na caixa **Novo Subgrupo** exibida, digite um **Nome do Grupo** para o subgrupo.
1. (Opcional) especifique qualquer uma das seguintes informações:

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
      <td>Digite uma descrição para o subgrupo. É possível digitar até 512 caracteres.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Está ativo</td> 
      <td> <p>(Ativado por padrão) Torna o grupo ativo na instância do Workfront.</p> <p>Em campos de digitação antecipada como o mostrado abaixo, quando os usuários regulares procuram um grupo para anexá-lo a um objeto ou compartilhar um objeto com ele, somente os grupos ativos são exibidos na lista.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para simplificar isso para seus usuários, você pode desativar a opção Está ativo para grupos que não estão em uso no momento.</p> <p>Você pode visualizar, filtrar e agrupar facilmente a lista Grupos com base no status ativo ou inativo usando esse campo. Para obter informações sobre como usar modos de exibição, filtros e agrupamentos em listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Elementos de relatório: filtros, modos de exibição e agrupamentos</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tornar este grupo e seus subgrupos públicos</td> 
      <td> <p>(Disponível somente se você estiver exibindo Detalhes para um grupo de nível superior, não para um subgrupo.) Ative esta opção para permitir que os usuários no subgrupo com acesso de edição de usuário (que não são administradores do grupo) adicionem esse grupo e seus subgrupos ao perfil de usuário de outros usuários.</p> <p>Para um grupo público, qualquer usuário (dentro ou fora do grupo) que tenha acesso de usuário de edição pode adicionar o grupo ao perfil de outros usuários. Eles não podem fazer isso para um grupo privado.</p> <p>Você pode editar essa opção somente no grupo pai superior em uma hierarquia de grupos que tenha mais de um nível. Todos os subgrupos do grupo pai herdam sua configuração.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Você não pode tornar um subgrupo público por si só, mas pode torná-lo público, o que também torna públicos todos os subgrupos do pai.</li> 
         <li>Um subgrupo que pertence a um grupo público é público por padrão, portanto, qualquer usuário com acesso de usuário de edição também pode adicionar o subgrupo a outros usuários.</li> 
        </ul> </p> <p>Se precisar de informações sobre o acesso necessário para editar usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Conceder acesso aos usuários</a>. Para obter informações sobre como editar usuários, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Editar perfil de usuário</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Líder de negócios </td> 
      <td> <p>Você pode atribuir um usuário como Líder de negócios para um subgrupo que gerencia. Um Líder de negócios é alguém que toma decisões de negócios para o subgrupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral do Líder de negócios</a><span>.</span></p> <p>Se a pessoa ainda não for membro do subgrupo, adicionar seu nome a esse campo também a adicionará ao grupo.</p> <p><b>NOTA</b>:  
        <ul> 
         <li>Antes de remover o Líder Comercial de um subgrupo, você deve remover o nome dele do campo Líder Comercial.</li> 
         <li>Se você remover o nome do campo Líder de negócios, esse usuário permanecerá membro do subgrupo, a menos que você o remova dele. Para obter instruções sobre como remover alguém de um grupo, consulte a seção <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gerenciar associações de um grupo</a> no artigo <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Gerenciar um grupo</a>.</li> 
        </ul> </p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Visão geral do Líder de negócios</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membros do Grupo e Administradores de Grupos</td> 
      <td> 
       <ul> 
        <li> <p>Membros do grupo: para adicionar usuários e grupos ao subgrupo, comece digitando o nome de um usuário ou grupo existente que deseja adicionar e, em seguida, selecione o nome quando ele for exibido.</p> <p>Os usuários e grupos adicionados têm acesso a todos os objetos compartilhados com o grupo.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Administradores de grupo: um subgrupo herda os administradores do grupo acima dele, portanto, especificar um usuário como administrador de grupo para um subgrupo é opcional. Você pode atribuir um membro do grupo como administrador do grupo usando o menu suspenso à direita do nome do usuário.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Procurar pessoas e grupos na lista</td> 
      <td> Se você precisar encontrar um usuário ou grupo já atribuído a este subgrupo, digite o nome dele aqui e selecione-o quando ele aparecer.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar.**
