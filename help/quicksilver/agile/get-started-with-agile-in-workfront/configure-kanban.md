---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurar Kanban
description: Você pode configurar as seguintes opções para as equipes móveis Kanban durante ou após a criação da equipe.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# Configurar [!UICONTROL Kanban]

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

Você pode configurar histórias para serem estimadas usando pontos ou horas.

Para configurar como as histórias são estimadas para sua equipe ágil:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** em seguida, selecione uma nova equipe no menu suspenso ou pesquise por uma equipe na barra de pesquisa.
1. Selecione a equipe ágil que deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.\
   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Ágil]** na seção **[!UICONTROL Estime Histórias em]** , selecione se deseja usar pontos ou horas para estimar o tamanho (carga de trabalho) das histórias. Se você selecionar Pontos, especifique quantas horas são iguais a 1 ponto. (O padrão é 1 ponto = 8 horas.) Esse é o número de Horas Planejadas que são adicionadas à história.

   **Exemplo:** Se você tiver selecionado para estimar histórias em pontos e 1 ponto for igual a 8 horas, e uma história for estimada em 3 pontos, 24 Horas Planejadas serão adicionadas à história.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar colunas de status no quadro de história ágil

Você pode definir os status que existem no quadro de histórias para a equipe ágil. Esses são os únicos status exibidos no quadro de histórias.

Para definir os status que estão disponíveis para a placa de história associada à equipe ágil:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!UICONTROL Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecione a equipe ágil que deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Ágil]** localize a **[!UICONTROL Quadro de história]** área.

1. (Opcional) Clique em **[!UICONTROL Adicionar coluna]** para adicionar uma coluna de status adicional ao quadro de matérias.
1. (Opcional) Arraste qualquer coluna de status usando o indicador arrastar e soltar para reorganizar as colunas de status no quadro de matérias. A primeira coluna não pode ser movida e não é possível arrastar outra coluna na frente da primeira coluna.

   ![Arrastar e soltar](assets/agile-story-card-drag-and-drop.png)

1. Selecione os status da tarefa.

   >[!IMPORTANT]
   >
   >Só estão disponíveis para seleção os status bloqueados em todo o sistema; não é possível selecionar status específicos do grupo. Além disso, o status da primeira coluna sempre corresponde a **[!UICONTROL Novo]**.

   Você pode adicionar status personalizados se [!DNL Workfront] O administrador os configurou; os status personalizados podem ser configurados conforme descrito em [Criar ou editar um status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Clique em **[!UICONTROL Salvar alterações]**.

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

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecione a equipe ágil que deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Ágil]** digite um nome de campo para localizá-lo.

   ![Campos adicionais](assets/agile-additional-fields-kanban.png)

1. Selecione o nome do campo que deseja adicionar.
1. Digite o **[!UICONTROL Nome de exibição]** para o campo ser exibido na história ou no cartão de edição.
1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar o limite de trabalho em andamento (WIP)

Kanban em [!DNL Workfront] permite controlar a quantidade de trabalho que a equipe está trabalhando no momento, limitando o número de tarefas que podem aparecer no [!UICONTROL Em Andamento] na coluna [!UICONTROL Kanban] quadro.

Quando o limite WIP está configurado, você pode exibir o limite WIP ou até mesmo atualizá-lo do [!UICONTROL Kanban] quadro de história ágil, conforme descrito em [Gerenciar o limite de trabalho em andamento (WIP) no [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Para limitar o WIP para sua equipe de Kanban:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecione a equipe Kanban que você deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Ágil]** na seção **[!UICONTROL Metodologia]** verifique se Kanban está selecionado.

1. No **[!UICONTROL Quadro de história]** na seção **[!UICONTROL LIMITE WIP]** , especifique o número máximo de itens permitidos em cada coluna do [!UICONTROL Kanban] quadro de histórias ágeis. É possível definir um limite diferente para cada coluna. O limite máximo que pode ser definido para cada coluna é 100.\
   Quando definido, o limite WIP exibe uma mensagem de aviso no [!UICONTROL Kanban] quadro de história ágil sempre que o limite é excedido para qualquer coluna no quadro de história. Essa mensagem de aviso é exibida somente na primeira vez que o limite WIP é excedido. Essa mensagem de aviso não é exibida em nenhuma coluna com status que seja igual a [!UICONTROL Concluído].\
   O limite WIP é simplesmente um aviso visual e não restringe a equipe de ter mais itens em uma única coluna do que o limite definido.

   ![Limite WIP](assets/wip-limit-350x193.png)

1. Clique em **Salvar alterações**.

## Configure histórias para serem adicionadas automaticamente do backlog

Você pode configurar histórias do backlog para serem automaticamente adicionadas à primeira coluna no [!UICONTROL Kanban] quadro imediatamente depois que um item é movido dessa coluna.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

1. Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecione a equipe Kanban que você deseja gerenciar.
1. Clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. Selecionar **[!UICONTROL Adicionar automaticamente a próxima história do registro retroativo]** para configurar histórias a serem adicionadas automaticamente do backlog à primeira coluna no [!UICONTROL Kanban] quadro de histórias.

   Isso ocorre sempre que uma história é movida para uma coluna no quadro de história que representa um status Concluído (um status que equivale a Concluído). Quando adicionada a partir do backlog, a história com a maior prioridade é adicionada ao quadro de matérias.selecione essa opção para configurar o próximo item do backlog a ser adicionado automaticamente ao **[!UICONTROL Em Andamento]** quando um item é movido para fora da coluna **[!UICONTROL Em Andamento]** coluna.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configure quantos cartões longos permanecem no [!UICONTROL Kanban] quadro

Você pode escolher por quanto tempo os cartões concluídos permanecem [!UICONTROL Kanban] quadro. Tarefas que caem do [!UICONTROL Kanban] o quadro ainda pode ser acessado em seu projeto original.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), em seguida, selecione uma nova equipe de Kanban no menu suspenso ou procure por uma equipe na barra de pesquisa.
1. Selecione a equipe Kanban.
1. Clique no botão **[!UICONTROL Mais]** e selecione **Edit**.

   Somente membros da equipe com uma [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Número de dias de permanência dos cartões concluídos no quadro Kanban]** selecione um valor no menu suspenso.
1. Clique em **[!UICONTROL Salvar alterações]**.
