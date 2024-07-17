---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Criar ou editar um quadro
description: No painel [!UICONTROL painéis], é possível criar um novo painel ou editar um existente.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 1%

---

# Criar ou editar um quadro

<!-- Audited: 12/2023 -->

No painel [!UICONTROL painéis], é possível criar um novo painel ou editar um existente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: Colaborador ou superior </p>
 <p>ou</p> 
<p>Atual: [!UICONTROL Request] ou superior </p> 
</td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um novo quadro

{{step1-to-boards}}

1. Clique em **[!UICONTROL Adicionar painel]**.

1. Selecione um modelo para o quadro.

   | Modelo | Descrição |
   |---------|----------|
   | Quadro básico | Três colunas padrão são fornecidas no quadro. É possível adicionar novas colunas e renomear ou excluir as colunas padrão. <p>Três colunas padrão são fornecidas no quadro. É possível adicionar novas colunas e renomear ou excluir as colunas padrão. |
   | Quadro Kanban | As seguintes colunas são fornecidas na placa: Backlog, Novo, Em Andamento, Concluído e Em Retenção. É possível adicionar novas colunas e renomear ou excluir as colunas padrão.<p>Para usar o backlog, você deve configurar filtros para a coluna de entrada. Para obter informações, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Para examinar as políticas padrão de cada coluna, clique no menu [!UICONTROL **Mais**] em uma coluna e selecione [!UICONTROL **Editar**]. É possível alterar qualquer uma dessas políticas predefinidas. Para obter informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Quadro retrospectivo | As seguintes colunas são fornecidas no quadro: O que deu certo? O que pode ser melhorado? Quem devemos comemorar? O que podemos fazer para agilizar? É possível adicionar novas colunas e renomear ou excluir as colunas padrão. <p>Nenhuma política de coluna aplicada. |
   | Quadro dinâmico | As seguintes colunas são fornecidas no quadro: Não selecionado, Novo, Em andamento, Em espera e Concluído. É possível adicionar novas colunas e renomear ou excluir as colunas padrão. (A coluna Não selecionada pode ser renomeada, mas não excluída. Essa coluna contém todos os cartões com um status que não corresponde a nenhum dos outros status de coluna.) <p>As políticas de coluna padrão atribuem cartões às colunas com base em seus status. Para obter informações, consulte [Gerenciar colunas do quadro](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Para um quadro dinâmico somente, siga as etapas do assistente de configuração:

   1. Digite um nome para o quadro e clique em [!UICONTROL **Avançar**].
   1. Procure e selecione [!DNL Workfront] [!UICONTROL **Projetos**] para trazer tarefas e problemas para o painel.
   1. Procure por e selecione [!UICONTROL **Atribuições**] para trazer tarefas e problemas para o quadro.

      Todos os objetos aparecem no quadro como cartões conectados.

      O contador [!UICONTROL **Cartões adicionados**] mostra quantos cartões estarão no quadro. Por exemplo, se você selecionar um projeto com 100 tarefas e problemas, o contador mostrará 100. Se você adicionar uma atribuição de usuário e essa pessoa for atribuída a cinco tarefas no projeto, o contador mostrará cinco.

      >[!NOTE]
      >
      >O limite de placas para placas dinâmicas é de 700 tarefas e 700 problemas, para um total de 1.400 placas. O alto número de placas na placa pode afetar o desempenho da placa.

   1. (Opcional) Selecione [!UICONTROL **Não arquivar cartões concluídos**] para trazer tarefas concluídas e problemas para o quadro como cartões visíveis na coluna Concluído. Quando essa opção não está selecionada, os cartões concluídos no momento da criação do quadro são trazidos para o quadro como cartões arquivados.

      >[!NOTE]
      >
      >Por padrão, os cartões arquivados não são exibidos no quadro. Para exibir cartões arquivados, você deve ativar uma definição de configuração e filtrar a placa para mostrar cartões arquivados. Para obter detalhes, consulte [Personalizar quais campos são exibidos em um cartão](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) e [Filtrar e pesquisar em um quadro](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Opcional) Clique em [!UICONTROL **Usar filtros avançados**] para exibir opções de filtro adicionais.

      Esse é o mesmo processo que criar um filtro em uma coluna de entrada. Para obter mais informações, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Se você atualizar os filtros em um quadro dinâmico após sua criação, as configurações do cartão que não fazem parte da tarefa ou problema do Workfront (como tags) serão redefinidas.

   1. Depois de adicionar os filtros, clique em [!UICONTROL **Criar quadro**].

1. Digite um nome para o quadro no campo **[!UICONTROL Quadro]** e pressione Enter.
1. Configure a placa conforme necessário.

   Para obter informações, consulte [Adicionar ou remover membros de um quadro](../../agile/get-started-with-boards/add-members-to-board.md), [Gerenciar colunas do quadro](../../agile/get-started-with-boards/manage-board-columns.md), [Adicionar um cartão ad hoc a um quadro](../../agile/get-started-with-boards/add-card-to-board.md) e [Usar cartões conectados em quadros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Clique em **[!UICONTROL Todos os painéis]** para retornar ao painel de painéis.

   Você também pode localizar o menu suspenso rotulado com o nome do quadro atual e clicar nele para alternar para outro quadro.

   ![Lista de painéis](assets/boards-button-list-of-boards-350x188.png)

## Editar um quadro existente

{{step1-to-boards}}

1. No painel, selecione o quadro a ser aberto.
1. Edite o quadro conforme necessário. Você pode clicar no nome do quadro para renomeá-lo.

   Para obter informações, consulte [Adicionar ou remover membros de um quadro](../../agile/get-started-with-boards/add-members-to-board.md), [Gerenciar colunas do quadro](../../agile/get-started-with-boards/manage-board-columns.md) e [Adicionar um cartão a um quadro](../../agile/get-started-with-boards/add-card-to-board.md).

1. Clique em **[!UICONTROL Todos os painéis]** para retornar ao painel de painéis.

   Você também pode localizar o menu suspenso rotulado com o nome do quadro atual e clicar nele para alternar para outro quadro.

