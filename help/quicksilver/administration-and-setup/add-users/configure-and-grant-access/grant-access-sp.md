---
title: Conceder acesso ao Planejador de cenários
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário ao Planejador de cenários.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4343f0ff-2f78-4556-801f-db9d94f80c95
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Conceder acesso ao Planejador de cenários

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário ao Scenario Planner, conforme explicado na [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Além do acesso ao Planejador de Cenários, um usuário com um nível de acesso que não seja Administrador do Sistema também deve ter acesso a dados financeiros para ver qualquer informação financeira contida em um plano, como orçamentos, custos e taxas de funções de trabalho. Para obter mais informações, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Pacote do Adobe Workfront</p> </td> 
   <td>Business ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Leve ou superior</p>
   <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve adquirir uma licença adicional para o Planejador de cenários do Adobe Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir acesso ou superior ao Planejador de cenários</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permissões de objeto</p> </td> 
   <td> <p>Exibir permissões ou superiores para um plano</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o acesso do usuário ao Planejador de cenários usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, conforme explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique na opção à direita de **Planejador de cenários** que você deseja usar para este nível de acesso.

   >[!NOTE]
   >
   >O tipo de licença Solicitação ou Externa não permite acesso de Exibição ou Edição ao Planejador de Cenários.

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

## Acesso ao Scenario Planner por tipo de licença

Para obter informações sobre o que os usuários de cada nível de acesso podem fazer com o Planejador de cenários, consulte a seção [Área do Planejador de cenários](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#scenario) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acesso do Planejador de cenários por configuração de nível de acesso

As informações a seguir podem ajudá-lo a entender como usar as configurações de Nível de acesso para controlar o acesso dos usuários às informações no Planejador de cenários do Workfront.

* [Sem acesso](#no-access)
* [Acesso de visualização](#view-access)
* [Editar acesso](#edit-access)

### Sem acesso {#no-access}

Um usuário sem acesso ao Planejador de cenários não pode ver o ícone Cenários no Menu principal quando ele é adicionado ao modelo de layout, nem visualizar planos e iniciativas compartilhados com ele. Se o link para um plano for compartilhado com um usuário que não tem acesso ao Planejador de cenários, o usuário não poderá visualizar ou editar o plano.

### Exibir acesso {#view-access}

Os usuários com acesso de Exibição ao Planejador de cenários podem fazer o seguinte:

* Veja o ícone Cenários no Menu Principal ![](assets/esp-icon-in-main-menu.png), embora a área Planos esteja vazia, a menos que o usuário clique em um link de plano compartilhado por outro usuário.
* Exibir um plano quando outro usuário compartilhar o link com ele.

  Isso inclui todas as informações de função de trabalho no plano.

  Também inclui taxas de função de trabalho e informações de custo no plano se o usuário destinatário também tiver acesso a dados financeiros. Para obter mais informações, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

### Editar acesso {#edit-access}

Os usuários com acesso de Edição ao Planejador de cenários podem fazer o seguinte:

* Consulte o ícone Cenários no Menu Principal ![](assets/esp-icon-in-main-menu.png) e use-o para acessar os dados do plano.
* Criar planos.
* Exibir, editar e excluir os planos que eles criam.
* Exibir, editar e excluir os planos de outros usuários que eles acessam usando um link compartilhado.

  Isso inclui todas as informações de função de trabalho em um plano.

  Também inclui taxas de função de trabalho e informações de custo no plano se o usuário destinatário tiver acesso a dados financeiros. Para obter mais informações, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
