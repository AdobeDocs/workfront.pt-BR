---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Índice de Desempenho de Custo (CPI)
description: O Índice de Desempenho de Custo (CPI) descreve a relação no nível do projeto ou da tarefa entre o custo planejado e o custo real. Os Gerentes de projeto revisam essa métrica para identificar tarefas ou projetos que atualmente rastreiam o custo abaixo ou acima de um ponto específico.
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Calcular Índice de Desempenho de Custo (CPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

O Índice de Desempenho de Custo (CPI) descreve a relação no nível do projeto ou da tarefa entre o custo planejado e o custo real. Os Gerentes de projeto revisam essa métrica para identificar tarefas ou projetos que atualmente rastreiam o custo abaixo ou acima de um ponto específico. O custo pode ser medido em horas ou dólares, dependendo do seu Método de Índice de Desempenho (PIM). Para obter mais informações sobre como configurar o Método de Índice de Desempenho, consulte [Definir o PIM (Performance Index Method)](../../../manage-work/projects/project-finances/set-pim.md).

Somente organizações que exigem entrada de tempo podem usar a CPI. Além disso, os valores PIM baseados em custos são precisos apenas em organizações que têm taxas de custo definidas para os destinatários da tarefa (funções de trabalho ou usuários).

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
   <td> <p>Exibir acesso a Projetos e Dados Financeiros</p> <p> Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões mais altas para o projeto com permissões para Exibir Finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Visão Geral do Índice de Desempenho de Custo (CPI)

* [O valor da IPC](#the-cpi-value)
* [Como a IPC é calculada](#how-cpi-is-calculated)

### O valor da IPC {#the-cpi-value}

Os gerentes de projeto entendem que um valor de IPC de 1 significa que o projeto está exatamente no orçamento. Os valores maiores que 1 indicam que um projeto está sob orçamento (menos horas ou despesas foram registradas do que o planejado originalmente) e os valores menores que 1 significam que um projeto está acima do orçamento (mais horas ou despesas foram registradas do que o planejado originalmente). Mais de 1, maior desvio em relação ao plano.

| **Valor de CPI** | **Indicação sobre o orçamento** |
|---|---|
| 1 | Em plano ou orçamento |
| > 1 (maior que 1) | Orçamento |
| &lt; 1 (menos de 1) | Orçamento excedente |


### Como a IPC é calculada {#how-cpi-is-calculated}

No Adobe Workfront, o cálculo da CPI depende do Método de Índice de Desempenho selecionado para o projeto. Para obter mais informações sobre como configurar o Método de Índice de Desempenho, consulte [Definir o PIM (Performance Index Method)](../../../manage-work/projects/project-finances/set-pim.md).

* [Cálculos de CPI ao usar o PIM baseado em hora](#cpi-calculations-when-using-hour-based-pim)
* [Cálculos de CPI ao usar o PIM baseado em custo](#cpi-calculations-when-using-cost-based-pim)

#### Cálculos de CPI ao usar o PIM baseado em hora {#cpi-calculations-when-using-hour-based-pim}

Se

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Caso contrário

```
CPI = 1
```

* **Para uma tarefa não pai:**

   ```
   Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
   ```

* **Para uma tarefa pai:**
Custo Total Orçado Trabalho Executado = a soma do campo Custo Total Orçado Trabalho Executado para todas as tarefas-filho diretas.

* **Para um projeto:**
Custo Total Orçado Trabalho Executado = a soma do campo Custo Total Orçado Trabalho Executado para todas as tarefas de nível superior (pais e tarefas independentes).

Para obter informações sobre o Custo Total do Trabalho Desenvolvido em Orçamento (BCWP), consulte [Calcular Custo Orçamentado Trabalho Executado (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### Cálculos de CPI ao usar o PIM baseado em custo {#cpi-calculations-when-using-cost-based-pim}

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

Os campos neste cálculo são descritos abaixo:

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Despesa Incorrido é a despesa na qual o Custo Real > 0

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* O Custo Planejado do Trabalho Executado é calculado pela seguinte fórmula:

   ```
   Planned Cost of Work Performed = Planned cost * Percent Complete / 100
   ```

O Custo Total Orçado do Trabalho Executado é calculado para o seguinte:

* **Para uma tarefa não pai:**

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

Você pode exibir o CPI de um projeto ou de uma tarefa em um projeto, uma lista de tarefas ou um relatório. Além disso, é possível exibi-la no nível do projeto ou da tarefa.

1. Vá para o projeto ou tarefa onde deseja exibir a CPI.
1. Expandir **Detalhes do projeto** ou **Detalhes da tarefa** no painel esquerdo, dependendo se você está visualizando a CPI de um projeto ou tarefa.

1. Clique em **Finanças**.

   O CPI é exibido na **IPC/ IPC/ IPC/** campo.

   ![](assets/cpi-on-project-nwe.png)
