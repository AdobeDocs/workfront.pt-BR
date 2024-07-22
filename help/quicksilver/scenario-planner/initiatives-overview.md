---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visão geral das iniciativas no Planejador de cenários
description: O Planejador de cenários está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte A visão geral do Planejador de cenários.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Visão geral das iniciativas no [!DNL Scenario Planner]

Como gerente de negócios, você pode criar iniciativas para planos no [!DNL Adobe Workfront Scenario Planner]. Para obter informações sobre como criar planos, consulte o artigo [Criar e editar planos no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Visão geral das iniciativas

Usando o [!DNL Workfront Scenario Planner], você pode estimar e revisar as seguintes informações para cada iniciativa:

* Estime o tipo e a quantidade de funções de trabalho que podem ser necessárias para concluir a iniciativa. Isso aumenta a contagem de funções de trabalho necessárias para o plano e calcula os Custos de pessoas que podem ser revisados para uma iniciativa.
* Estime os Custos fixos associados ao trabalho necessário para concluir a iniciativa.
* Estime o Benefício Planejado que sua empresa pode ganhar quando a iniciativa for concluída.

Para exibir informações sobre suas iniciativas, você pode acessar iniciativas individuais em um plano. Para obter informações sobre como criar e acessar iniciativas, consulte o artigo [Criar e editar iniciativas no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Considerações sobre iniciativas

Considere o seguinte ao criar iniciativas:

* Você deve criar um plano antes de criar uma iniciativa.
* É possível criar iniciativas do zero ou importar projetos em um plano. Os projetos se tornam iniciativas dentro do plano.

  Para obter informações sobre como criar iniciativas do zero, consulte [Criar e editar iniciativas no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

  Para obter informações sobre como importar projetos para um plano para criar iniciativas de projetos, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* As iniciativas são unidades de planejamento menores que os planos e são criadas apenas como parte de um plano.
* A iniciativa mais curta pode ter uma duração de 1 mês. A iniciativa mais longa pode ter uma duração de 5 anos.
* Não é possível realizar um trabalho real em uma iniciativa. No nível da iniciativa, você pode definir quais recursos são necessários e quais custos eles incorrerão para que você possa começar a executar uma das demandas do plano. Por exemplo, se sua empresa tem um plano para expandir e adquirir um novo escritório em um novo local, seu departamento pode ter uma iniciativa para instalar a infraestrutura de rede para esse novo local.
* É possível criar várias iniciativas em um plano. Com cada iniciativa, você pode destacar uma estratégia de alto nível para realizar o trabalho em seu departamento.
* É possível priorizar iniciativas em um plano para garantir que a iniciativa mais importante receba o maior orçamento e os maiores recursos.
* Quando você cria iniciativas em um plano, todos os usuários que visualizam esse plano também podem visualizar todas as iniciativas dentro do plano.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* É possível publicar iniciativas para criar projetos ou atualizar os projetos vinculados a eles. Para obter informações sobre como publicar iniciativas, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Informações financeiras sobre iniciativas

Você pode revisar informações financeiras sobre iniciativas individuais para entender como as iniciativas se encaixam no plano. Para obter informações sobre como acessar uma iniciativa, consulte o artigo [Criar e editar iniciativas no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Você pode exibir os seguintes indicadores financeiros sobre uma iniciativa acessando-a dentro de um plano:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor total de custos]</td> 
   <td> <p style="font-weight: normal;">Este é um cálculo do custo total de uma iniciativa. </p> <p style="font-weight: normal;">[!DNL Workfront] calcula o valor total de Custos de uma iniciativa usando esta fórmula:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custos Fixos]</td> 
   <td> <p><span style="font-weight: normal;">Esta é uma entrada manual em que você pode estimar <span>uma quantidade mensal de Custos fixos para cada mês da iniciativa.</span> Isso não inclui os custos associados às funções adicionadas à iniciativa que são capturadas no campo [!UICONTROL Custo de Pessoas].</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custos de Pessoas]</td> 
   <td> <p style="font-weight: normal;">É um cálculo total dos custos associados às funções de trabalho da iniciativa durante a sua duração. Esse número depende de quantos FTEs ou horas você estima para uma função de trabalho para cada mês da iniciativa. </p> 
     <p><b>DICAS</b>  
     <ul> 
      <li> <p>O número de FTEs mensais para a mesma função de trabalho pode ser diferente de mês para mês.</p> </li> 
      <li> <p>[!DNL Workfront] considera que existem 160 horas de trabalho num mês. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] calcula os [!UICONTROL Custos de Pessoas] de uma iniciativa usando a seguinte fórmula:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] calcula os Custos Mensais com Pessoas para cada mês durante a duração da Iniciativa usando a seguinte fórmula:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>EXEMPLO</b></p>
      <p>Se você tiver uma iniciativa com uma duração de 6 meses que exija uma Designer com uma taxa horária de US$ 50 por mês para 1 FTE e uma Web Designer com uma taxa horária de US$ 100 por 2 meses da iniciativa, os Custos de pessoas da iniciativa serão calculados da seguinte maneira:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benefício Planejado]</td> 
   <td>Esta é uma entrada manual na qual você pode estimar o benefício geral que seu departamento ganharia ao concluir esta iniciativa. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor Líquido]</td> 
   <td> <p style="font-weight: normal;">Isso representa o valor da sua iniciativa quando leva em conta os custos gerais e o Benefício Planejado estimado na iniciativa. [!DNL Workfront] calcula o Valor líquido de uma iniciativa usando a seguinte fórmula:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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

## Informações da iniciativa em relatórios

É possível exibir informações da iniciativa em relatórios, conforme descrito na tabela abaixo. Essas informações estão disponíveis na instância do Workfront somente quando sua empresa adquiriu uma licença do Planejador de cenários da Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Tipo de relatório</b></td> 
   <td><b>Informações da iniciativa</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Iniciativa] </td> 
   <td>Nome, Duração, Datas de início e término, Informado por, ID, Data da última publicação*, Todos os campos do projeto, incluindo campos personalizados*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Função de Trabalho da Iniciativa]</td> 
   <td>Todas as informações da iniciativa conforme listado acima, ID (função de trabalho), Projeto*, Horas planejadas de atribuição do projeto*, Horas de função de trabalho da iniciativa, Contagem (função de trabalho), Todos os campos do projeto, incluindo campos personalizados*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Projeto]*</p></td> 
   <td> <p>Todas as informações da iniciativa conforme listado acima*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Esses campos são preenchidos com informações do projeto vinculadas à iniciativa, somente quando a iniciativa foi criada a partir de um projeto ou foi publicada em um projeto pelo menos uma vez. Para obter informações sobre como publicar iniciativas, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
