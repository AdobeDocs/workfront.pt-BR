---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Gerenciar fluxos de trabalho
description: Um fluxo de trabalho é um grupo configurável de quadros e cartões para colaborar no trabalho.
author: Lisa
feature: Agile
source-git-commit: 16e96d55932116cb475eecbe8b6ebfd4661eb494
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# Gerenciar fluxos de trabalho

{{highlighted-preview}}

>[!NOTE]
>
>Os fluxos de trabalho estão disponíveis no ambiente de Visualização e em Produção por meio da opção inicial de aceitação de recursos para [!UICONTROL [!DNL Workfront] Quadros]. Para obter detalhes, consulte [Opt-in de recurso antecipado para placas Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

Um fluxo de trabalho é um grupo configurável de quadros e cartões para colaborar no trabalho. Fluxos de trabalho podem incluir diferentes tipos de quadros criados a partir de modelos, <span class="preview">e uma lista de cartões de itens de trabalho. Em uma sequência de trabalho, você pode rastrear o trabalho em iterações ou impressões.</span>

<span class="preview">Para obter mais informações, consulte [Usar a lista de cartões](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) e [Criar uma iteração](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).</span>

Os fluxos de trabalho são exibidos no painel junto com quadros individuais aos quais você tem acesso que não fazem parte de uma fluxo de trabalho. Para obter informações sobre o painel de quadros, consulte [Usar o painel de quadros](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Você pode clicar em qualquer nome de quadro no painel para abri-lo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar uma sequência de trabalho

{{step1-to-boards}}

1. Clique em **[!UICONTROL Adicionar fluxo de trabalho]** no [!UICONTROL Fluxos de trabalho] área do painel.
1. Digite um nome para substituir **[!UICONTROL Fluxo de trabalho sem título]** e pressione Enter.

   Você pode adicionar quadros à fluxo de trabalho ou clicar em [!UICONTROL **Todas as placas**] para retornar ao painel.

## Criar um novo quadro em uma sequência de trabalho

1. Se você ainda não estiver em uma sequência de trabalho, clique em [!UICONTROL **Exibir fluxo de trabalho**] no painel para abrir um fluxo de trabalho existente.
1. Clique em **[!UICONTROL Adicionar quadro]** no [!UICONTROL Quadros] da sequência de trabalho.
1. Selecione um modelo para o quadro.

| Modelo | Descrição |
|---------|----------|
| Quadro básico | Três colunas padrão são fornecidas no quadro. Você pode adicionar novas colunas e renomear ou excluir as colunas padrão. <p>Nenhuma política de coluna é aplicada. |
| Quadro Kanban | As seguintes colunas são fornecidas no quadro: Backlog, Novo, Em Andamento, Concluído e Em Retenção. Você pode adicionar novas colunas e renomear ou excluir as colunas padrão.<p>Para usar o backlog, você deve configurar filtros para a coluna de entrada. Para obter mais informações, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Para revisar as políticas padrão de cada coluna, clique no botão [!UICONTROL **Mais** menu] em uma coluna e selecione [!UICONTROL **Editar**]. Você pode alterar qualquer uma dessas políticas predefinidas. Para obter mais informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Quadro retrospectivo | As seguintes colunas são fornecidas no quadro: O que deu certo? O que pode ser melhorado? O que devemos comemorar? O que podemos fazer para agilizar? Você pode adicionar novas colunas e renomear ou excluir as colunas padrão. <p>Nenhuma política de coluna é aplicada. |
| <span class="preview">Processo de iteração</span> | <span class="preview">Este é o quadro usado para definir e executar uma iteração. <p>As seguintes colunas são fornecidas no quadro: Backlog, Novo, Em Andamento, Concluído e Em Retenção. Não é possível adicionar nenhuma coluna ao quadro. <p>Para revisar as políticas padrão de cada coluna, clique no botão [!UICONTROL **Mais**] em uma coluna e selecione [!UICONTROL **Editar**]. Você pode alterar qualquer uma dessas políticas predefinidas. Para obter mais informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

Para obter mais informações sobre como configurar o quadro, consulte [Criar ou editar um quadro](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrar a lista de quadros em uma sequência de trabalho

Quando filtros diferentes dos padrões são aplicados na lista de quadros, um indicador é exibido no ícone de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png). Clique em [!UICONTROL **Limpar tudo**] para remover todos os filtros e clique em [!UICONTROL **Ocultar filtros**] para fechar o painel de filtro.

{{step1-to-boards}}

1. No painel, clique em [!UICONTROL **Exibir fluxo de trabalho**] para abrir um fluxo de trabalho.
1. Clique no botão [!UICONTROL **Quadros**] se já não for exibida.
1. Clique em [!UICONTROL **Filtro**].
1. Selecione os quadros que deseja visualizar por status (quadros arquivados, quadros ativos ou todos os quadros).
1. Selecione os quadros que deseja visualizar por modelo.

## Adicionar membros a uma sequência de trabalho

Pessoas e equipes devem ser adicionadas à sequência de trabalho como membros antes de poderem exibir a sequência de trabalho e seu conteúdo. Um membro de fluxo de trabalho pode adicionar e remover membros na sequência de trabalho e ver quais quadros estão na sequência de trabalho.

>[!NOTE]
>
>Um membro da sequência de trabalho não pode abrir um quadro em uma sequência de trabalho até que seja adicionado a esse quadro específico como membro.

{{step1-to-boards}}

1. No painel, clique em [!UICONTROL **Exibir fluxo de trabalho**] para abrir um fluxo de trabalho.
1. Clique no botão **[!UICONTROL Adicionar membro]** ícone ![Adicionar membros](assets/boards-addmember-spectrum-25x25.png) para adicionar membros e equipes ao fluxo de trabalho.

   Esse é o mesmo processo que adicionar membros a um quadro. Para obter mais informações, consulte [Adicionar ou remover membros de um quadro](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

<div class="preview">

## Configurar uma sequência de trabalho

{{step1-to-boards}}

1. No painel, clique em [!UICONTROL **Exibir fluxo de trabalho**] para abrir um fluxo de trabalho.
1. Clique em [!UICONTROL **Configurar**] para abrir o [!UICONTROL Configurar fluxo de trabalho] painel.
1. (Opcional) Digite uma descrição da sequência de trabalho. Essa descrição é exibida no painel.

   O número total de cartões, o número de cartões apontados e o número de iterações são exibidos na seção Lista de cartões . Clique em [!UICONTROL **Exibir lista**] para abrir a lista e adicionar cartões. Para obter mais informações, consulte [Usar a lista de cartões](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Se uma iteração tiver sido definida, sua data inicial, número de cartões e número de pontos serão exibidos. Clique em [!UICONTROL **Exibir quadro de iteração**] para abrir o quadro. Para obter mais informações, consulte [Criar uma iteração](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).

1. Clique em [!UICONTROL **Adicionar origem**] para definir uma origem para importar cartões na sequência de trabalho. No momento, a única fonte disponível é [!DNL Adobe Workfront].
1. Adicione filtros para importar tarefas e problemas do Workfront como cartões.

   Adicionar filtros para fontes de fluxo de trabalho é o mesmo que adicionar filtros para uma coluna de entrada em um quadro básico ou um quadro Kanban. Para obter mais informações, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

</div>
