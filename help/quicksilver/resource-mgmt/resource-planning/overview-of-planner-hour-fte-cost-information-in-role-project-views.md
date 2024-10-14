---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: Visão Geral das Informações de Horas, FTE e Custo nas Visualizações de Projeto e Função do Planejador de Recursos
description: Visão geral de horas, FTE e informações de custo nas visualizações Projeto e Função do Planejador de recursos
author: Lisa
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 2ccf2775a858371aacdb6e8637fd5a30a212a82d
workflow-type: tm+mt
source-wordcount: '2977'
ht-degree: 0%

---

# Visão geral de horas, FTE e informações de custo nas visualizações Projeto e Função do Planejador de recursos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

Orçar seus recursos pelo trabalho que devem realizar em um projeto é a principal função do Planejador de recursos. Você pode visualizar o tempo disponível dos seus recursos, bem como alocar o tempo deles para os projetos em que são atribuídos.

Para obter informações sobre recursos de orçamento no Planejador de recursos, consulte [Recursos de orçamento no Planejador de recursos usando as exibições de Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

Este artigo descreve alguns dos principais conceitos que você precisa conhecer antes de começar a fazer o orçamento de seus recursos no Planejador de recursos.

## Visão geral dos recursos de orçamento

Considere o seguinte ao estimar recursos usando o Planejador de Recursos:

* Você pode estimar a alocação de seus recursos especificando uma quantidade de Horas, FTE ou Custo que seus recursos podem usar para concluir o trabalho nos projetos. Quando você faz o orçamento de tempo ou custo de um recurso, as Horas Disponíveis, FTE ou Custo do recurso diminuem pela quantia prevista em orçamento. Como resultado, os valores de Horas Disponíveis, FTE ou Custo para os projetos que seguem o projeto para o qual você está fazendo o orçamento diminuem para esses usuários e funções nesses projetos.

  >[!IMPORTANT]
  >
  >Você pode estimar seus recursos por um período de 15 anos. Se você orçar recursos para um projeto com duração superior a 15 anos, as informações de orçamento podem não ser precisas.

* Você pode estimar Horas, FTE ou Custo para seus recursos para qualquer intervalo de tempo exibido no Planejador de recursos, independentemente da linha do tempo do projeto. Por exemplo, se você quiser indicar que seus recursos podem não estar disponíveis durante a linha do tempo do projeto (em que estão associados às Horas planejadas), mas podem estar disponíveis durante outro tempo, você pode fazer isso orçando-os para períodos em que as Horas planejadas são zero, se for quando elas estiverem disponíveis para trabalhar. Você pode alterar manualmente a linha do tempo do projeto para corresponder à disponibilidade de recursos depois de fazer isso.

  >[!NOTE]
  >
  >Recomendamos que você faça um orçamento manual de Horas, FTE ou Custo para funções de trabalho ou para usuários primeiro. Você pode usar as opções automáticas para estimar o tempo de seus projetos e recursos apenas quando tiver certeza de que a quantia de Horas Planejadas, FTE ou Custo deve sempre corresponder às Horas Orçadas, FTE ou Custo.\
  >Para obter informações sobre como usar as opções automáticas para orçamento no Planejador de Recursos, consulte a seção &quot;Budget project and roles automatically&quot; no artigo [Revise a disponibilidade e a alocação de recursos usando o Planejador de Recursos da Adobe Workfront](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* O orçamento de FTE ou custos é idêntico às horas de orçamento, em que o Adobe Workfront usa os valores de FTE e custo em vez de horas para os recursos orçados.

  Para obter mais informações sobre como entender como os custos são calculados no Planejador de recursos, consulte [Calcular custos no Planejador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* A alocação de orçamento para seus recursos no Planejador de recursos é feita das seguintes maneiras:

   * Manual

     Ou

   * Automaticamente, usando as opções de projeto e função nos modos de exibição **Exibir por Projeto** e **Exibir por Função**.

  Para obter mais informações, consulte [Recursos de orçamento no Planejador de recursos usando as exibições de Projeto e Função](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* Quando um usuário altera funções de trabalho, é excluído, desativado ou removido de um Conjunto de recursos, as horas orçadas para a função não são alteradas e são redistribuídas aos usuários restantes na função. Se nenhum usuário estiver mais associado à função de trabalho, as horas orçadas para a função se tornarão zero.

Para obter mais informações sobre as opções de projeto e função, consulte a seção [Entender os valores de Horas, FTE e Custo no Planejador de Recursos](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) neste artigo.

## Compreender os valores de Horas, FTE e Custo no Planejador de Recursos {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

Antes de elaborar o orçamento de seus recursos e atualizar as informações de Horas orçadas no Planejador de recursos, você deve estar familiarizado com os seguintes conceitos

* **Horas planejadas, FTE ou Custo**: o trabalho que precisa ser feito conforme definido em tarefas e problemas.
* **Horas Disponíveis, FTE ou Custo**: a quantidade de tempo em que os usuários ou funções de trabalho estão disponíveis para trabalhar, de acordo com os agendamentos associados aos usuários.

Estas informações são exibidas no Planejador de recursos para cada recurso (usuário ou função) e para cada projeto.

Para obter informações sobre o que é exibido nas Exibições de Projeto e Função do projeto, consulte o artigo [Visão geral da navegação do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

Para obter informações sobre como entender como os custos são calculados no Planejador de recursos, consulte o artigo [Calcular custos no Planejador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>O orçamento por custo é idêntico ao orçamento por horas ou FTE, mas você deve entender como o Workfront calcula o custo para o Planejador de recursos.
>
>Para obter informações sobre como os custos são calculados no Planejador de recursos, consulte o artigo [Calcular custos no Planejador de recursos](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

As tabelas a seguir mostram as informações de alocação e disponibilidade exibidas no Planejador de recursos ao aplicar a visualização Projeto ou Função. É possível exibir essas informações por Horas, FTE ou Custo:

* [A coluna AVL (Disponível)](#the-avl-available-column)
* [A coluna PLN (Planejado)](#the-pln-planned-column)
* [A coluna BDG (Orçada)](#the-bdg-budgeted-column)
* [A coluna VAR (Variação)](#the-var-variance-column)
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
   <td> <p>O total de Horas, FTEs ou Custo para o qual todos os usuários do projeto estão disponíveis para trabalhar de acordo com seu cronograma, para o período selecionado. </p> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>O total de Horas, FTEs ou Custo para o qual todos os usuários associados a esta função estão disponíveis para trabalhar de acordo com seu cronograma e sua <strong>Porcentagem de Disponibilidade de FTE</strong> para a função específica, para o período selecionado. </p> <p>Considere o seguinte: </p> 
    <ul> 
     <li>Se nenhum usuário estiver associado a uma função de trabalho, o valor das Horas Disponíveis para a função de trabalho será zero. </li> 
     <li>Se um usuário estiver associado a uma Função de Trabalho Principal, mas a <strong>Porcentagem de Disponibilidade de FTE</strong> para a função for 0%, o valor Horas Disponíveis da função de trabalho será zero.</li> 
     <li>Se o usuário estiver associado a Outras Funções e o <strong>Percentual de Disponibilidade de FTE</strong> para as funções for 0%, as Outras Funções não serão listadas no Planejador de Recursos e o usuário será exibido somente em sua Função Principal.</li> 
    </ul> <p>Para obter mais informações sobre a <strong>Porcentagem de Disponibilidade de FTE</strong> para uma função de trabalho, consulte o artigo <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de um usuário</a>.</p> <p>Para obter mais informações sobre como a disponibilidade de funções de trabalho é calculada no Planejador de Recursos, consulte a seção "Calcular as Horas Disponíveis e o FTE para uma função de trabalho no Planejador de Recursos" no artigo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de Recursos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>Horas, FTEs ou Custo em que o usuário está disponível para trabalhar, de acordo com seu cronograma, para o período selecionado. Esse número subtrai as horas associadas ao seguinte:</p> 
    <ul> 
     <li>exceções de programação</li> 
     <li>tempo de folga do usuário</li> 
     <li>horas orçadas para outros projetos. </li> 
    </ul> <p>As Horas Disponíveis, FTEs ou Custo para um usuário são alterados de acordo com o seguinte: </p> 
    <ul> 
     <li>como a programação e o FTE são calculados com base nas Preferências de gerenciamento de recursos no nível do sistema.<br><p>Para obter mais informações sobre o cálculo da disponibilidade de usuários e funções de trabalho, consulte o artigo <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Visão geral do cálculo de horas e FTE para usuários e funções no Planejador de recursos</a>.</p>
     Para obter mais informações sobre como configurar preferências de Gerenciamento de Recursos no Workfront, consulte <a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configurar preferências de Gerenciamento de Recursos</a></li> 
    </ul> 
    <ul> 
     <li>a <strong>Prioridade de Planejamento do Projeto</strong>, se o usuário estiver orçado para trabalho.<br>Para obter mais informações sobre como a Prioridade de Planejamento de Projeto afeta as Horas Disponíveis de um usuário, consulte <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Visão geral da navegação do Planejador de Recursos </a>. </li> 
    </ul> <p>Se o usuário estiver programado para desativação, as Horas Disponíveis, os FTEs ou o Custo para os dias após a data de desativação serão zero. <br>Para obter mais informações sobre como desativar usuários, consulte o artigo <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Desativar ou reativar um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>



### A coluna PLN (Planejado) {#the-pln-planned-column}

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
   <td> <p>O total de Horas Planejadas, FTEs ou Custo de todas as funções de trabalho ou usuários listados no projeto, incluindo nas seções <strong>Nenhuma Função</strong> ou <strong>Nenhum Usuário</strong>, para o período selecionado e conforme exibido na guia Detalhes do Projeto do projeto. </p> <p><b>Nota</b>

Os ajustes manuais das alocações diárias de usuários podem alterar o valor semanal, mensal ou trimestral das Horas Planejadas no Planejador de Recursos. Você pode ajustar manualmente as alocações diárias de usuários para tarefas e problemas usando o Balanceador de carga de trabalho. Para obter mais informações, consulte <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">Gerenciar alocações de usuário no Balanceador de carga de trabalho</a>.</p> </td>
</tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>O total de Horas Planejadas de todas as tarefas atribuídas à função, durante o período selecionado. </p> <p>A seção <strong>Sem Função</strong> mostrará as Horas Planejadas associadas às tarefas que não estão atribuídas, atribuídas a equipes (cujas horas estão listadas na seção <strong>Sem Usuário</strong>) ou atribuídas a usuários que não estão associados a uma função de trabalho. </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>As horas planejadas de todas as tarefas atribuídas ao usuário em uma função específica, durante o período selecionado. </p> <p>A seção <strong>Nenhum usuário</strong> mostrará as Horas planejadas associadas às tarefas que não foram atribuídas ou estão atribuídas a equipes. </p> </td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte ao exibir as Horas planejadas:

* Embora não seja possível ver as informações sobre alocações de tarefas no Planejador de recursos nas visualizações Projeto e Função, a quantidade de Horas planejadas vem das Horas planejadas nas tarefas nos projetos.
* As horas planejadas são distribuídas igualmente a cada dia dentro da duração das tarefas, para cada recurso atribuído a elas. A duração da tarefa é baseada nas datas planejadas de início e conclusão da tarefa e inclui todos os dias dentro desse período de tempo.\
  O Workfront leva em conta a programação do usuário ou do projeto ao distribuir Horas planejadas aos usuários ou projetos. Nesse caso, as Horas planejadas são distribuídas igualmente a cada dia dentro da Duração das tarefas, excluindo fins de semana, dias de folga e exceções de programação.\
  Se você exibir o Planejador de recursos por semana, por exemplo, e tiver tarefas que abrangem várias semanas em projetos, o número de Horas planejadas por semana dependerá de quantos dias nessa semana fazem parte da Duração da tarefa. Isso funciona de forma semelhante ao exibir o Planejador de recursos por mês ou trimestre e quando as tarefas abrangem vários meses ou trimestres.\
  Os dias de fim de semana, as exceções de programação e os dias de folga são excluídos desta distribuição.
* As seguintes categorias de tarefas são incluídas no cálculo das Horas planejadas para cada recurso:

   * tarefas atribuídas a usuários em Conjuntos de Recursos, funções de trabalho ou equipes no projeto\
     Se tarefas forem atribuídas a equipes, sua alocação aparecerá nas seções **Sem Função** e **Sem Usuário**. Você pode ver as Horas planejadas associadas com as equipes, mas não pode estimar as horas, porque nenhuma função ou usuário está associado com as tarefas.

   * tarefas não atribuídas

* As horas planejadas no Planejador de recursos não incluem as horas planejadas associadas com o seguinte:

   * tarefas pai
   * tarefas atribuídas a usuários sem Conjuntos de Recursos
   * problemas, quando a configuração **Incluir horas a partir de Problemas** estiver desativada.

* As horas planejadas não são exibidas no Planejador de recursos se a duração da tarefa for zero.
* As horas planejadas associadas a usuários desativados não são exibidas.

### A coluna BDG (Orçado) {#the-bdg-budgeted-column}

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
   <td> <p>Uma entrada manual para estimar quantas horas, FTE ou Custo você prevê em orçamento para um projeto, para um intervalo de tempo selecionado. </p> <p>Na visualização Projeto, as horas orçadas para o projeto são distribuídas às funções de trabalho listadas no projeto. A quantidade de Horas planejadas para cada função determina como as Horas orçadas são distribuídas para as funções. As horas orçadas são distribuídas para as funções com valores mais altos de Horas planejadas. </p> <p>Na visualização Função, as horas orçadas para o projeto não são distribuídas às funções ou aos usuários no projeto. </p> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>Uma entrada manual para estimar quantas horas você faz um orçamento para uma função, para um período selecionado. </p> <p>Se nenhum usuário estiver associado à função de trabalho, você não poderá estimar as Horas orçadas para a função de trabalho. </p> <p>Na visualização Função, as horas orçadas para a função são distribuídas aos projetos listados na função. A quantidade de Horas Planejadas para cada projeto determina como as Horas Orçadas são distribuídas aos projetos. As horas orçadas são distribuídas aos projetos com valores de horas planejadas mais altos.</p> <p>Na exibição Projeto, as horas orçadas para a função não são distribuídas aos projetos ou usuários associados à função. </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>Uma entrada manual para estimar quantas horas você calcula para um usuário, para um intervalo de tempo selecionado. </p> <p> <p><b>OBSERVAÇÃO</b>   Você pode estimar as horas orçadas para usuários que não estão atribuídos a tarefas, mas que estão associados a um Conjunto de recursos em um projeto porque esses usuários também aparecem no Planejador de recursos. Suas horas planejadas devem ser zero, no entanto, se não estiverem atribuídas a tarefas. </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Considere o seguinte ao trabalhar com Horas orçadas:

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* Você pode estimar recursos somente quando tem acesso de Edição a Gerenciamento de Recursos e Dados Financeiros e de Gerenciamento de Permissões financeiras nos projetos.

  Para obter informações sobre o acesso necessário para recursos de orçamento, consulte o artigo [Acesso necessário para recursos de orçamento no Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* Por padrão, as horas orçadas no Planejador de recursos são zero para todos os recursos e para todos os projetos.
* Você pode estimar manualmente as Horas Orçadas para usuários e funções, ou pode usar um dos links nos menus Projeto ou Função **Mais** para atualizá-las de acordo com o número de Horas Planejadas.\
  Para obter mais informações sobre as opções de projeto e função, consulte a seção [Visão geral de horas, FTE e informações de custo nas exibições de Projeto e Função do Planejador de Recursos](#Budget) neste artigo.

* O menor período para o qual você pode estimar horas, FTE ou Custo é uma semana. Você não pode estimar horas, FTE ou Custo para um dia.
* As horas orçadas são distribuídas igualmente a cada dia dentro da Duração de tarefas, para cada recurso atribuído a elas. A duração da tarefa é baseada nas datas planejadas de início e conclusão da tarefa e inclui todos os dias dentro desse período de tempo.\
  O Workfront leva em conta a programação do usuário ou do projeto ao distribuir Horas orçadas a usuários ou projetos. Nesse caso, as horas orçadas são distribuídas igualmente a cada dia dentro da Duração de tarefas, excluindo fins de semana, mas incluindo exceções de folga e agendamento.\
  Se você exibir o Planejador de Recursos por Semana, por exemplo, e tiver tarefas que abrangem várias semanas, o número de Horas Orçadas por semana dependerá de quantos dias dentro dessa semana fazem parte da Duração da tarefa. Os dias de fim de semana são excluídos desta distribuição. Isso funciona de forma semelhante ao exibir o Planejador de recursos por mês ou trimestre e quando as tarefas abrangem vários meses ou trimestres.

* Você pode criar relatórios sobre Horas orçadas selecionando Hora orçada como seu objeto de relatório para um novo relatório.\
  Para obter informações sobre quais objetos você pode relatar no Workfront, consulte a seção &quot;Relatório sobre objetos&quot; no artigo [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
  Para obter informações sobre como criar um relatório de Horas orçadas, consulte o artigo [Relatório: Hora orçada](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* As horas orçadas anteriormente para usuários que foram desativados posteriormente não são exibidas.

### A coluna VAR (Variance) {#the-var-variance-column}

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
   <td> <p>A Variação de Hora, FTE ou Custo mostra se você tem Horas Orçadas suficientes para o projeto realizar todas as Horas Planejadas do projeto. </p> <p>A Variação de Horas, FTE ou Custo do Projeto é calculada usando a seguinte fórmula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> <p>A variação de Hora, FTE ou Custo mostra se você tem Horas Orçadas, FTE ou Custo suficientes para a função realizar as Horas Planejadas atribuídas a ela. </p> <p>A Hora da Função, FTE ou Variação de Custo é calculada usando a seguinte fórmula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td> <p>As Horas, FTE ou Variação de Custo mostram se você tem Horas Orçadas suficientes para o usuário realizar as Horas Planejadas atribuídas a ele. </p> <p>As Horas de Usuário, FTE ou Variação de Custo são calculadas usando a seguinte fórmula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando as Horas, FTE ou Variação de custo são exibidas em vermelho, você estima menos Horas orçadas do que as Horas planejadas do trabalho real que precisam ser concluídas. Nesse caso, as horas orçadas podem não ser suficientes para concluir o trabalho.

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
     <p>As Horas Líquidas, FTE ou Custo do projeto podem mostrar um dos seguintes: </p> 
     <ul> 
      <li> <p>A diferença entre o Tempo ou custo Disponível e o Tempo ou custo Orçado do projeto:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>A diferença entre o Tempo ou custo disponível e o Tempo ou custo planejado para o projeto, quando a configuração Usar valores planejados (PLN) na configuração Cálculos líquidos está habilitada: </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>DICA</b></p>        
  <p>Essa opção é aplicada somente quando você personaliza a exibição na seção Exibir itens selecionados.</p>
  <p>Para obter mais informações, consulte <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Revisar disponibilidade e alocação de recursos usando o Planejador de Recursos da Adobe Workfront</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>Função</td> 
   <td> 
    <div> 
     <p>A função Horas líquidas, FTE ou Custo pode mostrar uma das seguintes opções: </p> 
     <ul> 
      <li> <p>A diferença entre o tempo ou custo Disponível e o tempo ou custo Orçado para a função:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>A diferença entre o Tempo ou custo Disponível e o Tempo ou custo Planejado para a função, quando os valores de Usar Planejado (PLN) na configuração de cálculos LÍQUIDOS estão habilitados:</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>DICA</b> <span>

Esta opção é aplicada somente quando você personaliza o modo de exibição na seção Exibir itens selecionados.</span> </p> <p><span>Para obter mais informações, consulte </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Revisar disponibilidade e alocação de recursos usando o Planejador de Recursos da Adobe Workfront</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>Usuário</td> 
   <td> 
    <div> 
     <p>As Horas Líquidas, FTE ou Custo do usuário podem mostrar um dos seguintes: </p> 
     <ul> 
      <li> <p>A diferença entre o Tempo ou custo disponível e o Tempo ou custo orçado para o usuário:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>A diferença entre o Tempo ou custo Disponível e o Tempo ou custo Planejado para o usuário, quando os valores de Usar Planejado (PLN) na configuração de cálculos LÍQUIDOS estão habilitados:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>DICA</b> <span>

Esta opção é aplicada somente quando você personaliza o modo de exibição na seção Exibir itens selecionados.</span> </p> <p><span>Para obter mais informações, consulte </span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Revisar disponibilidade e alocação de recursos usando o Planejador de Recursos da Adobe Workfront</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Quando as Horas LÍQUIDAS, FTE ou Custo são exibidos em vermelho, não há tempo ou orçamento Disponível suficiente para cobrir o tempo ou custo Orçado ou Planejado associado ao trabalho. Nesse caso, os recursos estão superalocados.

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
