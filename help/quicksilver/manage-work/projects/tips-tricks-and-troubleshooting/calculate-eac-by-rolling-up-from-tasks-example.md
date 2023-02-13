---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Exemplo de cálculo - Calcular EAC como uma totalização de tarefas
description: PIM = Baseado em Hora
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 8%

---

# Exemplo de cálculo - Calcular EAC como uma totalização de tarefas

## Método EAC: acumular de tarefas ou subtarefas

* [PIM= Baseado em Hora](#pim-hour-based)
* [PIM= Baseado em Custo](#pim-cost-based)

### PIM= Baseado em Hora {#pim-hour-based}

* [Exemplo simples: projeto não tem tarefas filho](#simple-example-project-has-no-children-tasks)
* [Exemplo complicado: projeto tem tarefas filho](#complicated-example-project-has-children-tasks)

#### Exemplo simples: projeto não tem tarefas filho {#simple-example-project-has-no-children-tasks}

PIM = Baseado em Hora

Método EAC = Acumulado de tarefas/subtarefas

1. Crie o Projeto A com três tarefas (sem tarefas filho) todas atribuídas ao Usuário 1, cujo custo/hora é US$ 100,00.
1. Adicione horas planejadas/reais a cada tarefa e % Concluído de acordo com a tabela abaixo:

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

1. Recalcular Finanças
1. **IPC para a Tarefa 1** = 0,04 calculado da seguinte forma:\
   **IPC para a Tarefa 1** = *IF* Horas reais > 0 *THEN* CPI = TotalBudgetedCostWorkPerformance/Horas Reais\
       *ELSE* IPC = 1\
   **IPC para a Tarefa 1** = 1 / 25\
   **IPC para a Tarefa 1** = .04

1. **EAC para a Tarefa 1** = 125 horas, calculadas do seguinte modo:\
   **EAC para a Tarefa 1** = *IF* IPC &lt;> 0 *THEN* EAC = Horas Planejadas/IPC\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC para a Tarefa 1** = 5 / .04\
   **EAC para a Tarefa 1** = 125 horas

1. O IPC / EAC para as Tarefas 2 e 3 são:\
   Tarefa 2 = 0,12 / 83,33 h\
   Tarefa 3 = 0,24 / 62,5 h

1. **CPI para projeto** = .13 calculado da seguinte forma:\
   **CPI para projeto** = *IF* Horas reais > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **CPI para projeto** = 10 / 75\
   **CPI para projeto** = .13

1. **EAC para o Projeto** = 270,83 horas, calculadas do seguinte modo\
   **EAC para o Projeto** = Tarefa EAC 1 + Tarefa EAC 2 + Tarefa EAC 3\
   **EAC para o Projeto** = 125 + 83,33 + 62,5\
   **EAC para o Projeto** = 270,83 horas

#### Exemplo complicado: projeto tem tarefas filho {#complicated-example-project-has-children-tasks}

PIM = Baseado em Hora

Método EAC = Acumulado de tarefas/subtarefas

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

1. Adicione 50 horas diretamente ao projeto (Mais>Horas>Horas de Log) para que haja $5.000,00 do custo real da mão de obra registrado diretamente no projeto.
1. Executar Recalcular Finanças
1. **IPC para a Tarefa 2** = .1 calculado do seguinte modo:\
   **IPC para a Tarefa 2** = *IF* Horas reais > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **IPC para a Tarefa 2** = 1 / 10\
   **IPC para a Tarefa 2** = .1

1. **EAC para a Tarefa 2** = 50 horas, calculadas do seguinte modo:\
   **EAC para a Tarefa 2** = *IF* IPC &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = Horas Planejadas + Horas Reais\
   **EAC para a Tarefa 2** = 5 / .1\
   **EAC para a Tarefa 2** = 50 horas

1. CPI / EAC para a Tarefa 4, Tarefa 5 e Tarefa 6:\
   Tarefa 4 = 0,4 / 25 horas\
   Tarefa 5 = 0,75 / 20 horas\
   Tarefa 6 = 1,2 / 16,67 h

1. **IPC para a Tarefa 3** = .38\
   **IPC para a Tarefa 3** = *IF* Horas reais > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **IPC para a Tarefa 3** = 11,5 / 30\
   **IPC para a Tarefa 3** = .38

1. **EAC para a Tarefa 3** = Tarefa EAC 4 + Tarefa EAC 5\
   **EAC para a Tarefa 3** = 25 + 20\
   **EAC para a Tarefa 3** = 45 horas

1. **IPC para a Tarefa 1** = 0,25 calculado da seguinte forma:\
   **IPC para a Tarefa 1** = *IF* Horas reais > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **IPC para a Tarefa 1** = 12,5 / 50\
   **IPC para a Tarefa 1** = .25

1. **EAC para a Tarefa 1** = Tarefa EAC 2 + Tarefa EAC 3\
   **EAC para a Tarefa 1** = 50 + 45\
   **EAC para a Tarefa 1** = 95 horas

1. CPI para Projeto = 0,22, calculado da seguinte forma:\
   **CPI para projeto** = *IF* Horas reais > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* IPC = 1\
   **CPI para projeto** = 24,5 / 110\
   **CPI para projeto** = .22272\
   **CPI para projeto** = .22

1. **EAC para o projeto** = Tarefa EAC 1 + Tarefa EAC 6\
   **EAC para o projeto** = 95 + 16,67\
   **EAC para o projeto** = 111,67 h

### PIM= Baseado em Custo {#pim-cost-based}

* [Exemplo simples: projeto não tem tarefas filho](#simple-example-project-has-no-children-tasks)

#### Exemplo simples: projeto não tem tarefas filho {#simple-example-project-has-no-children-tasks-1}

PIM = Baseado em Custo

Método EAC = Acumulado de tarefas/subtarefas

1. Crie o Projeto A com três tarefas (sem tarefas filho) todas atribuídas ao Usuário 1 cujo custo/hora é de US$ 100,00.
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
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Em Ações do Projeto, execute Recalcular Financiamento
1. **CPI****para Tarefa 1** = 0,14 calculado da seguinte forma:\
   **CPI****para Tarefa 1**  = *IF* Custo Real da Mão-de-Obra + CustoRealExpenseCusto &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****para Tarefa 1**  = (100+300) / (2500+400)\
   **CPI****para Tarefa 1**  = 400 / 2900\
   **CPI****para Tarefa 1**  = .14

1. **EAC****para a Tarefa 1** = US$ 13.400,00\
   **Mão de obra de CPI***para Tarefa 1** = IF Custo Real Da Mão De Obra &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **Mão de obra de CPI***para Tarefa 1** = 100/2500\
   **Mão de obra de CPI***para Tarefa 1** = .04

   **Trabalho EAC****para a Tarefa 1** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC Mão de obra = Custo Planejado da Mão de obra + Custo Real da Mão de obra\
   **Trabalho EAC****para a Tarefa 1** = 500.00/.04\
   **Trabalho EAC****para a Tarefa 1** = US$ 12.500,00

   **Despesa EAC****para Tarefa 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **Despesa EAC****para Tarefa 1** = US$ 400,00 + US$ 500,00\
   **Despesa EAC****para Tarefa 1** = US$ 900,00

   **EAC****para a Tarefa 1** = Mão de obra EAC + Despesa EAC\
   **EAC****para a Tarefa 1**  = US$ 12.500,00 + US$ 900,00\
   **EAC****para a Tarefa 1**  = US$ 13.400,00

1. Estes são os valores CPI / EAC para a Tarefa 2 e a Tarefa 3:\
   Tarefa 2 = .19 / $8.433.33\
   Tarefa 3 = .44 / $6.950.00****

1. O IPC do projeto = 0,32\
   **CPI****para projeto** = *IF* Custo Real da Mão-de-Obra + CustoRealExpenseCusto &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****para projeto** = (1000 + 2300) / (7500 + 2700)\
   **CPI****para projeto** = 3300 / 10200\
   **CPI****para projeto** = .32

1. O EAC para o projeto é de $28.783,33\
   **EAC****para o projeto** = Tarefa EAC 1 + Tarefa EAC 2 + Tarefa EAC 3\
   **EAC****para o projeto** = US$ 13.400,00 + US$ 8.433,33 + US$ 6.950,00\
   **EAC****para o projeto** = US$ 28.783,33
