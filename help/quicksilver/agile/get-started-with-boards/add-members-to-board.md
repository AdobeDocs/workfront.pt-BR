---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Adicionar ou Remover Membros de um Quadro
description: As pessoas devem ser adicionadas ao painel como membros antes de visualizarem o painel e serem atribuídas a cartões.
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: bf8d566ba9d24310e75d2fbaf523fe5464bb6657
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Adicionar ou remover membros de um quadro

{{highlighted-preview}}

Pessoas e equipes devem ser adicionadas ao painel como membros antes de visualizarem o painel.

Por padrão, o criador de um quadro é o proprietário. O proprietário do painel é a única pessoa que pode excluir esse painel ou atualizar seus filtros no painel Configurar. <span class="preview">Somente um administrador do sistema ou o proprietário atual do painel pode alterar o proprietário do painel.</span>

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> 
   <p>Novo: [!UICONTROL Contributor] ou superior</p> 
   <p>ou</p>
   <p>Atual: [!UICONTROL Request] ou superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar membros a um quadro

{{step1-to-boards}}

1. Crie um novo painel ou edite um existente. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique no ícone **[!UICONTROL Adicionar membro]** ![Adicionar membros](assets/boards-addmember-spectrum-25x25.png).
1. Na caixa **[!UICONTROL Adicionar membros]**, comece digitando um nome e, em seguida, selecione-o quando ele for exibido na lista.

   Você pode selecionar um membro individual ou uma equipe. Se você escolher um grupo, o próprio grupo é adicionado ao quadro.

   >[!NOTE]
   >
   >Um usuário individual deve ter a opção **[!UICONTROL Exibir]** ou **[!UICONTROL Editar]** definida em seu nível de acesso para equipes, caso contrário, não poderá exibir o quadro.


   ![Adicionar membros ao painel](assets/boards-add-members.png)

## Remover membros de um quadro

{{step1-to-boards}}

1. Crie um novo painel ou edite um existente. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique no ícone **[!UICONTROL Adicionar membro]** ![Adicionar membros](assets/boards-addmember-spectrum-25x25.png).
1. Na caixa **[!UICONTROL Adicionar membros]**, clique no X ao lado do nome de uma pessoa ou equipe para removê-los do quadro.

   ![Remover membro do painel](assets/boards-remove-member-from-board-350x367.png)

   Ao remover um membro de um quadro, ele não é removido de nenhum cartão ao qual esteja atribuído. Para cartões conectados, as atribuições também são atualizadas na tarefa ou problema [!DNL Workfront].

   Os membros só são removidos deste quadro. Eles não são removidos de outros painéis aos quais pertencem.

   >[!NOTE]
   >
   >Você não pode remover o proprietário do painel.

<div class="preview">

## Alterar o proprietário do quadro

>[!NOTE]
>
>Somente um administrador do sistema ou o proprietário atual do painel pode alterar o proprietário do painel. Um quadro só pode ter um proprietário.
>
>A capacidade de alterar o proprietário do quadro está disponível nos quadros básico, retrospectivo e Kanban, mas não nos dinâmicos.

1. Acesse o quadro.
1. Clique no menu **[!UICONTROL Mais]** ![Mais menu](assets/more-icon-spectrum.png) ao lado do nome do quadro e escolha **[!UICONTROL Alterar proprietário do quadro]**.
1. Na caixa de diálogo Alterar proprietário do quadro, procure e selecione o usuário que deseja tornar o proprietário.

   Não é possível pesquisar usuários que já são membros do painel. Para tornar um membro existente o proprietário, primeiro você deve removê-lo do quadro. Transformar um usuário em proprietário do quadro o adiciona ao quadro.

   Somente um usuário pode ser o proprietário do quadro. Uma equipe não pode ser um proprietário.

1. Clique em [!UICONTROL **Atualizar**].

</div>
