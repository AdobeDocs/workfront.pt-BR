---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemplo de cálculo - calcular EAC no Nível do Projeto
description: PIM = Baseado em Hora
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 9%

---

# Exemplo de cálculo - calcular EAC no Nível do Projeto

## Método EAC: Calcular no nível do projeto

* [PIM = Baseado em Hora](#pim-hour-based)
* [PIM= Baseado em Custo](#pim-cost-based)

### PIM = Baseado em Hora {#pim-hour-based}

* [Exemplo simples: projeto não tem tarefas filho](#simple-example-project-has-no-children-tasks)
* [Exemplo complicado: projeto tem tarefas filho](#complicated-example-project-has-children-tasks)

#### Exemplo simples: projeto não tem tarefas filho {#simple-example-project-has-no-children-tasks}

PIM = Baseado em Hora

Método EAC = Calcular no nível do projeto ****

1. Crie o Projeto A com três tarefas (sem tarefas filho) todas atribuídas ao Usuário 1, cujo custo/hora é US$ 100,00.
1. Adicione Horas Planejadas e Reais a cada tarefa e % Concluídas de acordo com a tabela abaixo:

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

1. Recalcular as finanças no projeto.
1. **IPC para a Tarefa 1** = 0,04 calculado da seguinte forma:\
   **IPC para a Tarefa 1** = *IF* Horas reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformance/Horas Reais\
      *ELSE* IPC = 1\
   **IPC para a Tarefa 1** = 1 / 25\
   **IPC para a Tarefa 1** = .04

1. **EAC para a Tarefa 1** = 125 horas, calculadas do seguinte modo:\
   **EAC para a Tarefa 1** = *IF* IPC &lt;> 0 *THEN* EAC = Horas/IPC Planejadas\
       *ELSE* EAC = Horas Planejadas + Horas Reais\
   **EAC para a Tarefa 1** = 5 / .04\
   **EAC para a Tarefa 1** = 125 horas***

1. O IPC / EAC para as Tarefas 2 e 3 são:\
   Tarefa 2 = 0,12 / 83,33 h\
   Tarefa 3 = 0,24 / 62,5 h

1. **CPI para projeto** = .13 calculado da seguinte forma:\
   **CPI para projeto** = *IF* Horas reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformance/Horas Reais\
       *ELSE* IPC = 1\
   **CPI para projeto** = 10 / 75\
   **CPI para projeto** = .13

1. **EAC para o Projeto** = 225 horas, calculadas do seguinte modo:\
   **EAC para o Projeto** = *IF* IPC &lt;> 0 *THEN* EAC = Horas/IPC Planejadas\
       *ELSE* EAC = Horas Planejadas + Horas Reais\
   **EAC para o Projeto** = 30 / .13333\
   **EAC para o Projeto** = 225 horas

#### Exemplo complicado: projeto tem tarefas filho {#complicated-example-project-has-children-tasks}

PIM = Baseado em Hora

Método EAC = Calcular no nível do projeto

1. Crie o Projeto A com seis tarefas, onde a Tarefa 3 é a responsável das Tarefas 4 e 5 e a Tarefa 1 é a responsável das Tarefas 2 e 3, conforme mostrado abaixo:\
   Tarefa 1\
      Tarefa 2\
      Tarefa 3\
         Tarefa 4\
         Tarefa 5\
   Tarefa 6

1. Atribua Tarefas 2, 4, 5 e 6 ao Usuário 1 cuja taxa de custo/hora é de $100,00.
1. Adicione horas planejadas/reais a cada tarefa e % Concluído de acordo com a tabela abaixo.

   >[!NOTE]
   >
   >Para as Tarefas 1 e 3, você só está adicionando horas reais.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Tarefa</strong> </p> </th> 
   <th> <br> <p><strong>Horas planejadas</strong> </p> </th> 
   <th> <br> <p><strong>Hrs atuais</strong> </p> </th> 
   <th> <p><strong>% Completo</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> </td> 
   <td> <p>10 Hrs</p> </td> 
   <td> </td> 
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

1. Adicione 50 horas diretamente ao projeto (Mais>Horas>Horas de Log).
1. **IPC para a Tarefa 2** = .1 calculado do seguinte modo:\
   **IPC para a Tarefa 2** = *IF* Horas reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformance/Horas Reais\
       *ELSE* IPC = 1\
   **IPC para a Tarefa 2** = 1 / 10\
   **IPC para a Tarefa 2** = .1

1. **EAC para a Tarefa 2** = 50 horas, calculadas do seguinte modo:\
   **EAC para a Tarefa 2** = *IF* IPC &lt;> 0 *THEN* EAC = Horas/IPC Planejadas\
       *ELSE* EAC = Horas Planejadas + Horas Reais\
   **EAC para a Tarefa 2** = 5 / .1\
   **EAC para a Tarefa 2** = 50 horas

1. O IPC / EAC para as Tarefas 4, 5 e 6 são os seguintes:\
   Tarefa 4: 0,4 / 25 horas\
   Tarefa 5: 0,75 / 20 horas\
   Tarefa 6: 1,2 / 16,67 h

1. **IPC para a Tarefa 3** = 0,38 calculado da seguinte forma:\
   **IPC para a Tarefa 3** = *IF* Horas reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformance/Horas Reais\
       *ELSE* IPC = 1\
   **IPC para a Tarefa 3** = 11,5 / 30\
   **IPC para a Tarefa 3** = .38

1. **EAC para a Tarefa 3** = 65,22 horas, calculadas do seguinte modo:\
   **EAC para a Tarefa 3** = *IF* IPC &lt;> 0 *THEN* EAC = Horas/IPC Planejadas\
       *ELSE* EAC = Horas Planejadas + Horas Reais\
   **EAC para a Tarefa 3** = 25 / .383333\
   **EAC para a Tarefa 3** = 65,22 horas

1. **IPC para a Tarefa 1** = 0,25 calculado da seguinte forma:\
   **IPC para a Tarefa 1** = *IF* Horas reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformance/Horas Reais\
       *ELSE* IPC = 1\
   **IPC para a Tarefa 1** = 12,5 / 50\
   **IPC para a Tarefa 1** = .25

1. **EAC para a Tarefa 1** = 120 horas, calculadas do seguinte modo:\
   **EAC para a Tarefa 1** = *IF* IPC &lt;> 0 *THEN* EAC = Horas Planejadas / CPI\
       *ELSE* EAC = Horas Planejadas + Horas Reais\
   **EAC para a Tarefa 1** = 30/ .25\
   **EAC para a Tarefa 1** = 120 horas

1. **CPI para projeto** = .22 calculado da seguinte forma:\
   **CPI para projeto** = *IF* Horas reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformance/Horas Reais\
       *ELSE* IPC = 1\
   **CPI para projeto** = 24,5 / 110\
   **CPI para projeto** = .22272\
   **CPI para projeto** = .22

1. **EAC para o Projeto** = 224,49 horas, calculadas do seguinte modo:\
   **EAC para o Projeto** = *IF* IPC &lt;> 0 *THEN* EAC = Horas/IPC Planejadas\
       *ELSE* EAC = Horas Planejadas + Horas Reais\
   **EAC para o Projeto** = 50 / .22272\
   **EAC para o Projeto** = 224,49 horas

### PIM= Baseado em Custo {#pim-cost-based}

* [Exemplo simples: projeto não tem tarefas filho](#simple-example-project-has-no-children-tasks)
* [Exemplo complicado: projeto tem tarefas filho](#complicated-example-project-has-children-tasks)

#### Exemplo simples: projeto não tem tarefas filho {#simple-example-project-has-no-children-tasks-1}

PIM = Baseado em Custo

Método EAC = Calcular no nível do projeto

1. Crie o Projeto A com três tarefas (sem tarefas filho) todas atribuídas ao Usuário 1, cujo custo/hora é US$ 100,00.
1. Adicione horas planejadas/reais a cada tarefa e % Concluído de acordo com a tabela abaixo:

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
   <th> <br> <p><strong>Custo de Lbr Pln</strong> </p> </th> 
   <th> <br> <p><strong>Hrs atuais</strong> </p> </th> 
   <th> <br> <p><strong>Custo Lbr da Lei</strong> </p> </th> 
   <th> <p><strong>% Completo</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 horas</p> </td> 
   <td> <p>$2,500.00</p> </td> 
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
   <td> <p>Tarefa 1 Exp. 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>Tarefa 1 Exp. 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Exp</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> <p>Tarefa 3 Exp</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
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
   <td> <p>Exp. Projeto 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 1 Exp. 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
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
   <th> <p><strong>Despesa Planejada Não Assegurada</strong> </p> </th> 
   <th> <p><strong>Despesas Planejadas Incorridas</strong> </p> </th> 
   <th> <p><strong>Despesa Real Assegurada</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Em Ações do Projeto, execute Recalcular Financiamento
1. **IPC para a Tarefa 1** = .14
1. **CPI****para Tarefa 1** = 0,14 calculado da seguinte forma:\
   **CPI**  **para a Tarefa 1** = *IF* Custo Real da Mão-de-Obra + CustoRealExpenseCusto &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **CPI****para Tarefa 1** = (100+300) / (2500+400)\
   **CPI**  **para a Tarefa 1** = 400 / 2900\
   **CPI**  **para a Tarefa 1**  = .14****

1. **EAC****para a Tarefa 1** = US$ 13.400,00\
   **Mão de obra de IPC**  **para a Tarefa 1** = IF Custo Real Da Mão De Obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mão de obra de IPC**  **para a Tarefa 1** = 100/2500\
   **Mão de obra de IPC**  **para a Tarefa 1** = .04 ****** Trabalho EAC ****para a Tarefa 1 **=*IF *CPI_Labor &lt;> 0*THEN *EAC Mão de obra = Custo Planejado da Mão de obra/CPI_Mão de obra\
   *    ELSE* EAC Mão de obra = Custo Planejado da Mão de obra + Custo Real da Mão de obra\
   **Trabalho EAC ****para a Tarefa 1** = 500.00/.04\
   **Trabalho EAC****para a Tarefa 1** = US$ 12.500,00\
   **Despesa EAC****para Tarefa 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Despesa EAC****para Tarefa 1** = US$ 400,00 + US$ 500,00\
   **Despesa EAC****para Tarefa 1** = US$ 900,00\
   **EAC****para a Tarefa 1** = Mão de obra EAC + Despesa EAC\
   **EAC****para a Tarefa 1**  = US$ 12.500,00 + US$ 900,00\
   **EAC****para a Tarefa 1**  = US$ 13.400,00

1. Estes são os valores CPI / EAC para a Tarefa 2 e a Tarefa 3:\
   Tarefa 2 = .19 / $8.433.33\
   Tarefa 3 = .44 / $6.950.00

1. **CPI para projeto** = .32 calculado da seguinte forma:\
   **CPI****para projeto** = *IF* Custo Real da Mão-de-Obra + CustoRealExpenseCusto &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****para projeto** = (1000 + 2300) / (7500 + 2700)\
   **CPI****para projeto** = 3300 / 10200\
   **CPI****para projeto** = .32

1. **EAC para o Projeto** = US$ 28.200,00 calculado da seguinte maneira:\
   **Mão de obra de CPI***para projeto** = IF Custo Real Da Mão De Obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mão de obra de CPI***para projeto** = 1000 / 7500\
   **Mão de obra de CPI***para projeto** = .13333\
   **Mão de obra de CPI***para projeto** = .13

   **Trabalho EAC****para Projeto** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC Mão de obra = Custo Planejado da Mão de obra + Custo Real da Mão de obra\
   **Trabalho EAC****para Projeto** = 3000/ .13333\
   **Trabalho EAC****para Projeto** = US$ 22.500,00

   **Despesas EAC****Projeto** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **Despesas EAC****Projeto** = US$ 3000,00 + 2.700,00\
   **Despesas EAC****Projeto** = US$ 5.700,00

   **EAC****Projeto** = Mão de obra EAC + Despesa EAC\
   **EAC****Projeto**  = US$ 22.500,00 + US$ 5.700,00\
   **EAC****Projeto**  = US$ 28.200,00

#### Exemplo complicado: projeto tem tarefas filho {#complicated-example-project-has-children-tasks-1}

PIM = Baseado em Custo

Método EAC = Calcular no nível do projeto

1. Crie o Projeto A com seis tarefas, onde a Tarefa 3 é a responsável das Tarefas 4 e 5 e a Tarefa 1 é a responsável das Tarefas 2 e 3, conforme mostrado abaixo:\
   Tarefa 1\
      Tarefa 2\
      Tarefa 3\
         Tarefa 4\
         Tarefa 5\
   Tarefa 6

1. Atribua Tarefas 2, 4, 5 e 6 ao Usuário 1 cuja taxa de custo/hora é de $100,00.
1. Adicione horas planejadas/reais a cada tarefa e % Concluído de acordo com a tabela abaixo.

   >[!NOTE]
   >
   >Para as Tarefas 1 e 3, você só está adicionando horas reais.

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
   <th> <br> <p><strong>Custo de Lbr Pln</strong> </p> </th> 
   <th> <br> <p><strong>Hrs atuais</strong> </p> </th> 
   <th> <br> <p><strong>Custo Lbr da Lei</strong> </p> </th> 
   <th> <p><strong>% Completo</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>5 horas</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 Hrs</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>15 horas</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 6</p> </td> 
   <td> <p>20 horas</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10 horas</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Adicione 50 horas diretamente ao projeto (Mais>Horas>Horas de Log) para que haja $5.000,00 do custo real da mão de obra registrado diretamente no projeto. ****
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
   <td> <p>Tarefa 1 Exp. 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>Tarefa 1 Exp. 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>Tarefa 1 Exp. 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Exp. 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Exp. 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Exp. 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>Tarefa 2 Exp. 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> <p>Tarefa 3 Exp</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4</p> </td> 
   <td> <p>Tarefa 4 Exp. 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4</p> </td> 
   <td> <p>Tarefa 4 Exp. 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4 </p> </td> 
   <td> <p>Tarefa 4 Exp. 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>Tarefa 5 Exp. 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>Tarefa 5 Exp. 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>Tarefa 5 Exp. 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 6</p> </td> 
   <td> <p>Tarefa 6 Exp. 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 6</p> </td> 
   <td> <p>Tarefa 6 Exp. 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
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
   <td> <p>Exp. Projeto 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 1 Exp. 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p> $0.00 <strong></strong></p> </td> 
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
   <th> <p><strong>Despesa Planejada Não Assegurada</strong> </p> </th> 
   <th> <p><strong>Despesas Planejadas Incorridas</strong> </p> </th> 
   <th> <p><strong>Despesa Real Assegurada</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Tarefa 1</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tarefa 6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projeto</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Em Ações do Projeto, execute Recalcular Financiamento
1. **CPI** para a Tarefa 2 = 0,17, calculada da seguinte forma:\
   **Tarefa de IPC 2** = *IF* Custo Real da Mão-de-Obra + CustoRealExpenseCusto &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformance + IncurredPlannedExpenseCost) / (RealLaborCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI***Tarefa 2** = (100+300) / (1000+1300)\
   **CPI***Tarefa 2**  = 400 / 2300\
   **CPI***Tarefa 2**  = .17

1. **EAC** para Tarefa 2 = US$ 5.900,00\
   **Mão de obra de IPC***Tarefa 2** = IF Custo Real da Mão-de-Obra &lt;> 0 ENTÃO CPI_Mão-de-Obra = TotalBudgetedCostWorkPerformance / Custo Real da Mão-de-Obra\
      ELSE CPI_Labor = 1\
   **Mão de obra de IPC***Tarefa 2** = 100/1000\
   **Mão de obra de IPC***Tarefa 2** = .1

   **Trabalho EAC****Tarefa 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC Mão de obra = Custo Planejado da Mão de obra + Custo Real da Mão de obra\
   **Trabalho EAC****Tarefa 2** = 500.00/.1\
   **Trabalho EAC****Tarefa 2** = US$ 5.000,00 ****** Despesa da EAC ****Tarefa 2 **= IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Despesa da EAC ****Tarefa 2** = US$ 1.300,00 + - US$ 400,00\
   **Despesa EAC****Tarefa 2** = US$ 900,00

   **EAC****Tarefa 2** = Mão de obra EAC + Despesa EAC\
   **EAC****Tarefa 2**  = US$ 5.000,00 + US$ 900,00\
   **EAC****Tarefa 2**  = US$ 5.900,00

1. O CPI/EAC para as Tarefas 4, 5 e 6 são determinados da mesma forma, então irei fornecer os valores abaixo:\
   Tarefa 4: 0,23 / US$ 3.400,00\
   Tarefa 5: 0,64 / US$ 3.100,00\
   Tarefa 6: 1,06 / US$ 2.366,67

1. IPC para a Tarefa 3 = .31, calculada da seguinte forma:\
   **IPC***Tarefa 3** = *IF* Custo Real da Mão-de-Obra + CustoRealExpenseCusto &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **IPC***Tarefa 3**  = (1,150 + 500) / (3000 + 2400)\
   **IPC***Tarefa 3**  = 1650 / 5400\
   **IPC***Tarefa 3**  = .31 ****** EAC para a Tarefa 3 **= US$ 9.521,74 calculado da seguinte maneira:\
   **Mão de obra de CPI ****Tarefa 3** = IF Custo Real Da Mão De Obra &lt;> 0 ENTÃO

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mão de obra IPC***Tarefa 3** = 1150/3000\
   **Mão de obra IPC***Tarefa 3** = .383333\
   **Mão de obra IPC***Tarefa 3** = .38

   **Trabalho EAC****Tarefa 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC Mão de obra = Custo Planejado da Mão de obra + Custo Real da Mão de obra\
   **Trabalho EAC****Tarefa 3** = US$ 2.500,00 / .383333\
   **Trabalho EAC****Tarefa 3** = US$ 6.521,74

   **Despesa EAC****Tarefa 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Despesa EAC****Tarefa 3** = US$ 2.400,00 + US$ 600,00\
   **Despesa EAC****Tarefa 3** = US$ 3.000,00

   **EAC****Tarefa 3** = Mão de obra EAC + Despesa EAC\
   **EAC****Tarefa 3**  = US$ 6.521,74 + US$ 3.000,00\
   **EAC****Tarefa 3**  = US$ 9.521,74

1. CPI para a Tarefa 1 = 0,16, calculado da seguinte forma:\
   **CPI***Tarefa 1** = *IF* Custo Real da Mão-de-Obra + CustoRealExpenseCusto &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI***Tarefa 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI***Tarefa 1**  = 1550 / 9500=\
   **CPI***Tarefa 1**  = .16

1. O EAC para a Tarefa 1 é de $17.100.00 calculado da seguinte maneira:\
   **Mão de obra de CPI***Tarefa 1** = IF Custo Real Da Mão De Obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mão de obra de CPI***Tarefa 1** = 1250 / 5000\
   **Mão de obra de CPI***Tarefa 1** = .25

   **Trabalho EAC****Tarefa 1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC Mão de obra = Custo Planejado da Mão de obra / CPI_Mão de obra\
   *   ELSE* EAC Mão de obra = Custo Planejado da Mão de obra + Custo Real da Mão de obra\
   **Trabalho EAC****Tarefa 1** = US$ 3.000,00 / .25\
   **Trabalho EAC****Tarefa 1** = US$ 12.000,00

   **Despesa EAC****Tarefa 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Despesa EAC****Tarefa 1** = US$ 4500 + 600\
   **Despesa EAC****Tarefa 1** = US$ 5.100,00

   **EAC****Tarefa 1** = Mão de obra EAC + Despesa EAC\
   **EAC****Tarefa 1**  = US$ 12.000,00 + 5.100,00\
   **EAC****Tarefa 1**  = US$ 17.100,00

1. A CPI do projeto é .25\
   **CPI****para projeto** = *IF* Custo Real da Mão-de-Obra + CustoRealExpenseCusto &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **CPI****para projeto** = (2450 + 1900) / (11000 + 6700)\
   **CPI****para projeto** = 4350 / 17700\
   **CPI****para projeto** = .25

1. **EAC para o Projeto** = US$ 32.248,98 calculado da seguinte maneira:\
   **Mão de obra de CPI***para projeto** = IF Custo Real Da Mão De Obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mão de obra de CPI***para projeto** = 2450 / 11000\
   **Mão de obra de CPI***para projeto** = .22272\
   **Mão de obra de CPI***para projeto** = .22

   **Trabalho EAC****para Projeto** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC Mão de obra = Custo Planejado da Mão de obra + Custo Real da Mão de obra\
   **Trabalho EAC****para Projeto** = US$ 5.000,00 / .22272\
   **Trabalho EAC****para Projeto** = US$ 22.448,97959\
   **Trabalho EAC****para Projeto** = US$ 22.448,98

   **Despesas EAC****Projeto** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Despesas EAC****Projeto** = US$ 3.100,00 + US$ 6.700,00\
   **Despesas EAC****Projeto** = US$ 9.800,00

   **EAC****Projeto** = Mão de obra EAC + Despesa EAC\
   **EAC****Projeto**  = US$ 22.448,98 + 9.800,00\
   **EAC****Projeto**  = US$ 32.248,98
