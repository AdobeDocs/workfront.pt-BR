---
title: Visualização da capacidade do grupo na Análise aprimorada
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: A visualização da capacidade da equipe mostra a quantidade total de capacidade que uma equipe inicial tem, se está com alocação excessiva ou com alocação insuficiente, e a dinâmica da capacidade ao longo do tempo.
author: Nolan
feature: Reports and Dashboards
exl-id: cfeb1a87-01be-4088-9e33-53a97e3871ad
source-git-commit: 1b1f3c22b8112cfde5b10bef39076eed11630d0f
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Visualização da capacidade do grupo na Análise aprimorada

A visualização da capacidade da equipe mostra a quantidade total de capacidade que uma equipe inicial tem, se está com alocação excessiva ou com alocação insuficiente, e a dinâmica da capacidade ao longo do tempo.

![](assets/team-capacity-350x110.png)

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

## Entender a visualização da capacidade do grupo

A Visualização da capacidade do grupo exibe o volume de trabalho atribuído à equipe inicial em um determinado dia.

* **Burnout**: Quando a cor de preenchimento azul mais escura estiver acima da linha pontilhada, a equipe inicial terá mais horas de trabalho atribuídas a ela do que pode ser concluída no número de horas em que a equipe está disponível para trabalhar. Isso indica que a equipe está sobrealocada e pode estar se aproximando do esgotamento.

   ![](assets/team-capacity-over-capacity.png)

* **Não contestado**: Quando a cor de preenchimento azul mais escura estiver abaixo da linha pontilhada, a equipe inicial terá mais horas disponíveis para trabalhar do que a quantidade de trabalho atribuída a ela. Isso indica que a equipe está sub-alocada e pode não ser contestada.

   ![](assets/team-capacity-under-capacity.png)

* **Saldo**: Quando a cor de preenchimento azul mais clara ou transparente estiver logo acima, logo abaixo ou na linha pontilhada, a equipe residencial tem uma quantidade de horas de trabalho atribuídas a ela e deve ser capaz de concluir dentro do horário de trabalho disponível. Isso indica que a carga de trabalho da equipe é mais equilibrada.

   ![](assets/team-capacity-at-capacity.png)

Passar o mouse sobre qualquer ponto da visualização mostra os seguintes detalhes de um determinado dia:

* **Horas programadas**: Esse é o número de horas de trabalho planejadas que a equipe precisa concluir.
* **Horas disponíveis**: Esse é o número de horas de trabalho que a equipe está disponível para trabalhar.
* **Capacidade**: Além de uma porcentagem de capacidade, também são exibidas as designações Em capacidade, Em capacidade ou Em excesso de capacidade.

Ver essas informações ajuda a determinar:

* Quando a equipe de origem foi atribuída em excesso ou subalocada.
* Se a equipe de origem for objeto de uma atribuição excessiva ou de uma subatribuição diária.
* Qual é a consistência da carga de trabalho de uma equipe doméstica de dia para dia.
* Se você estiver criando problemas de capacidade com o novo trabalho.

Para saber como obter os melhores dados para essa visualização, consulte [Visão geral da análise aprimorada](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualizar a capacidade do grupo

1. Clique no ícone do Menu principal ![](assets/main-menu-icon-16x12.png), em seguida selecione **Analytics**.
1. No painel esquerdo, selecione **Pessoas**.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Opcional) Para usar um intervalo de datas diferente, selecione novas datas de início e término no filtro de intervalo de datas.

   ![](assets/filters-select-date-range-350x344.png)

   Para obter informações sobre como usar o filtro de intervalo de datas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Condicional) Se você não definiu seu filtro Equipe , adicione o filtro Equipe e selecione cada equipe para a qual deseja visualizar os dados.

   Para obter mais informações sobre como adicionar filtros nas Análises aprimoradas, consulte [Aplicar filtros no Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Após adicionar filtros, os dados de até 50 projetos são exibidos e os filtros permanecem ativos mesmo depois que você sai da página ou faz logoff do Workfront.

1. Na Visualização da capacidade do recurso, clique em uma equipe para ver mais informações.

   A Visualização da capacidade do grupo é exibida.

   Para obter mais informações sobre a visualização da capacidade do recurso, consulte [Visualizar a Visualização da capacidade dos recursos no Enhanced Analytics](../enhanced-analytics/resource-capacity-overview.md).

1. (Opcional) Para ampliar um intervalo de datas, selecione um ponto na visualização do início do intervalo de datas e arraste até o final do intervalo de datas.

   Todas as outras visualizações são atualizadas para o mesmo intervalo de datas, e um filtro de período é criado.

   ![](assets/timeframe-filter-350x220.png)

1. Passe o mouse sobre um ponto na linha em gráfico para ver as horas programadas e as horas planejadas para a data especificada, bem como a porcentagem de capacidade e se a equipe inicial estava sobre, abaixo ou na capacidade no momento.

   ![](assets/team-capacity-capacity-pop-up-350x351.png)

1. (Opcional) Para exportar os dados de visualização, clique no botão **Ícone Exportar** ![](assets/export.png) no canto superior direito da visualização, selecione o formato de exportação:

   * **Gráfico (PNG)**
   * **Tabela de dados (XSLX)**

