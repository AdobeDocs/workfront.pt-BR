---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Índice de Desempenho de Custo (CPI)
description: O Índice de Desempenho de Custo (CPI) descreve o relacionamento no nível do projeto ou da tarefa entre o custo planejado e o custo real. Os gerentes de projeto revisam essa métrica para identificar tarefas ou projetos que atualmente rastreiam com custo baixo ou acima em um determinado momento.
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Calcular Índice de Desempenho de Custo (CPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

O Índice de Desempenho de Custo (CPI) descreve o relacionamento no nível do projeto ou da tarefa entre o custo planejado e o custo real. Os gerentes de projeto revisam essa métrica para identificar tarefas ou projetos que atualmente rastreiam com custo baixo ou acima em um determinado momento. O custo pode ser medido em horas ou dólares, dependendo do seu Método de Índice de Desempenho (PIM). Para obter mais informações sobre como definir o Método de Índice de Desempenho, consulte [Definir o Método de Índice de Desempenho (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Somente organizações que exigem entrada de tempo podem usar CPI. Além disso, os valores do PIM com base no custo são precisos somente em organizações que definiram taxas de custo para os atribuídos da tarefa (funções de trabalho ou usuários).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Claro ou superior</p>
   <p>ou</p>
   <p>Atual: revisão ou superior</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Exibir acesso a Projetos e Dados Financeiros</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Exibir ou permissões mais altas para o projeto com permissões para Exibir Finanças</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visão Geral do Índice de Desempenho de Custo (CPI)

* [O valor da CPI](#the-cpi-value)
* [Como a CPI é calculada](#how-cpi-is-calculated)

### O valor CPI {#the-cpi-value}

Os gerentes de projeto entendem que um valor de CPI de 1 significa que o projeto está exatamente dentro do orçamento. Valores maiores que 1 indicam que um projeto está abaixo do orçamento (menos horas ou despesas foram registradas do que o planejado originalmente) e valores menores que 1 significam que um projeto está acima do orçamento (mais horas ou despesas foram registradas do que o planejado originalmente). Quanto mais distante de 1, maior o desvio em relação ao plano.

| **Valor CPI** | **Indicação no orçamento** |
|---|---|
| 1 | No plano ou orçamento |
| > 1 (maior que 1) | Abaixo do orçamento |
| &lt; 1 (menos de 1) | Acima do orçamento |


### Como a CPI é calculada {#how-cpi-is-calculated}

No Adobe Workfront, o cálculo da CPI depende do Método de índice de desempenho selecionado para o projeto. Para obter mais informações sobre como definir o Método de Índice de Desempenho, consulte [Definir o Método de Índice de Desempenho (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [Cálculos de CPI ao usar o PIM baseado em Horas](#cpi-calculations-when-using-hour-based-pim)
* [Cálculos de CPI ao usar PIM baseado em custo](#cpi-calculations-when-using-cost-based-pim)

#### Cálculos de CPI ao usar o PIM baseado em horas {#cpi-calculations-when-using-hour-based-pim}

Se

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Caso contrário

```
CPI = 1
```

* **Para uma tarefa que não seja pai:**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **Para uma tarefa pai:**
Total de Trabalho de Custo Orçado Executado = a soma do campo Total de Trabalho de Custo Orçado Executado para todas as tarefas filho diretas.

* **Para um projeto:**
Total de Trabalho de Custo Orçado Executado = a soma do campo Total de Trabalho de Custo Orçado Executado para todas as tarefas de nível superior (tarefas pai e independente).

Para obter informações sobre o BCWP (Trabalho de Custo Orçado Realizado), consulte [Calcular BCWP (Trabalho de Custo Orçado Realizado)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### Cálculos de CPI ao usar PIM baseado em custo {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

Se

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



Caso contrário

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

Os campos nesse cálculo estão descritos abaixo:

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Despesa Incorrida é a despesa na qual o Custo Efetivo > 0

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* O Custo Planejado do Trabalho Realizado é calculado pela seguinte fórmula:

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

O Trabalho de Custo Total Orçado Executado é calculado para o seguinte:

* **Para uma tarefa que não seja pai:**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **Para uma tarefa pai:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* **Para um projeto:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
  ```



## Localizar CPI em um projeto ou tarefa

Você pode exibir a CPI de um projeto ou de uma tarefa em um projeto ou em uma lista de tarefas ou relatório. Além disso, você pode visualizá-lo no nível do projeto ou da tarefa.

1. Vá para o projeto ou tarefa em que deseja exibir a CPI.
1. Expanda **Detalhes do projeto** ou **Detalhes da tarefa** no painel esquerdo, dependendo se você está visualizando a CPI de um projeto ou tarefa.

1. Clique em **Finanças**.

   A CPI é exibida no campo **CPI/ SPI/ CSI**.

   ![](assets/cpi-on-project-nwe.png)
