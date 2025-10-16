---
title: Conceder acesso ao gerenciamento de recursos
user-type: administrator
product-area: system-administration;resource-management
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário ao Gerenciamento de recursos no Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 14948e33-3dd7-4ef3-9307-51628dedd1f5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 5%

---

# Conceder acesso ao Gerenciamento de recursos

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário ao Gerenciamento de Recursos, conforme explicado na [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o acesso do usuário às ferramentas de Gerenciamento de recursos usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, conforme explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no botão **Exibir** ou **Editar** à direita de Gerenciamento de Recursos e selecione as capacidades que deseja conceder em **Ajustar suas configurações**.

   ![](assets/resource-management-details-of-edit-in-the-access-level.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Editar prioridades e horas de orçamento no Planejador</td> 
      <td> <p>Permite que os usuários com esta licença façam o seguinte:</p> <p>Priorizar projetos no Planejador de recursos.</p> <p>Alocação de orçamento para recursos nas ferramentas de Planejamento de Recursos (a seção Planejador de Recursos e Orçamento de Recursos no Business Case de um projeto).</p> <p>Essa opção está ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar Conjuntos de Recursos</td> 
      <td> <p>Permite que os usuários com esta licença criem, editem e excluam Conjuntos de Recursos. Essa opção está desabilitada por padrão.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>Atualizar horas planejadas no Balanceador de carga de trabalho</span> </td> 
      <td> <p>Permite que os usuários com esta licença atualizem as Horas planejadas dos itens de trabalho quando atualizam as alocações de usuário no Balanceador de carga de trabalho. O número total de horas alocadas torna-se as Horas Planejadas dos itens de trabalho.</p> <p>Essa opção está desabilitada por padrão.</p> <p> Para obter mais informações, consulte <a href="../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuário no Balanceador de carga de trabalho</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

   Após criar o nível de acesso, você pode atribuí-lo a um usuário. Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acesso ao Gerenciamento de recursos por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com o Gerenciamento de Recursos, consulte a seção [Gerenciamento de Recursos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#resource) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acesso a problemas compartilhados

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Quando você compartilha um objeto com outro usuário, os direitos do recipient ao orçar ou exibir a alocação de recursos nele são determinados por uma combinação de 3 itens:

* A configuração do nível de acesso do recipient para o Gerenciamento de recursos
* O acesso do usuário a dados financeiros, conforme explicado em [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* Quaisquer permissões para dados financeiros que o compartilhador concedeu para o objeto

Para obter informações sobre permissões que os usuários podem conceder a dados financeiros em um objeto ao compartilhá-lo, consulte [Compartilhar permissões financeiras em um objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).
