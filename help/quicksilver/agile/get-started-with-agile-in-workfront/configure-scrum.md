---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurar Sombra
description: Você pode configurar as seguintes opções para as equipes do Scrum agile durante ou após a criação da equipe.
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1667'
ht-degree: 0%

---

# Configurar [!UICONTROL Scrum]

Você pode configurar as seguintes opções para equipes ágeis durante ou após a criação da equipe. Você cria uma equipe ágil (Kanban ou Scrum) em [!DNL Adobe Workfront] conforme descrito em [Criar uma equipe ágil](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

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
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com seu [!DNL Workfront] administrador.

## Configure se as histórias são estimadas em pontos ou horas

>[!NOTE]
>
>Essa configuração não pode ser alterada se a equipe tiver iterações em andamento no momento.

Você pode configurar histórias para serem estimadas usando pontos ou horas.

Para configurar como as histórias são estimadas para sua equipe ágil:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!UICONTROL Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** em seguida, selecione uma nova equipe no menu suspenso ou pesquise por uma equipe na barra de pesquisa.
1. Selecione a equipe ágil que deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.\
   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Ágil]** na seção **[!UICONTROL Estime Histórias em]** , selecione se deseja usar pontos ou horas para estimar o tamanho (carga de trabalho) das histórias. Se você selecionar Pontos, especifique quantas horas são iguais a 1 ponto. (O padrão é 1 ponto = 8 horas.) Esse é o número de Horas Planejadas que são adicionadas à história.

   **Exemplo:** Se você tiver selecionado para estimar histórias em pontos e 1 ponto for igual a 8 horas, e uma história for estimada em 3 pontos, 24 Horas Planejadas serão adicionadas à história.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar colunas de status no quadro de história ágil

Você pode configurar quais colunas são exibidas no quadro de história ágil para todas as iterações atribuídas à sua equipe ou para um determinado projeto.

* [Configurar colunas de status para iterações](#configure-status-columns-for-iterations)
* [Configurar colunas de status para projetos](#configure-status-columns-for-projects)

### Configurar colunas de status para iterações {#configure-status-columns-for-iterations}

Você pode definir os status que existem no quadro de histórias para a equipe ágil. Esses são os únicos status exibidos no quadro de histórias.

Para definir os status que estão disponíveis para a placa de história associada à equipe ágil:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecione a equipe ágil que deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Ágil]** localize a **[!UICONTROL Quadro de história]** área.

1. (Opcional) Clique em **[!UICONTROL Adicionar coluna]** para adicionar uma coluna de status adicional ao quadro de matérias.
1. (Opcional) Arraste qualquer coluna de status usando o indicador arrastar e soltar para reorganizar as colunas de status no quadro de matérias. A primeira coluna não pode ser movida e não é possível arrastar outra coluna na frente da primeira coluna.

   ![Arrastar e soltar](assets/agile-story-card-drag-and-drop.png)

1. Selecione os status da tarefa e da emissão. Os status da tarefa são exibidos como o título da coluna para cada coluna no quadro de história. O status do problema é que você seleciona mapear para os status da tarefa. Isso significa que quando você move um problema para outra coluna do quadro de história, o status da edição muda para os status de edição mostrados aqui, e não para o nome da coluna no quadro de história (que reflete o status da tarefa).

   >[!IMPORTANT]
   >
   >Só estão disponíveis para seleção os status bloqueados em todo o sistema; não é possível selecionar status específicos do grupo. Além disso, o status da primeira coluna sempre corresponde a **[!UICONTROL Novo]**.

   Você pode adicionar status personalizados se [!DNL Workfront] O administrador os configurou; os status personalizados podem ser configurados conforme descrito em [Criar ou editar um status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   >[!NOTE]
   >
   >Ao selecionar os status da ocorrência, a terceira coluna sempre assume o padrão de [!UICONTROL Fechado]. Se você tiver mais de três colunas, atualize as colunas manualmente para refletir os status adequados.

1. Clique em **[!UICONTROL Salvar alterações]**.

### Configurar colunas de status para projetos {#configure-status-columns-for-projects}

Para obter informações sobre como configurar colunas de status para um projeto, consulte a seção [Crie ou personalize um [!UICONTROL Ágil] exibir](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view) no artigo [Criar ou editar exibições em [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Configure campos adicionais para exibir em cartões de história no quadro de história ágil

Ao adicionar campos a cartões de história, os campos são somente visualização e somente exibição quando o campo é preenchido.

Por padrão, os seguintes tipos de dados são exibidos no cartão de história para tarefas e problemas:

* Nome da história com um link diretamente para a tarefa ou problema
* O nome do projeto com um link diretamente para o projeto
* Este link é exibido somente para histórias, não para subtarefas
* A descrição da tarefa ou do problema
* Compromisso atual
* Exibir e editar a porcentagem concluída ajustando a porcentagem concluída ou ajustando o número de pontos ou horas concluídas
* Usuários atribuídos

Você pode exibir dados adicionais (incluindo dados personalizados) em cartões de história. Talvez você queira exibir campos adicionais em cartões de história por qualquer motivo. Por exemplo, talvez você queira exibir a ID do cliente se estiver trabalhando em histórias para vários clientes dentro da iteração ou desejar exibir a Data de início do projeto ou a Data de conclusão do projeto.

>[!NOTE]
>
>Se você usar um campo personalizado em um cartão de história, ele não poderá conter ponto/ponto no nome.

Para configurar cartões de história atribuídos à equipe ágil para exibir campos adicionais:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!UICONTROL Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecione a equipe ágil que deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Ágil]** digite um nome de campo para localizá-lo.

   ![Campos adicionais](assets/agile-additional-fields-scrum.png)

1. Selecione o nome do campo que deseja adicionar.
1. Digite o **[!UICONTROL Nome de exibição]** para o campo ser exibido na história ou no cartão de edição.
1. Clique em **[!UICONTROL Salvar alterações]**.

## Configure como os indicadores de cores são usados para histórias no quadro de histórias ágeis

Por padrão, os blocos de quadro de história em uma iteração ágil são codificados por cores de acordo com o projeto ao qual a história está associada. Cada projeto recebe uma cor arbitrariamente no quadro de histórias. Você pode alterar esse comportamento padrão para cada equipe ágil. As cores de histórias ágeis podem ser vinculadas à prioridade da história, ao dono e assim por diante.

Para alterar o comportamento de como as cores são atribuídas às histórias de uma equipe ágil:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecione a equipe ágil que deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No [!UICONTROL Ágil] na seção [!UICONTROL Associar cor do cartão a] selecione uma das seguintes opções:

   * **[!UICONTROL Projeto]**: As cores estão associadas ao projeto ao qual a história está vinculada. (Quando uma história é criada, ela deve ser associada a um projeto, conforme descrito em [Criar uma história ágil](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md). Todas as tarefas do mesmo projeto são exibidas com a mesma cor.
   * **[!UICONTROL Forma livre]**: Todos os cartões são exibidos como azul por padrão até que o usuário altere a cor manualmente, conforme descrito em [[!UICONTROL Categorizar histórias por cor] no quadro de crum](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md).
   * **[!UICONTROL Prioridade]**: As cores estão associadas à prioridade da história, da seguinte maneira:

      * Alto = Vermelho
      * Médio = Amarelo
      * Baixo = Verde\

         Se o administrador do sistema configurou prioridades personalizadas para o [!DNL Workfront] sistema, a prioridade mais alta é vermelha, a segunda mais alta é amarela e a terceira mais alta é verde.
   * **[!UICONTROL Proprietário da Tarefa]**: Todas as histórias com o mesmo destinatário principal têm a mesma cor. O destinatário principal é o usuário que foi atribuído pela primeira vez à tarefa.


1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar como as datas são aplicadas ao adicionar itens de trabalho a uma iteração

Por padrão, quando você adiciona um item de trabalho a uma iteração de Soma, a Data Inicial Planejada e a Data de Conclusão Planejada no item de trabalho são modificadas para corresponder às datas inicial e final da iteração. Você pode optar por manter as datas originais em todos os itens de trabalho da equipe.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Equipes]**.
1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png)e, em seguida, selecione uma nova equipe de Soma no menu suspenso ou procure por uma equipe na barra de pesquisa.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.
1. No [!UICONTROL Ágil] na seção [!UICONTROL Quando um item de trabalho é adicionado a uma iteração] selecione uma das seguintes opções:

   * **[!UICONTROL Modifique a Data Inicial Planejada e a Data de Conclusão Planejada para corresponder às datas inicial e final da iteração]**: Quando os itens de trabalho são adicionados a uma iteração, as datas dos itens de trabalho são alteradas para as datas de iteração.\

      Para obter mais informações sobre como as datas são modificadas, consulte a seção [Entender como a adição de histórias afeta as datas da tarefa](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understa) no artigo [Adicionar histórias a uma iteração existente](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).
   * **[!UICONTROL Não modifique a Data Inicial Planejada e a Data de Conclusão Planejada para corresponder às datas inicial e final da iteração]**: Quando os itens de trabalho são adicionados a uma iteração, os itens de trabalho mantêm suas datas originais.

   Se você alterar a opção de data, as datas dos itens de trabalho que já estão na iteração não serão ajustadas.

   Essas opções podem afetar datas quando equipes atribuem itens de trabalho às iterações umas das outras. Por exemplo, a equipe A modifica datas de item de trabalho para datas de iteração e a equipe B não modifica datas de item de trabalho. Se a equipe B atribuir um item de trabalho à iteração da equipe A, as datas do item de trabalho serão alteradas. No entanto, se a equipe A atribuir um item de trabalho à iteração da equipe B, as datas não serão alteradas.

1. Clique em **[!UICONTROL Salvar alterações]**.
