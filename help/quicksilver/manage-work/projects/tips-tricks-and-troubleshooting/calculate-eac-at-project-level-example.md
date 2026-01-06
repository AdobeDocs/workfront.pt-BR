---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemplo de cálculo - calcular EAC no nível do projeto
description: Este artigo fornece um exemplo de cálculo da EAC (Estimativa no término) de um projeto no nível do projeto no Adobe Workfront.
author: Lisa
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '2213'
ht-degree: 1%

---

# Exemplo de cálculo - calcular EAC no nível do projeto

## Método EAC: calcular no nível do projeto

* [PIM = Baseado em Hora](#pim-hour-based)
* [PIM= Baseado em Custo](#pim-cost-based)

### PIM = Baseado em Hora {#pim-hour-based}

* [Exemplo simples: o projeto não tem tarefas filhas](#simple-example-project-has-no-children-tasks)
* [Exemplo complicado: o projeto tem tarefas filhas](#complicated-example-project-has-children-tasks)

#### Exemplo simples: o projeto não tem tarefas filhas {#simple-example-project-has-no-children-tasks}

PIM = Baseado em Hora

Método EAC = Calcular no nível do projeto **&#x200B;**

1. Crie o Projeto A com três tarefas (sem tarefas-filho), todas atribuídas ao Usuário 1 cujo custo/hr é de US$100,00.
1. Adicione horas planejadas e reais a cada tarefa e % concluídas de acordo com a tabela abaixo:

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>Tarefa</strong></p></th>
      <th><br><p><strong>Horas planejadas</strong></p></th>
      <th><br><p><strong>Hrs atuais</strong></p></th>
      <th><p><strong>% concluído</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>Tarefa 1</p></td>
      <td><p>5 horas</p></td>
      <td><p>25 horas</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>Tarefa 2</p></td>
      <td><p>10 horas</p></td>
      <td><p>25 horas</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>Tarefa 3</p></td>
      <td><p>15 horas</p></td>
      <td><p>25 horas</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. Recalcular Finanças no projeto.
1. A **CPI para a Tarefa 1** = 0,04 é calculada da seguinte forma:\
   **CPI para Tarefa 1** = *IF* Horas Reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Atual Hours\
   *ELSE* CPI = 1\
   **CPI da Tarefa 1** = 1 / 25\
   **CPI para Tarefa 1** = .04

1. **EAC para a Tarefa 1** = 125 horas calculado da seguinte maneira:\
   **EAC para Tarefa 1** = *IF* CPI &lt;> 0 *THEN* EAC = Horas Planejadas/CPI\
   *ELSE* EAC = Horas Planejadas + Horas Efetivas\
   **EAC para Tarefa 1** = 5 / .04\
   **EAC para Tarefa 1** = 125 horas&#x200B;**&#x200B;**

1. CPI / EAC para Tarefas 2 e 3 são:\
   Tarefa 2 = 0,12 / 83,33 horas\
   Tarefa 3 = 0,24 / 62,5 horas

1. **CPI para Projeto** = .13 calculado da seguinte maneira:\
   **CPI do Projeto** = *IF* Horas Reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Atual Hours\
   *ELSE* CPI = 1\
   **CPI do Projeto** = 10 / 75\
   **CPI para Projeto** = .13

1. **EAC para Projeto** = 225 horas calculado da seguinte forma:\
   **EAC para Projeto** = *IF* CPI &lt;> 0 *THEN* EAC = Planned Hours/CPI\
   *ELSE* EAC = Horas Planejadas + Horas Efetivas\
   **EAC para Projeto** = 30 / 0,13333\
   **EAC para Projeto** = 225 horas

#### Exemplo complicado: o projeto tem tarefas filhas {#complicated-example-project-has-children-tasks}

PIM = Baseado em Hora

Método EAC = Calcular no nível do projeto

1. Crie o Projeto A com seis tarefas em que a Tarefa 3 é a principal das Tarefas 4 e 5 e a Tarefa 1 é a principal das Tarefas 2 e 3 conforme mostrado abaixo:\
   Tarefa 1\
   Tarefa 2\
   Tarefa 3\
   Tarefa 4\
   Tarefa 5\
   Tarefa 6

1. Atribua as Tarefas 2, 4, 5 e 6 ao Usuário 1 cuja taxa de custo/hora é de US$100,00.
1. Adicione as horas planejadas/reais de cada tarefa e o % concluído de acordo com a tabela abaixo.

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

1. Adicione 50 horas diretamente ao projeto (Mais>Horas>Registrar horas).
1. A **CPI da Tarefa 2** = .1 é calculada da seguinte maneira:\
   **CPI para Tarefa 2** = *IF* Horas Reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Atual Hours\
   *ELSE* CPI = 1\
   **CPI da Tarefa 2** = 1 / 10\
   **CPI para Tarefa 2** = .1

1. **EAC para a Tarefa 2** = 50 horas calculado da seguinte maneira:\
   **EAC para Tarefa 2** = *IF* CPI &lt;> 0 *THEN* EAC = Horas Planejadas/CPI\
   *ELSE* EAC = Horas Planejadas + Horas Efetivas\
   **EAC para Tarefa 2** = 5 / .1\
   **EAC para Tarefa 2** = 50 horas

1. A CPI/EAC para as tarefas 4, 5 e 6 são as seguintes:\
   Tarefa 4: 0,4 / 25 horas\
   Tarefa 5: 0,75 / 20 horas\
   Tarefa 6: 1,2 / 16,67 horas

1. A **CPI da Tarefa 3** = 0,38 é calculada da seguinte maneira:\
   **CPI da Tarefa 3** = *IF* Horas Reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Atual Hours\
   *ELSE* CPI = 1\
   **CPI da Tarefa 3** = 11.5 / 30\
   **CPI para Tarefa 3** = .38

1. **EAC para Tarefa 3** = 65,22 horas calculado da seguinte forma:\
   **EAC para Tarefa 3** = *IF* CPI &lt;> 0 *THEN* EAC = Horas Planejadas/CPI\
   *ELSE* EAC = Horas Planejadas + Horas Efetivas\
   **EAC para Tarefa 3** = 25 / 0,383333\
   **EAC para Tarefa 3** = 65,22 horas

1. A **CPI da Tarefa 1** = 0,25 é calculada da seguinte maneira:\
   **CPI para Tarefa 1** = *IF* Horas Reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Atual Hours\
   *ELSE* CPI = 1\
   **CPI da Tarefa 1** = 12,5 / 50\
   **CPI para Tarefa 1** = .25

1. **EAC para a Tarefa 1** = 120 horas calculado da seguinte maneira:\
   **EAC para Tarefa 1** = *IF* CPI &lt;> 0 *THEN* EAC = Horas Planejadas / CPI\
   *ELSE* EAC = Horas Planejadas + Horas Efetivas\
   **EAC para Tarefa 1** = 30/.25\
   **EAC para Tarefa 1** = 120 horas

1. **CPI para Projeto** = .22 calculado da seguinte maneira:\
   **CPI do Projeto** = *IF* Horas Reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Atual Hours\
   *ELSE* CPI = 1\
   **CPI do Projeto** = 24.5 / 110\
   **CPI para Projeto** = .22272\
   **CPI para Projeto** = .22

1. **EAC para Projeto** = 224,49 horas calculado da seguinte forma:\
   **EAC para Projeto** = *IF* CPI &lt;> 0 *THEN* EAC = Planned Hours/CPI\
   *ELSE* EAC = Horas Planejadas + Horas Efetivas\
   **EAC para Projeto** = 50 / .22272\
   **EAC para Projeto** = 224,49 horas

### PIM= Baseado em Custo {#pim-cost-based}

* [Exemplo simples: o projeto não tem tarefas filhas](#simple-example-project-has-no-children-tasks)
* [Exemplo complicado: o projeto tem tarefas filhas](#complicated-example-project-has-children-tasks)

#### Exemplo simples: o projeto não tem tarefas filhas {#simple-example-project-has-no-children-tasks-1}

PIM = Baseado em Custo

Método EAC = Calcular no nível do projeto

1. Crie o Projeto A com três tarefas (sem tarefas-filho), todas atribuídas ao Usuário 1 cujo custo/hr é de US$100,00.
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
   <td> <p> $ 2.700,00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Em Ações do Projeto, execute Recalcular Finanças
1. **CPI para Tarefa 1** = .14
1. A **CPI**&#x200B;**&#x200B; para a Tarefa 1** = .14 é calculada da seguinte maneira:\
   **CPI** **para Tarefa 1** = *IF* Custo Real do Trabalho + IncurredAtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**&#x200B; para Tarefa 1** = (100+300) / (2500+400)\
     **CPI** **para Tarefa 1** = 400 / 2900\
     **CPI** **para Tarefa 1** = .14&#x200B;**&#x200B;**

1. **EAC**&#x200B;**para a Tarefa 1** = $13.400,00\
   **Mão-de-Obra CPI** **para a Tarefa 1** = SE o Custo Efetivo do Trabalho &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **Mão-de-Obra CPI** **para a Tarefa 1** = 100/2500\
   **Mão-de-Obra CPI** **para a Tarefa 1** = .04&#x200B;**&#x200B;**&#x200B;**Mão-de-Obra EAC &#x200B;**&#x200B;**para a Tarefa 1**=* IF *CPI_Labor &lt;> 0* THEN *Mão-de-Obra EAC = Custo de Trabalho Planejado/CPI_Labor
   * ELSE* Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado + Custo de Mão-de-Obra Efetivo\
     **Mão-de-Obra EAC**&#x200B;**&#x200B; para a Tarefa 1** = 500.00/.04\
     **Mão-de-Obra EAC**&#x200B;**&#x200B; para a Tarefa 1** = $12.500,00\
     **Despesa EAC**&#x200B;**&#x200B; para a Tarefa 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
     **Despesa EAC***para a Tarefa 1** = $400,00 + $500,00\
     **Despesa EAC***para a Tarefa 1** = $900,00\
     **EAC**&#x200B;**para a Tarefa 1** = Mão-de-Obra EAC + Despesa EAC\
     **EAC**&#x200B;**para a Tarefa 1** = $12.500,00 + $900,00\
     **EAC**&#x200B;**para a Tarefa 1** = $13.400,00

1. Estes são os valores de CPI/EAC para a Tarefa 2 e a Tarefa 3:\
   Tarefa 2 = 0,19 / US$ 8.433,33\
   Tarefa 3 = 0,44 / US$ 6.950,00

1. **CPI para Projeto** = .32 calculado da seguinte maneira:\
   **CPI*** para Projeto** = *IF* Custo Real do Trabalho + IncurredAtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI*** para Projeto** = (1000 + 2300) / (7500 + 2700)\
     **CPI*** para Projeto** = 3300 / 10200\
     **CPI*** para Projeto** = .32

1. **EAC para Projeto** = $28.200,00 calculado da seguinte forma:\
   **Mão-de-Obra CPI***para o Projeto** = SE Custo Efetivo do Trabalho &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **Mão de obra CPI***para o Projeto** = 1000 / 7500\
   **Trabalho CPI***para o Projeto** = .13333\
   **Mão-de-Obra CPI***para o Projeto** = .13

   **Mão-de-Obra EAC**&#x200B;**para o Projeto** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   * ELSE* Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado + Custo de Mão-de-Obra Efetivo\
     **Mão-de-Obra EAC**&#x200B;**&#x200B; para o Projeto** = 3000/ .13333\
     **Mão-de-Obra EAC*** para o Projeto** = $22.500,00

   **Despesa EAC***Projeto** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **Despesa EAC***Projeto** = $3000,00 + 2.700,00\
   **Despesa EAC***Projeto** = US$ 5.700,00

   **EAC**&#x200B;**Projeto** = Mão-de-Obra EAC + Despesa EAC\
   **EAC**&#x200B;**Projeto** = $22.500,00 + $5.700,00\
   **EAC**&#x200B;**Projeto** = $28.200,00

#### Exemplo complicado: o projeto tem tarefas filhas {#complicated-example-project-has-children-tasks-1}

PIM = Baseado em Custo

Método EAC = Calcular no nível do projeto

1. Crie o Projeto A com seis tarefas em que a Tarefa 3 é a principal das Tarefas 4 e 5 e a Tarefa 1 é a principal das Tarefas 2 e 3 conforme mostrado abaixo:\
   Tarefa 1\
   Tarefa 2\
   Tarefa 3\
   Tarefa 4\
   Tarefa 5\
   Tarefa 6

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
   <td> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>$ 1.500,00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 6</p> </td> 
   <td> <p>20 horas</p> </td> 
   <td> <p>$ 2.000,00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Adicione 50 horas diretamente ao projeto (Mais>Horas>Registre as horas) para que haja US$ 5.000,00 do custo real do trabalho registrado diretamente no projeto. **&#x200B;**
1. Adicione despesas a cada tarefa de acordo com a tabela abaixo (adicionei uma linha em branco entre cada tarefa para facilitar a leitura):

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
   <td> <p>-$400,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>Tarefa 1 Despesa 2</p> </td> 
   <td> <p>-$500,00</p> </td> 
   <td> <p>$ 800,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>Tarefa 1 Despesa 3</p> </td> 
   <td> <p>$ 400,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Despesa 1</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>$ 700,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Exp 2</p> </td> 
   <td> <p>-$400,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Despesa 3</p> </td> 
   <td> <p>-$200,00</p> </td> 
   <td> <p>$ 600,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Despesa 4</p> </td> 
   <td> <p>$ 700,00</p> </td> 
   <td> <p>-$200,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> <p>Tarefa 3 Exp</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4</p> </td> 
   <td> <p>Tarefa 4 Exp 1</p> </td> 
   <td> <p>$ 800,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4</p> </td> 
   <td> <p>Tarefa 4 Exp 2</p> </td> 
   <td> <p>-$100,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4 </p> </td> 
   <td> <p>Tarefa 4 Exp 3</p> </td> 
   <td> <p>-200,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>Tarefa 5 Exp 1</p> </td> 
   <td> <p>$ 700,00</p> </td> 
   <td> <p>$ 800,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>Tarefa 5 Exp 2</p> </td> 
   <td> <p>-$100,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>Tarefa 5 Exp 3</p> </td> 
   <td> <p>-$400,00</p> </td> 
   <td> <p>-$200,00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 6</p> </td> 
   <td> <p>Tarefa 6 Exp 1</p> </td> 
   <td> <p>$ 600,00</p> </td> 
   <td> <p>$ 700,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 6</p> </td> 
   <td> <p>Tarefa 6 Exp 2</p> </td> 
   <td> <p>$ 500,00</p> </td> 
   <td> <p>-$300,0</p> </td> 
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
   <td> <p> $ 0,00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Com base nos valores acima, os Custos Incorridos/Não Incorridos são determinados da seguinte forma:

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
   <td> <p>$ 400,00</p> </td> 
   <td> <p>-$500,00</p> </td> 
   <td> <p>$ 800,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>-$400,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
   <td> <p>$ 1.300,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4</p> </td> 
   <td> <p>$ 600,00</p> </td> 
   <td> <p>-$100,00</p> </td> 
   <td> <p>$ 300,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 600,00</p> </td> 
   <td> <p>$ 1.100,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 6</p> </td> 
   <td> <p>$ 0,00</p> </td> 
   <td> <p>$ 600,00</p> </td> 
   <td> <p>$ 700,00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>$ 2.500,00</p> </td> 
   <td> <p>$ 1.000,00</p> </td> 
   <td> <p>$ 1.500,00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Em Ações do Projeto, execute Recalcular Finanças
1. A **CPI** para a Tarefa 2 = .17 é calculada da seguinte maneira:\
   **Tarefa CPI 2** = *IF* Custo de Trabalho Real + IncurredAtualExpenseCost &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (AtualLaborCost + IncurredAtualExpenseCost)
   * ELSE* CPI = CPI_Labor\
     **CPI***Tarefa 2** = (100+300) / (1000+1300)\
     **CPI**&#x200B;**Tarefa 2** = 400 / 2300\
     **CPI**&#x200B;**Tarefa 2** = .17

1. **EAC** para a Tarefa 2 = $5.900,00\
   **Mão-de-Obra CPI***Tarefa 2** = SE Custo Efetivo do Trabalho &lt;> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / Custo Efetivo do Trabalho\
   ELSE CPI_Labor = 1\
   **Mão de obra CPI***Tarefa 2** = 100/1000\
   **Mão-de-Obra CPI***Tarefa 2** = .1

   **Mão-de-Obra EAC**&#x200B;**Tarefa 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   * ELSE* Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado + Custo de Mão-de-Obra Efetivo\
     **Mão-de-Obra EAC***Tarefa 2** = 500.00/.1\
     **Mão-de-Obra EAC**&#x200B;**Tarefa 2** = $5.000,00 **&#x200B;**&#x200B;**&#x200B; Despesa EAC &#x200B;**&#x200B;**Tarefa 2 &#x200B;**= IncurredActualExpenseCost + NotIncurredPlannedExpense\
     **Despesa EAC &#x200B;**&#x200B;**Tarefa 2** = US$ 1.300,00 + - US$ 400,00\
     **Despesa EAC***Tarefa 2** = $900,00

   **EAC**&#x200B;**Tarefa 2** = Mão-de-Obra EAC + Despesa EAC\
   **EAC**&#x200B;**Tarefa 2** = US$ 5.000,00 + US$ 900,00\
   **EAC**&#x200B;**Tarefa 2** = US$ 5.900,00

1. A CPI/EAC para as Tarefas 4, 5 e 6 é determinada da mesma forma, portanto, fornecerei esses valores abaixo:\
   Tarefa 4: 0,23 / US$ 3.400,00\
   Tarefa 5: 0,64 / US$ 3.100,00\
   Tarefa 6: 1,06 / US$ 2.366,67

1. CPI para Tarefa 3 = 0,31 calculado da seguinte maneira:\
   **CPI**&#x200B;**Tarefa 3** = *IF* Custo Real do Trabalho + IncurredAtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**Tarefa 3** = (1.150 + 500) / (3000 + 2400)\
     **CPI**&#x200B;**Tarefa 3** = 1650 / 5400\
     **CPI**&#x200B;**Tarefa 3** = .31 **&#x200B;**&#x200B;**&#x200B; EAC para a Tarefa 3 &#x200B;**= $9.521,74 calculado da seguinte maneira:\
     **Mão-de-Obra CPI &#x200B;**&#x200B;**Tarefa 3** = SE Custo Real do Trabalho &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **Mão de obra CPI***Tarefa 3** = 1150/3000\
   **Mão de obra CPI***Tarefa 3** = .383333\
   **Mão-de-Obra CPI***Tarefa 3** = .38

   **Mão-de-Obra EAC**&#x200B;**Tarefa 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado + Custo de Mão-de-Obra Efetivo\
     **Mão-de-Obra EAC**&#x200B;**Tarefa 3** = $2.500,00 / .383333\
     **Mão-de-Obra EAC**&#x200B;**Tarefa 3** = US$ 6.521,74

   **Despesa EAC***Tarefa 3** = IncurredAtualExpenseCost + NotIncurredPlannedExpense\
   **Despesa EAC***Tarefa 3** = $2.400,00 + $600,00\
   **Despesa EAC***Tarefa 3** = $3.000,00

   **EAC**&#x200B;**Tarefa 3** = Mão-de-Obra EAC + Despesa EAC\
   **EAC**&#x200B;**Tarefa 3** = US$ 6.521,74 + US$ 3.000,00\
   **EAC**&#x200B;**Tarefa 3** = US$ 9.521,74

1. CPI para Tarefa 1 = 0,16 calculado da seguinte maneira:\
   **CPI**&#x200B;**Tarefa 1** = *SE* Custo Real do Trabalho + IncurredAtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor\
     **CPI**&#x200B;**Tarefa 1** = (1250 + 300) / (5000 + 4500)\
     **CPI**&#x200B;**Tarefa 1** = 1550 / 9500=\
     **CPI**&#x200B;**Tarefa 1** = .16

1. A EAC para a Tarefa 1 é de US$ 17.100,00 calculado da seguinte maneira:\
   **Mão-de-Obra CPI***Tarefa 1** = SE Custo Real do Trabalho &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **Mão de obra CPI***Tarefa 1** = 1250 / 5000\
   **Mão-de-Obra CPI***Tarefa 1** = .25

   **Mão-de-Obra EAC**&#x200B;**Tarefa 1** = *IF* CPI_Labor &lt;> 0 *THEN* Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado / CPI_Labor
   * ELSE* Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado + Custo de Mão-de-Obra Efetivo\
     **Mão-de-Obra EAC**&#x200B;**Tarefa 1** = US$ 3.000,00 / 0,25\
     **Mão-de-Obra EAC***Tarefa 1** = $12.000,00

   **Despesa EAC***Tarefa 1** = IncurredAtualExpenseCost + NotIncurredPlannedExpense\
   **Despesa EAC***Tarefa 1** = US$ 4.500 + 600\
   **Despesa EAC***Tarefa 1** = US$ 5.100,00

   **EAC**&#x200B;**Tarefa 1** = Mão-de-Obra EAC + Despesa EAC\
   **EAC**&#x200B;**Tarefa 1** = $12.000,00 + 5.100,00\
   **EAC**&#x200B;**Tarefa 1** = $17.100,00

1. CPI para Projeto é .25\
   **CPI*** para Projeto** = *IF* Custo Real do Trabalho + IncurredAtualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   * ELSE* CPI = CPI_Labor

   **CPI*** para Projeto** = (2450 + 1900) / (11000 + 6700)\
   **CPI*** para Projeto** =   4350/17700\
   **CPI*** para Projeto** = .25

1. **EAC para Projeto** = $32.248,98 calculado da seguinte forma:\
   **Mão-de-Obra CPI***para o Projeto** = SE Custo Efetivo do Trabalho &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **Mão de obra CPI***para o Projeto** = 2450 / 11000\
   **Mão de obra CPI***para o Projeto** = .22272\
   **Mão-de-Obra CPI***para o Projeto** = .22

   **Mão-de-Obra EAC**&#x200B;**para o Projeto** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   * ELSE* Mão-de-Obra EAC = Custo de Mão-de-Obra Planejado + Custo de Mão-de-Obra Efetivo\
     **Mão de obra EAC**&#x200B;**&#x200B; para o Projeto** = $5.000,00 / .22272\
     **Mão de obra EAC**&#x200B;**&#x200B; para o Projeto** = $22.448.97959\
     **Mão de obra EAC**&#x200B;**&#x200B; para o Projeto** = $22.448,98

   **Despesa EAC**&#x200B;**Projeto** = IncurredAtualExpenseCost + NotIncurredPlannedExpense\
   **Despesa EAC***Projeto** = US$ 3.100,00 + US$ 6.700,00\
   **Despesa EAC***Projeto** = $9.800,00

   **EAC**&#x200B;**Projeto** = Mão-de-Obra EAC + Despesa EAC\
   **EAC**&#x200B;**Projeto** = $22.448,98 + 9.800,00\
   **EAC**&#x200B;**Projeto** = $32.248,98
