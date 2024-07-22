---
product-area: enterprise-scenario-planner-product-area
keywords: plano,permissões,compartilhamento,iniciativas,cenários,cenário
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Compartilhar um plano no Planejador de cenários
description: Você pode compartilhar um plano criado no Planejador de cenários do Adobe Workfront com outros usuários.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# Compartilhar um plano no [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Você pode compartilhar um plano no [!DNL Adobe Workfront Scenario Planner] com outros usuários para que eles possam colaborar no mesmo trabalho que você faz.

>[!TIP]
>
>Se você enviar um link para um plano para outras pessoas, também deverá compartilhar o plano com elas para que elas possam exibi-lo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plano*</p> </td> 
   <td> <p>Atual: [!UICONTROL Business] ou superior</p>
   <p>Novo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td> <p>Novo: Claro ou superior</p> 
   <p>Atual: [!UICONTROL Review] ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto* </td> 
   <td> 
   <p>Para os planos atuais do Workfront: </p>
   <p>Você deve comprar uma licença adicional para o [!DNL Adobe Workfront Scenario Planner] acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre acesso e permissões para o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nível de acesso </td> 
   <td> <p>[!UICONTROL Editar] acesso à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>[!UICONTROL Gerenciar] permissões para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* Os usuários que recebem permissões para o plano devem ter acesso à área [!DNL Scenario Planner] em seus Níveis de Acesso, conforme concedido pelo administrador do [!DNL Workfront], para receber permissões para um plano.

  Por exemplo, [!UICONTROL Solicitantes] não podem exibir, criar ou editar planos. Lembre-se disso ao compartilhar um plano com um usuário que tenha uma licença de Solicitante.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Para obter mais informações sobre o acesso ao [!DNL Scenario Planner] para vários tipos de licença, consulte [Conceder acesso ao [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Considerações sobre o compartilhamento do plano

* Todos os usuários, incluindo administradores do sistema, têm acesso somente aos planos que criaram.
* Você pode compartilhar um único plano ou vários planos em massa.
* Não é possível exibir planos que você não criou ou que não estão compartilhados com você.
* Você só pode compartilhar um plano com outros usuários. Não é possível compartilhar planos com grupos, equipes ou empresas.
* Primeiro, salve um plano antes de compartilhá-lo.
* Você pode compartilhar um URL para um plano com outro usuário. Se o usuário não tiver permissões para pelo menos exibir o plano, poderá solicitar acesso ao plano a outro usuário quando receber o URL. Para obter informações sobre como solicitar acesso a um plano, consulte [Solicitar acesso a um plano no [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Ao compartilhar vários planos que já foram compartilhados com outras pessoas, os usuários com os quais você compartilha não substituem, mas são adicionados aos usuários existentes em cada plano selecionado.

## Opções de permissão do plano

A tabela a seguir lista as permissões que você pode conceder ao compartilhar um plano. Para obter mais informações sobre o acesso que os usuários obtêm com base em suas licenças, consulte [Conceder acesso ao [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Ações</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL gerenciar]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Exibição]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Exibir plano </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Exibir iniciativas </p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p>✓ µ</p> </td> 
  </tr> 
  <tr> 
   <td>Exibir cenários</td> 
   <td>✓ µ</td> 
   <td>✓ <span style="font-weight: normal;"></span> </td> 
  </tr> 
  <tr> 
   <td>Exibir funções de trabalho</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td>Exibir informações de custo e orçamento*</td> 
   <td>✓ µ</td> 
   <td>✓ µ </td> 
  </tr> 
  <tr> 
   <td>Gerenciar informações de custo e orçamento*</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Criar iniciativas</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Criar cenários</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Excluir iniciativas ou cenários</p> </td> 
   <td> <p>✓ µ</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Copiar cenários</td> 
   <td>✓ µ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Cenários do Publish**</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Você deve ter acesso aos Dados Financeiros para visualizar ou gerenciar informações financeiras nos planos, mesmo se tiver permissões de gerenciamento para os planos. Para obter informações sobre acesso a dados financeiros, consulte [Conceder acesso a dados financeiros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**É necessário ter acesso para criar e gerenciar projetos e permissões para poder publicar cenários.

Para obter informações sobre o nível de acesso do projeto, consulte [Conceder acesso aos projetos](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obter informações sobre permissões de projeto, consulte [Compartilhar um projeto em [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

## Compartilhar planos

{{step1-to-scenario-planner}}

1. Clique no nome de um plano para abri-lo

   Ou

   Selecione vários planos para compartilhá-los em massa.

   >[!TIP]
   >
   >Você pode compartilhar um plano clicando nos avatares dos usuários com os quais o plano é compartilhado no canto superior direito do cabeçalho do plano.

1. (Condicional) Se você abriu um plano, clique no ícone **[!UICONTROL Mais]** ![](assets/more-icon.png) à direita do nome do [!UICONTROL Plano] e clique em **[!UICONTROL Compartilhar]**

   Ou

   Se você selecionou vários planos para compartilhá-los em massa, clique no ícone **[!UICONTROL Compartilhar]** ![](assets/share-icon-26x26.png) na parte superior da lista de planos para abrir a caixa de acesso [!UICONTROL Plano].

   >[!TIP]
   >
   >* Os usuários que têm permissões para todos os planos selecionados são exibidos na caixa de acesso [!UICONTROL Plano].
   >* Usuários adicionais são adicionados a e não substituem os usuários existentes em todos os planos selecionados.

1. No campo **[!UICONTROL Conceder acesso ao plano]**, comece digitando o nome dos usuários com os quais deseja compartilhar o plano e selecione-os quando eles aparecerem na lista.
1. No menu suspenso de permissões à direita do nome do usuário, selecione o nível de permissão que deseja conceder a elas para o plano.
1. Selecione entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Exibir]</td> 
      <td>Os usuários com os quais você compartilha o plano terão permissões para exibir o plano. Eles não podem editar informações sobre o plano, adicionar iniciativas, cenários ou publicar cenários. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Gerenciar]</td> 
      <td> <p>Os usuários com os quais você compartilha o plano têm permissões para gerenciar o plano, o que inclui editar informações, adicionar iniciativas, cenários e publicar o plano. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Você pode deletar um plano somente quando o criou. Não é possível excluir planos compartilhados com você.

1. Clique em **[!UICONTROL Salvar]**.

   O plano agora é compartilhado com os usuários especificados.

   Você pode exibir os usuários que têm permissões para o plano na coluna Compartilhado comigo em uma lista de planos ou no canto superior direito do cabeçalho do plano.

   >[!TIP]
   >
   >Você pode exibir planos compartilhados com você aplicando o filtro [!UICONTROL Compartilhado comigo] em uma lista de planos.


