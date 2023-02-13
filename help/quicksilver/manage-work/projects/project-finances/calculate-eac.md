---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Calcular Estimativa na Conclusão (EAC)
description: Como métrica de desempenho, a Estimativa na conclusão (EAC) representa o custo total projetado do seu projeto ou tarefa quando é concluída.
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Calcular Estimativa na Conclusão (EAC)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Como métrica de desempenho, a Estimativa na conclusão (EAC) representa o custo total projetado do seu projeto ou tarefa quando é concluída.

Como configuração, permite definir como o valor EAC deve ser calculado. 

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
   <td> <p>Exibir acesso a Projetos e Dados Financeiros</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões mais altas para o projeto com permissões para Exibir Finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Definir como calcular EAC

Como parte das preferências do sistema do projeto, o administrador do Adobe Workfront pode definir como calcular o EAC. O EAC pode ser calculado de uma das duas formas seguintes:

* [Calcular no nível do projeto](#calculate-at-the-project-level)
* [Rolar de tarefas e subtarefas](#roll-up-from-tasks-and-subtasks)

Para obter mais informações sobre como configurar preferências de projeto no Workfront, incluindo como calcular a Estimativa na conclusão, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Como gerente de projeto, também é possível alterar essa preferência no nível do projeto, na subguia Finanças do projeto. Para obter mais informações sobre como editar a subguia Finanças de um projeto, consulte [Gerenciar informações na área de finanças do projeto](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Calcular no nível do projeto {#calculate-at-the-project-level}

O EAC para a tarefa-pai e o projeto são determinados inserindo as horas reais/custo real da mão de obra nas Fórmulas EAC. Esse cálculo inclui Horas/custos e despesas reais adicionados diretamente à tarefa pai ou ao projeto.

### Rolar de tarefas e subtarefas {#roll-up-from-tasks-and-subtasks}

EAC para a tarefa pai e o projeto são determinados pela soma do EAC para cada tarefa filho. Esse cálculo exclui Horas/custos e despesas reais adicionados diretamente à tarefa-pai ou ao projeto.

## Como calcular EAC com base no Método de Índice de Desempenho (PIM)

No Workfront, o cálculo para EAC depende do Método de Índice de Desempenho (PIM) selecionado do projeto. Para obter mais informações sobre como configurar o PIM para seu sistema ou para seu projeto, consulte [Definir o PIM (Performance Index Method)](../../../manage-work/projects/project-finances/set-pim.md).

* [Calcular EAC usando o PIM baseado em hora](#calculate-eac-using-hour-based-pim)
* [Calcular EAC usando PIM baseado em custo](#calculate-eac-using-cost-based-pim)

### Calcular EAC usando o PIM baseado em hora {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Se o Índice de Desempenho de Custo [Calcular Índice de Desempenho de Custo (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = Total de Horas Planejadas + Horas Reais. Isso ocorre quando as horas são capturadas, mas o projeto/tarefa está 0% concluído.

Para obter mais informações sobre o cálculo de CPI, consulte [Calcular Índice de Desempenho de Custo (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Calcular EAC usando PIM baseado em custo {#calculate-eac-using-cost-based-pim}

O EAC de um projeto é calculado usando a seguinte fórmula:

```
EAC = EAC Labor + EAC Expense 
```

<pre>Trabalho EAC =  <em>IF</em> Mão de obra do IPC &lt;&gt; 0 ENTÃO Mão de obra EAC = Custo da Mão de obra planejada/IPC Mão de obra</pre><pre><em>ELSE</em> EAC Mão de obra = Custo Planejado da Mão de obra + Custo Real da Mão de obra</pre><pre>Mão-de-Obra IPC = Custo Real da Mão-de-Obra IF &lt;&gt; 0 ENTÃO Mão-de-Obra IPC = TotalBudgetedCostWorkPerformance / Custo Real da Mão-de-Obra</pre><pre>Mão de obra da CPI ELSE = 1 </pre>Os seguintes campos são considerados ao calcular o EAC:

* Custo Total do Trabalho Orçamentado Executado (BCWP) = Resultado da multiplicação do custo orçamentado do trabalho planejado (custo orçado) e a porcentagem da tarefa que foi concluída até agora.

   Para obter informações sobre o Custo Total do Trabalho Desenvolvido em Orçamento (BCWP), consulte [Calcular Custo Orçamentado Trabalho Executado (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **Para uma tarefa não pai:**

      ```
      Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
      ```

   * **Para uma tarefa pai:**
Custo Total Orçado Trabalho Executado = a soma do campo Custo Total Orçado Trabalho Executado para todas as tarefas-filho diretas.

   * **Para um projeto:**
Custo Total Orçado Trabalho Executado = a soma do campo Custo Total Orçado Trabalho Executado para todas as tarefas de nível superior (pais e tarefas independentes). 

* Despesa EAC = o resultado da adição do Custo de Despesa Real Incorrido ao Custo de Despesa Planejada Não Incorrido. É calculada pela seguinte fórmula:

   ```
   EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
   ```

   * Custo de Despesa Real Incorrido = A soma do campo Quantia Planejada para todas as despesas em que o campo Quantia Real > 0. Por exemplo, se você criar uma despesa para a Tarefa 1 e inserir $500.00 no campo Quantia Planejada e uma quantia > 0 no campo Quantia Real (ou seja, $600,00), o Custo de Despesa Planejada Incorrido para esta tarefa é de $500,00.
   * Despesa Planejada Não Incorrido = A soma do campo Quantia Planejada para todas as despesas em que o campo Quantia Real = 0. Por exemplo, se você criar duas despesas para a Tarefa 1, onde para a primeira despesa o valor no campo Quantia Planejada é $500,00 e o valor na Quantia Real é $600,00 e para a segunda despesa, o valor no campo Quantia Planejada é $300,00 e o valor do campo Quantia Real é $0,00, o valor do A Despesa Planejada Não Assegurada para esta tarefa é de $300,00. 

## Localize o EAC em um projeto ou tarefa

1. Vá para o projeto ou tarefa onde deseja exibir o EAC.
1. Expandir **Detalhes do projeto** ou **Detalhes das tarefas** no painel esquerdo do projeto ou da tarefa, dependendo de onde você visualiza o EAC.

1. Clique em **Finanças**. 

   O valor EAC é exibido no **Estimativa na conclusão** campo.

   ![](assets/eac-highlighted-on-project-350x112.png)
