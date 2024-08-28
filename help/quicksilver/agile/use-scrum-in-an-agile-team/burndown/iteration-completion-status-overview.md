---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Visão geral do status de conclusão da iteração
description: As informações de conclusão descritas neste artigo são exibidas acima do gráfico de burndown.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 0%

---

# Visão geral do status de conclusão da iteração

As informações de conclusão descritas neste artigo são exibidas acima do gráfico de burndown.

Porcentagem de conclusão em uma iteração:

![](assets/burndown-percentcomplete-350x47.png)

Essas informações indicam o status de conclusão da iteração para o dia atualmente selecionado no gráfico de burndown. Por padrão, o status de conclusão é exibido com base na data do dia atual.

As seguintes informações estão disponíveis:

* **[!UICONTROL Percentual Concluído]:** Progresso geral da iteração

  [!UICONTROL Percentual concluído] ajusta com base no percentual concluído de cada história ou tarefa dentro da iteração, incluindo histórias ou tarefas que estão apenas parcialmente concluídas.

  A cor da barra de status [!UICONTROL Percentual concluído] é exibida em vermelho ou verde para corresponder à cor da taxa de burndown real. É mostrado em vermelho quando a taxa de burndown é menor que a ideal (mais pontos ou horas restantes por dia do que o cálculo de burndown ideal) e é mostrado em verde quando a taxa de burndown é igual ou melhor do que a ideal (pontos iguais ou menos pontos restantes por dia do que o cálculo de burndown ideal).

* **[!UICONTROL Histórias Concluídas]:** (Disponível somente em iterações) O número de histórias marcadas como [!UICONTROL Concluídas]. Isso é mostrado em relação ao número total de histórias na iteração. Por exemplo, &quot;3 de 6&quot; indica que 3 das 6 matérias na iteração foram marcadas como [!UICONTROL Concluídas].
* **[!UICONTROL Pontos/Horas Concluídos]:** (Disponível somente em iterações) O número de pontos ou horas marcados como [!UICONTROL Concluídos]. Mostrado em relação ao número total de pontos ou horas na iteração. Por exemplo, &quot;5 de 11&quot; indica que 5 das 11 matérias na iteração foram marcadas como [!UICONTROL Concluídas]. Este número está diretamente relacionado ao cálculo do [!UICONTROL Percentual Concluído] e é atualizado ao mesmo tempo que [!UICONTROL Percentual Concluído] é atualizado.

  Pontos e horas estão associados a histórias. Quando uma matéria é marcada como [!UICONTROL Concluída], os pontos ou horas associados a essa matéria são marcados como Concluídos.

  Por padrão, são usados pontos. Você pode alterar modificando as configurações da sua equipe, conforme descrito em [Criar uma equipe ágil](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Pontos / Horas por dia]:** (Disponível somente em iterações) O número médio de pontos ou horas marcados como [!UICONTROL Concluído] todos os dias desde o início da iteração até o dia atual.

  Isso é calculado pelo total de pontos ou horas concluídas, dividido pelo número total de dias até o dia atual. (Dias parciais são registrados como um dia inteiro.)

  Essas informações podem ser úteis ao planejar uma iteração futura.

* **[!UICONTROL Conclusão estimada]:** A data estimada em que a iteração será concluída, com base na taxa atual em Pontos / Horas por Dia (para iterações).

  Quando a data de [!UICONTROL Conclusão estimada] for posterior à data de término definida para a iteração, o número de dias úteis restantes será exibido entre parênteses ao lado da data de [!UICONTROL Conclusão estimada].

  Quando a [!UICONTROL Data de conclusão estimada] é anterior à data planejada de término da iteração, o número de dias úteis restantes é exibido em verde. (A data de término da iteração é especificada quando a iteração é planejada, conforme descrito em [Criar uma iteração](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); a data de término do projeto é a [!UICONTROL Data de Término Planejada] ou será a data atual se a [!UICONTROL Data de Término Planejada] estiver no passado. A [!UICONTROL Data de conclusão planejada] para o projeto é calculada com base na duração das tarefas no projeto.) Ao planejar a iteração, se você definir a data final da iteração para um dia não útil e a iteração estiver rastreando para terminar no prazo, a Data de conclusão estimada será definida para o último dia útil anterior à data final da iteração definida (porque o trabalho não está programado para ser reduzido em dias não úteis).

  Por exemplo, &quot;(+9 dias)&quot; indica que a data de conclusão estimada é 9 dias úteis depois da data de término planejada da iteração.

  Para obter mais informações, consulte [Visão geral do status de conclusão da iteração](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
