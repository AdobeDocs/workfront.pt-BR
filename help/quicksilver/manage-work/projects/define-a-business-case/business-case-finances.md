---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Visão geral dos campos financeiros do Business Case
description: A subguia Business Case inclui campos financeiros para o projeto. Para que alguns campos financeiros tenham valores, as áreas correspondentes do Business Case devem ser preenchidas.
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 2%

---

# Visão geral dos campos financeiros do Business Case

A subguia Business Case inclui campos financeiros para o projeto. Para que alguns campos financeiros tenham valores, as áreas correspondentes do Business Case devem ser preenchidas.  

Os seguintes campos financeiros do projeto são exibidos no Business Case:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">Nome do campo</th> 
   <th scope="col">Descrição</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Alinhado </td> 
   <td> <p>Exibe o alinhamento do projeto de acordo com seu cartão de pontuação. Um valor alto de porcentagem indica que o projeto está bem alinhado à finalidade e às metas da organização. <br>Para obter mais informações sobre como usar cartões de pontuação, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Criar um cartão de pontuação</a>.</p> <p>Esse campo é exibido na área Resumo de Business Case. </p> </td> 
  </tr> 
  <tr> 
   <td>Custo Orçado</td> 
   <td> <p>O custo total estimado que será associado ao projeto quando o projeto for iniciado.</p> <p>O Custo Orçado do projeto é calculado pela seguinte fórmula:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>O Adobe Workfront usa as horas orçadas do Planejador de recursos para calcular o custo do trabalho orçado.<br>Para obter mais informações sobre como calcular o Custo Orçado, consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular Custo Orçado</a>. </p> <p>Esse campo é exibido na área Resumo de Business Case.</p> </td> 
  </tr> 
  <tr> 
   <td>Custo de despesa do orçamento</td> 
   <td> <p>O custo orçado de todas as despesas do projeto. </p> <p>Isso é calculado pela seguinte fórmula:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Para obter mais informações sobre como calcular despesas, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gerenciar despesas do projeto </a>.</p> <p>Esse campo é exibido na área Expenses.</p> </td> 
  </tr> 
  <tr> 
   <td>Custo do Trabalho Orçado</td> 
   <td> <p>O custo associado aos recursos atribuídos para concluir o trabalho no projeto.</p> <p>O Custo do Trabalho Orçado para o projeto é calculado pela seguinte fórmula:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>O Workfront usa as horas orçadas do Planejador de recursos para calcular o custo do trabalho orçado.<br>Para obter mais informações sobre como calcular o Custo do Trabalho Orçado, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Entender o Custo do Trabalho Orçado e as Horas Orçadas dos projetos</a>.</p> <p>Esse campo é exibido na área Orçamento de Recursos do Business Case. </p> </td> 
  </tr> 
  <tr> 
   <td>Custo Planejado de Despesas</td> 
   <td> <p>É o mesmo que Custo de Despesas Orçado. </p> <p>Nota: O Custo Planejado das Despesas é diferente do Custo Planejado do Projeto. O Custo Planejado de Despesas é calculado com a Quantia Planejada das despesas no projeto, enquanto o Custo Planejado é calculado usando as Horas Planejadas no projeto. </p> <p>Esse campo é exibido na área Expenses para cada despesa.</p> </td> 
  </tr> 
  <tr> 
   <td>Valor líquido</td> 
   <td> <p>Este é o valor total esperado do projeto após o cálculo do seu benefício e a remoção dos custos.</p> <p>O Valor Líquido do projeto é calculado pela seguinte fórmula:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Para obter mais informações sobre como calcular o Valor Líquido, consulte <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcular Valor Líquido</a>.<br></p> <p>Esse campo é exibido na área Resumo de Business Case.</p> </td> 
  </tr> 
  <tr> 
   <td>Benefício Planejado</td> 
   <td>Uma estimativa manual do benefício monetário para sua organização quando esse projeto for concluído. Pode ser qualquer valor de moeda e é específico para você e para cada projeto que você gerencia. O Benefício Planejado não pode ter um valor negativo. Esse campo é exibido na área Resumo de business case e pode ser editado na área Informações do projeto do business case. </td> 
  </tr> 
  <tr> 
   <td>Custo Potencial de Riscos</td> 
   <td> <p>Esse é o custo potencial de todos os riscos do projeto. </p> <p>Isso é calculado usando a seguinte fórmula:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Para obter mais informações sobre riscos no projeto, consulte <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Criar e editar riscos em projetos</a>.</p> <p>Esse campo é exibido na área Resumo de Business Case.</p> </td> 
  </tr> 
  <tr> 
   <td>Risco Potencial</td> 
   <td> <p>No Resumo de business case, essa é a quantia do custo de todos os riscos, se eles tiverem que ocorrer, com base em sua probabilidade. Por exemplo, se um Risco tiver um Custo Potencial de US$ 100 e uma Probabilidade de ocorrência de 10%, o Risco Potencial será de US$ 10. O Risco Potencial no Resumo de Business Case é calculado pela seguinte fórmula:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> para todos os riscos. </p> </td> 
  </tr> 
  <tr> 
   <td>Custo de Mitigação de Risco</td> 
   <td> <p>O custo do plano de mitigação para os riscos que você está estimando pode ocorrer no projeto.<br>Para obter mais informações sobre riscos no projeto, consulte <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Criar e editar riscos em projetos</a>.</p> <p>Esse campo é exibido na área Riscos para cada risco especificado no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td>Custo Potencial para um Risco</td> 
   <td> <p>O custo financeiro estimado quando os riscos definidos no projeto realmente ocorreriam, independentemente de sua probabilidade. </p> <p>Este é um campo atualizado manualmente que é exibido em cada risco na área Riscos do Business Case. </p> </td> 
  </tr> 
  <tr> 
   <td>Riscos Custo Potencial Total</td> 
   <td> <p>Total do custo financeiro estimado de todos os riscos definidos no projeto quando realmente ocorreram. </p> <p>Isso é calculado pela seguinte fórmula:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>É exibido como um número de moeda ao lado do título da área Riscos do Business Case.</p> </td> 
  </tr> 
 </tbody> 
</table>
