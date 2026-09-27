---
product-area: agile-and-teams
navigation-topic: burndown
title: Usar uma Programação de Equipe Alternativa para Gráficos de Burndown
description: Os cronogramas definidos em [!DNL Adobe Workfront] afetam o gráfico de burndown excluindo dias de folga (finais de semana e feriados) do burndown.
author: Courtney
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/BWnnytUMaoygpGpDdjQ5dmdBZrR1IWAu7onkwVizvUc'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 16%
---
# Usar um cronograma de equipe alternativo para gráficos de burndown

Os cronogramas definidos em [!DNL Adobe Workfront] afetam o gráfico de burndown excluindo dias de folga (finais de semana e feriados) do burndown.

Por padrão, o gráfico de burndown usa a programação padrão. Além da programação padrão, as equipes Agile podem optar por usar também uma programação alternativa para incorporar dias não úteis específicos da equipe. Esse cronograma alternativo é refletido no gráfico de burndown de qualquer iteração atribuída à equipe. A programação alternativa afeta somente o gráfico de burndown. (Para obter mais informações sobre o agendamento padrão, bem como sobre como o administrador do [!DNL Workfront] pode criar um agendamento específico de equipe, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

O gráfico de burndown não considera dias parciais. Por exemplo, se sua equipe trabalha 4 horas todas as sextas-feiras, isso é representado como um dia inteiro no gráfico de burndown.

Para obter mais informações sobre como usar o gráfico de burndown, consulte a [visão geral do gráfico de burndown Agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

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

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usar um cronograma de equipe alternativo para gráficos de burndown

1. Verifique se o administrador [!DNL Workfront] já criou o agendamento alternativo, conforme descrito em [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a equipe Agile que você deseja gerenciar.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

1. Na seção **[!UICONTROL Agile]**, na área **[!UICONTROL Agendar]**, selecione o novo agendamento no menu suspenso.

1. Clique em **[!UICONTROL Salvar alterações]**.
