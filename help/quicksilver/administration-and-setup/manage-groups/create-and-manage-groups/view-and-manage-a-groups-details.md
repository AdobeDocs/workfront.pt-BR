---
title: Exibir e gerenciar os detalhes de um grupo
description: Você pode exibir e editar a página Detalhes do Grupo de um grupo ou subgrupo que gerencia.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 1%

---

# Exibir e gerenciar os detalhes de um grupo

Você pode exibir e editar a página Detalhes do Grupo de um grupo ou subgrupo que gerencia. Esta página inclui:

* Uma descrição do grupo
* Os nomes do Líder de negócios e dos administradores de grupo
* Uma opção que permite tornar o grupo e seus subgrupos públicos ou privados

Para obter informações sobre outras maneiras de gerenciar um grupo, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Para obter informações sobre como desativar ou reativar um grupo, consulte [Desativar ou reativar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

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

## Exibir e gerenciar os detalhes de um grupo

{{step-1-to-setup}}

1. Clique em **Grupos**.

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo de nível superior que deseja editar.
1. Se desejar desativar ou reativar o grupo,
1. No menu esquerdo, clique em **Detalhes do grupo** e siga um destes procedimentos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td> <p>É possível digitar até 512 caracteres.</p> <p>Se o campo estiver em branco, clique em <strong>Adicionar</strong> para digitar uma descrição.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Está ativo</td> 
      <td> <p>(Ativado por padrão) Torna o grupo ativo na instância do Workfront.</p> <p>Em campos de digitação antecipada como o mostrado abaixo, quando os usuários regulares procuram um grupo para anexá-lo a um objeto ou compartilhar um objeto com ele, somente os grupos ativos são exibidos na lista.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Para simplificar isso para seus usuários, você pode desativar a opção Está ativo para grupos que não estão em uso no momento.</p> <p>Você pode visualizar, filtrar e agrupar facilmente a lista Grupos com base no status ativo ou inativo usando esse campo. Para obter informações sobre como usar modos de exibição, filtros e agrupamentos em listas, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Elementos de relatório: filtros, modos de exibição e agrupamentos</a>.</p> <p>Para obter informações sobre grupos inativos, consulte a seção <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Considerações para grupos inativos</a> no artigo <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Excluir ou desativar um formulário personalizado</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Acessibilidade de grupo</td> 
      <td> <p>(Disponível somente se você estiver visualizando Detalhes de um grupo, não de um subgrupo.) Habilite ou desabilite a opção <strong>Tornar este grupo e seus subgrupos privados</strong>.</p> <p>Para um grupo público, qualquer usuário (dentro ou fora do grupo) que tenha acesso de usuário de edição pode adicionar o grupo ao perfil de outros usuários. Eles não podem fazer isso para um grupo privado.</p> <p>Você pode editar essa opção somente no grupo pai superior em uma hierarquia de grupos que tenha mais de um nível. Todos os subgrupos do grupo pai herdam sua configuração.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Partes interessadas do grupo</td> 
      <td> 
       <ul> 
        <li><strong>Administradores de Grupo</strong>: adicionar ou remover usuários com uma licença de Planejador como administradores de grupo para o grupo. Comece digitando o nome de um usuário e clique no nome quando ele aparecer no menu suspenso.</li> 
        <li><strong>Líder de negócios</strong>: siga um destes procedimentos:
         <ul>
          <li>Se você ainda não atribuiu um Líder de negócios ao grupo, clique em <strong>Adicionar</strong>, comece digitando o nome do usuário que deseja atribuir e, em seguida, clique no nome da pessoa quando ele for exibido.</li>
          <li>Se o grupo já tiver um Líder de negócios e você quiser alterá-lo, clique duas vezes no nome do Líder de negócios existente. Exclua o nome, comece digitando o nome do usuário que deseja atribuir e, em seguida, clique no nome da pessoa quando ele for exibido.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adicionar um formulário personalizado</td> 
      <td>Se o seu nível de acesso permitir gerenciar formulários personalizados, adicione um formulário personalizado ao grupo. Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Formulários personalizados</a>.</td> 
     </tr> 
    </tbody> 
   </table>
