---
title: Visualização da Capacidade da equipe na Análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização Capacidade da equipe mostra a quantidade total de capacidade de uma equipe doméstica, se está superalocada ou subalocada, e o quão dinâmica a capacidade é ao longo do tempo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 81118e794dca746b482b8355c24fa997a9f0edc9
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 0%

---

# Visualização da Capacidade da equipe na Análise aprimorada

<!-- Audited: 01/2024 -->

A visualização Capacidade da equipe mostra a quantidade total de capacidade de uma equipe doméstica, se está superalocada ou subalocada, e o quão dinâmica a capacidade é ao longo do tempo.

![Capacidade da equipe](assets/team-capacity.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>
      <p>Novo: Qualquer um</p>
      <p>ou</p>
      <p>Atual: Comercial ou superior</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td>
   <td>
      <p>Novo: Claro ou superior</p>
      <p>ou</p>
      <p>Atual: revisão ou superior</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Visualizar acesso aos projetos</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Exibir </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

Para obter os pré-requisitos para usar o Enhanced Analytics, consulte a seção &quot;Pré-requisitos&quot; em [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Entender a visualização da capacidade da equipe

A visualização Capacidade da equipe exibe o volume de trabalho atribuído à equipe inicial em um determinado dia.

* **Burnout**: quando a cor de preenchimento azul mais escura está acima da linha pontilhada, a equipe da página inicial tem mais horas de trabalho atribuídas a ela do que o número de horas que pode concluir para que a equipe esteja disponível para trabalhar. Isso indica que a equipe está superalocada e pode estar se aproximando do esgotamento.

  ![Acima da capacidade](assets/team-capacity-over-capacity.png)

* **Sem desafio**: quando a cor de preenchimento azul mais escura estiver abaixo da linha pontilhada, a equipe da página inicial terá mais horas disponíveis para trabalhar do que a quantidade de trabalho atribuída a ela. Isso indica que a equipe está subalocada e pode não ser desafiada.

  ![Abaixo da capacidade](assets/team-capacity-under-capacity.png)

* **Saldo**: quando a cor de preenchimento azul mais clara ou mais transparente está logo acima, logo abaixo ou na linha pontilhada, a equipe da página inicial tem uma quantidade de horas de trabalho atribuídas a ela que deve ser capaz de concluir dentro de suas horas de trabalho disponíveis. Isso indica que a carga de trabalho do grupo é mais equilibrada.

  ![Na capacidade](assets/team-capacity-at-capacity.png)

Passar o mouse sobre qualquer ponto na visualização mostra os seguintes detalhes para um determinado dia:

* **Horas programadas**: este é o número de horas planejadas de trabalho que a equipe precisa concluir.
* **Horas disponíveis**: este é o número de horas de trabalho que a equipe está disponível para trabalhar.
* **Capacidade**: Além de uma porcentagem de capacidade, as designações At capacity, Sub capacity ou Over capacity também são exibidas.

Ver essas informações ajuda a determinar:

* Quando a equipe inicial estava superalocada ou subalocada.
* Se a equipe inicial estiver superalocada ou subalocada diariamente.
* Quão consistente é a carga de trabalho de uma equipe doméstica no dia a dia.
* Se você estiver criando problemas de capacidade com um novo trabalho.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Exibir a visualização Capacidade da equipe

{{step1-to-analytics}}

1. No painel esquerdo, selecione **Pessoas**.

   ![Selecionar pessoas](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![Filtro de intervalo de datas](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre o uso do filtro de intervalo de datas, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se você não definiu o filtro Equipe, adicione o filtro Equipe e selecione cada equipe cujos dados você deseja ver.

   Para obter mais informações sobre como adicionar filtros na Análise aprimorada, consulte [Aplicar filtros na análise aprimorada](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Depois de adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois de sair da página ou do Workfront.

1. Na visualização Capacidade do recurso, clique em uma equipe para ver mais informações.

   A visualização Capacidade da equipe é exibida.

   Para obter mais informações sobre a visualização Capacidade do recurso, consulte [Exibir a visualização Capacidade do recurso na Análise aprimorada](../enhanced-analytics/resource-capacity-overview.md).

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização para o início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas e um filtro de período é criado.

   ![Filtro de cronograma](assets/timeframe-filter-350x220.png)

1. Passe o mouse sobre um ponto da linha do gráfico para ver as horas programadas e as horas planejadas para uma determinada data, bem como a porcentagem de capacidade e se a equipe inicial estava acima, abaixo ou na capacidade no momento.

   ![Pop-up de capacidade da equipe](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Opcional) Para exportar os dados de visualização, clique no link **Exportar** ícone ![Ícone Exportar](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * Gráfico (PNG)
   * Tabela de dados (XSLX)

