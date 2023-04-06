---
title: Conceder acesso ao Planejador de cenário
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário ao Planejador de Cenário.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# Conceder acesso ao Planejador de cenário

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário ao Planejador de Cenário, como explicado em [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Além do acesso ao Planejador de Cenário, um usuário com um nível de acesso que não seja Administrador do Sistema também deve ter acesso aos dados financeiros para ver quaisquer informações financeiras contidas em um plano, como orçamentos, custos e taxas de função do cargo. Para obter mais informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Plano Adobe Workfront*</p> </td> 
   <td>Empresa ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revise ou superior. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref" data-mc-variable-override="">Visão geral de licenças herdadas</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve comprar uma licença adicional para o Adobe Workfront Scenario Planner para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o Workfront Scenario Planner, consulte <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref" data-mc-variable-override="">Acesso necessário para usar o Planejador de cenário</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Visualizar acesso ou superior ao Planejador de cenário</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permissões de objeto</p> </td> 
   <td> <p>Exibir permissões ou superior para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../../../scenario-planner/request-access-to-plan.md" class="MCXref xref" data-mc-variable-override="">Solicitar acesso a um plano no Planejador de Cenário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Configurar o acesso do usuário ao Scenario Planner usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, como explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique na opção à direita de **Planejador de Cenário** que você deseja usar para esse nível de acesso.

   >[!NOTE]
   >
   >O tipo de licença Solicitação ou Externa não permite o acesso de Exibição ou Edição ao Planejador de Cenário.

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configuração do acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

## Acesso ao Scenario Planner por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com o Planejador de Cenário, consulte a seção [Área do Planejador de Cenário](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acesso do Planejador de cenário por definição de nível de acesso

As informações a seguir podem ajudar você a entender como usar as configurações de nível de acesso para controlar o acesso dos usuários às informações no Workfront Scenario Planner.

* [Sem acesso](#no-access)
* [Exibir acesso](#view-access)
* [Editar acesso](#edit-access)

### Sem acesso {#no-access}

Um usuário sem acesso ao Planejador de Cenário não pode ver o ícone Cenários no Menu Principal quando ele é adicionado ao modelo de layout, nem visualizar planos e iniciativas compartilhados com ele. Se o link para um plano for compartilhado com um usuário que não tem acesso ao Planejador de Cenário, o usuário não poderá visualizar ou editar o plano.

### Exibir acesso {#view-access}

Os usuários com acesso de Exibição ao Planejador de Cenário podem fazer o seguinte:

* Consulte o ícone Cenários no Menu principal ![](assets/esp-icon-in-main-menu.png), embora a área Planos esteja vazia, a menos que o usuário clique em um link de plano compartilhado por outro usuário.
* Exiba um plano quando outro usuário compartilhar o link com ele.

   Isso inclui qualquer informação de função de cargo no plano.

   Também inclui taxas de função de cargo e informações de custo sobre o plano se o usuário do recipient também tiver acesso a dados financeiros. Para obter mais informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Editar acesso {#edit-access}

Os usuários com acesso Editar ao Planejador de Cenário podem fazer o seguinte:

* Consulte o ícone Cenários no Menu principal ![](assets/esp-icon-in-main-menu.png) e usá-lo para acessar os dados do plano.
* Crie planos.
* Exiba, edite e exclua planos que eles criarem.
* Exiba, edite e exclua os planos de outros usuários que eles acessam usando um link compartilhado.

   Isso inclui qualquer informação sobre a função de cargo em um plano.

   Também inclui taxas de função de cargo e informações de custo sobre o plano se o usuário do recipient tiver acesso a dados financeiros. Para obter mais informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
