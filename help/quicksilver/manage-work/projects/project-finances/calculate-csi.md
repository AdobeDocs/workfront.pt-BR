---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular CSI (Cost Schedule Performance Index, Índice de Desempenho da Programação de Custo)
description: O Índice de Desempenho da Programação de Custo (CSI) é um cálculo automático que combina o Índice de Desempenho de Custo (CPI) e o Índice de Desempenho da Programação (SPI) em uma métrica geral que equilibra custo e programação.
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Calcular CSI (Cost Schedule Performance Index, Índice de Desempenho da Programação de Custo)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Visão Geral do Índice de Desempenho da Programação de Custos (CSI)

O Índice de Desempenho da Programação de Custo (CSI) é um cálculo automático que combina o Índice de Desempenho de Custo (CPI) e o Índice de Desempenho da Programação (SPI) em uma métrica geral que equilibra custo e programação. Ao multiplicar esses valores, uma única métrica pode contabilizar uma programação prolongada em um orçamento menor ou vice-versa. Os gerentes de projeto podem usar isso para determinar a integridade geral do projeto ou da tarefa quando o custo é sacrificado para direcionar a programação no meio do projeto.

>[!TIP]
>
>A Adobe Workfront calcula o CSI para tarefas e projetos. A Workfront não calcula um valor CSI para problemas.

Você pode se beneficiar das informações fornecidas por essa métrica somente se o seguinte existir em sua organização:

* Seus usuários estão registrando o tempo para o trabalho que concluem.\
   Isso calcula o CSI com base em Horas.
* Seus usuários ou funções de trabalho têm taxas de Custo por Hora associadas a eles. 

   Isso calcula o CSI com base em Custos.

## Como a Workfront calcula o Índice de Desempenho da Programação de Custo (CSI)

O Workfront calcula o Índice de Desempenho de Custo (CSI) de um projeto ou tarefa usando a seguinte fórmula:

```
CSI = CPI x SPI
```

Para obter informações sobre a CPI, consulte o artigo [Calcular Índice de Desempenho de Custo (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Para obter informações sobre SPI, consulte o artigo [Calcular o Índice de Desempenho da Programação (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

O CSI tem os três valores possíveis a seguir:

* 1 = Segue o plano geral   
* 
   >1 = Combinação de programação de suborçamento
* &lt;1 = Combinação de programação de orçamento excedente

![](assets/csi-highlighted.png)

## Localize o Índice de Desempenho da Programação de Custo (CSI)

>[!CAUTION]
>
>Você deve ter acesso a Exibir dados financeiros em seu Nível de acesso e permissões para Visualizar o projeto ou tarefa para poder ver o valor CSI de um projeto ou tarefa.

Você pode localizar o CSI nas seguintes áreas do Workfront:

* Área de finanças na seção Detalhes do projeto .
* Área de finanças na seção Detalhes da tarefa.
* Uma visualização de projeto ou tarefa
* Um relatório de projeto ou tarefa
