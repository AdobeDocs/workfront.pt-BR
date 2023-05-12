---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Criar ou editar um quadro
description: No [!UICONTROL quadros] no painel, você pode criar um novo quadro ou editar um quadro existente.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 5e73603b695ff7456216ca7a4e15ce527b01559d
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 3%

---

# Criar ou editar um quadro

No [!UICONTROL quadros] no painel, você pode criar um novo quadro ou editar um quadro existente.

Para adicionar um quadro a um fluxo de trabalho, consulte [Gerenciar fluxos de trabalho](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Criar um novo quadro

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Quadros]**.
1. Para criar um quadro independente, clique em **[!UICONTROL Adicionar quadro]** no [!UICONTROL Quadros] área. Para adicionar um quadro a um fluxo de trabalho, consulte [Gerenciar fluxos de trabalho](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

1. Selecione um modelo para o quadro.

   | Modelo | Descrição |
   |---------|----------|
   | Quadro básico | Três colunas padrão são fornecidas no quadro. Você pode adicionar novas colunas e renomear ou excluir as colunas padrão. <p>Três colunas padrão são fornecidas no quadro. Você pode adicionar novas colunas e renomear ou excluir as colunas padrão. |
   | Quadro Kanban | As seguintes colunas são fornecidas no quadro: Backlog, Novo, Em Andamento, Concluído e Em Retenção. Você pode adicionar novas colunas e renomear ou excluir as colunas padrão.<p>Para usar o backlog, você deve configurar filtros para a coluna de entrada. Para obter mais informações, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Para revisar as políticas padrão de cada coluna, clique no botão [!UICONTROL **Mais** menu] em uma coluna e selecione [!UICONTROL **Editar**]. Você pode alterar qualquer uma dessas políticas predefinidas. Para obter mais informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Quadro retrospectivo | As seguintes colunas são fornecidas no quadro: O que deu certo? O que pode ser melhorado? O que devemos comemorar? O que podemos fazer para agilizar? Você pode adicionar novas colunas e renomear ou excluir as colunas padrão. <p>Nenhuma política de coluna é aplicada. |
   | Quadro dinâmico | As seguintes colunas são fornecidas no quadro: Não selecionado, Novo, Em Andamento, Em Retenção e Concluído. Você pode adicionar novas colunas e renomear ou excluir as colunas padrão. (A coluna Não selecionada pode ser renomeada, mas não excluída. Esta coluna contém todos os cartões com um status que não corresponde a nenhum dos outros status de coluna.) <p>As políticas de coluna padrão atribuem cartões a colunas com base em seu status. Para obter mais informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). <p>**OBSERVAÇÃO:** A placa dinâmica está disponível somente por meio da opção inicial de aceitação de recursos para placas Workfront. |

1. Para um quadro dinâmico apenas, siga as etapas do assistente de configuração:

   1. Procure e selecione [!DNL Workfront] [!UICONTROL **Projetos**] para trazer tarefas e problemas para o quadro.
   1. Procure e selecione [!UICONTROL **Atribuições**] para trazer tarefas e problemas para o quadro.

      Todos os objetos aparecem no quadro como placas conectadas.

      O [!UICONTROL **Cartões adicionados**] mostra quantos cartões estarão no quadro. Por exemplo, se você selecionar um projeto com 100 tarefas e problemas, o contador exibirá 100. Se você adicionar uma atribuição de usuário e essa pessoa for atribuída a 5 tarefas no projeto, o contador mostrará 5.

   1. (Opcional) Selecione [!UICONTROL **Incluir trabalho concluído**] para incluir cartões preenchidos no quadro.

      >[!NOTE]
      >
      >Se essa opção não estiver selecionada, quando cartões em outros status forem marcados como concluídos, eles &quot;desistirão&quot; do quadro e não serão mais exibidos.

   1. (Opcional) Clique em [!UICONTROL **Usar filtros avançados**] para exibir opções de filtro adicionais.

      Esse é o mesmo processo que criar um filtro em uma coluna de entrada. Para obter mais informações, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. Depois de adicionar os filtros, clique em [!UICONTROL **Criar quadro**].

1. Digite um nome para o quadro na **[!UICONTROL Placa]** e pressione Enter.
1. Configure a placa conforme necessário.

   Para obter mais informações, consulte [Adicionar ou remover membros de um quadro](../../agile/get-started-with-boards/add-members-to-board.md), [Gerenciar colunas do quadro](../../agile/get-started-with-boards/manage-board-columns.md), [Adicionar um cartão ad hoc a um quadro](../../agile/get-started-with-boards/add-card-to-board.md)e [Usar placas conectadas em placas](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Clique em **[!UICONTROL Todas as placas]** para retornar ao painel de quadros.

   Também é possível localizar o menu suspenso com o nome da placa atual e clicar nele para alternar para outra placa.

   ![Lista de quadros](assets/boards-button-list-of-boards-350x188.png)

## Editar um quadro existente

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Quadros]**.
1. No painel, selecione o quadro a ser aberto.
1. Edite o quadro conforme necessário. Você pode clicar no nome do quadro para renomeá-lo.

   Para obter mais informações, consulte [Adicionar ou remover membros de um quadro](../../agile/get-started-with-boards/add-members-to-board.md), [Gerenciar colunas do quadro](../../agile/get-started-with-boards/manage-board-columns.md)e [Adicionar um cartão a um quadro](../../agile/get-started-with-boards/add-card-to-board.md).

1. Clique em **[!UICONTROL Todas as placas]** para retornar ao painel de quadros.

   Também é possível localizar o menu suspenso com o nome da placa atual e clicar nele para alternar para outra placa.
