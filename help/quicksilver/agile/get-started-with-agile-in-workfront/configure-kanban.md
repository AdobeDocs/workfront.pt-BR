---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurar Kanban
description: Você pode configurar as seguintes opções para as equipes ágeis Kanban durante ou após a criação da equipe.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 7fc6230643d0a24c3b483df8165294ceca6dcce7
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# Configurar [!UICONTROL Kanban]

Você pode configurar as seguintes opções para grupos Agile durante ou após a criação do grupo. Crie uma equipe ágil (Kanban ou Scrum) no [!DNL Adobe Workfront] conforme descrito em [Criar uma equipe ágil](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td> <p>[!UICONTROL Work] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber que tipo de plano ou licença você tem, entre em contato com o [!DNL Workfront] administrador.

## Configure se as histórias são estimadas em pontos ou horas

Você pode configurar histórias para serem estimadas usando pontos ou horas.

Para configurar como as histórias são estimadas para sua equipe ágil:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront]e, em seguida, clique em **[!UICONTROL Equipes]**.

1. Clique em **[!UICONTROL Trocar equipe]** , selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Selecione a Equipe Ágil que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com um [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.\
   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** seção, no campo **[!UICONTROL Estimar Histórias em]** selecione se deseja usar pontos ou horas para estimar o tamanho (carga de trabalho) das matérias. Se você selecionar Pontos, especifique quantas horas são iguais a 1 ponto. (O padrão é 1 ponto = 8 horas.) Este é o número de Horas planejadas que são adicionadas à história.

   **Exemplo:** Se você selecionou estimar histórias em pontos e 1 ponto é igual a 8 horas, e uma história é estimada em 3 pontos, 24 horas planejadas são adicionadas à história.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar colunas de status no storyboard Agile

Você pode definir os status existentes no storyboard da Equipe Ágil. Esses são os únicos status exibidos no storyboard.

Para definir os status disponíveis para o storyboard associado à Equipe Ágil:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!UICONTROL Workfront]e, em seguida, clique em **[!UICONTROL Equipes]**.

1. Clique em **[!UICONTROL Trocar equipe]** ícone ![Ícone Trocar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a Equipe Ágil que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com um [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** localize a **[!UICONTROL Story Board]** área.

1. (Opcional) Clique em **[!UICONTROL Adicionar coluna]** para adicionar outra coluna de status ao storyboard.
1. (Opcional) Arraste qualquer coluna de status usando o indicador de arrastar e soltar para reordenar as colunas de status no storyboard. A primeira coluna não pode ser movida e você não pode arrastar outra coluna na frente da primeira coluna.

   ![Arrastar e soltar](assets/agile-story-card-drag-and-drop.png)

1. Selecione os status da tarefa.

   >[!IMPORTANT]
   >
   >Somente os status bloqueados em todo o sistema estão disponíveis para seleção; não é possível selecionar status específicos do grupo. Além disso, o status da primeira coluna sempre corresponde a **[!UICONTROL Novo]**.

   Você pode adicionar status personalizados se seu [!DNL Workfront] administrador configurou; os status personalizados podem ser configurados conforme descrito em [Criar ou editar um status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar campos adicionais para exibir em cartões de história no storyboard Agile

Ao adicionar campos a cartões de matéria, os campos são somente visualização e somente exibição quando o campo é preenchido.

Por padrão, os seguintes tipos de dados são exibidos no cartão de história para tarefas e problemas:

* Nome da história com um link diretamente para a tarefa ou problema
* O nome do projeto com um link direto para o projeto
* Esse link é exibido apenas para histórias, não para subtarefas
* A descrição da tarefa ou do problema
* Compromisso atual
* Exiba e edite o percentual concluído ajustando o próprio percentual concluído ou ajustando o número de pontos ou horas concluídos
* Usuários atribuídos

É possível exibir dados adicionais (incluindo dados personalizados) em cartões de história. Talvez você queira exibir campos adicionais em cartões de história por vários motivos. Por exemplo, você pode exibir a ID do cliente se estiver trabalhando em histórias para vários clientes dentro da iteração, ou exibir a Data de início do projeto ou a Data de conclusão do projeto.

>[!NOTE]
>
>Se você usar um campo personalizado em um cartão de matéria, ele não poderá conter um ponto no nome.

Para configurar storycards atribuídos à equipe ágil para exibir campos adicionais:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront]e, em seguida, clique em **[!UICONTROL Equipes]**.

1. Clique em **[!UICONTROL Trocar equipe]** ícone ![Ícone Trocar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a Equipe Ágil que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\
   Somente membros da equipe com um [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** digite um nome de campo para localizá-lo.

   ![Campos adicionais](assets/agile-additional-fields-kanban.png)

1. Selecione o nome do campo que deseja adicionar.
1. Digite o **[!UICONTROL Nome de exibição]** para que o campo seja exibido na história ou no cartão de problema.
1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar o limite do trabalho em andamento (WIP)

Kanban em [!DNL Workfront] permite controlar a quantidade de trabalho que a equipe está trabalhando, limitando o número de tarefas que podem aparecer na variável [!UICONTROL Em andamento] coluna na [!UICONTROL Kanban] placa.

Quando o limite WIP estiver configurado, você poderá exibir o limite WIP ou até mesmo atualizá-lo a partir do [!UICONTROL Kanban] storyboard ágil, conforme descrito em [Gerencie o limite de trabalho em andamento (WIP) na [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Para limitar o WIP para a equipe Kanban:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Equipes]**.

1. Clique em **[!UICONTROL Trocar equipe]** ícone ![Ícone Trocar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a equipe Kanban que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com um [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** seção, no campo **[!UICONTROL Metodologia]** verifique se Kanban está selecionado.

1. No **[!UICONTROL Story Board]** seção, no campo **[!UICONTROL LIMITE WIP]** especifique o número máximo de itens permitidos em cada coluna do campo [!UICONTROL Kanban] storyboard ágil. É possível definir um limite diferente para cada coluna. O limite máximo que pode ser definido para cada coluna é 100.\
   Quando definido, o limite WIP exibe uma mensagem de aviso no [!UICONTROL Kanban] storyboard ágil sempre que o limite for excedido em qualquer coluna no storyboard. Essa mensagem de aviso é exibida somente na primeira vez que o limite de WIP é excedido. Esta mensagem de aviso não é exibida em nenhuma coluna com status igual a [!UICONTROL Concluído].\
   O limite de WIP é simplesmente um aviso visual e não impede que sua equipe tenha mais itens em uma única coluna do que o limite definido.

   ![Limite de WIP](assets/wip-limit-350x193.png)

1. Clique em **Salvar alterações**.

## Configurar matérias a serem adicionadas automaticamente a partir do backlog

Você pode configurar histórias do backlog para serem adicionadas automaticamente à primeira coluna no [!UICONTROL Kanban] quadro imediatamente após um item ser movido dessa coluna.

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Equipes]**.

1. Clique em **[!UICONTROL Trocar equipe]** ícone ![Ícone Trocar equipe](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a equipe Kanban que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Somente membros da equipe com um [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. Selecionar **[!UICONTROL Adicionar automaticamente a próxima história do backlog]** para configurar matérias a serem adicionadas automaticamente do backlog à primeira coluna no [!UICONTROL Kanban] storyboard.

   Isso ocorre sempre que uma matéria é movida para uma coluna no storyboard que representa um status Concluído (um status que equivale a Concluído). Quando adicionada do backlog, a matéria com a maior prioridade é adicionada ao storyboard.selecione essa opção para configurar o próximo item do backlog para ser adicionado automaticamente ao **[!UICONTROL Em andamento]** quando um item é movido para fora da **[!UICONTROL Em andamento]** coluna.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configure por quanto tempo os cartões permanecem no [!UICONTROL Kanban] quadro

Você pode escolher por quanto tempo os cartões concluídos permanecem no [!UICONTROL Kanban] placa. Tarefas que caem do [!UICONTROL Kanban] O quadro ainda pode ser acessado em seu projeto original.

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no link **[!UICONTROL Trocar equipe]** ícone ![Ícone Trocar equipe](assets/switch-team-icon.png), selecione uma nova equipe Kanban no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Selecione a equipe Kanban.
1. Clique em **[!UICONTROL Mais]** e selecione **Edit**.

   Somente membros da equipe com um [!UICONTROL Plano] ou [!UICONTROL Trabalho] consulte esta opção.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Número de dias que os cartões Concluídos permanecem no quadro Kanban]** selecione um valor.
1. Clique em **[!UICONTROL Salvar alterações]**.
