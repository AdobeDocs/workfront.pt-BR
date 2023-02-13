---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Visão geral da pontuação do Portfolio Otimizer
description: Você pode encontrar a pontuação do Portfolio Otimizer no Portfolio Otimizer. Ele é exibido no [!UICONTROL Pontuação] para cada projeto. Isso representa uma pontuação para cada projeto no portfólio.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 4451b1a3-57ae-4c66-a6a1-a85bd51a1648
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 1%

---

# Visão geral da [!UICONTROL Portfolio Otimizer] Pontuação

Você pode encontrar a variável [!UICONTROL Portfolio Otimizer] na [!UICONTROL Portfolio Otimizer]. Ele é exibido no **[!UICONTROL Pontuação]** para cada projeto. Isso representa uma pontuação para cada projeto no portfólio.

Para obter informações sobre como localizar a variável [!UICONTROL Portfolio Otimizer], consulte o artigo [[!UICONTROL Portfolio Otimizer] visão geral](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

Para obter informações sobre como [!DNL Adobe Workfront] O usa a Pontuação do projeto e outras informações do projeto para otimizar projetos na [!UICONTROL Portfolio Otimizer], consulte [Otimizar projetos no Portfolio Otimizer](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

## Diferença entre [!UICONTROL Pontuação de alinhamento] e [!UICONTROL Pontuação de otimização de Portfolio]

Há uma diferença entre a pontuação de alinhamento e a pontuação do otimizador de portfólio de um projeto.

A pontuação de alinhamento de um projeto é calculada com base nos pontos obtidos após a conclusão do scorecard. Essa pontuação é então usada para determinar a pontuação de alinhamento do portfólio. A pontuação de alinhamento é exibida como uma porcentagem.\
A pontuação de alinhamento de um projeto é exibida na **[!UICONTROL Alinhamento]** da coluna [!UICONTROL Portfolio Otimizer] ou na [!UICONTROL Alinhamento] do [!UICONTROL Resumo do caso de negócios].

![](assets/business-case-summary-aligned-field-highlighted.png)

![](assets/project-alignment-score-portfolio-optimizer-highlighted-350x174.png)

Para obter mais informações sobre como gerar a pontuação de alinhamento de um projeto, consulte o artigo [Aplicar um scorecard a um projeto e gerar uma Pontuação de alinhamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

O [!UICONTROL otimizador de portfólio] é uma classificação calculada automaticamente no [!UICONTROL Portfolio Otimizer] segundo as quais os projetos podem ser priorizados. A pontuação do otimizador de portfólio é exibida como um ícone de indicador acompanhado por um número e é exibida no **[!UICONTROL Pontuação]** da coluna [!UICONTROL Portfolio Otimizer].

>[!NOTE]
>
>Um projeto pode ser pontuado na variável [!UICONTROL Portfolio Otimizer] somente se o Business Case tiver sido concluído. Para obter mais informações sobre como concluir um Caso de negócios, consulte o artigo [[!UICONTROL Criar um caso de negócios] para um projeto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

![](assets/portfolio-optimizer-project-score-highlighted-350x132.png)

A pontuação para cada projeto é calculada com base na importância das seguintes categorias:

* [!UICONTROL Custo]
* [!UICONTROL Alinhamento]
* [!UICONTROL Valor líquido]
* [!UICONTROL Risco para benefício]
* [!UICONTROL ROI]

## Calcule o [!UICONTROL Portfolio Otimizer] Pontuação

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This was edited based on this issue, per Anna: https://hub.workfront.com/issue/603d0c58000095ea0bc00ce5e2110693/overview)</p>
-->

[!DNL Workfront] produz uma pontuação usando o [!UICONTROL Portfolio Otimizer] que é um ranking para auxiliar na priorização de projetos. Os valores no portfólio se baseiam em valores inseridos nos casos de negócios dos projetos e são usados para calcular uma pontuação para o projeto. Os projetos com uma pontuação mais elevada podem ser considerados de maior importância e podem ser priorizados para serem concluídos primeiro.

Para descobrir a classificação de um projeto, faça o seguinte:

1. Vá para o [!UICONTROL Portfolio Otimizer].
1. Passe o mouse sobre o ícone de classificação para ver a pontuação do otimizador de portfólio para um projeto.

![ranking_icon_in_portfólio_otimizer_new.png](assets/ranking-icon-in-portfolio-optimizer-new-350x160.png)

O algoritmo para calcular as pontuações leva em consideração os valores descritos nos Casos de negócios dos projetos e os pesos que eles carregam. Ele fornece a cada projeto no otimizador uma pontuação e normaliza essa pontuação para que haja sempre um projeto com uma pontuação de 100. Isso dá uma pontuação alta ao melhor projeto.

**Exemplo:** Por exemplo, se você fizer [!UICONTROL alinhamento superior] o único fator a ser considerado, o projeto com o alinhamento mais alto obtém a pontuação de 100.

A seguir estão os critérios pelos quais você pode pontuar um projeto:

* [!UICONTROL Custo]
* [!UICONTROL Alinhamento]
* [!UICONTROL Valor]
* [!UICONTROL Risco para benefício]
* [!UICONTROL ROI]

![](assets/optimizer-sliding-value-options-350x77.png)

Para obter informações sobre como otimizar projetos no portfólio, consulte [Otimize projetos na [!UICONTROL Portfolio Otimizer]](../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).

Cada critério no painel de configuração ([!UICONTROL Custo], [!UICONTROL Alinhamento], [!UICONTROL ROI], [!UICONTROL Valor líquido], [!UICONTROL Risco para benefício]) recebem seus pesos no intervalo de 0 a 100 com base no que você selecionou.

Para cada projeto com um caso comercial completo, uma pontuação por critério é gerada usando a seguinte fórmula:

```
Score Per Criteria = (Project Value For The Criteria - AVG(all the project values for this criteria)) / Standard Deviation of that value for that project
```

**Exemplo:** Para o [!UICONTROL Pontuação de alinhamento] para o Projeto A, você terá o seguinte:

```
Alignment Score = (Project A Alignment Score - AVG (of all the project Alignments)) / Standard Deviation of alignment score for that project
```

Assim que tiver tudo [!UICONTROL Pontuação por critério] calculada, você pode adicioná-las levando em conta seus pesos para obter a pontuação completa por projeto. A pontuação do projeto é calculada usando a seguinte fórmula:

```
Score = Cost Score * Cost Weight + Alignment Score * Alignment Weight + ROI Score * ROI Weight + Net Value Score * Net Value Weight + Risk Score * Risk Weight
```

Para o custo do projeto e [!UICONTROL risco] a lógica funciona de forma inversa à maneira como os outros critérios funcionam: se desejar [!UICONTROL Custo baixo] para ser importante para você, não vai aumentar mas diminuir a pontuação geral do projeto por `Cost Score * Cost Weight`.

Depois que você tiver pontuações calculadas para cada projeto, a variável [!UICONTROL Pontuação de otimização] é definida para os projetos da seguinte forma:

1. [!UICONTROL Mínimo] e [!UICONTROL Máximo] as pontuações são definidas.
1. O intervalo entre esses valores é calculado.
1. Para cada projeto, a variável [!UICONTROL Pontuação de otimização] é calculada usando a seguinte fórmula:

   ```
   Optimization Score = Rounded ((Score - Minimum / Range)*100)
   ```
