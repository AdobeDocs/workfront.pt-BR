---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Estimativa no Término (EAC)
description: Como métrica de desempenho, a EAC (Estimativa no término) representa o custo total projetado de seu projeto ou tarefa quando ela é concluída.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# Calcular Estimativa no Término (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Como métrica de desempenho, a EAC (Estimativa no término) representa o custo total projetado de seu projeto ou tarefa quando ela é concluída.

Como configuração, permite definir como o valor de EAC deve ser calculado. 

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
   <td> <p>Exibir acesso a Projetos e Dados Financeiros</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir ou permissões mais altas para o projeto com permissões para Exibir Finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Definir como calcular EAC

Como parte das preferências do sistema do projeto, o administrador do Adobe Workfront pode definir como calcular o EAC. A EAC pode ser calculada de uma das duas formas seguintes:

* [Calcular no nível do projeto](#calculate-at-the-project-level)
* [Extrair de tarefas e subtarefas](#roll-up-from-tasks-and-subtasks)

Para obter mais informações sobre como configurar as preferências do projeto no Workfront, incluindo como calcular a Estimativa no Término, consulte [Configurar as preferências do projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Como gerente de projeto, você também pode alterar essa preferência no nível do projeto, na subguia Finanças do projeto. Para obter mais informações sobre como editar a subguia Finanças de um projeto, consulte [Gerenciar informações na área Finanças do projeto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calcular no nível do projeto {#calculate-at-the-project-level}

A EAC da tarefa-pai e do projeto é determinada informando as horas reais/custo de mão de obra real nas Fórmulas da EAC. Esse cálculo inclui Horas Reais/custos e despesas adicionadas diretamente à tarefa ou ao projeto principal.

### Extrair de tarefas e subtarefas {#roll-up-from-tasks-and-subtasks}

A EAC da tarefa pai e do projeto é determinada pela soma da EAC de cada tarefa filho. Esse cálculo exclui Horas Reais/custos e despesas adicionadas diretamente à tarefa ou ao projeto principal.

## Como calcular o EAC com base no Método de Índice de Desempenho (PIM)

No Workfront, o cálculo de EAC depende do Método de índice de desempenho (PIM) selecionado do projeto. Para obter mais informações sobre como configurar o PIM para o seu sistema ou projeto, consulte [Definir o PIM (Método de Índice de Desempenho)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calcular EAC usando PIM baseado em Hora](#calculate-eac-using-hour-based-pim)
* [Calcular EAC usando PIM baseado em custo](#calculate-eac-using-cost-based-pim)

### Calcular EAC usando PIM baseado em horas {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Se o Índice de Desempenho de Custo [Calcular o Índice de Desempenho de Custo (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Total de Horas Planejadas + Horas Efetivas. Isso ocorre quando as horas foram capturadas, mas o projeto/tarefa está em 0% concluído.

Para obter mais informações sobre o cálculo da CPI, consulte [Calcular Índice de Desempenho de Custo (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Calcular EAC usando PIM baseado em custo {#calculate-eac-using-cost-based-pim}

A EAC de um projeto é calculada usando a seguinte fórmula:

```
EAC = EAC Labor + EAC Expense 
```

<pre>Mão de obra EAC =  <em>SE</em> Mão-de-Obra CPI &lt;&gt; 0 ENTÃO Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado / Mão-de-Obra CPI</pre><pre><em>MAIS</em> EAC  Mão-de-Obra = Custo de Mão-de-Obra Planejado + Custo de Mão-de-Obra Efetivo</pre><pre>CPI Mão-de-Obra = SE Custo Real do Trabalho &lt;&gt; 0 ENTÃO CPI Mão-de-Obra = TotalBudgetedCostWorkPerformed / Custo Real do Trabalho</pre><pre>SENÃO Mão de obra CPI = 1 </pre>Os seguintes campos são considerados ao calcular o EAC:

* Custo Total Orçado Trabalho Realizado (COTR) = O resultado da multiplicação do custo orçado do trabalho planejado (custo orçado) e o percentual da tarefa que foi concluída até o momento.

  Para obter informações sobre o BCWP (Trabalho de Custo Orçado Realizado), consulte [Calcular BCWP (Trabalho de Custo Orçado Realizado)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Para uma tarefa que não seja pai:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **Para uma tarefa pai:**
Total de Trabalho de Custo Orçado Executado = a soma do campo Total de Trabalho de Custo Orçado Executado para todas as tarefas filho diretas.

   * **Para um projeto:**
Total de Trabalho de Custo Orçado Executado = a soma do campo Total de Trabalho de Custo Orçado Executado para todas as tarefas de nível superior (tarefas pai e independente). 

* Despesa EAC = o resultado da adição do Custo Efetivo de Despesas Incorrido ao Custo de Despesas Planejadas Não Incorrido. É calculada pela seguinte fórmula:

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Custo Efetivo de Despesas Incorrido = A soma do campo Valor Planejado para todas as despesas em que o campo Valor Efetivo > 0. Por exemplo, se você criar uma despesa para a Tarefa 1 e informar $500,00 no campo Quantia Planejada e uma quantia > 0 no campo Quantia Real (isto é, $600,00), o Custo de Despesa Planejada Incorrido para esta tarefa será de $500,00.
   * Despesa Planejada Não Incorrida = A soma do campo Quantia Planejada para todas as despesas onde o campo Quantia Real = 0. Por exemplo, se você criar duas despesas para a Tarefa 1, onde para a primeira despesa o valor no campo Quantia Planejada é de US$500,00 e o valor no campo Quantia Real é de US$600,00, e para a segunda despesa, o valor no campo Quantia Planejada é de US$300,00 e o valor do campo Quantia Real é de US$0,00, o valor da Despesa Planejada Não Incorrida para essa tarefa é de US$300,00. 

## Localizar o EAC em um projeto ou tarefa

1. Vá para o projeto ou tarefa em que deseja exibir o EAC.
1. Expanda **Detalhes do projeto** ou **Detalhes das tarefas** no painel esquerdo do projeto ou da tarefa, dependendo de onde você exibir o EAC.

1. Clique em **Finanças**. 

   O valor EAC é exibido no campo **Estimativa na Conclusão**.

   ![](assets/eac-highlighted-on-project-350x112.png)
