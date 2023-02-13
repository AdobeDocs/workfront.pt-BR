---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Gerenciar o backlog ágil
description: Tarefas e problemas podem ser atribuídos a uma equipe ágil e adicionados ao backlog dessa equipe como histórias, dependendo da metodologia ágil que a equipe está usando.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: b855f032b24079ff27435fb833cd3ed8a382a77c
workflow-type: tm+mt
source-wordcount: '1376'
ht-degree: 0%

---

# Gerenciar o backlog ágil

Os seguintes itens de trabalho podem ser atribuídos a uma equipe ágil e adicionados ao backlog dessa equipe como histórias, dependendo da metodologia ágil que a equipe está usando:

* **[!UICONTROL Equipes ágeis do crum]:** Tarefas e problemas podem ser atribuídos à equipe ágil e adicionados ao backlog.
* **[!UICONTROL Equipes de Ágil Kanban]:** As tarefas podem ser atribuídas à equipe ágil e adicionadas ao backlog. Os usuários podem exibir o backlog diretamente do painel de história ágil, conforme descrito em [[!UICONTROL Adicionar o backlog] ao quadro Kanban](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). A equipe usa esse backlog para priorizar e gerenciar sua fila de trabalho.

Tarefas ou problemas podem ser atribuídos à equipe (e subsequentemente adicionados ao backlog da equipe) de qualquer lugar em [!DNL Adobe Workfront]. Por exemplo, uma única equipe pode receber atribuições de trabalho de vários projetos.

>[!NOTE]
>
>Se você adicionar várias equipes a um item de backlog, a tarefa ou problema será exibido somente no backlog da equipe primária. A equipe principal é a primeira equipe atribuída.

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
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso do [!UICONTROL Gerenciar] ao projeto no qual a história está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Criar e gerenciar histórias no backlog

* [Reordenar histórias](#reorder-stories)
* [[!UICONTROL Quebra] histórias inativas](#break-down-stories)
* [Editar histórias](#edit-stories)
* [Criar novas histórias no backlog](#create-new-stories-on-the-backlog)
* [Mover histórias do backlog para um quadro de iteração ou Kanban](#move-stories-from-the-backlog-to-an-iteration-or-kanban-board)

### Reordenar histórias {#reorder-stories}

Você pode reorganizar histórias na lista de backlog usando o método arrastar e soltar.

1. Vá para o backlog ágil onde deseja reordenar as histórias.
1. No **[!UICONTROL Exibir]** selecione o menu suspenso **[!UICONTROL Backlog]** ou uma exibição personalizada que contenha a variável **[!UICONTROL Pedido]** coluna.

   >[!NOTE]
   >
   >Se uma tarefa ou problema tiver uma equipe ágil atribuída e o projeto não estiver em um status que seja igual a Atual, elas não serão exibidas no backlog. No entanto, elas ainda afetam a contagem de backlog na coluna Ordem .

1. Selecione uma ou mais histórias e arraste as histórias até a ordem em que deseja que apareçam no backlog.\
   ![Arrastar e soltar itens de backlog](assets/agile-backlog-drag-and-drop.png)

### Analisar histórias {#break-down-stories}

Como as histórias em um backlog variam em tamanho, os usuários podem dividi-las em tamanhos viáveis para uma iteração. Dividir uma história cria subtarefas na tarefa que a história representa e substitui a tarefa original no backlog. Você pode ter uma tarefa pai ou suas subtarefas atribuídas a uma equipe ágil, mas não pode ter ambas atribuídas a uma equipe simultaneamente.

>[!NOTE]
>
>Considere as seguintes limitações ao detalhar histórias:
>
>* Somente histórias que representam tarefas podem ser detalhadas. Não é possível detalhar histórias que representam problemas.
>* As histórias só podem ser detalhadas se estiverem associadas a um projeto.



Para detalhar uma história:

1. Vá para o backlog que contém a história que você deseja detalhar.
1. Selecione a história que deseja analisar e clique em **[!UICONTROL História de detalhamento]**.\
   O [!UICONTROL História de detalhamento] será exibida.\
   ![Caixa de diálogo História de detalhamento](assets/backlog-breakdown-dialog.png)

1. Especifique um nome e uma estimativa para a história e selecione se a história está pronta.
1. Clique em **[!UICONTROL Adicionar história]** criar outra história a partir da história original.
1. Clique em **[!UICONTROL Salvar]**.

### Editar histórias {#edit-stories}

Você pode editar histórias diretamente do [!UICONTROL Histórias] ou [!UICONTROL Problemas] guias no Backlog da mesma forma que você editaria qualquer tarefa ou problema em um projeto em massa, conforme descrito em [Editar tarefas em massa](../../manage-work/tasks/manage-tasks/edit-tasks.md#editing-tasks-in-bulk) em [Editar tarefas](../../manage-work/tasks/manage-tasks/edit-tasks.md) e [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md#bulk-editing-issues) em [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md).

## Criar novas histórias no backlog {#create-new-stories-on-the-backlog}

Você pode criar novas histórias no backlog criando a história diretamente do backlog ou atribuindo uma tarefa ou problema existente a uma equipe ágil.

* [Criar uma história no backlog](#create-a-story-from-the-backlog)
* [Atribuir uma tarefa ou problema a uma equipe ágil](#assign-a-task-or-issue-to-an-agile-team)

### Criar uma história no backlog {#create-a-story-from-the-backlog}

Quando você cria uma história no backlog, a história é criada como uma tarefa ou problema dentro de um projeto. Não é possível criar uma história no backlog como um problema.

Para criar uma história no backlog:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png)e, em seguida, selecione uma nova equipe de Soma no menu suspenso ou procure por uma equipe na barra de pesquisa.

1. Selecionar **[!UICONTROL Backlog]** no painel esquerdo.
1. Siga um destes procedimentos, dependendo de se deseja criar uma tarefa ou um problema:

   * **Para criar uma tarefa:** Clique em **[!UICONTROL Histórias]**.

   * **Para criar um problema:** Clique em **[!UICONTROL Problemas]**.

1. Clique em **[!UICONTROL Nova história]** ou **[!UICONTROL Novo problema]**.

1. Especifique as seguintes informações:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Nome da história]</strong></td>
      <td> Digite um nome para a história.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong></td>
      <td>(Opcional) Digite uma descrição para a história.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Pronto]</strong></td>
      <td> Selecione se a história está pronta para ser adicionada a uma iteração. Essa configuração é apenas informativa. Histórias podem ser adicionadas a uma iteração independentemente do status dessa configuração.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimativa]</strong></td>
      <td>Especifique uma estimativa de ponto ou de hora em hora para a história. As estimativas afetam o gráfico de detalhamento. O gráfico de detalhamento de uma iteração é preciso somente se cada história contiver uma estimativa precisa. (Se você fornecer uma estimativa pontual, já deverá ter designado nas configurações da equipe quantas horas cada ponto representa.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Projeto pai]</strong></td>
      <td>Comece digitando o nome do projeto no qual esta história será criada e clique no nome quando ela for exibida na lista suspensa.<br>O status do projeto deve ser definido como [!UICONTROL Atual]. Se o status do projeto for qualquer coisa menos [!UICONTROL Atual], ele não será exibido no menu suspenso.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tarefa pai]</strong></td>
      <td>(Opcional) Comece a digitar o nome da tarefa pai à qual essa história está secundária e clique no nome quando ela aparecer na lista suspensa.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Forms personalizado]</strong></td>
      <td> (Opcional) Selecione todos os formulários personalizados que deseja adicionar a esta história.</td>
     </tr>
    </tbody>
   </table>

1. Clique em **[!UICONTROL Salvar história]**.

### Atribuir uma tarefa ou problema a uma equipe ágil {#assign-a-task-or-issue-to-an-agile-team}

Você pode atribuir uma tarefa ou um problema a uma equipe ágil. Depois de atribuída, a tarefa ou o problema aparece como uma nova história no backlog da equipe.

Para atribuir uma tarefa ou problema a uma equipe ágil:

1. Vá para o Projeto que contém a tarefa que deseja atribuir novamente.
1. Selecione a tarefa ou o problema na lista.
1. Clique em **[!UICONTROL Editar]**.
1. Clique em **[!UICONTROL Atribuições]**.
1. (Opcional) Exclua quaisquer destinatários existentes.
1. Clique em **[!UICONTROL Adicionar Destinatário]**.
1. Comece digitando o nome da equipe ágil que deseja atribuir à tarefa ou problema e clique no nome da equipe quando ele for exibido na lista suspensa.
1. Clique em **[!UICONTROL Salvar alterações]**.\
   A tarefa ou problema agora está disponível no backlog da equipe.

## Mover histórias do backlog para uma iteração ou + quadro {#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [Mover histórias existentes para o backlog](#move-existing-stories-to-the-backlog)
* [Exportar histórias do backlog](#export-stories-from-the-backlog)

1. Vá para o backlog da equipe ágil.
1. Selecione as histórias que você deseja mover para um quadro de iteração ou Kanban e clique em **[!UICONTROL Mais]** > **[!UICONTROL Mover para]**.\
   Se mover a história para uma [!UICONTROL Kanban] quadro, o [!UICONTROL Mover História para o Kanban] O quadro é exibido.\
   Se mover a história para uma iteração, a variável [!UICONTROL Mover história para uma iteração] será exibida.\
   ![Caixa de diálogo Mover história](assets/agile-backlog-addtoiteration.png)

1. Siga um destes procedimentos:

   * **Para equipes de Scrum:** No **[!UICONTROL Selecionar Iteração]** selecione a iteração onde deseja mover as histórias.

   * **Para equipes kanban:** No **[!UICONTROL Selecionar Quadro Kanban]** selecione sua equipe [!UICONTROL Kanban] quadro. (As equipes kanban podem ter apenas um [!UICONTROL Kanban] quadro.)

1. Clique em **[!UICONTROL Mover história]**.

### Mover histórias existentes para o backlog {#move-existing-stories-to-the-backlog}

Se você decidir que sua equipe ainda não está pronta para trabalhar em uma história, você pode mover a história para o backlog.

Para obter mais informações, consulte [Mover uma história ágil](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Exportar histórias do backlog {#export-stories-from-the-backlog}

Você pode exportar uma ou mais histórias (incluindo tarefas e problemas) diretamente do backlog.

Você exporta histórias do backlog da mesma forma que exporta outros dados no [!DNL Workfront], conforme descrito em [Exportar dados](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).
