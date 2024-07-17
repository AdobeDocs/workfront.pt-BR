---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcular o Risco de Valor Líquido em um portfólio
description: No Otimizador de Portfolio, o indicador [!UICONTROL Risco para o valor líquido] mede o Risco potencial levando em conta o Valor líquido fornecido por todos os projetos exibidos no Otimizador de Portfolio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Calcular o [!UICONTROL Risco de Valor Líquido] em um portfólio

No [!UICONTROL Otimizador de Portfolio], o indicador [!UICONTROL Risco para o Valor Líquido] mede o Risco Potencial levando em consideração o [!UICONTROL Valor Líquido] fornecido por todos os projetos exibidos no [!UICONTROL Otimizador de Portfolio]. 

Para obter a maior eficiência do portfólio, verifique se o indicador [!UICONTROL Risco] é baixo e o indicador [!UICONTROL Valor Líquido] é alto. 

Os indicadores [!UICONTROL Risco] e [!UICONTROL Valor Líquido] são representados da perspectiva de como se relacionam entre si.

[!DNL Adobe Workfront] calcula os indicadores [!UICONTROL Risco] e [!UICONTROL Valor Líquido] usando as seguintes fórmulas:

* O indicador [!UICONTROL Risco] é calculado pela seguinte fórmula:

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* O indicador [!DNL Net Value] é calculado pelas seguintes fórmulas:

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  Ou

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>O indicador [!UICONTROL Risco para o valor líquido] é calculado com base nos projetos exibidos no [!UICONTROL Portfolio Otimizer] e não em todos os projetos associados ao portfólio. 
