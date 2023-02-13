---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Visão geral do status de conclusão de iteração
description: As informações de conclusão descritas neste artigo são exibidas acima do gráfico de detalhamento.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
source-git-commit: 373f2522b85196d6395f189ae6cfe03449cac61a
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Visão geral do status de conclusão de iteração

As informações de conclusão descritas neste artigo são exibidas acima do gráfico de detalhamento.

Porcentagem de conclusão em uma iteração:

![](assets/burndown-percentcomplete-350x47.png)

Essas informações indicam o status de conclusão da iteração do dia atualmente selecionado no gráfico suspenso. Por padrão, o status de conclusão é exibido com base na data do dia atual.

As seguintes informações estão disponíveis:

* **[!UICONTROL Porcentagem concluída]:** Progresso geral da iteração

   [!UICONTROL Porcentagem concluída] ajustes baseados na porcentagem completa de cada história ou tarefa dentro da iteração, incluindo histórias ou tarefas que são apenas parcialmente concluídas.

   A cor do [!UICONTROL Porcentagem concluída] a barra de status é exibida em vermelho ou verde para corresponder à cor da taxa de detalhamento real. Ele é mostrado em vermelho quando a taxa de detalhamento é menor do que o ideal (mais pontos ou horas restantes por dia do que o cálculo de detalhamento ideal) e é mostrado em verde quando a taxa de detalhamento é igual ou melhor do que o ideal (igual ou menos pontos restantes por dia do que o cálculo de detalhamento ideal).

* **[!UICONTROL Histórias concluídas]:** (Disponível somente em iterações) O número de histórias marcadas [!UICONTROL Concluído]. Isso é mostrado em relação ao número total de histórias na iteração. Por exemplo, &quot;3 de 6&quot; indica que 3 das 6 histórias da iteração foram marcadas [!UICONTROL Concluído].
* **[!UICONTROL Pontos/Horas Concluídos]:** (Disponível apenas em iterações) O número de pontos ou horas marcados [!UICONTROL Concluído]. Mostrado em relação ao número total de pontos ou horas na iteração. Por exemplo, &quot;5 de 11&quot; indica que 5 das 11 histórias da iteração foram marcadas [!UICONTROL Concluído]. Esse número está diretamente relacionado ao [!UICONTROL Porcentagem concluída] e é atualizado ao mesmo tempo [!UICONTROL Porcentagem concluída] é atualizado.

   Pontos e horas são associados a histórias. Quando uma história é marcada [!UICONTROL Concluído], os pontos ou horas associados a essa história são marcados como Concluído.

   Por padrão, pontos são usados. Você pode alterar isso modificando as configurações para sua equipe, conforme descrito em [Criar uma equipe ágil](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Pontos / Horas Por Dia]:** (Disponível apenas em iterações) O número médio de pontos ou horas marcados [!UICONTROL Concluído] cada dia desde o início da iteração até o dia atual.

   Isso é calculado pelo total de pontos ou horas concluídas, dividido pelo número total de dias até o dia atual. (Dias parciais são registrados como um dia inteiro.)

   Essas informações podem ser úteis ao planejar uma iteração futura.

* **[!UICONTROL Conclusão estimada]:** A data estimada em que a iteração será concluída, com base na taxa atual em Pontos / Horas por Dia (para iterações).

   Quando a variável [!UICONTROL Conclusão estimada] for posterior à data de término definida para a iteração, o número de dias úteis restantes será exibido em vermelho entre parênteses ao lado da [!UICONTROL Conclusão estimada] data.

   Quando a variável [!UICONTROL Conclusão estimada] for anterior à data de término planejada da iteração, o número de dias úteis restantes será exibido em verde. (A data final da iteração é especificada quando a iteração é planejada, conforme descrito em [Criar uma iteração](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); a data de término do projeto é [!UICONTROL Data de Conclusão Planejada]ou é a data atual se a variável [!UICONTROL Data de Conclusão Planejada] está no passado. O [!UICONTROL Data de Conclusão Planejada] para o projeto é calculado com base na duração das tarefas do projeto.) Ao planejar a iteração, se você definir a data final da iteração para um dia que não seja útil e a iteração estiver rastreando para terminar no tempo, a Data de conclusão estimada será definida para o último dia útil antes da data de término da iteração que você definir (porque o trabalho não está programado para ser gravado em dias que não sejam úteis).

   Por exemplo, &quot;(+9 dias)&quot; indica que a Data de conclusão estimada é 9 dias úteis depois da data de término planejada da iteração.

   Para obter mais informações, consulte [Visão geral do status de conclusão de iteração](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
