---
product-area: agile-and-teams
navigation-topic: iterations
title: Criar uma iteração
description: As iterações são um componente essencial para as equipes ágeis de Scrum no planejamento da capacidade de trabalho. [!DNL Adobe Workfront] permite que equipes ágeis do Scrum gerenciem seu trabalho criando várias iterações para acomodar as necessidades da equipe.
author: Jenny
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 0%

---

# Criar uma iteração

As iterações são um componente essencial para as equipes ágeis de Scrum no planejamento da capacidade de trabalho. [!DNL Adobe Workfront] permite que equipes ágeis do Scrum gerenciem seu trabalho criando várias iterações para acomodar as necessidades da equipe.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Leve ou superior</p> 
   <p>Revisar ou superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar uma iteração

Você pode adicionar uma iteração à lista para criar rapidamente uma iteração e adicionar tarefas e problemas a ela posteriormente.

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Na guia **[!UICONTROL Iterações]**, clique em **[!UICONTROL Adicionar iteração]**.

   ![Clique em Adicionar iteração](assets/click-add-iteration.png)

1. Especifique o seguinte:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome da Iteração]</strong></td> 
      <td>Insira o nome da iteração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Meta]</strong></td> 
      <td>Adicione metas à iteração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data de Início]</strong></td> 
      <td>Insira a data em que a iteração deve começar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data de Término]</strong></td> 
      <td><p>Insira a data em que a iteração deve terminar. A [!DNL Workfront] recomenda definir uma data de término não superior a 4 semanas a partir da data de início.</p><p>Dica: certifique-se de escolher um dia útil como a data final. O gráfico de burndown usa apenas dias úteis em seus cálculos.<br>Por padrão, o gráfico de burndown usa o agendamento padrão para definir dias úteis (conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>). Ou, para incorporar dias não úteis específicos da equipe, as equipes ágeis podem optar por usar um agendamento alternativo (conforme descrito em "Definindo um Agendamento de Equipe Alternativo para Gráficos de Burndown" em <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Criar uma equipe ágil</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacidade]</strong></td> 
      <td> Especifique a capacidade da iteração. Este é o número de pontos ou horas que sua equipe consegue completar na iteração. O número inserido deve ser igual ou maior que o número de pontos ou horas a partir da soma de todas as histórias na iteração.O <br>[!DNL Workfront] preenche este campo previamente com 50 caracteres por padrão. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Foco]</strong></td> 
      <td>Especificar a porcentagem de foco da equipe. Se todos os membros da equipe estiverem totalmente focados nessa iteração, o foco será 100%.O <br>[!DNL Workfront] preenche este campo previamente com 100% por padrão. </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Adicionar iteração]**. Agora que você criou uma iteração, é necessário adicionar histórias. Para obter mais informações, consulte [Adicionar histórias a uma iteração existente](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planejar uma iteração na guia [!UICONTROL Backlog]

Use o recurso [!UICONTROL Planejar Iteração] para criar uma iteração usando tarefas em sua lista de pendências.

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione **[!UICONTROL Lista de pendências]** no painel esquerdo.

1. Na guia **Histórias** ou **Problemas**, selecione os itens de trabalho que deseja adicionar à iteração e clique em **[!UICONTROL Planejar Iteração]**.

>[!NOTE]
>
> Não é possível alternar entre as guias Histórias ou Problemas ou adicionar outras tarefas ao planejar uma iteração na guia Backlog. Você pode adicionar histórias ou problemas existentes depois que a iteração for criada. Para obter mais informações, consulte [Adicionar tarefas ou problemas a uma iteração existente na guia Lista de Pendências](#add-tasks-or-issues-to-an-existing-iteration-on-the-backlog-tab) abaixo.


1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome da Iteração]</strong></td> 
      <td>Especifique um nome para a iteração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data de Início]</strong></td> 
      <td> Especifique a data em que a iteração deve começar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data Final]</strong> </td> 
      <td><p>Especifique a data em que a iteração deve terminar. A [!DNL Workfront] recomenda definir uma data de término não superior a 4 semanas a partir da data de início.</p><p>Dica: certifique-se de escolher um dia útil como a data final. O gráfico de burndown usa apenas dias úteis em seus cálculos.<br>Por padrão, o gráfico de burndown usa o agendamento padrão para definir dias úteis (conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>). Ou, para incorporar dias não úteis específicos da equipe, as equipes ágeis podem optar por usar um agendamento alternativo (conforme descrito em <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Usar um agendamento de equipe alternativo para gráficos de burndown</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Foco]</strong></td> 
      <td>Especificar a porcentagem de foco da equipe. Se todos os membros da equipe estiverem totalmente focados nessa iteração, o foco será 100%.<br>[!DNL Workfront] preenche este campo previamente com o valor médio das iterações anteriores da sua equipe. Se esta for a primeira iteração da sua equipe, o valor deste campo será 0 por padrão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacidade]</strong></td> 
      <td> Especifique a capacidade da iteração. Este é o número de pontos ou horas que sua equipe consegue completar na iteração. O número inserido deve ser igual ou maior que o número de pontos ou horas a partir da soma de todas as histórias na iteração.<br>[!DNL Workfront] preenche este campo previamente com o valor médio das iterações anteriores da sua equipe. Se esta for a primeira iteração da sua equipe, o valor deste campo será 0 por padrão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Meta]</strong></td> 
      <td> Especifique uma meta para a iteração. Este campo não é obrigatório.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar].** A iteração foi criada.

## Adicionar tarefas ou problemas a uma iteração existente na guia Backlog

1. Na guia **Backlog**, clique na guia **Histórias** ou **Problemas**.

1. Selecione as histórias ou problemas que deseja adicionar à iteração. As histórias no topo do backlog têm prioridade mais alta.

   ![mover um item de trabalho](assets/move-to-iteration.png)

   >[!NOTE]
   >
   >  Ao adicionar tarefas a uma iteração, a data de início da tarefa é calculada conforme descrito em [[!UICONTROL Entender] como as datas de início da tarefa são calculadas quando adicionadas a uma iteração](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).


## Entender como as datas de início da tarefa são calculadas quando adicionadas a uma iteração {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Quando você adiciona uma tarefa como uma história a uma iteração, a restrição [!UICONTROL Deve Terminar na tarefa] é usada para cada história. Na maioria dos casos, a data de início planejada da tarefa é calculada com base na seguinte fórmula:

[!UICONTROL Data de Término da Iteração] menos (-) [!UICONTROL Duração da Tarefa] igual (=) [!UICONTROL Data de Início Planejada da Tarefa]

A [!UICONTROL Data Final do Projeto] será usada em vez da Data Final da Iteração se a data inicial do projeto for posterior à data inicial da iteração e a data final do projeto for posterior à data final da iteração.

Você pode configurar equipes Scrum individuais para usar as datas do projeto por padrão, em vez das datas de iteração. Para obter informações, consulte a seção [Configurar como as datas são aplicadas ao adicionar itens de trabalho a uma iteração](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) no artigo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
