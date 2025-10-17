---
product-area: agile-and-teams
navigation-topic: burndown
title: Usar uma Programação de Equipe Alternativa para Gráficos de Burndown
description: Os cronogramas definidos em [!DNL Adobe Workfront] afetam o gráfico de burndown excluindo dias de folga (finais de semana e feriados) do burndown.
author: Jenny
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# Usar uma programação de equipe alternativa para gráficos de burndown

Os cronogramas definidos em [!DNL Adobe Workfront] afetam o gráfico de burndown excluindo dias de folga (finais de semana e feriados) do burndown.

Por padrão, o gráfico de burndown usa a programação padrão. Além da programação padrão, as equipes ágeis podem optar por usar também uma programação alternativa para incorporar dias não úteis específicos da equipe. Esse cronograma alternativo é refletido no gráfico de burndown de qualquer iteração atribuída à equipe. A programação alternativa afeta somente o gráfico de burndown. (Para obter mais informações sobre o agendamento padrão, bem como sobre como o administrador do [!DNL Workfront] pode criar um agendamento específico de equipe, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

O gráfico de burndown não considera dias parciais. Por exemplo, se sua equipe trabalha 4 horas todas as sextas-feiras, isso é representado como um dia inteiro no gráfico de burndown.

Para obter mais informações sobre como usar o gráfico de burndown, consulte a [visão geral do gráfico de burndown Agile](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

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
   <td> <p>Standard</p> 
   <p>Trabalhar ou superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usar uma programação de equipe alternativa para gráficos de burndown

1. Verifique se o administrador [!DNL Workfront] já criou o agendamento alternativo, conforme descrito em [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Selecione a Equipe Ágil que deseja gerenciar.
1. Clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

1. Na seção **[!UICONTROL Agile]**, na área **[!UICONTROL Agendar]**, selecione o novo agendamento no menu suspenso.

1. Clique em **[!UICONTROL Salvar alterações]**.
