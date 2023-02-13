---
title: Visualizar a Visualização da capacidade dos recursos no Enhanced Analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização da capacidade do recurso mostra se uma equipe terminou, está abaixo ou está na capacidade. Este cálculo é baseado em - EDIT ME.
author: Nolan
feature: Reports and Dashboards
exl-id: 5bb45ef6-9e49-4063-8e53-c9f3bc994870
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Visualizar a Visualização da capacidade dos recursos no Enhanced Analytics

A visualização da capacidade do recurso mostra se uma equipe terminou, está abaixo ou está na capacidade.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano Adobe Workfront</a>*</td> 
   <td> <p>Empresa ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar o acesso a Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso.<br>Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização da capacidade do recurso

A visualização da capacidade do recurso mostra se uma equipe terminou, está abaixo ou está na capacidade. Este cálculo é baseado em:

* **Capacidade disponível**: A quantidade total de horas que uma equipe doméstica tem disponível para trabalhar no período filtrado

   >[!NOTE]
   >
   >Se você estiver olhando para um período futuro, a capacidade disponível é calculada com base na capacidade da equipe nos últimos 7 dias. Por esta razão, qualquer PTO programado não é considerado.

* **Capacidade planejada**: A quantidade total de horas de trabalho programadas esperadas da equipe de origem no período filtrado

Essa comparação das horas planejadas de uma equipe doméstica e das horas agendadas reais pode ajudar você a determinar se você não está atribuindo trabalho suficiente à equipe inicial ou se eles podem estar experimentando um esgotamento de uma carga de trabalho pesada.

![](assets/resource-capacity-350x110.png)

Na visualização da capacidade do recurso, você pode ver os seguintes detalhes:

* **Capacidade planejada**: Em linha com o nome de uma equipe inicial, o círculo azul representa o número de horas planejadas atribuídas à equipe inicial.

   ![](assets/resource-capacity-blue-circle.png)

* **Capacidade real**: Em linha com o nome de uma equipe inicial, a linha vertical representa o número de horas disponíveis para a equipe inicial.

   ![](assets/resource-capacity-vertical-line.png)

* **Capacidade excedentária**: Quando a linha horizontal e o círculo azul são exibidos à direita da linha vertical, a equipe inicial recebeu mais trabalho do que pode ser concluído no número de horas disponíveis. Isso significa que a equipe pode estar acima da capacidade do período filtrado. O número restante de horas que a equipe precisa concluir é exibido à direita do círculo azul.

   ![](assets/resource-capacity-over-capacity.png)

* **Em termos de capacidade**: Quando a linha horizontal e o círculo azul são exibidos à esquerda da linha vertical, a equipe inicial tem mais horas disponíveis do que o número de horas de trabalho planejadas que foram atribuídas. Isso significa que a equipe pode estar com capacidade para o período filtrado. O número adicional de horas disponíveis para a equipe inicial concluir o trabalho é exibido à esquerda do círculo azul.

   ![](assets/resource-capacity-under-capacity.png)

Passar o mouse sobre uma linha mostra o número exato de horas de capacidade planejada e disponível, bem como o número de horas em que a equipe inicial está acima ou abaixo da capacidade.

Ver essas informações ajuda a determinar:

* Se a equipe inicial tiver sido atribuída em excesso ou atribuída em subalocação.
* Quais foram os maiores projetos em que a equipe residencial estava focada.
* Quais equipes domésticas estão disponíveis para trabalho.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizar a capacidade do recurso

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. No painel esquerdo, selecione **Pessoas**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se você não definiu seu filtro Equipe , adicione o filtro Equipe e selecione cada equipe para a qual deseja visualizar os dados.

   Para obter mais informações sobre como adicionar filtros nas Análises aprimoradas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Após adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois que você sai da página ou faz logoff do Workfront.

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização do início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas, e um filtro de período é criado.

   ![](assets/timeframe-filter-350x220.png)

1. Passe o mouse sobre a linha da equipe inicial para ver quantas horas ainda estão disponíveis para serem programadas, a quantidade de horas planejadas para a equipe inicial ser concluída e o número total de horas trabalhadas, que é rotulado como sobre, abaixo ou na capacidade.

   ![](assets/resource-capacity-capacity-pop-up-350x213.png)

1. (Opcional) Para exportar os dados de visualização, clique no botão **Ícone Exportar** ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

1. Clique em um nome de equipe inicial para ver mais informações na visualização de capacidade da equipe.

   Para saber mais sobre a visualização da capacidade da equipe, consulte [Visualização da capacidade do grupo na Análise aprimorada](../enhanced-analytics/team-capacity-overview.md).


