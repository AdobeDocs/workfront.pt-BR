---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular o Índice de Desempenho da Programação (SPI)
description: O Índice de Desempenho de Programação (SPI) descreve a relação entre a programação planejada e a programação real.
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# Calcular o Índice de Desempenho da Programação (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

O Índice de Desempenho de Programação (SPI) descreve a relação entre a programação planejada e a programação real. O Adobe Workfront calcula o SPI nos níveis do projeto e da tarefa. Os gerentes de projeto revisam essa métrica para identificar se as tarefas ou os projetos estão rastreando com antecedência ou atrás da programação.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Exibir acesso a Projetos e Dados Financeiros</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões mais altas para o projeto com permissões para Exibir Finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Visão geral do Índice de desempenho de agendamento (SPI)

* [O que o valor de SPI mostra](#what-the-spi-value-shows)
* [Como a Workfront calcula o SPI](#how-workfront-calculates-spi)

### O que o valor de SPI mostra {#what-the-spi-value-shows}

Os gerentes de projeto entendem que um valor de SPI de 1 significa que o projeto está no plano ou no agendamento.  Valores maiores que 1 indicam que um projeto está adiantado da programação, e valores menores que 1 significam que um projeto está atrasado na programação.  Mais de 1, maior desvio em relação ao plano.

| **Valor de SPI** | **Indicação de &quot;Em Horário&quot;** |
|---|---|
| 1 | Em plano ou programado |
| > 1 (maior que 1) | Antes do horário |
| &lt; 1 (menos de 1) | Programação atrasada |

{style=&quot;table-layout:auto&quot;}

### Como a Workfront calcula o SPI  {#how-workfront-calculates-spi}

O Workfront calcula o SPI de acordo com a seguinte fórmula:

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;Se as Horas Planejadas Estiverem Programadas para Data = 0, SPI = 1*.

Programação de Horas Planejadas até a Data são calculadas no minuto em que você executa os cálculos. Ele mostra o número de Horas Planejadas planejadas para a data atual. Ele pode ser recalculado automaticamente quando você altera seus dados financeiros para serem precisos. Não há nenhum campo no Workfront que indique esse valor.

Por exemplo, se você tiver um projeto com 1 tarefa e a tarefa tiver 10 horas planejadas e uma Duração de 10 dias, a Programação de Horas Planejadas até a Data no 5º dia será 5. 

## Localizar SPI em um projeto ou tarefa

1. Vá para o projeto ou tarefa onde deseja exibir o SPI.
1. Dependendo de você deseja exibir o SPI em um projeto ou uma tarefa, execute um dos seguintes procedimentos:

   1. Clique em **Detalhes do projeto** no painel esquerdo, em seguida, visualize o **Finanças** área.

   1. Clique em **Detalhes da tarefa** no painel esquerdo, em seguida, visualize o **Finanças** área.

      ![](assets/spi-on-project-nwe.png)

1. Encontre a **IPC/ IPC/ IPC/** campo.
