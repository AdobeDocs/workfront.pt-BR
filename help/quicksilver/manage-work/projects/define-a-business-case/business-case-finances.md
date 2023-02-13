---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Visão geral dos campos financeiros do Caso de negócios
description: A subguia Caso de negócios inclui campos financeiros para o projeto. Para que alguns dos campos financeiros tenham valores, devem ser preenchidas as áreas correspondentes do Business Case.
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# Visão geral dos campos financeiros do Caso de negócios

A subguia Caso de negócios inclui campos financeiros para o projeto. Para que alguns dos campos financeiros tenham valores, devem ser preenchidas as áreas correspondentes do Business Case.  

Os seguintes campos financeiros do projeto são exibidos no Caso de negócios:

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
   <td> <p>Exibe o alinhamento do projeto de acordo com seu scorecard. Um valor de alto percentual indica que o projeto está bem alinhado com a finalidade e as metas da organização. <br>Para obter mais informações sobre o uso de scorecards, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Criar um scorecard</a>.</p> <p>Esse campo é exibido na área Resumo do caso de negócios . </p> </td> 
  </tr> 
  <tr> 
   <td>Custo Orçado</td> 
   <td> <p>O custo total estimado para ser associado ao projeto quando o projeto for iniciado.</p> <p>O Custo Orçado do projeto é calculado pela seguinte fórmula:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>O Adobe Workfront usa as Horas Orçadas do Planejador de Recursos para calcular o Custo de Mão-de-Obra Orçada.<br>Para obter mais informações sobre o cálculo do Custo Orçamentado, consulte <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Calcular Custo Orçamentado</a>. </p> <p>Esse campo é exibido na área Resumo do caso de negócios .</p> </td> 
  </tr> 
  <tr> 
   <td>Custo de despesa do orçamento</td> 
   <td> <p>O custo orçamentado de todas as despesas do projeto. </p> <p>Isso é calculado pela seguinte fórmula:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Para obter mais informações sobre o cálculo de despesas, consulte <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Gerenciar despesas do projeto </a>.</p> <p>Esse campo é exibido na área Expenses .</p> </td> 
  </tr> 
  <tr> 
   <td>Custo do Trabalho Orçado</td> 
   <td> <p>O custo associado aos recursos atribuídos para concluir o trabalho no projeto.</p> <p>O Custo da Mão-de-Obra Orçada para o projeto é calculado pela seguinte fórmula:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code></p> <p>O Workfront usa as Horas Orçadas do Planejador de Recursos para calcular o Custo de Mão-de-Obra Orçada.<br>Para obter mais informações sobre o cálculo do Custo da Mão-de-Obra Orçada, consulte <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Entender o Custo da Mão de obra Orçada e as Horas Orçamentadas para Projetos</a>.</p> <p>Este campo é exibido na área Orçamento de Recursos do Caso de Negócios. </p> </td> 
  </tr> 
  <tr> 
   <td>Despesas Planejadas</td> 
   <td> <p>É o mesmo que Custo de Despesa Orçada. </p> <p>Observação: O Custo Planejado de Despesas é diferente do Custo Planejado do Projeto. O Custo Planejado das Despesas é calculado com a Quantia Planejada das Despesas do projeto, enquanto o Custo Planejado é calculado com o uso das Horas Planejadas do projeto. </p> <p>Esse campo é exibido na área Expenses , para cada despesa.</p> </td> 
  </tr> 
  <tr> 
   <td>Valor líquido</td> 
   <td> <p>Valor total esperado do projeto após o cálculo do seu benefício e a eliminação dos custos.</p> <p>O Valor Líquido do projeto é calculado pela seguinte fórmula:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Para obter mais informações sobre o cálculo do Valor Líquido, consulte <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcular valor líquido</a>.<br></p> <p>Esse campo é exibido na área Resumo do caso de negócios .</p> </td> 
  </tr> 
  <tr> 
   <td>Benefício Planejado</td> 
   <td>Uma estimativa manual do benefício monetário para a sua organização quando este projeto for concluído. Pode ser qualquer quantidade de moeda e é específica para você e para cada projeto que você gerencia. O Benefício Planejado não pode ter um valor negativo. Esse campo é exibido na área Resumo do caso de negócios e pode ser editado na área Informações do projeto do caso de negócios. </td> 
  </tr> 
  <tr> 
   <td>Custo potencial dos riscos</td> 
   <td> <p>Este é o Custo Potencial de todos os riscos do projeto. </p> <p>Isso é calculado usando a seguinte fórmula:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Para obter mais informações sobre riscos no projeto, consulte <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Criar e editar riscos em projetos</a>.</p> <p>Esse campo é exibido na área Resumo do caso de negócios .</p> </td> 
  </tr> 
  <tr> 
   <td>Risco Potencial</td> 
   <td> <p>No Resumo do Caso de Negócios, essa é a quantia do custo de todos os riscos se eles devem ocorrer, com base na sua probabilidade. Por exemplo, se um Risco tem um Custo Potencial de $100 e uma Probabilidade de ocorrer de 10%, o Risco Potencial é de $10. O Risco Potencial no Resumo do Caso de Negócio é calculado pela seguinte fórmula:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> para todos os riscos. </p> </td> 
  </tr> 
  <tr> 
   <td>Custo da mitigação do risco</td> 
   <td> <p>O custo do plano de mitigação para os riscos que você está estimando pode ocorrer no projeto.<br>Para obter mais informações sobre riscos no projeto, consulte <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Criar e editar riscos em projetos</a>.</p> <p>Esse campo é exibido na área Riscos para cada risco especificado no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td>Custo Potencial para um Risco</td> 
   <td> <p>O custo financeiro estimado quando os riscos definidos no projeto se verificariam efetivamente, independentemente da sua probabilidade. </p> <p>Este é um campo atualizado manualmente que é exibido em cada risco na área Riscos do Caso de negócios. </p> </td> 
  </tr> 
  <tr> 
   <td>Custo potencial total dos riscos</td> 
   <td> <p>Trata-se do custo financeiro total estimado de todos os riscos definidos no projeto quando efetivamente ocorreram. </p> <p>Isso é calculado pela seguinte fórmula:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>É exibido como um número de moeda ao lado do título da área Riscos do Caso de negócios.</p> </td> 
  </tr> 
 </tbody> 
</table>
