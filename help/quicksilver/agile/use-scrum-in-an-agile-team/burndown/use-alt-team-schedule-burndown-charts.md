---
product-area: agile-and-teams
navigation-topic: burndown
title: Usar um Cronograma de Equipe Alternativo para Gráficos de Burndown
description: Os agendamentos definidos em [!DNL Adobe Workfront] afetam o gráfico de burndown excluindo dias de folga (finais de semana e feriados) do burndown.
author: Courtney
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 18%

---

# Usar um cronograma de equipe alternativo para gráficos de burndown

Os agendamentos definidos em [!DNL Adobe Workfront] afetam o gráfico de burndown excluindo dias de folga (finais de semana e feriados) do burndown.

Por padrão, o gráfico de burndown usa a programação padrão. Além da programação padrão, as equipes Ágeis podem optar por usar também uma programação alternativa para incorporar dias de folga específicos da equipe. Esse cronograma alternativo é refletido no gráfico de burndown de qualquer iteração atribuída à equipe. A programação alternativa afeta somente o gráfico de burndown. (Para obter mais informações sobre o agendamento padrão, bem como sobre como o administrador do [!DNL Workfront] pode criar um agendamento específico da equipe, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

O gráfico de detalhamento não leva em consideração dias parciais. Por exemplo, se sua equipe trabalha 4 horas por sexta-feira, isso é representado como um dia inteiro no gráfico de burndown.

Para obter mais informações sobre como usar o gráfico de detalhamento, consulte a [Visão geral do gráfico de detalhamento ágil](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <td> <p>Padrão</p> 
   <p>Trabalho ou maior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usar um cronograma de equipe alternativo para gráficos de burndown

1. Verifique se o administrador do [!DNL Workfront] já criou o agendamento alternativo, conforme descrito em [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Alternar equipe]** ![Ícone Alternar equipe](assets/switch-team-icon.png) e, em seguida, selecione uma nova equipe Scrum no menu suspenso ou pesquise uma equipe na barra de pesquisa.

1. Selecione a equipe ágil que deseja gerenciar.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

1. Na seção **[!UICONTROL Ágil]**, na área **[!UICONTROL Agendamento]**, selecione o novo agendamento no menu suspenso.

1. Clique em **[!UICONTROL Salvar alterações]**.
