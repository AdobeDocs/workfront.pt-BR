---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Gerenciar fluxos de trabalho
description: Um fluxo de trabalho é um grupo configurável de placas e cartões para colaborar no trabalho.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 1%

---

# Gerenciar fluxos de trabalho

>[!IMPORTANT]
>
>Os fluxos de trabalho só estão disponíveis para um grupo específico de clientes.

Um fluxo de trabalho é um grupo configurável de placas e cartões para colaborar no trabalho. Os fluxos de trabalho podem incluir diferentes tipos de quadros criados a partir de modelos e uma lista de cartões de itens de trabalho. Em um fluxo de trabalho, é possível rastrear o trabalho em iterações ou sprints.

Para obter mais informações, consulte [Usar a lista de cartões](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) e [Criar uma iteração em um fluxo de trabalho](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Fluxos de trabalho são exibidos no painel, juntamente com painéis individuais a que você tem acesso que não fazem parte de um fluxo de trabalho. Para obter informações sobre o painel de painéis, consulte [Usar o painel de painéis](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Você pode clicar em qualquer nome de quadro no painel para abri-lo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Criar um workflow

{{step1-to-boards}}

1. Clique em **[!UICONTROL Adicionar fluxo de trabalho]** na área [!UICONTROL Fluxos de trabalho] do painel.
1. Digite um nome para substituir **[!UICONTROL Fluxo de trabalho sem título]** e pressione Enter.

   Você pode adicionar quadros ao fluxo de trabalho ou clicar em [!UICONTROL **Todos os quadros**] para retornar ao painel.

## Criar um novo quadro em um fluxo de trabalho

1. Se você ainda não estiver em um fluxo de trabalho, clique em [!UICONTROL **Exibir fluxo de trabalho**] no painel para abrir um fluxo de trabalho existente.
1. Clique em **[!UICONTROL Adicionar quadro]** na guia [!UICONTROL Quadros] do fluxo de trabalho.
1. Selecione um modelo para o quadro.

| Modelo | Descrição |
|---------|----------|
| Quadro básico | Três colunas padrão são fornecidas no quadro. É possível adicionar novas colunas e renomear ou excluir as colunas padrão. <p>Nenhuma política de coluna aplicada. |
| Quadro Kanban | As seguintes colunas são fornecidas na placa: Backlog, Novo, Em Andamento, Concluído e Em Retenção. É possível adicionar novas colunas e renomear ou excluir as colunas padrão.<p>Para usar o backlog, você deve configurar filtros para a coluna de entrada. Para obter informações, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Para examinar as políticas padrão de cada coluna, clique no menu [!UICONTROL **Mais**] em uma coluna e selecione [!UICONTROL **Editar**]. É possível alterar qualquer uma dessas políticas predefinidas. Para obter informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Quadro retrospectivo | As seguintes colunas são fornecidas no quadro: O que deu certo? O que pode ser melhorado? Quem devemos comemorar? O que podemos fazer para agilizar? É possível adicionar novas colunas e renomear ou excluir as colunas padrão. <p>Nenhuma política de coluna aplicada. |
| Processo de iteração | Este é o quadro usado para definir e executar uma iteração. <p>As seguintes colunas são fornecidas na placa: Backlog, Novo, Em Andamento, Concluído e Em Retenção. Não é possível adicionar colunas ao quadro. <p>Para examinar as políticas padrão de cada coluna, clique no menu [!UICONTROL **Mais**] em uma coluna e selecione [!UICONTROL **Editar**]. É possível alterar qualquer uma dessas políticas predefinidas. Para obter informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Para obter mais informações sobre como configurar o quadro, consulte [Criar ou editar um quadro](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtrar a lista de quadros em um fluxo de trabalho

Quando filtros diferentes dos padrões são aplicados na lista de quadros, um indicador é exibido no ícone de filtro ![Filtro aplicado](assets/boards-filterapplied-30x30.png). Clique em [!UICONTROL **Limpar tudo**] para remover todos os filtros e em [!UICONTROL **Ocultar filtros**] para fechar o painel de filtros.

{{step1-to-boards}}

1. No painel, clique em [!UICONTROL **Exibir fluxo de trabalho**] para abrir um fluxo de trabalho.
1. Clique na guia [!UICONTROL **Quadros**] se ela ainda não estiver sendo exibida.
1. Clique em [!UICONTROL **Filtro**].
1. Selecione os quadros que deseja ver por status (quadros arquivados, quadros ativos ou todos os quadros).
1. Selecione os painéis de discussão que deseja ver por modelo.

## Adicionar membros a um fluxo de trabalho

Pessoas e equipes devem ser adicionadas ao fluxo de trabalho como membros antes de visualizarem o fluxo de trabalho e seu conteúdo. Um membro do fluxo de trabalho pode adicionar e remover membros do fluxo de trabalho e ver quais placas estão no fluxo de trabalho.

>[!NOTE]
>
>Um membro do fluxo de trabalho não pode abrir um quadro em um fluxo de trabalho até que ele seja adicionado a esse quadro específico como um membro.

{{step1-to-boards}}

1. No painel, clique em [!UICONTROL **Exibir fluxo de trabalho**] para abrir um fluxo de trabalho.
1. Clique no ícone **[!UICONTROL Adicionar membro]** ![Adicionar membros](assets/boards-addmember-spectrum-25x25.png) para adicionar membros e equipes ao fluxo de trabalho.

   Esse é o mesmo processo que adicionar membros a um quadro. Para obter mais informações, consulte [Adicionar ou remover membros de um quadro](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Adicionar fontes a um fluxo de trabalho

Uma origem determina de onde vêm os cartões na sequência de trabalho.

{{step1-to-boards}}

1. Clique no ícone [!UICONTROL **Fontes**] ![Ícone Fontes](assets/sources-icon.png) para definir uma fonte para importar cartões para o fluxo de trabalho. No momento, a única origem disponível é [!DNL Adobe Workfront].
1. Adicione filtros para importar tarefas e problemas do Workfront como cartões.

   Adicionar filtros para fontes de fluxo de trabalho é o mesmo que adicionar filtros avançados para uma coluna de entrada em um quadro básico ou quadro Kanban. Para obter mais informações, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Configurar um fluxo de trabalho

{{step1-to-boards}}

1. No painel, clique em [!UICONTROL **Exibir fluxo de trabalho**] para abrir um fluxo de trabalho.
1. Clique em [!UICONTROL **Configurar**] para abrir o painel [!UICONTROL Configurar Fluxo de Trabalho].
1. (Opcional) Expanda [!UICONTROL **Workstream**] e digite uma descrição do fluxo de trabalho. Essa descrição é exibida no painel.
1. (Opcional) Expanda [!UICONTROL **Iterações**] para definir um processo de iteração para este fluxo de trabalho.

   O número total de cartões, o número de cartões apontados e o número de iterações são exibidos na seção Lista de cartões. Clique em [!UICONTROL **Exibir lista**] para abrir a lista e adicionar cartões. Para obter mais informações, consulte [Usar a lista de cartões](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Se uma iteração já tiver sido definida, sua data de início, número de cartões e número de pontos serão exibidos. Clique em [!UICONTROL **Exibir quadro**] para abrir o quadro de iteração. Para obter mais informações, consulte [Criar uma iteração em um fluxo de trabalho](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Opcional) Expanda [!UICONTROL **Marcas**] para adicionar marcas ao fluxo de trabalho. Procure uma tag ou digite um novo nome de tag na caixa de pesquisa e pressione Enter para criá-la.
