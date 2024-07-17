---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Índice de Desempenho de Agendamento (SPI)
description: O Índice de Desempenho de Cronograma (SPI) descreve a relação entre o cronograma planejado e o cronograma real.
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Calcular Índice de Desempenho de Agendamento (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

O Índice de Desempenho de Cronograma (SPI) descreve a relação entre o cronograma planejado e o cronograma real. O Adobe Workfront calcula a SPI nos níveis de projeto e tarefa. Os gerentes de projeto analisam essa métrica para identificar se as tarefas ou os projetos estão atualmente rastreando antes ou depois do cronograma.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Exibir acesso a Projetos e Dados Financeiros</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir ou permissões mais altas para o projeto com permissões para Exibir Finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Visão geral do Índice de desempenho de cronograma (SPI)

* [O que o valor SPI mostra](#what-the-spi-value-shows)
* [Como o Workfront calcula a SPI](#how-workfront-calculates-spi)

### O que o valor SPI mostra {#what-the-spi-value-shows}

Os gerentes de projeto entendem que um valor de SPI de 1 significa que o projeto está no plano ou dentro da programação.  Valores maiores que 1 indicam que um projeto está adiantado em relação ao cronograma e valores menores que 1 significam que um projeto está atrasado.  Quanto mais distante de 1, maior o desvio em relação ao plano.

| **Valor SPI** | **Indicação de &quot;Na Programação&quot;** |
|---|---|
| 1 | Planejado ou programado |
| > 1 (maior que 1) | Antes do agendamento |
| &lt; 1 (menos de 1) | Fora do cronograma |

{style="table-layout:auto"}

### Como o Workfront calcula a SPI  {#how-workfront-calculates-spi}

O Workfront calcula o SPI pela seguinte fórmula:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Se as Horas Planejadas Programadas até o Momento = 0, SPI = 1*.

O Agendamento de Horas Planejadas até a Data é calculado no minuto em que você executa os cálculos. Ela mostra o número de Horas Planejadas planejadas até a data atual. Ele pode ser recalculado automaticamente quando você altera os dados financeiros para que sejam precisos. Não há um campo no Workfront que indique esse valor.

Por exemplo, se você tiver um projeto com 1 tarefa e a tarefa tiver 10 horas planejadas e uma Duração de 10 dias, o Cronograma de Horas Planejadas para Data no 5º dia será 5. 

## Localizar SPI em um projeto ou tarefa

1. Vá para o projeto ou tarefa em que deseja exibir a SPI.
1. Dependendo de você querer ou não exibir a SPI em um projeto ou em uma tarefa, execute um dos seguintes procedimentos:

   1. Clique em **Detalhes do projeto** no painel esquerdo e exiba a área **Finanças**.

   1. Clique em **Detalhes da tarefa** no painel esquerdo e exiba a área **Finanças**.

      ![](assets/spi-on-project-nwe.png)

1. Localize o campo **CPI/ SPI/ CSI**.
