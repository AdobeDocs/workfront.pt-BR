---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcular o risco para o valor líquido em um portfólio
description: No Portfolio Otimizer, a variável [!UICONTROL Risco para o valor líquido] O indicador mede o Risco potencial levando em conta o Valor Líquido fornecido por todos os projetos exibidos no Portfolio Otimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Calcule o [!UICONTROL Risco para o valor líquido] em um portfólio

No [!UICONTROL Portfolio Otimizer], o [!UICONTROL Risco para o valor líquido] O indicador mede o Risco Potencial tendo em consideração a [!UICONTROL Valor líquido] fornecidos por todos os projetos exibidos no [!UICONTROL Portfolio Otimizer]. 

Para obter a maior eficiência no portfólio, você quer ver que a variável [!UICONTROL Risco] estiver baixo e o indicador [!UICONTROL Valor líquido] O indicador está alto. 

O [!UICONTROL Risco] e [!UICONTROL Valor líquido] os indicadores são representados na perspectiva de como se relacionam entre si.

[!DNL Adobe Workfront] calcula o [!UICONTROL Risco] e [!UICONTROL Valor líquido] indicadores que usam as seguintes fórmulas:

* O [!UICONTROL Risco] é calculado pela seguinte fórmula:

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* O [!DNL Net Value] O indicador é calculado pelas seguintes fórmulas:

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   Ou

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>O [!UICONTROL Risco para o valor líquido] O indicador é calculado com base nos projetos exibidos no [!UICONTROL Portfolio Otimizer], e não em todos os projetos associados ao portfólio. 
