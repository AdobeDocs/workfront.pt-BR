---
title: Conceder acesso ao gerenciamento de recursos
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário ao Gerenciamento de recursos no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 3%

---

# Conceder acesso ao gerenciamento de recursos

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário ao Gerenciamento de Recursos, como explicado em [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Configurar o acesso do usuário às ferramentas de Gerenciamento de Recursos usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, como explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no **Exibir** ou **Editar** à direita de Gerenciamento de Recursos, selecione as capacidades que deseja conceder em **Ajustar as configurações**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Editar prioridades e horas de orçamento no Planejador</td> 
      <td> <p>Permite que os usuários com esta licença façam o seguinte:</p> <p>Priorize projetos no Planejador de Recursos.</p> <p>Alocação de orçamento para recursos nas ferramentas de Planejamento de Recursos (o Planejador de Recursos e a seção Orçamento de Recursos no Caso de Negócios de um projeto).</p> <p>Essa opção é ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar Conjuntos de Recursos</td> 
      <td> <p>Permite que usuários com esta licença criem, editem e excluam Pools de Recursos. Essa opção é desativada por padrão.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Atualizar horas planejadas no Balanceador de carga de trabalho</span> </td> 
      <td> <p>Permite que os usuários com esta licença atualizem as Horas Planejadas dos itens de trabalho quando atualizarem as alocações de usuário no Balanceador de Carga de Trabalho. O número total de horas alocadas se torna as Horas Planejadas dos itens de trabalho.</p> <p>Essa opção é desativada por padrão.</p> <p> Para obter mais informações, consulte <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuários no Balanceador de Carga de Trabalho</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configuração do acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

   Depois que o nível de acesso é criado, você pode atribuí-lo a um usuário. Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acesso ao Gerenciamento de Recursos por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com o Gerenciamento de Recursos, consulte a seção [Gerenciamento de recursos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acesso a problemas compartilhados

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Quando você compartilha um objeto com outro usuário, os direitos do recipient de orçar ou exibir a alocação de recursos nele são determinados por uma combinação de três itens:

* A configuração de nível de acesso do recipient para o Gerenciamento de Recursos
* O acesso do usuário aos dados financeiros, como explicado em [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Permissões para dados financeiros que o compartilhador concedeu para o objeto

Para obter informações sobre permissões que os usuários podem conceder aos dados financeiros de um objeto ao compartilhá-lo, consulte [Compartilhar permissões financeiras em um objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
