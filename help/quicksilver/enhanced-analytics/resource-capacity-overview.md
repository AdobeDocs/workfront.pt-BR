---
title: Exibir a visualização Capacidade do recurso na Análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Você pode avaliar se uma equipe terminou, está abaixo ou na capacidade ao visualizar o gráfico de visualização Capacidade de recursos de análise aprimorada no Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 3b3ba7cc6a975af71205f7f524e1a9a91a9d3810
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 0%

---

# Exibir a visualização Capacidade do recurso na Análise aprimorada

Você pode avaliar se uma equipe terminou, está abaixo ou na capacidade ao visualizar o gráfico de visualização Capacidade de recursos de análise aprimorada no Adobe Workfront.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>plano do Adobe Workfront</a>*</td> 
   <td> <p>Atual: Comercial ou superior</p>
   Ou
   <p>Novo: Qualquer um</p>
    </td> 
  </tr> 
  <tr> 
   <td>Licença da Adobe Workfront*</td> 
   <td> <p>Atual: revisão ou superior</p>
   Ou
   <p>Novo: Padrão</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Visualizar acesso aos projetos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissão em um projeto</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender o gráfico de capacidade de recursos

O gráfico Capacidade do recurso mostra se uma equipe está acima, abaixo ou na capacidade. Este cálculo é baseado em:

* **Capacidade disponível**: a quantidade total de horas que uma equipe da página inicial tem disponíveis para trabalhar no período filtrado

  >[!NOTE]
  >
  >Se você estiver olhando para um período futuro, a capacidade disponível é calculada com base na capacidade da equipe para os últimos 7 dias. Por esse motivo, nenhum PTO programado é levado em consideração.

* **Capacidade planejada**: a quantidade total de horas de trabalho planejadas esperadas da equipe inicial no período filtrado

Essa comparação das horas planejadas de uma equipe doméstica e das horas programadas reais pode ajudar você a determinar se não está atribuindo trabalho suficiente à equipe doméstica ou se ela pode estar com esgotamento devido a uma carga de trabalho pesada.

![](assets/resource-capacity-350x110.png)

Na visualização Capacidade do recurso, você pode ver os seguintes detalhes:

* **Capacidade planejada**: em linha com um nome de equipe inicial, o círculo azul representa o número de horas planejadas atribuídas à equipe inicial.

  ![](assets/resource-capacity-blue-circle.png)

* **Capacidade real**: em linha com um nome de equipe da página inicial, a linha vertical representa o número de horas disponíveis para a equipe da página inicial.

  ![](assets/resource-capacity-vertical-line.png)

* **Acima da capacidade**: quando a linha horizontal e o círculo azul são exibidos à direita da linha vertical, a equipe inicial recebe mais trabalho do que pode ser concluído em termos do número de horas disponíveis. Isso significa que o grupo pode estar acima da capacidade no período de tempo filtrado. O número restante de horas que o grupo precisa completar é exibido à direita do círculo azul.

  ![](assets/resource-capacity-over-capacity.png)

* **Abaixo da capacidade**: quando a linha horizontal e o círculo azul são exibidos à esquerda da linha vertical, a equipe da página inicial tem mais horas disponíveis do que o número de horas planejadas de trabalho que foram atribuídas a ela. Isso significa que o grupo pode estar abaixo da capacidade pelo período de tempo filtrado. O número adicional de horas disponíveis para a equipe da página inicial concluir o trabalho é exibido à esquerda do círculo azul.

  ![](assets/resource-capacity-under-capacity.png)

Passar o mouse sobre uma linha mostra o número exato de horas para a capacidade planejada e a capacidade disponível, bem como o número de horas em que a equipe doméstica está acima ou abaixo da capacidade.

Ver essas informações ajuda a determinar:

* Se a equipe inicial estava superalocada ou subalocada.
* Quais eram os maiores projetos nos quais a equipe da casa se concentrava.
* Quais equipes domésticas estão disponíveis para trabalho.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Exibir a visualização de capacidade do recurso

1. Clique no ícone Menu principal ![](assets/main-menu-icon-16x12.png)e selecione **Analytics**.
1. No painel esquerdo, selecione **Pessoas**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre o uso do filtro de intervalo de datas, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se você não definiu o filtro Equipe, adicione o filtro Equipe e selecione cada equipe cujos dados você deseja ver.

   Para obter mais informações sobre como adicionar filtros na Análise aprimorada, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Depois de adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois de sair da página ou do Workfront.

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização para o início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas e um filtro de período é criado.

   ![](assets/timeframe-filter-350x220.png)

1. Passe o mouse sobre a linha de equipe doméstica para ver quantas horas ainda estão disponíveis para serem programadas, a quantidade de horas planejadas para a equipe doméstica ser concluída e o número total de horas trabalhadas, rotulado como acima, abaixo ou na capacidade.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Opcional) Para exportar os dados de visualização, clique no link **Ícone Exportar** ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

1. Clique no nome de uma equipe inicial para ver mais informações na visualização Capacidade da equipe.

   Para saber mais sobre a visualização Capacidade da equipe, consulte [Visualização da Capacidade da equipe na Análise aprimorada](../enhanced-analytics/team-capacity-overview.md).


