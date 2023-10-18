---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o Índice de Desempenho de Tempo (CSI)
description: O Índice de Desempenho de Programação de Custo (CSI) é um cálculo automático que combina o Índice de Desempenho de Custo (CPI) e o Índice de Desempenho de Programação (SPI) em uma métrica geral que equilibra custo e programação.
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: 1cf679376517293f0e0f28b461bd9ecab9283035
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Calcular o Índice de Desempenho de Tempo (CSI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## Visão geral do Índice de Desempenho de Agendamento de Custo (CSI)

O Índice de Desempenho de Programação de Custo (CSI) é um cálculo automático que combina o Índice de Desempenho de Custo (CPI) e o Índice de Desempenho de Programação (SPI) em uma métrica geral que equilibra custo e programação. Ao multiplicar esses valores, uma única métrica pode contabilizar uma programação prolongada com um orçamento menor ou vice-versa. Os gerentes de projeto podem usar isso para determinar a integridade geral do projeto ou da tarefa quando o custo é sacrificado para gerar o cronograma no meio do projeto.

>[!TIP]
>
>A Adobe Workfront calcula o CSI para tarefas e projetos. A Workfront não calcula um valor de CSI para problemas.

Você pode se beneficiar das informações fornecidas por essa métrica somente se houver o seguinte em sua organização:

* Seus usuários estão registrando o tempo para o trabalho que concluíram.\
  Isso calcula o CSI com base em Horas.
* Seus usuários ou funções de trabalho têm taxas de Custo por hora associadas a eles. 

  Isso calcula o CSI com base nos custos.

## Como a Workfront calcula o Índice de desempenho de cronograma de custo (CSI)

O Workfront calcula o Índice de Desempenho de Custo (CSI) de um projeto ou tarefa usando a seguinte fórmula:

`CSI = CPI x SPI`

Para obter informações sobre a CPI, consulte o artigo [Calcular Índice de Desempenho de Custo (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

Para obter informações sobre SPI, consulte o artigo [Calcular Índice de Desempenho de Agendamento (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

O CSI tem três valores possíveis a seguir:

* 1 = Segue o plano geral
* \>1 = Combinação abaixo da programação orçamentária
* &lt;1 = Combinação de programação de orçamento excedido

![](assets/csi-highlighted.png)

## Localize o Índice de Desempenho de Agendamento de Custo (CSI)

>[!CAUTION]
>
>Você deve ter acesso a Exibir dados financeiros em seu Nível de acesso e permissões para Exibir o projeto ou a tarefa para poder ver o valor CSI de um projeto ou tarefa.

Você pode localizar o CSI nas seguintes áreas do Workfront:

* Área Financeira na seção Detalhes do Projeto.
* Área Financeira na seção Detalhes da Tarefa.
* Uma visualização de projeto ou tarefa
* Um relatório de projeto ou tarefa
