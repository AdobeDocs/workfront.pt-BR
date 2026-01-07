---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemplo de Cálculo - Calcular EAC como um Acúmulo a partir de Tarefas
description: Este artigo fornece um exemplo de cálculo da EAC (Estimativa no término) de um projeto como um acúmulo de todas as tarefas do projeto no Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 2%

---

# Exemplo de cálculo - Calcular EAC como um acúmulo a partir de tarefas

## Método EAC: acumular de tarefas ou subtarefas

* [PIM= Baseado em Hora](#pim-hour-based)
* [PIM= Baseado em Custo](#pim-cost-based)

### PIM= Baseado em Hora {#pim-hour-based}

* [Exemplo simples: o projeto não tem tarefas filhas](#simple-example-project-has-no-children-tasks)
* [Exemplo complicado: o projeto tem tarefas filhas](#complicated-example-project-has-children-tasks)

#### Exemplo simples: o projeto não tem tarefas filhas {#simple-example-project-has-no-children-tasks}

PIM = Baseado em Hora

Método EAC = Extrair de tarefas/subtarefas

1. Crie o Projeto A com três tarefas (sem tarefas-filho), todas atribuídas ao Usuário 1 cujo custo/hr é de US$100,00.
1. Adicione horas planejadas/reais a cada tarefa e % concluídas de acordo com a tabela abaixo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tarefa</strong> </p> </th> 
   <th> <br> <p><strong>Horas planejadas</strong> </p> </th> 
   <th> <br> <p><strong>Horas atuais</strong> </p> </th> 
   <th> <p><strong>% concluído</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Recalcular finanças
1. A **CPI para a Tarefa 1** = 0,04 é calculada da seguinte forma:\
   **CPI para Tarefa 1** = *IF* Horas Reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Atual Hours\
   *ELSE* CPI = 1\
   **CPI da Tarefa 1** = 1 / 25\
   **CPI para Tarefa 1** = .04

1. **EAC para a Tarefa 1** = 125 horas calculado da seguinte maneira:\
   **EAC para Tarefa 1** = *IF* CPI &lt;> 0 *THEN* EAC = Horas Planejadas/ CPI\
   *MAIS*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC para Tarefa 1** = 5 / .04\
   **EAC para Tarefa 1** = 125 horas

1. CPI / EAC para Tarefas 2 e 3 são:\
   Tarefa 2 = 0,12 / 83,33 horas\
   Tarefa 3 = 0,24 / 62,5 horas

1. **CPI para Projeto** = .13 calculado da seguinte maneira:\
   **CPI do Projeto** = *SE* Horas Efetivas > 0 *ENTÃO*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   **CPI do Projeto** = 10 / 75\
   **CPI para Projeto** = .13

1. **EAC para Projeto** = 270,83 horas calculado da seguinte forma\
   **EAC do Projeto** = Tarefa da EAC 1 + Tarefa da EAC 2 + Tarefa da EAC 3\
   **EAC para Projeto** = 125 + 83,33 + 62,5\
   **EAC para Projeto** = 270,83 horas

#### Exemplo complicado: o projeto tem tarefas filhas {#complicated-example-project-has-children-tasks}

PIM = Baseado em Hora

Método EAC = Extrair de tarefas/subtarefas

1. Crie o Projeto A com seis tarefas em que a Tarefa 3 é a principal das Tarefas 4 e 5 e a Tarefa 1 é a principal das Tarefas 2 e 3 conforme mostrado abaixo:

   ```
   Task 1  
      Task 2  
      Task 3  
         Task 4  
         Task 5  
   Task 6
   ```

1. Atribua as Tarefas 2, 4, 5 e 6 ao Usuário 1 cuja taxa de custo/hora é de US$100,00.
1. Adicione horas planejadas/reais de cada tarefa e % concluídas de acordo com a tabela abaixo.

   >[!NOTE]
   >
   >Para as Tarefas 1 e 3, você está adicionando apenas as horas reais.

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <thead> 
   <tr> 
      <th> <br> <p><strong>Tarefa</strong> </p> </th> 
      <th> <br> <p><strong>Horas planejadas</strong> </p> </th> 
      <th> <br> <p><strong>Horas atuais</strong> </p> </th> 
      <th> <p><strong>% concluído</strong> </p> </th> 
   </tr> 
   </thead> 
   <tbody> 
   <tr> 
      <td> <p>Tarefa 1</p> </td> 
      <td> </td> 
      <td> <p>10 horas</p> </td> 
      <td> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 2</p> </td> 
      <td> <p>5 horas</p> </td> 
      <td> <p>10 horas</p> </td> 
      <td> <p>20%</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 3</p> </td> 
      <td> </td> 
      <td> <p>10 horas</p> </td> 
      <td> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 4</p> </td> 
      <td> <p>10 horas</p> </td> 
      <td> <p>10 horas</p> </td> 
      <td> <p>40%</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 5</p> </td> 
      <td> <p>15 horas</p> </td> 
      <td> <p>10 horas</p> </td> 
      <td> <p>50%</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 6</p> </td> 
      <td> <p>20 horas</p> </td> 
      <td> <p>10 horas</p> </td> 
      <td> <p>60%</p> </td> 
   </tr> 
   </tbody> 
   </table>

1. Adicione 50 horas diretamente ao projeto (Mais>Horas>Registre as horas) para que haja US$ 5.000,00 do custo real do trabalho registrado diretamente no projeto.
1. Executar Recalcular Finanças
1. A **CPI da Tarefa 2** = .1 é calculada da seguinte maneira:\
   **CPI para Tarefa 2** = *IF* Horas Efetivas > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   **CPI da Tarefa 2** = 1 / 10\
   **CPI para Tarefa 2** = .1

1. **EAC para a Tarefa 2** = 50 horas calculado da seguinte maneira:\
   **EAC para Tarefa 2** = *IF* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

   *ELSE* EAC = Horas Planejadas + Horas Efetivas\
   **EAC para Tarefa 2** = 5 / .1\
   **EAC para Tarefa 2** = 50 horas

1. CPI / EAC para Tarefa 4, Tarefa 5 e Tarefa 6:\
   Tarefa 4 = 0,4 / 25 horas\
   Tarefa 5 = 0,75 / 20 horas\
   Tarefa 6 = 1,2 / 16,67 horas

1. **CPI para Tarefa 3** = .38\
   **CPI da Tarefa 3** = *IF* Horas Efetivas > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   **CPI da Tarefa 3** = 11.5 / 30\
   **CPI para Tarefa 3** = .38

1. **EAC para Tarefa 3** = Tarefa 4 da EAC + Tarefa 5 da EAC\
   **EAC para Tarefa 3** = 25 + 20\
   **EAC para Tarefa 3** = 45 horas

1. A **CPI da Tarefa 1** = 0,25 é calculada da seguinte maneira:\
   **CPI da Tarefa 1** = *SE* Horas Efetivas > 0 *ENTÃO*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   **CPI da Tarefa 1** = 12,5 / 50\
   **CPI para Tarefa 1** = .25

1. **EAC para Tarefa 1** = Tarefa 2 da EAC + Tarefa 3 da EAC\
   **EAC para Tarefa 1** = 50 + 45\
   **EAC para Tarefa 1** = 95 horas

1. CPI para Projeto = 0,22 calculado da seguinte forma:\
   **CPI do Projeto** = *SE* Horas Efetivas > 0 *ENTÃO*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   **CPI do Projeto** = 24.5 / 110\
   **CPI para Projeto** = .22272\
   **CPI para Projeto** = .22

1. **EAC do projeto** = Tarefa 1 da EAC + Tarefa 6 da EAC\
   **EAC para projeto** = 95 + 16,67\
   **EAC para projeto** = 111,67 horas

### PIM= Baseado em Custo {#pim-cost-based}

* [Exemplo simples: o projeto não tem tarefas filhas](#simple-example-project-has-no-children-tasks)

#### Exemplo simples: o projeto não tem tarefas filhas {#simple-example-project-has-no-children-tasks-1}

PIM = Baseado em Custo

Método EAC = Extrair de tarefas/subtarefas

1. Crie o Projeto A com três tarefas (sem tarefas filhas) todas atribuídas ao Usuário 1 cujo custo/hora seja de $100,00.
1. Adicione horas planejadas/reais a cada tarefa e % concluídas de acordo com a tabela abaixo:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <col> 
   <col> 
   <thead> 
   <tr> 
      <th> <br> <p><strong>Tarefa</strong> </p> </th> 
      <th> <br> <p><strong>Horas planejadas</strong> </p> </th> 
      <th> <br> <p><strong>Custo de Trab Planej</strong> </p> </th> 
      <th> <br> <p><strong>Horas atuais</strong> </p> </th> 
      <th> <br> <p><strong>Custo de Lbr da Lei</strong> </p> </th> 
      <th> <p><strong>% concluído</strong> </p> </th> 
   </tr> 
   </thead> 
   <tbody> 
   <tr> 
      <td> <p>Tarefa 1</p> </td> 
      <td> <p>5 horas</p> </td> 
      <td> <p>$ 500,00</p> </td> 
      <td> <p>25 horas</p> </td> 
      <td> <p>$ 2.500,00</p> </td> 
      <td> <p>20%</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 2</p> </td> 
      <td> <p>10 horas</p> </td> 
      <td> <p>$ 1.000,00</p> </td> 
      <td> <p>25 horas</p> </td> 
      <td> <p>$ 2.500,00</p> </td> 
      <td> <p>30%</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 3</p> </td> 
      <td> <p>15 horas</p> </td> 
      <td> <p>$ 1.500,00</p> </td> 
      <td> <p>25 horas</p> </td> 
      <td> <p>$ 2.500,00</p> </td> 
      <td> <p>40%</p> </td> 
   </tr> 
   </tbody> 
   </table>

1. Adicione despesas a cada tarefa de acordo com a tabela abaixo:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <thead> 
   <tr> 
      <th> <p><strong>Tarefa</strong> </p> </th> 
      <th> <p><strong>Despesa</strong> </p> </th> 
      <th> <p><strong>Valor Planejado</strong> </p> </th> 
      <th> <p><strong>Valor Efetivo</strong> </p> </th> 
   </tr> 
   </thead> 
   <tbody> 
   <tr> 
      <td> <p>Tarefa 1</p> </td> 
      <td> <p>Tarefa 1 Exp 1</p> </td> 
      <td> <p>$ 300,00</p> </td> 
      <td> <p>$ 400,00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 1</p> </td> 
      <td> <p>Tarefa 1 Despesa 2</p> </td> 
      <td> <p>$ 500,00</p> </td> 
      <td> <p>$ 0,00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 2</p> </td> 
      <td> <p>Tarefa 2 Exp</p> </td> 
      <td> <p>$ 200,00</p> </td> 
      <td> <p>$ 100,00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 3</p> </td> 
      <td> <p>Tarefa 3 Exp</p> </td> 
      <td> <p>$ 800,00</p> </td> 
      <td> <p>$ 700,00</p> </td> 
   </tr> 
   </tbody> 
   </table>

1. Adicione duas despesas ao projeto (ou seja, não vinculadas a uma tarefa) da seguinte maneira:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <thead> 
   <tr> 
      <th> <p><strong>Despesa</strong> </p> </th> 
      <th> <p><strong>Valor Planejado</strong> </p> </th> 
      <th> <p><strong>Valor Efetivo</strong> </p> </th> 
   </tr> 
   </thead> 
   <tbody> 
   <tr> 
      <td> <p>Despesa de Projeto 1</p> </td> 
      <td> <p>$ 1.000,00</p> </td> 
      <td> <p>$ 1.500,00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 1 Despesa 2</p> </td> 
      <td> <p>$ 2.500,00</p> </td> 
      <td> <p>$ 0,00</p> </td> 
   </tr> 
   </tbody> 
   </table>

1. Com base nos valores acima, os Custos Incorridos/ Não Incorridos são determinados da seguinte forma:

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <thead> 
   <tr> 
      <th> <p><strong>Tarefa</strong> </p> </th> 
      <th> <p><strong>Despesa Planejada Não Incorrida</strong> </p> </th> 
      <th> <p><strong>Despesa planejada incorrida</strong> </p> </th> 
      <th> <p><strong>Despesas Reais Incorridas</strong> </p> </th> 
   </tr> 
   </thead> 
   <tbody> 
   <tr> 
      <td> <p>Tarefa 1</p> </td> 
      <td> <p>$ 500,00</p> </td> 
      <td> <p>$ 300,00</p> </td> 
      <td> <p>$ 400,00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 2</p> </td> 
      <td> <p>$ 0,00</p> </td> 
      <td> <p>$ 200,00</p> </td> 
      <td> <p>$ 100,00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Tarefa 3</p> </td> 
      <td> <p>$ 0,00</p> </td> 
      <td> <p>$ 800,00</p> </td> 
      <td> <p>$ 700,00</p> </td> 
   </tr> 
   <tr> 
      <td> <p>Projeto</p> </td> 
      <td> <p>$ 3.000,00</p> </td> 
      <td> <p>$ 2.300,00</p> </td> 
      <td> <p>$ 2.700,00</p> </td> 
   </tr> 
   </tbody> 
   </table>

1. Em Ações do Projeto, execute Recalcular Finanças
1. A **CPI**&#x200B;**&#x200B; para a Tarefa 1** = .14 é calculada da seguinte maneira:\
   **CPI**&#x200B;**para a Tarefa 1** = *IF* Custo Real do Trabalho + IncurredAtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**&#x200B; para Tarefa 1** = (100+300) / (2500+400)\
     **CPI**&#x200B;**&#x200B; para a Tarefa 1** = 400 / 2900\
     **CPI**&#x200B;**para a Tarefa 1** = .14

1. **EAC**&#x200B;**para a Tarefa 1** = $13.400,00\
   **Mão-de-Obra CPI***para a Tarefa 1** = SE Custo Efetivo do Trabalho &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **Mão de obra CPI***para a Tarefa 1** = 100/2500\
   **Mão de obra CPI***para a Tarefa 1** = .04

   **Mão-de-Obra EAC**&#x200B;**para a Tarefa 1** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado + Custo de Mão-de-Obra Efetivo\
     **Mão-de-Obra EAC**&#x200B;**&#x200B; para a Tarefa 1** = 500.00/.04\
     **Mão-de-Obra EAC**&#x200B;**&#x200B; para a Tarefa 1** = $12.500,00

   **Despesa EAC**&#x200B;**&#x200B; para a Tarefa 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Despesa EAC***para a Tarefa 1** = $400,00 + $500,00\
   **Despesa EAC***para a Tarefa 1** = $900,00

   **EAC**&#x200B;**para a Tarefa 1** = Mão-de-Obra EAC + Despesa EAC\
   **EAC**&#x200B;**para a Tarefa 1** = $12.500,00 + $900,00\
   **EAC**&#x200B;**para a Tarefa 1** = $13.400,00

1. Estes são os valores de CPI/EAC para a Tarefa 2 e a Tarefa 3:\
   Tarefa 2 = 0,19 / US$ 8.433,33\
   Tarefa 3 = 0,44 / US$ 6.950,00&#x200B;**&#x200B;**

1. A CPI do projeto = 0,32\
   **CPI*** para Projeto** = *IF* Custo Real do Trabalho + IncurredAtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI*** para Projeto** = (1000 + 2300) / (7500 + 2700)\
     **CPI*** para Projeto** = 3300 / 10200\
     **CPI*** para Projeto** = .32

1. A EAC do projeto é de US$ 28.783,33\
   **EAC**&#x200B;**para o projeto** = Tarefa da EAC 1 + Tarefa da EAC 2 + Tarefa da EAC 3\
   **EAC**&#x200B;**para o Projeto** = $13.400,00 + $8.433,33 + $6.950,00\
   **EAC**&#x200B;**&#x200B; para Projeto** = $28.783,33
