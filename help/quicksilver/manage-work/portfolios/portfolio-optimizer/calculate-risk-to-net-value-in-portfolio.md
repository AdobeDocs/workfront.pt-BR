---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Calcular o risco ao valor líquido de um portfólio
description: No Portfolio Otimizer, o indicador [!UICONTROL Risco para o valor líquido] mede o Risco potencial levando em conta o Valor líquido fornecido por todos os projetos exibidos no Portfolio Otimizer.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 5%

---

# Calcular o [!UICONTROL Risco de Valor Líquido] em um portfólio

No [!UICONTROL Portfolio Otimizer], o indicador [!UICONTROL Risco de Valor Líquido] mede o Risco Potencial levando em consideração o [!UICONTROL Valor Líquido] fornecido por todos os projetos exibidos no [!UICONTROL Portfolio Otimizer].

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
