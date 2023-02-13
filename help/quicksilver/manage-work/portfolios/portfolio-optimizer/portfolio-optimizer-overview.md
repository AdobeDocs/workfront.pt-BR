---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Visão geral do Portfolio Otimizer
description: O [!UICONTROL Portfolio Otimizer] é a ferramenta usada para avaliação e comparação de projetos. O processo de revisar e comparar valores de Caso de negócios para projetos atribuídos a um portfólio é como um gerente de portfólio pode priorizar projetos e gerar o maior valor para uma organização.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 0%

---

# [!UICONTROL Portfolio Otimizer] visão geral

O [!UICONTROL Portfolio Otimizer] é a ferramenta usada para avaliação e comparação de projetos. O processo de revisão e comparação [!UICONTROL Caso de negócios] para projetos atribuídos a um portfólio é como um gerente de portfólio pode priorizar projetos e gerar o maior valor para uma organização.

O objetivo da [!UICONTROL otimizador de portfólio] é fornecer uma interface através da qual um gerente de portfólio, comitê diretor ou escritório de gerenciamento de produtos pode exibir informações resumidas sobre o caso comercial de cada projeto. Os projetos podem então ser priorizados de acordo com valores e objetivos estratégicos, ou de acordo com sua pontuação geral.

O [!UICONTROL Portfolio Otimizer] O pode ajudá-lo somente se tiver concluído os seguintes pré-requisitos:


* O [!UICONTROL Casos de negócios] foram concluídas nos projetos. Para obter informações, consulte os artigos na seção [Definir um caso de negócios](../../projects/define-a-business-case/define-business-case.md).
* Um portfólio é definido na área Visão geral do projeto da seção Detalhes do projeto para os projetos que você deseja revisar
* Você indicou o Orçamento do Projeto e o Benefício Planejado para os projetos que deseja revisar. Custo Fixo e Receita Fixa são opcionais, mas acrescentam valor adicional. Para obter mais informações, consulte [Campos de finanças do projeto](../../projects/project-finances/project-finances-overview-1.md).


Para obter informações sobre como localizar a variável [!UICONTROL Portfolio Otimizer], consulte [Localize a variável [!UICONTROL Portfolio Otimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanças na [!UICONTROL Portfolio Otimizer]

* [As áreas financeiras da [!UICONTROL Portfolio Otimizer]](#the-financial-areas-in-the-portfolio-optimizer)
* [Os campos financeiros da [!UICONTROL Portfolio Otimizer]](#the-financial-fields-in-the-portfolio-optimizer)

Você pode ver o estado financeiro do seu portfólio a qualquer momento durante a vida útil dos projetos ao usar o [!UICONTROL Portfolio Otimizer].

Considere o seguinte ao trabalhar com as finanças na [!UICONTROL Portfolio Otimizer]:

* Cada projeto recebe uma pontuação quando sua [!UICONTROL Casos de negócios] são preenchidos de acordo com os critérios correspondentes na variável [!UICONTROL Portfolio Otimizer]. Por exemplo, projetos de baixo custo ou alinhamento alto recebem uma pontuação mais alta.

   Para obter mais informações sobre o cálculo da pontuação do otimizador de portfólio de um projeto, consulte o artigo [Visão geral da [!UICONTROL Portfolio Otimizer] Pontuação](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* Os cálculos financeiros para a [!UICONTROL Portfolio Otimizer] use o [!UICONTROL Custo orçado] no [!UICONTROL Caso de negócios] do projeto.
* Você pode priorizar manualmente seus projetos na variável [!UICONTROL Portfolio Otimizer], tendo em conta todas as informações sobre as mesmas. Isso inclui dados financeiros, alinhamento aos scorecards, ROI, por exemplo.

### As áreas financeiras da [!UICONTROL Portfolio Otimizer] {#the-financial-areas-in-the-portfolio-optimizer}

Você pode exibir informações financeiras nas seguintes áreas da variável [!UICONTROL Portfolio Otimizer]:

* **[!UICONTROL Cabeçalho Portfolio]**: Essa área exibe informações financeiras coletadas de todos os projetos do portfólio. Ele é exibido em cada guia do objeto Portfolio.
* **[!UICONTROL Finanças do Portfolio para projetos selecionados]**: Esta área apresenta informações financeiras obtidas a partir dos projetos selecionados no [!UICONTROL Portfolio Otimizer]. Você pode adicionar ou remover projetos e entender como isso afetará as finanças do portfólio ao exibir as informações nesta área.
* **[!UICONTROL Finanças de projetos]**: Essa área exibe as informações financeiras de cada projeto listado no [!UICONTROL Portfolio Otimizer].

### Os campos financeiros da [!UICONTROL Portfolio Otimizer] {#the-financial-fields-in-the-portfolio-optimizer}

Os seguintes campos financeiros são exibidos na variável [!UICONTROL Portfolio Otimizer]:

* [Cabeçalho Portfolio](#portfolio-header)
* [Portfolio para financiar projetos selecionados](#portfolio-finances-for-selected-projects)

#### Cabeçalho Portfolio {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] O calcula os campos financeiros no cabeçalho do portfólio usando informações de projetos com status que são iguais somente a [!UICONTROL Aprovado] ou [!UICONTROL Atual].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome do campo</strong> </th> 
   <th><strong>Descrição</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL No Horário]</td> 
   <td> <p>A porcentagem de projetos no portfólio que são considerados como [!UICONTROL no horário]. Isso é visível de qualquer guia dentro de um Portfolio.</p> <p>Um projeto é considerado [!UICONTROL no horário] quando o projeto <strong>[!UICONTROL Condição]</strong> é <strong>[!UICONTROL No Target]</strong>. <br>Para obter mais informações sobre as [!UICONTROL Condições do projeto], consulte o artigo <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Visão geral da condição do projeto e do tipo de condição</a>.</p> <p>O <strong>[!UICONTROL No Horário]</strong> a porcentagem é calculada usando a seguinte fórmula:</p> <p><em>[!UICONTROL na porcentagem de Portfolio de tempo] = Número de projetos [!UICONTROL no tempo]/ Número total de projetos em um status [!UICONTROL atual] ou [!UICONTROL aprovado]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL No Orçamento]</td> 
   <td> <p>A porcentagem de projetos na carteira que são considerados como [!UICONTROL On Budget]. Isso é visível de qualquer guia dentro de um [!UICONTROL Portfolio].</p> <p>Os projetos são <strong>[!UICONTROL No Orçamento]</strong> quando não tenham excedido o seu orçamento predefinido. <br>Para obter mais informações sobre o orçamento de um projeto, consulte o artigo <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">Informações do [!UICONTROL Gerenciar] na área de finanças do projeto</a>.</p> <p>A porcentagem de [!UICONTROL no orçamento] é calculada usando a seguinte fórmula:</p> <p><em>[!UICONTROL na porcentagem do Portfolio de orçamento] = Número de projetos [!UICONTROL no orçamento]/ Número total de projetos </em><em>em um status [!UICONTROL Atual] ou [!UICONTROL Aprovado]</em> </p> </td> 
  </tr> 
  <tr> 
   <td>ROI (para portfólio)</td> 
   <td> <p>O [!UICONTROL Retorno do investimento] (ROI) da carteira é calculado levando em conta o total [!UICONTROL Benefício] da [!UICONTROL Portfolio] e o total dos [!UICONTROL Custos orçados] dos projetos. Isso é visível de qualquer guia dentro de um Portfolio.</p> <p>O valor do ROI de Portfolio é calculado usando a seguinte fórmula:</p> <p><em>Portfolio ROI = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100</em> </p> <p>Para obter mais informações sobre como o ROI é calculado para um projeto, consulte o artigo <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Calcular o retorno sobre o investimento (ROI)</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Alinhado] ou [!UICONTROL Alignment Score] </td> 
   <td> <p>Uma média de todos os valores de [!UICONTROL Project Alignment Score] que são calculados após a conclusão do [!UICONTROL Scorecard] no [!UICONTROL Business Case] do projeto. A pontuação de alinhamento de cada projeto é listada na coluna [!UICONTROL Alinhamento] do [!UICONTROL Portfolio Otimizer]. Isso é visível de qualquer guia dentro de um portfólio.</p> <p>Para obter mais informações sobre a geração de uma pontuação de alinhamento para um projeto, consulte o artigo <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Aplicar um scorecard a um projeto e gerar uma Pontuação de alinhamento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Valor líquido]</td> 
   <td> <p>A soma de todos os [!UICONTROL Valores Líquidos] de todos os projetos no portfólio. Isso é visível de qualquer guia dentro de um portfólio.</p> <p>Para obter mais informações sobre como o [!UICONTROL Net Value] é calculado para um projeto, consulte o artigo <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Calcular valor líquido</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio para financiar projetos selecionados {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome do campo</strong> </th> 
   <th> <p><strong>Descrição</strong> </p> <p> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Número de projetos]</td> 
   <td> <p>O número total de projetos ativos no portfólio. Os projetos considerados ativos em um portfólio podem estar em qualquer um dos seguintes status:</p> 
    <ul> 
     <li>[!UICONTROL Atual]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Aprovado]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Orçamento]</td> 
   <td>Você pode atualizar manualmente esse campo para indicar qual é o orçamento total do portfólio inteiro. Este orçamento é usado para todos os projetos dentro do portfólio. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Restante]</td> 
   <td> <p>O orçamento restante depois de todos os [!UICONTROL Custos orçados] em todos os projetos dentro do portfólio foram subtraídos do Orçamento do portfólio.</p> <p>O [!UICONTROL Remaining Portfolio Budget] é calculado usando a seguinte fórmula:</p> <p><em>[!UICONTROL Restante Portfolio Budget] = [!UICONTROL Total Portfolio Budget] - Total [!UICONTROL Budgeted Cost] de Todos os Portfolio Projetos</em> </p> <p>O [!UICONTROL Custo orçado] geral de todos os projetos do portfólio é representado na barra de indicadores no campo Orçamento. </p> <p>Para obter mais informações sobre o rastreamento de custos em um projeto, consulte o artigo<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custo total]</td> 
   <td> <p>A soma dos custos de todos os projetos exibidos no [!UICONTROL Portfolio Otimizer]. O custo de cada projeto é igual ao [!UICONTROL Custo orçado] do projeto, pois é exibido no [!UICONTROL Business Case Summary]. </p> <p>Para obter mais informações sobre os campos financeiros dos projetos no [!UICONTROL Business Case], consulte a seção "Entendendo campos financeiros no business case" no artigo <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Criar um caso de negócios para um projeto </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risco] </td> 
   <td> <p>A soma de todos os [!UICONTROL Custos de Risco Potencial] de todos os projetos no portfólio. O [!UICONTROL Potencial Risk Cost] de cada projeto é listado na coluna [!UICONTROL Risk] do [!UICONTROL Portfolio Otimizer]. </p> <p>Para obter mais informações sobre o cálculo de riscos para projetos, consulte o artigo <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Calcular Custo de Risco Potencial </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefício]</td> 
   <td> <p>A soma de todos os valores de [!UICONTROL Planned Benefit] de todos os projetos do portfólio. O valor do Benefício Planejado de cada projeto é listado na coluna [!UICONTROL Benefício] do [!UICONTROL Portfolio Otimizer]. </p> <p>Para obter mais informações sobre o [!UICONTROL Planned Benefit] de um projeto, consulte o artigo <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Visão geral do benefício planejado do projeto</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Indicador [!UICONTROL Risco para valor líquido]</td> 
   <td> <p>Mede o valor do [!UICONTROL Potencial Risk] levando em conta o [!UICONTROL Net Value] fornecido por todos os projetos no portfólio. Para obter a maior eficiência no portfólio, você quer ver que o indicador [!UICONTROL Risco] é baixo e o indicador [!UICONTROL Net Value] é alto. </p> <p>Para obter mais informações sobre o cálculo do Risco para o [!UICONTROL Valor líquido], consulte o artigo <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Calcular o risco para o valor líquido em um portfólio</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalize o [!UICONTROL Portfolio Otimizer]

Você pode personalizar somente a área da lista de projetos da [!UICONTROL Portfolio Otimizer] usando as configurações para alterar as informações na lista.

Os ícones e opções a seguir estão disponíveis para a variável [!UICONTROL Portfolio Otimizer]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Ícone no Portfolio Otimizer</td> 
   <td>Nome</td> 
   <td>Função</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Definir prioridade do projeto]</td> 
   <td>Use esse ícone quando quiser salvar a ordem do projeto, com base em sua prioridade. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Otimizar portfólio]</td> 
   <td>Use este ícone para otimizar o portfólio com base nos seguintes valores financeiros dos projetos:
    <ul>
     <li>[!UICONTROL Custo]</li>
     <li>[!UICONTROL Alinhamento]</li>
     <li>[!UICONTROL Valor]</li>
     <li>[!UICONTROL Risco para benefício]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Para obter mais informações sobre como otimizar seu portfólio, consulte o artigo <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Otimizar projetos no [!UICONTROL Portfolio Otimizer] </a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>Ícones da [!UICONTROL Desfazer]/ [!UICONTROL Refazer]</td> 
   <td>Use esses ícones para cancelar ou refazer as alterações feitas no [!UICONTROL Portfolio Otimizer] antes de salvar.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unseleted_portfólio_otimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Exibir]/ [!UICONTROL Ocultar projetos desmarcados</td> 
   <td>Use esses ícones para exibir ou ocultar os projetos no portfólio que você desmarcou.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Exportar] </td> 
   <td> <p>Use esse ícone para exportar os dados na área [!UICONTROL Priorização de projeto] do [!UICONTROL Portfolio Otimizer]. Você pode exportá-la para os seguintes formatos:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Guia] Delimitado</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfólio_otimizer.png"> </td> 
   <td>[!UICONTROL Preferências]</td> 
   <td> <p>Use este ícone para modificar os campos do projeto exibidos nas colunas do [!UICONTROL Portfolio Otimizer] ou para modificar quais projetos você exibe no [!UICONTROL Otimizer], com base em seus status. </p> <p>Dica:  
     <ul> 
      <li> <p>Nem tudo [!DNL Workfront] os campos padrão estão disponíveis para adição nas colunas. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>É possível adicionar apenas os campos personalizados que têm um valor diferente de zero em qualquer projeto do portfólio.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
