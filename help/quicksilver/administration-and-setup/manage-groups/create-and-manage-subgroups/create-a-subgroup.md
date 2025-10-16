---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Criar um subgrupo
description: É possível criar um subgrupo em um grupo que você gerencia para organizar usuários e projetos e atribuir direitos de acesso no Adobe Workfront. Normalmente, os administradores de grupos gerenciam grupos e subgrupos. Eles podem usar a página Grupos para gerenciar seus grupos e subgrupos em um único local.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Criar um subgrupo

É possível criar um subgrupo em um grupo que você gerencia para organizar usuários e projetos e atribuir direitos de acesso no Adobe Workfront.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Normalmente, no entanto, os administradores de grupos gerenciam grupos e subgrupos. Eles podem usar a página Grupos para gerenciar seus grupos e subgrupos em um único local. Para obter informações sobre como grupos e subgrupos funcionam na Workfront, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md) e [Visão geral dos subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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
       <p>Plano</p></td>
  </tr>
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar um subgrupo

{{step-1-to-setup}}

1. Clique em **Grupos**.

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Selecione o grupo ou subgrupo existente ao qual deseja adicionar um novo subgrupo.
1. Clique em **Novo Subgrupo**.
1. Na caixa **Novo Subgrupo** exibida, digite um **Nome do grupo** para o subgrupo.
1. (Opcional) Insira qualquer uma das seguintes informações:

   * **Descrição**: digite uma descrição para o subgrupo. É possível digitar até 512 caracteres.
   * **Está ativo**: esta opção é habilitada por padrão e torna o grupo ativo na sua instância do Workfront.

     Em campos de digitação antecipada como o mostrado abaixo, quando os usuários regulares procuram um grupo para anexá-lo a um objeto ou compartilhar um objeto com ele, somente os grupos ativos são exibidos na lista.

     ![Campo de digitação antecipada para um grupo](assets/typeahead-for-group.png)

     Para simplificar isso para seus usuários, você pode desabilitar a opção **Está ativo** para grupos que não estão em uso no momento.

     Você pode visualizar, filtrar e agrupar facilmente a lista Grupos com base no status ativo ou inativo usando esse campo. Para obter informações sobre como usar modos de exibição, filtros e agrupamentos em listas, consulte [Elementos de relatório: filtros, modos de exibição e agrupamentos](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   * **Líder de negócios**: você pode atribuir um usuário como Líder de negócios para um subgrupo que você gerencia. Um Líder de negócios é alguém que toma decisões de negócios para o subgrupo. Para obter mais informações, consulte [Visão geral do Líder de negócios](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

     Se a pessoa ainda não for membro do subgrupo, adicionar seu nome a esse campo também a adicionará ao grupo.

     >[!NOTE]
     >
     >* Antes de remover o Líder Comercial de um subgrupo, você deve remover o nome dele do campo Líder Comercial.
     >* Se você remover o nome do campo Líder de negócios, esse usuário permanecerá membro do subgrupo, a menos que você o remova dele. Para obter instruções sobre como remover alguém de um grupo, consulte [Exibir e gerenciar as associações de um grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

   * **Membros do grupo e administradores do grupo**: para adicionar usuários e grupos como membros do subgrupo, comece digitando o nome de um usuário ou grupo existente que você deseja adicionar e, em seguida, selecione o nome quando ele aparecer.

     Os usuários e grupos adicionados têm acesso a todos os objetos compartilhados com o grupo.

     Um subgrupo herda os administradores do grupo acima dele, portanto, especificar um usuário como administrador de grupo para um subgrupo é opcional. Você pode atribuir um membro do grupo como administrador do grupo usando o menu suspenso à direita do nome do usuário.

   * **Pesquisar pessoas e grupos na lista**: se você precisar encontrar um usuário ou grupo já atribuído a este subgrupo, digite o nome dele aqui e selecione-o quando ele aparecer.

1. Clique em **Salvar.**
