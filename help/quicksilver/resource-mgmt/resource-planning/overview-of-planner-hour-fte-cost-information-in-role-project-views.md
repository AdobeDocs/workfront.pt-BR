---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos
description: Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2973'
ht-degree: 0%

---

# Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

A orçamentação dos recursos para o trabalho que devem realizar em um projeto é a função principal do Planejador de Recursos. Você pode visualizar o tempo disponível dos recursos, bem como alocar seu tempo para os projetos nos quais eles são atribuídos.

Para obter informações sobre como orçar recursos no Planejador de Recursos, consulte [Recursos de orçamento no Planejador de Recursos usando as exibições Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

Este artigo descreve alguns dos principais conceitos que você precisa saber antes de começar a orçar seus recursos no Planejador de Recursos.

## Visão geral dos recursos de orçamento

Considere o seguinte ao orçar recursos usando o Planejador de Recursos:

* Você pode orçar a alocação de seus recursos especificando uma quantidade de Horas, FTE ou Custo que seus recursos podem usar para concluir o trabalho em projetos. Ao calcular o tempo ou o custo de um recurso, as Horas Disponíveis, o FTE ou o Custo do recurso diminuem de acordo com a quantia orçada. Como resultado, os valores Horas Disponíveis, FTE ou Custo dos projetos que seguem o projeto para o qual você está orçando diminuições para esses usuários e funções nesses projetos.

   >[!IMPORTANT]
   >
   >Você pode orçar seus recursos por um período de 15 anos. Se você orçar recursos para um projeto com uma duração superior a 15 anos, as informações de orçamento podem não ser precisas.

* Você pode orçar Horas, FTE ou Custo dos recursos por qualquer período exibido no Planejador de Recursos, independentemente da linha do tempo do projeto. Por exemplo, se você quiser indicar que seus recursos podem não estar disponíveis durante a linha do tempo do projeto (onde estão associados às Horas Planejadas), mas podem estar disponíveis durante outro tempo, faça isso orçando-os para períodos de tempo em que as Horas Planejadas sejam zero, se isso for quando estiverem disponíveis para trabalhar. Depois disso, é possível alterar manualmente a linha do tempo do projeto para corresponder à disponibilidade dos recursos.

   >[!NOTE]
   >
   >Recomendamos que você faça manualmente o orçamento de Horas, FTE ou Custo para funções de trabalho ou para usuários primeiro. Você pode usar as opções automáticas para orçar tempo para seus projetos e recursos somente quando tiver certeza de que a quantidade de Horas Planejadas, FTE ou Custo sempre deve corresponder às Horas, FTE ou Custo Orçados.\
   >Para obter informações sobre o uso das opções automáticas para orçamento no Planejador de Recursos, consulte a seção &quot;Projeto de orçamento e funções automaticamente&quot; no artigo [Revise a disponibilidade e alocação de recursos usando o Adobe Workfront Resource Planner](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* O FTE ou os custos do orçamento são idênticos às horas do orçamento, em que o Adobe Workfront usa o FTE e os valores de custo em vez de horas para os recursos do orçamento.

   Para obter mais informações sobre como entender como os Custos são calculados no Planejador de Recursos, consulte [Calcular custos no Planejador de Recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* As alocações orçamentárias para seus recursos no Planejador de Recursos são feitas das seguintes maneiras:

   * Manualmente

      Ou

   * Automaticamente, usando as opções de projeto e função na **Exibir por projeto** e **Exibir por função** exibições.
   Para obter mais informações, consulte [Recursos de orçamento no Planejador de Recursos usando as exibições Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Quando um usuário altera funções de trabalho, é excluído, desativado ou removido de um Pool de Recursos, as horas orçadas para a função não são alteradas e são redistribuídas para os usuários restantes na função. Se nenhum usuário estiver mais associado à função de trabalho, as Horas Orçadas da função se tornarão zero.

Para obter mais informações sobre as opções de projeto e função, consulte a seção [Entender os valores de Horas, FTE e Custo no Planejador de Recursos](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) neste artigo.

## Entender os valores de Horas, FTE e Custo no Planejador de Recursos {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Antes de orçar seus recursos e atualizar as informações de Horas Orçadas no Planejador de Recursos, você deve estar familiarizado com os seguintes conceitos

* **Horas, FTE ou Custo Planejado**: O trabalho que precisa ser feito conforme definido em tarefas e problemas.
* **Horas, FTE ou Custo Disponíveis**: A quantidade de tempo que os usuários ou as funções do job estão disponíveis para trabalhar, de acordo com as programações associadas aos usuários.

Essas informações são exibidas no Planejador de Recursos para cada recurso (usuário ou função) e para cada projeto.

Para obter informações sobre o que é exibido nas Exibições de Projeto e Função do projeto, consulte o artigo [Visão geral da navegação do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Para obter informações sobre como entender como os Custos são calculados no Planejador de Recursos, consulte o artigo [Calcular custos no Planejador de Recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>O orçamento por Custo é idêntico ao orçamento por Horas ou FTE, mas você deve entender como o Workfront calcula o Custo para o Planejador de Recursos.
>
>Para obter informações sobre como os custos são calculados no Planejador de Recursos, consulte o artigo [Calcular custos no Planejador de Recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

As tabelas a seguir mostram as informações de alocação e disponibilidade exibidas no Planejador de Recursos ao aplicar a visualização Projeto ou Função. Você pode exibir essas informações por Horas, FTE ou Custo:

* [A coluna AVL (Disponível)](#the-avl-available-column)
* [Coluna PLN (planejada)](#the-pln-planned-column)
* [A coluna BDG (Orçada)](#the-bdg-budgeted-column)
* [A coluna VAR (Variância)](#the-var-variance-column)
* [A coluna NET](#the-net-column)

### A coluna AVL (Disponível) {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td><strong>Descrição</strong> </td> 
  </tr> 
  <tr> 
   <td>Projeto </td> 
   <td> <p>O total de Horas, FTEs ou Custo para o qual todos os usuários do projeto estão disponíveis para trabalhar de acordo com sua programação, para o período selecionado. </p> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>O total de Horas, FTEs ou Custo para o qual todos os usuários associados a essa função estão disponíveis para trabalhar de acordo com sua programação e seus <strong>Porcentagem de disponibilidade de FTE</strong> para essa função específica, para o período selecionado. </p> <p>Considere o seguinte: </p> 
    <ul> 
     <li>Se nenhum usuário estiver associado a uma função de trabalho, o valor das Horas Disponíveis para a função de trabalho será zero. </li> 
     <li>Se um usuário estiver associado a uma Função de Trabalho Principal, mas a variável <strong>Porcentagem de disponibilidade de FTE</strong> para a função for 0%, o valor Horas Disponíveis da função de trabalho é zero.</li> 
     <li>Se o usuário estiver associado a Outras funções e a <strong>Porcentagem de disponibilidade de FTE</strong> para as funções for 0%, as Outras Funções não serão listadas no Planejador de Recursos e o usuário será exibido somente em sua Função Principal.</li> 
    </ul> <p>Para obter mais informações sobre o <strong>Porcentagem de disponibilidade de FTE</strong> para obter uma função, consulte o artigo <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a>.</p> <p>Para obter mais informações sobre como a disponibilidade da função de trabalho é calculada no Planejador de Recursos, consulte a seção "Calcular as Horas e o FTE disponíveis para uma função de trabalho no Planejador de Recursos" no artigo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>Horas, FTEs ou Custo que o usuário está disponível para trabalhar, de acordo com sua programação, para o período selecionado. Esse número subtrai as horas associadas ao seguinte:</p> 
    <ul> 
     <li>exceções de programação</li> 
     <li>tempo limite do usuário</li> 
     <li>horas orçamentadas para outros projetos. </li> 
    </ul> <p>As Horas, FTEs ou Custo Disponíveis para um usuário mudam de acordo com o seguinte: </p> 
    <ul> 
     <li>como a programação e o FTE são calculados com base nas Preferências de Gerenciamento de Recursos no nível do sistema.<br><p>Para obter mais informações sobre o cálculo da disponibilidade de usuário e função de trabalho, consulte o artigo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos</a>.</p>
     Para obter mais informações sobre como configurar preferências de Gerenciamento de Recursos no Workfront, consulte <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências do Gerenciamento de recursos</a></li> 
    </ul> 
    <ul> 
     <li>o <strong>Prioridade de planejamento do projeto</strong>, se o usuário estiver orçado para trabalho.<br>Para obter mais informações sobre como a Prioridade de planejamento de projeto afeta as Horas Disponíveis de um usuário, consulte <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Visão geral da navegação do Planejador de recursos </a>. </li> 
    </ul> <p>Se o usuário estiver programado para desativação, as Horas Disponíveis, FTEs ou Custo para os dias após a data de desativação serão zero. <br>Para obter mais informações sobre como desativar usuários, consulte o artigo <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Coluna PLN (planejada) {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td><strong>Descrição</strong> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td> <p>O total de Horas Planejadas, FTEs ou Custo de todas as funções ou usuários de trabalho listados no projeto, incluindo no <strong>Sem função</strong> ou <strong>Sem usuário</strong> para o período selecionado e como exibido na guia Detalhes do projeto do projeto. </p> <p><b>Nota</b>

Ajustes manuais de alocações diárias de usuários podem alterar o valor semanal, mensal ou trimestral de Horas Planejadas no Planejador de Recursos. É possível ajustar manualmente as alocações diárias de usuários para tarefas e problemas usando o Balanceador de Carga de Trabalho. Para obter mais informações, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuários no Balanceador de Carga de Trabalho</a>.</p> </td>
</tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>O total de Horas Planejadas de todas as tarefas atribuídas à função, durante o período selecionado. </p> <p>O <strong>Sem função</strong> exibirá as Horas Planejadas associadas às tarefas que não foram atribuídas, atribuídas a equipes (cujas horas são listadas na seção <strong>Sem usuário</strong> ) ou atribuídas a usuários que não estão associados a uma função de trabalho. </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>As Horas Planejadas de todas as tarefas atribuídas ao usuário em uma função específica, durante o período selecionado. </p> <p>O <strong>Sem usuário</strong> exibirá as Horas Planejadas associadas às tarefas que não estão atribuídas ou atribuídas às equipes. </p> </td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte ao exibir as Horas Planejadas:

* Embora você não possa ver informações sobre alocações de tarefas no Planejador de Recursos nas exibições Projeto e Função, a quantidade de Horas Planejadas vem das Horas Planejadas nas tarefas dos projetos.
* As Horas Planejadas são igualmente distribuídas para cada dia dentro da Duração das tarefas, para cada recurso atribuído a elas. A tarefa Duração é baseada na tarefa Datas de Início e Conclusão Planejadas e inclui todos os dias de calendário dentro desse período de tempo.\
   A Workfront leva em conta o agendamento do usuário ou do projeto ao distribuir as Horas Planejadas para usuários ou projetos. Nesse caso, as Horas Planejadas são igualmente distribuídas para cada dia dentro da Duração das tarefas, excluindo fins de semana, dias de folga e exceções de programação.\
   Por exemplo, se você exibir o Planejador de Recursos por Semana e tiver tarefas que abrangem várias semanas em projetos, o número de Horas Planejadas por semana dependerá do número de dias nessa semana que fazem parte da Duração da tarefa. Isso funciona de forma semelhante ao exibir o Planejador de Recursos por Mês ou Trimestre e quando as tarefas abrangem vários meses ou trimestres.\
   Dias de fim de semana, exceções de agendamento e dias de folga são excluídos desta distribuição.
* As seguintes categorias de tarefas são incluídas no cálculo das Horas Planejadas para cada recurso:

   * tarefas atribuídas a usuários em Grupos de Recursos, funções de trabalho ou equipes no projeto\
      Se tarefas forem atribuídas a equipes, sua alocação será exibida em **Sem função** e **Sem usuário** seções. Você pode ver as Horas Planejadas associadas às equipes, mas não pode calcular as horas, pois nenhuma função ou usuário está associado às tarefas.

   * tarefas não atribuídas

* As Horas Planejadas no Planejador de Recursos não incluem as Horas Planejadas associadas ao seguinte:

   * tarefas pai
   * tarefas atribuídas a usuários sem pools de recursos
   * problemas, quando a variável **Incluir horas de problemas** está desativada.

* As Horas Planejadas não são exibidas no Planejador de Recursos se a tarefa Duração for zero.
* As Horas Planejadas associadas a usuários desativados não são exibidas.

### A coluna BDG (Orçada) {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td><strong>Descrição</strong> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td> <p>Uma entrada manual para estimar quantas horas, FTE ou Custo você orçou para um projeto, para um período selecionado. </p> <p>Na exibição Projeto, as horas que você orçar para o projeto são distribuídas para as funções de trabalho listadas no projeto. A quantidade de Horas Planejadas para cada função determina como as Horas Orçadas são distribuídas para as funções. As Horas Orçadas são distribuídas para as funções com valores de Horas Planejadas mais altos. </p> <p>Na exibição Função, as horas que você orçou para o projeto não são distribuídas para as funções ou para os usuários do projeto. </p> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>Uma entrada manual para estimar quantas horas você orçou para uma função, para um período selecionado. </p> <p>Se nenhum usuário estiver associado à função de cargo, você não poderá estimar as Horas Orçadas para a função de cargo. </p> <p>Na exibição Função, as horas que você orçou para a função são distribuídas para os projetos listados na função. A quantidade de Horas Planejadas para cada projeto determina como as Horas Orçadas são distribuídas aos projetos. As Horas Orçamentadas são distribuídas aos projetos com valores de Horas Planejadas mais altos.</p> <p>Na exibição Projeto, as horas que você orçou para a função não são distribuídas aos projetos ou aos usuários associados à função. </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>Uma entrada manual para estimar quantas horas você orçou para um usuário, para um período selecionado. </p> <p> <p><b>OBSERVAÇÃO</b>   Você pode fazer uma estimativa das Horas Orçadas para usuários que não estão atribuídos a tarefas, mas que estão associados a um Pool de Recursos em um projeto porque esses usuários também aparecem no Planejador de Recursos. Suas Horas Planejadas devem ser zero, no entanto, se não forem atribuídas a tarefas. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte ao trabalhar com Horas Orçadas:

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* Você pode orçar recursos somente quando tiver permissões Editar acesso ao Gerenciamento de Recursos e Dados Financeiros e Gerenciar Finanças nos projetos.

   Para obter informações sobre o acesso necessário para recursos de orçamento, consulte o artigo [Acesso necessário para recursos de orçamento no Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Por padrão, as Horas Orçadas no Planejador de Recursos são zero para todos os recursos e para todos os projetos.
* Você pode estimar manualmente as Horas Orçadas para usuários e funções, ou pode usar um dos links na Função do Projeto ou da Tarefa **Mais** para atualizá-los de acordo com o número de Horas Planejadas.\
   Para obter mais informações sobre as opções de projeto e função, consulte a seção [Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos](#Budget) neste artigo.

* O menor período de tempo para o qual você pode orçar horas, FTE ou Custo é uma semana. Não é possível orçar horas, FTE ou Custo por dia.
* As Horas Orçadas são igualmente distribuídas para cada dia dentro da Duração das tarefas, para cada recurso atribuído a elas. A tarefa Duração é baseada na tarefa Datas de Início e Conclusão Planejadas e inclui todos os dias de calendário dentro desse período de tempo.\
   O Workfront leva em conta a programação do usuário ou do projeto ao distribuir as Horas Orçadas aos usuários ou projetos. Nesse caso, as Horas Orçamentadas são igualmente distribuídas para cada dia dentro da Duração das tarefas, excluindo fins de semana, mas incluindo exceções de tempo limite e programação.\
   Se você exibir o Planejador de Recursos por Semana, por exemplo, e tiver tarefas que abrangem várias semanas, o número de Horas Orçadas por semana dependerá do número de dias nessa semana que fazem parte da Duração da tarefa. Os dias de fim de semana são excluídos desta distribuição. Isso funciona de forma semelhante ao exibir o Planejador de Recursos por Mês ou Trimestre e quando as tarefas abrangem vários meses ou trimestres.

* Você pode gerar relatórios sobre Horas Orçadas, selecionando Hora Orçadas como o objeto de relatório para um novo relatório.\
   Para obter informações sobre quais objetos você pode criar relatórios no Workfront, consulte a seção &quot;Relatório sobre objetos&quot; no artigo [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
   Para obter informações sobre como criar um relatório de Hora do Orçamento, consulte o artigo [Relatório: Hora do Orçamento](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* As horas anteriormente orçadas para usuários que foram desativados posteriormente não são exibidas.

### A coluna VAR (Variância) {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td><strong>Descrição</strong> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td> <p>A Variação de Hora, FTE ou Custo mostra se você tem Horas Orçadas suficientes para que o projeto realize todas as Horas Planejadas do projeto. </p> <p>A Hora do projeto, FTE ou Variação de custo é calculada usando a seguinte fórmula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>A Variação de Hora, FTE ou Custo mostra se você tem Horas Orçadas, FTE ou Custo suficientes para que a função possa realizar as Horas Planejadas atribuídas a ela. </p> <p>A Função Hora, FTE ou Variação de Custo é calculada usando a seguinte fórmula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>A Variação de Horas, FTE ou Custo mostra se você tem Horas Orçadas suficientes para que o usuário realize as Horas Planejadas atribuídas a ele. </p> <p>O Horário do Usuário, FTE ou Variação de Custo é calculado usando a seguinte fórmula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando as Horas, FTE ou Variação de Custo são exibidas em vermelho, você estimou menos Horas Orçadas do que as Horas Planejadas do trabalho real que precisa ser concluído. Neste caso, as Horas Orçamentadas poderão não ser suficientes para concluir o trabalho.

### A coluna NET  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Exibido por</strong> </td> 
   <td><strong>Descrição</strong> </td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td> 
    <div> 
     <p>O projeto Horas Líquidas, FTE ou Custo pode mostrar um dos seguintes itens: </p> 
     <ul> 
      <li> <p>A diferença entre o tempo ou custo Disponível e o tempo ou custo orçado do projeto:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>A diferença entre o tempo ou custo disponível e o tempo ou custo planejado para o projeto, quando os valores de Uso planejado (PLN) na configuração de cálculos LÍQUIDOS são ativados: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>DICA</b></p>        
  <p>Essa opção é aplicada somente quando você personaliza a exibição na seção Exibir itens selecionados .</p>
  <p>Para obter mais informações, consulte <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Revise a disponibilidade e alocação de recursos usando o Adobe Workfront Resource Planner</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> 
    <div> 
     <p>A função Hora líquida, FTE ou Custo pode mostrar um dos seguintes: </p> 
     <ul> 
      <li> <p>A diferença entre o tempo ou custo Disponível e o tempo ou custo Orçado para a função:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>A diferença entre o tempo ou custo Disponível e o tempo ou custo planejado para a função, quando os valores de Uso Planejado (PLN) na configuração de cálculos LÍQUIDOS são ativados:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>DICA</b> <span>

Essa opção é aplicada somente quando você personaliza a exibição na seção Exibir itens selecionados .</span> </p> <p><span>Para obter mais informações, consulte </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Revise a disponibilidade e alocação de recursos usando o Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Usuário</td> 
   <td> 
    <div> 
     <p>O usuário Net Hours, FTE ou Cost pode exibir um dos seguintes itens: </p> 
     <ul> 
      <li> <p>A diferença entre o tempo ou custo Disponível e o tempo ou custo Orçado para o usuário:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>A diferença entre o tempo ou custo Disponível e o tempo ou custo planejado para o usuário, quando os valores de Uso Planejado (PLN) na configuração de cálculos LÍQUIDOS são ativados:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>DICA</b> <span>

Essa opção é aplicada somente quando você personaliza a exibição na seção Exibir itens selecionados .</span> </p> <p><span>Para obter mais informações, consulte </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Revise a disponibilidade e alocação de recursos usando o Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Quando o NET Hours, FTE ou Custo é exibido em vermelho, não há tempo ou orçamento disponível suficiente para cobrir o Orçamento** ou o tempo ou custo planejado associado ao trabalho. Nesse caso, os recursos são sobrealocados.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
