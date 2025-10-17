---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Visão geral do gráfico de burndown ágil
description: O gráfico de burndown fornece uma representação visual de como as histórias estão progredindo pela iteração ou projeto . A taxa de burndown real é medida em relação à taxa de burndown ideal para a iteração ou linha do tempo do projeto.
author: Jenny
feature: Agile
exl-id: 414e3315-35ed-4aa4-a2d8-be42ec585f29
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Visão geral do gráfico de burndown ágil

O gráfico de burndown fornece uma representação visual de como as histórias estão progredindo na iteração. A taxa de burndown real é medida em relação à taxa de burndown ideal para a linha do tempo de iteração.

O gráfico de burndown é ajustado com base no dia selecionado. O dia atual é o padrão. Quando um dia anterior é selecionado, todos os dados no gráfico de burndown e todos os valores na seção [!UICONTROL status de conclusão] acima do gráfico de burndown são recalculados para representar os dados como estavam no final do dia selecionado. (Você pode selecionar dias passados ou o dia atual; não pode selecionar dias no futuro.)

![](assets/agile-iteration-burndown-350x88.png)

## Indicadores visuais

O gráfico de burndown contém os seguintes indicadores visuais:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-dottedblue.png" alt="Início da taxa de burndown ideal"> </td> 
   <td> <p>Taxa de burndown ideal com base em quando a iteração começou.</p> <p>Essa linha não será exibida se o escopo da iteração nunca for alterado (horas ou pontos nunca são adicionados ou removidos).</p> <p>Esta linha é exibida como simples quando o trabalho é concluído em um dia de folga. Para obter mais informações, consulte <a title="Uso do Gráfico de Burndown Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Como os dias de folga afetam o gráfico de burndown</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-solidblue.png" alt="Taxa de burndown ideal em histórias ou tarefas"> </td> 
   <td> <p>Taxa de burndown ideal com base em histórias ou tarefas atuais.</p> <p>A taxa de burndown ideal atual (linha azul sólida) difere da taxa de burndown ideal original (linha azul pontilhada) quando horas ou pontos são adicionados ou removidos da iteração após o início da iteração.</p> <p>Esta linha é exibida como simples quando o trabalho é concluído em um dia de folga.</p> <p>Para obter mais informações, consulte <a title="Uso do Gráfico de Burndown Agile" href="#how-days-off-affect-the-burndown-chart" class="MCXref xref">Como os dias de folga afetam o gráfico de burndown</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-red.png" alt="Taxa de burndown real em vermelho"> </td> 
   <td> <p>A taxa de burndown real é mostrada em vermelho quando a taxa de burndown é menor que a ideal (mais pontos ou horas restantes por dia do que o cálculo de burndown ideal).</p> <p>A fórmula a seguir é usada para calcular a taxa de burndown real:</p> <p>[SUM(Valor em Ponto ou Hora do Trabalho em Andamento * Percentual Concluído) + Valor em Ponto ou Hora do Trabalho Concluído]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-green.png" alt="Taxa de burndown real em verde"> </td> 
   <td> <p>A taxa de burndown real é mostrada em verde quando a taxa de burndown é igual ou melhor que o ideal (pontos iguais ou menos remanescentes por dia do que o cálculo de burndown ideal).</p> <p>A fórmula a seguir é usada para calcular a taxa de burndown real:</p> <p>[SUM(Valor em Ponto ou Hora do Trabalho em Andamento * Percentual Concluído) + Valor em Ponto ou Hora do Trabalho Concluído]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Alteração no escopo"> </td> 
   <td> <p>Alteração no escopo (horas ou pontos são adicionados ou removidos da iteração).</p> <p>As alterações de escopo são sempre mostradas como uma linha vertical no meio do dia. Além disso, um ponto azul é exibido no meio de qualquer dia em que ocorreu uma alteração de escopo.</p> <p>O eixo vertical do gráfico de burndown mostra os pontos da história ou as horas.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Alteração no intervalo de datas"> </td> 
   <td> <p>Alteração no intervalo de datas (a duração da iteração é aumentada ou diminuída).</p> <p>Um ponto azul é exibido no meio de qualquer dia em que a duração da iteração foi alterada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <img src="assets/agile-iteration-burndown-scope.png" alt="Ponto verde para trabalho queimado"> </td> 
   <td> <p>Um ponto verde ou vermelho é exibido na taxa de burndown real sempre que o trabalho é reduzido. (Quando a taxa de burndown real naquele dia é vermelha, o ponto é vermelho; quando a taxa de burndown real naquele dia é verde, o ponto é verde.)</p> <p>O trabalho é queimado quando qualquer uma das seguintes situações ocorre:</p> 
    <ul> 
     <li> A [!UICONTROL Percentual concluído] é aumentada na matéria.<br>[!UICONTROL Percentual Concluído] aumenta quando: 
      <ul> 
       <li> <p>Alterado manualmente</p> </li> 
       <li> <p>O número de pontos ou horas é atualizado na história</p> </li> 
      </ul></li>  
     <li>O status da história é alterado para [!UICONTROL Concluído]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Como os dias de folga afetam o gráfico de burndown {#how-days-off-affect-the-burndown-chart}

O agendamento padrão definido em [!DNL Workfront] afeta o gráfico de burndown excluindo dias de folga (finais de semana e feriados) do burndown. O gráfico de burndown usa a programação padrão para definir dias úteis (conforme descrito em  [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)).

As equipes Agile podem incorporar dias não úteis específicos da equipe definindo um agendamento alternativo (conforme descrito no artigo [Usar um agendamento de equipe alternativo para gráficos de burndown](../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md)). Esse cronograma alternativo é refletido no gráfico de burndown de qualquer iteração atribuída à equipe. A programação alternativa afeta somente o gráfico de burndown.

Os dias de folga são refletidos no gráfico de burndown somente se:

* O trabalho era registrado anteriormente em um dia de folga. (O dia em que o trabalho foi registrado é exibido.)

  Quando o trabalho é logado em um dia de folga:

   * Qualquer trabalho reportado não é incluído ao calcular o burndown ideal porque a equipe não está agendada para realizar qualquer trabalho.
   * As linhas de burndown ideais (a linha azul sólida e a linha azul tracejada) são exibidas como planas no gráfico de burndown para qualquer dia em que o trabalho tenha sido concluído ou no dia em que você estiver visualizando o gráfico de burndown (se estiver visualizando em um dia de folga).
   * O trabalho registrado é incluído ao calcular outras estatísticas de burndown, como a conclusão estimada e a média de pontos ou horas por dia.

* Você está visualizando o gráfico de burndown em um dia de folga. (O dia que você está visualizando é mostrado no gráfico de burndown.)
* Você conclui o trabalho total restante para a iteração em um dia de folga.

  Quando um usuário conclui o trabalho total restante para a iteração em um dia de folga, o campo [!UICONTROL Conclusão estimada] exibe a data em que a iteração foi concluída.

  Ao planejar a iteração, se você definir a data de término da iteração para um dia não útil e a iteração estiver rastreando para terminar no prazo, a [!UICONTROL Data de conclusão estimada] será definida para o último dia útil anterior à data de término da iteração definida (porque o trabalho não está agendado para ser reduzido em dias não úteis).

  A data de término da iteração é especificada quando ela é planejada, conforme descrito no artigo [Criar uma iteração](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).
