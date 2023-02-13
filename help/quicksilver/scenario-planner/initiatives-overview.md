---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visão geral das iniciativas no Planejador de cenário
description: O Planejador de cenário está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Workfront Scenario Planner, consulte A visão geral do Scenario Planner .
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# Visão geral das iniciativas na [!DNL Scenario Planner]

O [!DNL Scenario Planner] está disponível somente no novo [!DNL Adobe Workfront] e requer uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte [O [!DNL Scenario Planner] visão geral](../scenario-planner/scenario-planner-overview.md).
Como gerente de negócios, você pode criar iniciativas para planos na [!DNL Adobe Workfront Scenario Planner]. Para obter informações sobre como criar planos, consulte o artigo [Crie e edite planos na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Visão geral das iniciativas

Usar o [!DNL Workfront Scenario Planner], você pode estimar e revisar as seguintes informações para cada iniciativa:

* Estime o tipo e o número de funções que podem ser necessárias para concluir a iniciativa. Isso adiciona à contagem de função de cargo Obrigatório para o plano, bem como calcula os Custos de Pessoas que você pode revisar para uma iniciativa.
* Estime os Custos fixos associados ao trabalho necessário para concluir a iniciativa.
* Estime o Benefício Planejado que sua empresa pode ganhar quando a iniciativa for concluída.

Para visualizar informações sobre suas iniciativas, é possível acessar iniciativas individuais em um plano. Para obter informações sobre como criar e acessar iniciativas, consulte o artigo [Crie e edite iniciativas na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Considerações sobre iniciativas

Considere o seguinte ao criar iniciativas:

* Você deve criar um plano antes de criar uma iniciativa.
* É possível criar iniciativas do zero ou importar projetos para um plano. Os projetos se tornam iniciativas dentro do plano.

   Para obter informações sobre como criar iniciativa do zero, consulte [Crie e edite iniciativas na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   Para obter informações sobre como importar projetos para um plano de criação de iniciativas a partir de projetos, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Iniciativas são unidades de planejamento menores do que planos e são criadas apenas como parte de um plano.
* A iniciativa mais curta pode ter uma duração de 1 mês. A iniciativa mais longa pode ter uma duração de 5 anos.
* Não se pode fazer um trabalho real numa iniciativa. No nível da iniciativa, você pode definir quais recursos são necessários e o custo que esses recursos terão para que você possa começar a executar uma das demandas do plano. Por exemplo, se sua empresa tem um plano de expandir e adquirir um novo escritório em um novo local, seu departamento pode ter uma iniciativa de instalar a infraestrutura de rede para esse novo local.
* Você pode criar várias iniciativas em um plano. Com cada iniciativa, você pode delinear uma estratégia de alto nível para realizar o trabalho em seu departamento.
* Você pode priorizar iniciativas dentro de um plano, para garantir que a iniciativa mais importante receba o maior orçamento e mais recursos.
* Ao criar iniciativas dentro de um plano, todos que visualizarem esse plano também poderão visualizar todas as iniciativas dentro do plano.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* Você pode publicar iniciativas para criar projetos ou atualizar os projetos vinculados a eles. Para obter informações sobre iniciativas de publicação, consulte [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Informações financeiras sobre iniciativas

Você pode revisar informações financeiras sobre iniciativas individuais para entender como as iniciativas se encaixam no plano. Para obter informações sobre como acessar uma iniciativa, consulte o artigo [Crie e edite iniciativas na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Você pode exibir os seguintes indicadores financeiros sobre uma iniciativa acessando-a em um plano:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custo total valor]</td> 
   <td> <p style="font-weight: normal;">Este é um cálculo do custo total de uma iniciativa. </p> <p style="font-weight: normal;">[!DNL Workfront] O calcula o valor total de Custos de uma iniciativa usando esta fórmula:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custos fixos]</td> 
   <td> <p><span style="font-weight: normal;">Esta é uma entrada manual onde você pode estimar <span>um montante mensal de Custos fixos para cada mês da iniciativa.</span> Isso não inclui os custos associados às funções adicionadas à iniciativa que são capturadas no campo [!UICONTROL Custo de Pessoas].</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custos de pessoas]</td> 
   <td> <p style="font-weight: normal;">Trata-se de um cálculo total dos custos associados às funções da iniciativa em termos de emprego durante a duração da iniciativa. Esse número depende de quantas FTEs ou horas você estima para uma função de emprego para cada mês da iniciativa. </p> 
     <p><b>DICAS</b>  
     <ul> 
      <li> <p>O número de ETI mensais para a mesma função de trabalho pode ser diferente de mês para mês.</p> </li> 
      <li> <p>[!DNL Workfront] considera que há 160 horas de trabalho num mês. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] O calcula os [!UICONTROL Custos de pessoas] de uma iniciativa usando a seguinte fórmula:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] O calcula os Custos de Pessoas Mensais para cada mês durante a duração da Iniciativa usando a seguinte fórmula:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>EXEMPLO</b></p>
      <p>Se você tiver uma iniciativa com uma duração de 6 meses que exija um Designer com uma taxa de $50 por hora para 1 FTE a cada mês e um Web Designer com uma taxa por hora de $100 para 2 meses de iniciativa, os Custos de Pessoas da iniciativa serão calculados da seguinte maneira:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benefício planejado]</td> 
   <td>Esta é uma entrada manual na qual você pode estimar o benefício geral que seu departamento ganharia ao concluir esta iniciativa. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor líquido]</td> 
   <td> <p style="font-weight: normal;">Isso representa o valor da sua iniciativa ao considerar os custos gerais e o Benefício Planejado estimado na iniciativa. [!DNL Workfront] O calcula o Valor Líquido de uma iniciativa usando a seguinte fórmula:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## Informações sobre iniciativas em relatórios

Você pode exibir as informações da iniciativa nos relatórios, conforme descrito na tabela abaixo. Essas informações estão disponíveis na instância do Workfront somente quando a empresa adquiriu uma licença do Workfront Scenario Planner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Tipo de relatório</b></td> 
   <td><b>Informações da iniciativa</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Nome, Duração, Datas Iniciais e Finais, Inserido por, ID, Última Data de Publicação*, Todos os campos do Projeto incluindo campos personalizados*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>Todas as informações da Iniciativa conforme listado acima, (Função do Trabalho) ID, Projeto*, Atribuição do Projeto Horas Planejadas*, Horas da Função do Trabalho da Iniciativa, Contagem (Função do Trabalho), Todos os campos do Projeto incluindo campos personalizados*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Projeto]*</p></td> 
   <td> <p>Todas as informações da Iniciativa conforme listado acima*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Esses campos são preenchidos com informações do projeto vinculado à iniciativa, somente quando a iniciativa foi criada a partir de um projeto ou foi publicada em um projeto pelo menos uma vez. Para obter informações sobre iniciativas de publicação, consulte [Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
