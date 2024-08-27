---
filename: group-cards-on-board
content-type: reference
navigation-topic: boards
title: Usar grupos em um painel
description: Você pode agrupar cartões em um quadro por destinatário ou por tag. Quando você seleciona uma opção para agrupar por, os cartões são exibidos em formato de raia.
author: Lisa
feature: Agile
exl-id: 6f57a20e-0e47-4457-8605-9bce55c013ec
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Usar grupos em um quadro

Você pode agrupar cartões em um quadro por destinatário ou por tag. Quando você seleciona uma opção para agrupar por, os cartões são exibidos em formato de raia. Cartões não atribuídos ou cartões sem tags aparecem em suas próprias raias.

>[!NOTE]
>
>Quaisquer cartões na coluna de entrada não estão incluídos em um grupo, e a coluna de entrada está oculta quando um grupo é aplicado. Para obter informações sobre a coluna entrada, consulte [Adicionar uma coluna entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

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

## Agrupar cartões em um quadro

{{step1-to-boards}}

1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Grupo]** para abrir o painel de grupo à esquerda do quadro.

   >[!NOTE]
   >
   >A configuração padrão para agrupar por é **[!UICONTROL Nenhuma]**. Você pode selecionar essa opção a qualquer momento para remover um grupo e mostrar apenas as colunas no quadro.

1. Para agrupar os cartões, selecione **[!UICONTROL Atribuídos]** ou **[!UICONTROL Marcas]**.

   Os cartões são agrupados automaticamente. Clique na seta ao lado do nome do grupo para recolher e expandir o grupo.

   ![Cartões agrupados em um quadro](assets/group-by-assignee.png)

1. Selecione o que acontece quando um cartão é movido para outro grupo.

   * **[!UICONTROL Adicionar nos atribuídos] / [!UICONTROL Adicionar em marcas]:** Os atribuídos ou as marcas no novo grupo são adicionados à lista existente de atribuídos ou marcas no cartão.
   * **[!UICONTROL Substituir responsáveis] / [!UICONTROL Substituir marcas]:** Os responsáveis ou as marcas no novo grupo substituem todos os outros responsáveis ou marcas e tornam-se os únicos atribuídos ou marcas no cartão.

   ![[!UICONTROL Agrupar por opções]](assets/group-by-rail.png)

1. Clique em **[!UICONTROL Ocultar grupos]** para ocultar o painel de grupo e exibir o quadro completo.
