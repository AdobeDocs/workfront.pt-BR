---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Configurar Kanban
description: Crie uma equipe ágil de Kanban ou Scrum no [!DNL Adobe Workfront].
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---

# Configurar [!UICONTROL Kanban]

É possível criar uma equipe ágil no [!DNL Adobe Workfront] conforme descrito em [Criar uma equipe ágil](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Ao criar uma equipe ágil, é possível escolher a metodologia que a equipe usa para concluir o trabalho. Você pode escolher entre as seguintes opções:

* Scrum
* Kanban

Este artigo descreve como definir as configurações de uma equipe Kanban. Depois de criar uma Equipe Ágil e escolher a metodologia Kanban, consulte este artigo para atualizar as seguintes configurações:

* Se as histórias são estimadas em pontos ou horas
* As colunas de status no storyboard Agile
* Campos adicionais a serem exibidos em cartões de história no storyboard Agile
* O limite do trabalho em andamento (WIP)
* Como adicionar histórias automaticamente do backlog
* Quanto tempo os cartões permanecem no quadro Kanban

Para obter informações sobre como configurar uma equipe do Scrum, consulte [Configurar Scrum](../get-started-with-agile-in-workfront/configure-scrum.md).

## Requisitos de acesso

<!--Audited: 12/2023-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p> 
   ou
   <p>Atual: [!UICONTROL Trabalho] ou superior</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Nível de acesso</td> 
   <td> <p>Editar acesso a equipes</p>  </td> 
  </tr>

</tbody> 
</table>

*Para descobrir que tipo de plano ou licença você tem, entre em contato com o [!DNL Workfront] administrador.

## Configure se as histórias são estimadas em pontos ou horas

Você pode configurar histórias para serem estimadas usando pontos ou horas.

Para configurar como as histórias são estimadas para sua equipe ágil:

{{step1-to-team}}

1. Clique em **[!UICONTROL Trocar equipes]** ícone ![](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou pesquise por uma equipe na caixa de pesquisa.
1. Selecione a Equipe Ágil que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** menu ![](assets/more-menu.png) e selecione **[!UICONTROL Editar]**.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** seção, no campo **[!UICONTROL Estimar Histórias em]** selecione se deseja usar pontos ou horas para estimar o tamanho (carga de trabalho) das matérias. Se você selecionar Pontos, especifique quantas horas são iguais a 1 ponto. (O padrão é 1 ponto = 8 horas.) Este é o número de Horas planejadas que são adicionadas à história.

   **Exemplo:** Se você selecionou estimar histórias em pontos e 1 ponto é igual a 8 horas, e uma história é estimada em 3 pontos, 24 horas planejadas são adicionadas à história.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar colunas de status no storyboard Agile

Você pode definir os status existentes no storyboard da Equipe Ágil. Esses são os únicos status exibidos no storyboard.

Para definir os status disponíveis para o storyboard associado à Equipe Ágil:

{{step1-to-team}}

1. Clique em **[!UICONTROL Trocar equipes]** ícone ![Ícone Trocar equipes](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a Equipe Ágil que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** localize a **[!UICONTROL Story Board]** área.

1. (Opcional) Clique em **[!UICONTROL Adicionar coluna]** para adicionar outra coluna de status ao storyboard.
1. (Opcional) Arraste qualquer coluna de status usando o indicador de arrastar e soltar para reordenar as colunas de status no storyboard. A primeira coluna não pode ser movida e você não pode arrastar outra coluna na frente da primeira coluna.

   ![Arrastar e soltar](assets/agile-story-card-drag-and-drop.png)

1. Selecione os status da tarefa.

   >[!IMPORTANT]
   >
   >Somente os status bloqueados em todo o sistema estão disponíveis para seleção. Não é possível selecionar status específicos de grupo. O status da primeira coluna sempre corresponde a **[!UICONTROL Novo]**.

   Você pode adicionar status personalizados se seu [!DNL Workfront] o administrador as configurou. Para obter mais informações, consulte [Criar ou editar um status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar campos adicionais para exibir em cartões de história no storyboard Agile

Ao adicionar campos a cartões de matéria, os campos são somente visualização e são exibidos somente quando o campo é preenchido.

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

{{step1-to-team}}

1. Clique em **[!UICONTROL Trocar equipes]** ícone ![Ícone Trocar equipes](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a Equipe Ágil que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.\

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** digite um nome de campo para localizá-lo.

   ![Campos adicionais](assets/agile-additional-fields-kanban.png)

1. Selecione o nome do campo que deseja adicionar.
1. Digite o **[!UICONTROL Nome de exibição]** para que o campo seja exibido na história ou no cartão de problema.
1. Clique em **[!UICONTROL Salvar alterações]**.

## Configurar o limite do trabalho em andamento (WIP)

Ao definir o limite WIP de uma equipe Kanban, você pode controlar o número de itens nos quais a equipe está trabalhando no momento, limitando o número de tarefas que podem aparecer no [!UICONTROL Novo] ou o [!UICONTROL Em andamento] coluna na [!UICONTROL Kanban] placa.

Depois de configurar o limite WIP para uma equipe Kanban, você pode exibir o limite WIP e atualizá-lo a partir do [!UICONTROL Kanban] storyboard ágil, conforme descrito em [Gerencie o limite de trabalho em andamento (WIP) na [!UICONTROL Kanban] quadro](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

Para limitar o WIP para a equipe Kanban:

{{step1-to-team}}

1. Clique em **[!UICONTROL Trocar equipes]** ícone ![Ícone Trocar equipes](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a equipe Kanban que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** menu ![](assets/more-menu.png)e selecione **[!UICONTROL Editar]**.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Agile]** seção, no campo **[!UICONTROL Metodologia]** verifique se Kanban está selecionado.

1. No **[!UICONTROL Story Board]** seção, no campo **[!UICONTROL Limite de WIP]** especifique o número máximo de itens permitidos em cada coluna do campo [!UICONTROL Kanban] storyboard ágil. É possível definir um limite diferente para cada coluna. O limite máximo que pode ser definido para cada coluna é 100.\
   Quando definido, o limite WIP exibe uma mensagem de aviso no [!UICONTROL Kanban] storyboard ágil sempre que o limite for excedido em qualquer coluna no storyboard. Essa mensagem de aviso é exibida somente na primeira vez que o limite de WIP é excedido. Esta mensagem de aviso não é exibida em nenhuma coluna com status igual a [!UICONTROL Concluído].\
   O limite de WIP é simplesmente um aviso visual e não impede que sua equipe tenha mais itens em uma única coluna do que o limite definido.

   ![Limite de WIP](assets/wip-limit-350x193.png)

1. Clique em **Salvar alterações**.

## Configurar a adição automática de histórias do backlog

<!-- this functionality needs to be verified-->

Você pode configurar histórias do backlog para serem adicionadas automaticamente à primeira coluna no [!UICONTROL Kanban] quadro imediatamente após um item ser movido dessa coluna.

{{step1-to-team}}

1. Clique em **[!UICONTROL Trocar equipes]** ícone ![Ícone Trocar equipes](assets/switch-team-icon.png), selecione uma nova equipe no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a equipe Kanban que deseja gerenciar.
1. Clique em **[!UICONTROL Mais]** menu ![](assets/more-menu.png)e selecione **[!UICONTROL Editar]**.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. Selecionar **[!UICONTROL Adicionar automaticamente a próxima história do backlog]** para configurar que o próximo item do backlog seja adicionado automaticamente ao **[!UICONTROL Novo]** quando um item é movido para fora da **[!UICONTROL Em andamento]** coluna.

   Os usuários devem ativar o **Mostrar backlog** configuração no [!UICONTROL Kanban] para que essa funcionalidade entre em vigor. Quando os usuários ativarem a opção [!UICONTROL Mostrar backlog] configuração no [!UICONTROL Quadro Kanban], a seguinte funcionalidade ocorrerá:

   Sempre que uma história for movida de uma [!UICONTROL Em andamento] em uma coluna no storyboard que representa uma [!UICONTROL Concluído] status (ou um status que equivale a [!UICONTROL Concluído]), uma história da coluna Backlog será movida automaticamente para a [!UICONTROL Novo] coluna da [!UICONTROL Quadro Kanban].
Quando adicionada a partir do backlog, a matéria com a maior prioridade é adicionada ao storyboard.

1. Clique em **[!UICONTROL Salvar alterações]**.

## Configure por quanto tempo os cartões permanecem no [!UICONTROL Kanban] quadro

Você pode escolher por quanto tempo os cartões concluídos permanecem no [!UICONTROL Kanban] placa. Tarefas que caem do [!UICONTROL Kanban] O quadro ainda pode ser acessado em seu projeto original.

{{step1-to-team}}

1. (Opcional) Clique no link **[!UICONTROL Trocar equipes]** ícone ![Ícone Trocar equipes](assets/switch-team-icon.png), selecione uma nova equipe Kanban no menu suspenso ou procure uma equipe na barra de pesquisa.
1. Selecione a equipe Kanban.
1. Clique em **[!UICONTROL Mais]** menu ![](assets/more-menu.png) e selecione **[!UICONTROL Editar]**.

   ![Editar equipe](assets/edit-team-settings-350x205.png)

1. No **[!UICONTROL Número de dias que os cartões Concluídos permanecem no quadro Kanban]** selecione um valor.

   Você pode escolher um número de 1 a 30 dias.
1. Clique em **[!UICONTROL Salvar alterações]**.
