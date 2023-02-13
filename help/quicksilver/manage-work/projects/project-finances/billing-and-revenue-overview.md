---
content-type: overview
product-area: projects
navigation-topic: financials
title: Visão Geral da Faturamento e Receita
description: Como gerente de projeto, você pode usar as taxas de faturamento para capturar a receita em seus projetos.
author: Alina
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: 518a552845598a30fd547d432aa9d22dfef6ec8e
workflow-type: tm+mt
source-wordcount: '3313'
ht-degree: 0%

---

# Visão Geral da Faturamento e Receita

Como gerente de projeto, você pode usar as taxas de faturamento para capturar a receita em seus projetos.

Este artigo descreve o rastreamento de receita para projetos. A receita é calculada de forma diferente no Relatório de utilização. Para obter informações sobre cálculos de Receita no Relatório de Utilização, consulte [Exibir informações de utilização de recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Visão geral das Taxas de Faturamento

Considere o seguinte ao trabalhar com taxas de faturamento:

* Você precisa de uma licença do Plano com acesso de Edição a Dados Financeiros para gerenciar as taxas de faturamento.\
   Para obter mais informações sobre a concessão de acesso aos Dados Financeiros, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* As taxas de faturamento são quantias de receita por unidade de trabalho associadas a funções de trabalho ou usuários.

   Multiplicar as taxas pelas horas gastas no trabalho gera receita para seus projetos.

* Depois de estabelecer suas taxas de faturamento, você pode acompanhar a receita criando registros de faturamento para registrar o que foi ou não faturado.

   >[!TIP]
   >
   >Quando você marca um Registro de Faturamento como Faturado, ele nunca pode ser editado. Isso é importante quando suas taxas variam e você deseja bloquear as informações de receita e despesa do seu projeto. Adicioná-lo a um registro de faturamento e marcá-lo como Faturado impede que seja atualizado quando as taxas forem atualizadas em seu sistema.

   Para obter mais informações sobre como criar registros de faturamento, consulte o artigo [Criar registros de faturamento](../../../manage-work/projects/project-finances/create-billing-records.md).

* Você pode criar taxas de faturamento para usuários, funções de job ou pode ter uma taxa de faturamento única para um projeto ou tarefa.

>[!IMPORTANT]
>
>As taxas que calculam a receita pertencem ao usuário que está registrando a hora ou suas funções de trabalho.

* [Taxas de Faturamento do Usuário](#user-billing-rates)
* [Taxas de Faturamento da Função de Trabalho](#job-role-billing-rates)
* [Taxas de Faturamento Fixas para projetos ou tarefas](#fixed-billing-rates-for-projects-or-tasks)
* [Substituir Taxas de Faturamento](#override-billing-rates)

### Taxas de Faturamento do Usuário {#user-billing-rates}

Como administrador de usuário, ao criar um usuário, você pode associá-lo a uma Taxa de Faturamento especificando um valor para o campo Faturamento por hora em seu perfil.\
Para obter mais informações sobre como criar usuários, consulte o artigo [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md)

![](assets/qs-user-edit-ui-with-rp-and-billing-per-hour-field-1-350x152.png)

### Taxas de Faturamento da Função de Trabalho {#job-role-billing-rates}

Como administrador do Adobe Workfront, ao criar uma função de trabalho, você pode associá-la a uma Taxa de Faturamento especificando um valor para o campo Faturamento/Hora.

Você pode definir o valor de uma taxa de faturamento de função de cargo usando a Moeda de Base do seu sistema Workfront ou usando outra moeda personalizada.

Para obter mais informações sobre como criar funções de cargo e substituir sua moeda, consulte o artigo [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

![](assets/billing-rate-for-role-1-350x294.png)

### Taxas de Faturamento Fixas para projetos ou tarefas {#fixed-billing-rates-for-projects-or-tasks}

Além das taxas por hora do usuário e da função de cargo, você também pode ter as seguintes taxas de faturamento fixas:

* Valor fixo para tipo de receita horária fixa
* Quantia Fixa para Tipo de Receita Fixa

Para obter mais informações sobre como as taxas de faturamento fixas são usadas para calcular a receita, consulte [Visão geral dos tipos de receita da tarefa](#overview-of-task-revenue-types).

### Substituir Taxas de Faturamento {#override-billing-rates}

>[!IMPORTANT]
>
>Você pode sobrepor as taxas de faturamento associadas às funções de job. Não é possível substituir as taxas de faturamento do usuário ou as taxas fixas.

Você pode substituir as taxas de faturamento da função de trabalho por:

* Uma empresa específica

   Para obter mais informações sobre como criar taxas de faturamento de função de cargo específicas para uma empresa, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Um projeto específico

   Para obter mais informações sobre como criar taxas de faturamento de função de trabalho específicas a um projeto, consulte o artigo [Visão Geral das Taxas de Faturamento da Função do Trabalho e cálculo da Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Rastrear valores de receita

A Workfront pode rastrear a Receita Planejada automaticamente quando as tarefas são criadas com base nas Horas Planejadas das tarefas.

Ele também pode rastrear a Receita Real automaticamente quando Horas Reais estiverem conectadas às tarefas, problemas e ao projeto.

A tabela a seguir mostra os tipos de receita associados a tarefas, problemas e projetos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Receita Planejada</td> 
   <td> <p>Para tarefas, essa é a receita associada às Horas Planejadas de tarefas. As Horas Planejadas de todas as tarefas são acumuladas até as Horas Planejadas do projeto para contribuir com o cálculo das Horas Planejadas do projeto. </p> <p>Para obter mais informações sobre as Horas Planejadas no Workfront, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Visão geral das Horas Planejadas</a>. </p> <p>A Workfront calcula a Receita planejada para tarefas e projetos usando as seguintes fórmulas:</p> <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code> </p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) +&nbsp;Fixed Revenue</code> </p> 
   <p><b>Nota</b>

<p>A Receita Planejada do projeto exibida na área Detalhes do projeto e nos relatórios do projeto é diferente da Receita Planejada exibida no relatório Utilização. </p> <p>A Receita Planejada na área Detalhes do Projeto reflete a receita da tarefa associada à tarefa Horas Planejadas, bem como a Receita Fixa do projeto. A Receita Planejada no Relatório de Utilização exibe a Receita Planejada associada somente às Horas Planejadas das atribuições de tarefa no projeto. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Se o projeto tiver uma tarefa com 10 horas, atribuída a um Consultor com uma taxa de $20 por hora e o projeto tiver uma Receita Fixa de $100, o relatório Utilização exibirá $200 para Receita Planejada (a Receita Planejada associada às horas da tarefa). A seção Detalhes do projeto exibe $300 (a Receita planejada da tarefa e a Receita Fixa do projeto). </p> 
     </div> </p> <p>A Receita Planejada da Tarefa é calculada usando a Taxa por hora de Faturamento dos usuários ou funções de trabalho atribuídas às tarefas. O Tipo de receita das tarefas influencia qual taxa (usuário ou função) é usada para calcular a Receita planejada. Para obter mais informações, consulte as seguintes seções neste artigo:</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Visão geral dos tipos de receita da tarefa</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">Cálculos de receita para tarefas com base em atribuições de Usuário e Função</a> </p> </li> 
    </ul> <p>Para obter informações sobre os cálculos da Receita Planejada no relatório Utilização, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações de utilização de recursos </a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Receita Efetivo*</td> 
   <td> <p>Associado às Horas Reais de Tarefas, Problemas e Projetos. </p> <p>Geralmente, a Workfront calcula a Receita Real usando esta fórmula:</p> <p><code>Planned Revenue = Planned Hours * Billing rate</code> </p> <p>Para obter informações sobre cálculos de Receita Real no Relatório de Utilização, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações de utilização de recursos </a>. </p> <p><b>DICA</b>

Não é possível visualizar a Receita Real no nível da edição, mas a receita associada às Horas Reais nos problemas contribui para a Receita Real do projeto. </p> </td>
</tr> 
 </tbody> 
</table>

*Em Horas Reais, as taxas do usuário sempre se referem ao usuário que registra as horas ou às taxas de suas funções de trabalho. Para obter informações sobre quando o Workfront usa as taxas do usuário e quando ele usa as taxas de suas funções de trabalho, consulte o [Cálculos de receita](#revenue-calculations) neste artigo.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

Por exemplo, se uma tarefa com Tipo de receita por hora do usuário for planejada para levar 2 horas e o usuário atribuído a ela tiver uma taxa por hora de US$ 30 por hora, a Receita planejada da tarefa será de US$ 60. Quando a tarefa for concluída, se o usuário registrar apenas 1,5 horas como o tempo real gasto para concluir a tarefa, a Receita Real será de US$ 45. Se outro usuário que não estiver atribuído à tarefa registrar a hora, a Receita Real será calculada com base nas Taxas de Faturamento desse usuário.

Você pode registrar a receita das seguintes maneiras:

* Ao definir o Tipo de receita de suas tarefas e associar usuários ou funções atribuídos a itens de trabalho com taxas de faturamento. Isso calcula a receita pela quantidade de Horas Planejadas ou Reais nos itens de trabalho. Você pode definir um limite para o valor máximo cobrado por taxas horárias ou não.\
   Para obter mais informações sobre como especificar o Tipo de Receita de uma tarefa, consulte o artigo [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* Ao faturar uma taxa fixa de Receita para tarefas ou projetos.\
   Se você tiver tarefas com Receita Fixa, a Receita Fixa será adicionada como Receita Planejada de uma tarefa ou projeto, e a Receita Planejada de uma tarefa estará disponível para ser adicionada a um Registro de Faturamento como Receita Fixa.
* Ao definir uma taxa de faturamento fixo de Receita Fixa para um projeto e, em seguida, definir taxas horárias para as tarefas dentro do projeto. O Workfront adiciona as taxas horárias das tarefas à taxa fixa do projeto.\
   Por exemplo, um mecânico que usa o Workfront pode informar um custo para peças como receita fixa para o projeto e, em seguida, faturar por hora o tempo gasto com a correção de um carro. A Receita fixa em projetos ou tarefas é realizada na conclusão.

Você também pode marcar suas tarefas como &quot;Não faturável&quot;, nesse caso, não há Receita Planejada ou Real associada a elas.

## Visão geral dos tipos de receita da tarefa {#overview-of-task-revenue-types}

Por padrão, o Tipo de receita de todas as novas tarefas é definido de acordo com as Preferências de tarefa e ocorrência especificadas pelo seu Workfront ou administrador de grupo.\
Para obter mais informações sobre como definir a tarefa e as preferências de emissão para a instância do Workfront, consulte o artigo [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

O Proprietário do projeto pode modificar o Tipo de receita das tarefas e a Receita fixa dos projetos.\
Para obter mais informações sobre como especificar a Receita Fixa de um projeto, consulte o artigo [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).\
Para obter mais informações sobre como especificar o Tipo de Receita de uma tarefa, consulte o artigo [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Você pode aplicar os seguintes Tipos de receita a suas tarefas ou projetos:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de Receita</strong> </p> </th> 
   <th> <p><strong>Descrição</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Receita com Valor Fixo</p> </td> 
   <td> <p>Esse tipo pode ser usado com projetos e tarefas. </p> <p>Ao anexar um modelo a um projeto, a Receita fixa do modelo é adicionada à Receita fixa do projeto. Para obter mais informações, consulte <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Visão geral de anexar um modelo a um projeto</a>. </p> <p>Para tarefas, independentemente das atribuições de tarefa, a receita na tarefa é sempre calculada usando a Quantia Fixa especificada na tarefa. </p> <p>As tarefas Receita fixa de filhos são acumuladas até a Receita da tarefa pai e, em seguida, até a receita do Projeto. Se uma quantia fixa for definida na tarefa pai e/ou no projeto, a quantia será adicionada à receita planejada totalizada de qualquer tarefa filho.</p> <p>A quantidade de receita fixa nas tarefas pode ser incluída em um Registro de Faturamento no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Recurso</p> </td> 
   <td> <p>Esse tipo pode ser usado somente para tarefas. </p> <p>A taxa de faturamento que você definiu para um usuário específico multiplicada pelo número de Horas Planejadas para essa tarefa se torna a Quantidade de Receita Planejada da tarefa. A taxa de faturamento que você definiu para um usuário específico multiplicada pelo número de horas que o usuário faz logon na tarefa é o valor da Receita Real da tarefa. <br>Por exemplo, ao criar um usuário e definir $20 para o campo Faturamento por hora, em seguida, se o usuário enviar 5 horas para uma tarefa na folha de ponto, a quantia Faturamento real da tarefa será de $100.</p> <p><b>DICA</b>

Esse é o Tipo de receita padrão ao criar uma tarefa.</p> </td>
</tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Perfil</p> </td> 
   <td> <p>Esse tipo pode ser usado somente para tarefas.</p> <p>Esse tipo é semelhante a Horário do usuário, mas usa taxas de função de trabalho em vez de taxas do usuário.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Usuário por hora com Cap</p> </td> 
   <td> <p>Esse tipo pode ser usado somente para tarefas.</p> <p>As tarefas são faturadas por hora, como em Horário do usuário, mas têm uma Quantidade máxima de Cap que você pode especificar. <br>Por exemplo, se a taxa de faturamento de um usuário for de $25, mas a Quantia de Limite na tarefa for de $20, e o usuário registrar uma hora, a Receita Real na tarefa será de $20. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Função por hora com Cap</p> </td> 
   <td> <p>Esse tipo pode ser usado somente para tarefas.</p> <p>Esse tipo é semelhante a Horário do Usuário com Limite, mas usa taxas de função de cargo em vez de taxas do usuário. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Recurso mais Taxa Fixa</p> </td> 
   <td> <p>Esse tipo pode ser usado somente para tarefas. </p> <p>As tarefas são faturadas por hora como em Horário do usuário, mas têm uma Quantia fixa que pode ser adicionada à taxa de usuário. A Quantia Fixa especificada na tarefa pode ser incluída nos registros de faturamento do projeto. O Valor Fixo não é multiplicado pelas horas na tarefa. Somente a taxa de faturamento do usuário faz. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Perfil mais Taxa Fixa</p> </td> 
   <td> <p>Esse tipo pode ser usado somente para tarefas. </p> <p>As tarefas são faturadas por hora como na Função por hora, mas têm um Valor fixo adicional que pode ser adicionado à taxa de função. A Quantia Fixa especificada na tarefa pode ser incluída nos registros de faturamento do projeto. O Valor Fixo não é multiplicado pelas horas na tarefa. Somente a taxa de faturamento da função de trabalho faz. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor de Hora Fixo</p> </td> 
   <td> <p>Esse tipo pode ser usado somente para tarefas.</p> <p>O Limite ou Quantia Fixa que você definiu para a tarefa multiplicado pelo número de horas inseridas na tarefa (independentemente do usuário ou de suas funções de cargo) é a quantia de faturamento.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Não Faturável</p> </td> 
   <td> <p>Esse tipo pode ser usado somente para tarefas.</p> <p>Esse Tipo de receita não tem efeito na receita. </p> <p>Se um objeto pai tiver essa configuração, as tarefas filho com um tipo de faturamento ainda serão aplicadas normalmente.</p> <p>Quando um usuário sem acesso a dados financeiros ou um usuário sem permissões financeiras em um modelo cria um projeto a partir desse modelo, esse é o Tipo de receita padrão para as tarefas no projeto.</p> <p>Para obter informações sobre o acesso a Dados Financeiros, consulte o artigo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso aos dados financeiros</a>.<br>Para obter informações sobre permissões financeiras em objetos, consulte o artigo <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral do compartilhamento de permissões em objetos</a>.<br>Para obter informações sobre como criar projetos a partir de modelos, consulte o artigo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Criar um projeto usando um modelo</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão Geral da Receita para tarefas pai

Se você alterar uma tarefa independente com informações de faturamento em um pai, a nova tarefa pai ainda manterá as informações de faturamento aplicadas anteriormente, juntamente com as horas aplicadas anteriormente. Quaisquer informações de faturamento provenientes de horas registradas nas tarefas secundárias serão acumuladas como Receita Real na nova tarefa pai.

A Receita Planejada das tarefas filho também é acumulada na tarefa pai.

## Visão geral da receita para problemas

Os problemas não têm valores de Receita Planejada ou Real, mas podem ter Custo Real.

Se você registrar horas para um problema e usar um tipo de hora marcado como &quot;Contagem como receita&quot;, a Workfront calculará uma quantia de Custo real de acordo com a taxa do usuário que está fazendo logon no tempo. Esse número é adicionado ao Custo Real do projeto. As horas também podem ser incluídas em um registro de faturamento.

Para obter mais informações sobre custos de rastreamento, consulte o artigo [Rastrear custos](../../../manage-work/projects/project-finances/track-costs.md).

Para obter mais informações sobre tipos de hora, consulte o artigo [Gerenciar tipos de hora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Cálculos de receita

* [Cálculos de receita para tarefas com base em atribuições de Usuário e Função](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### Cálculos de receita para tarefas com base em atribuições de Usuário e Função {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Ao calcular a receita de uma tarefa, considere o seguinte:

* Se um usuário ou uma função de trabalho mostrar uma taxa de US$ 0,00, o Workfront lê isso como uma quantia válida e multiplica essa quantia pelo número de horas na tarefa para calcular a receita. Se não quiser mostrar nenhuma receita para suas tarefas, verifique se o campo para a taxa de faturamento do seu usuário ou função de trabalho está vazio.
* Quando as taxas de faturamento da função de trabalho são aplicadas, o Workfront usa a taxa de sobreposição no nível do projeto, em vez da taxa de faturamento dessa função definida no nível do sistema sempre que houver uma taxa de sobreposição no projeto.
* No caso de vários destinatários nas tarefas, os cenários descritos abaixo se aplicam a cada destinatário.

Existe uma hierarquia da qual a taxa é usada nos cálculos de receita com base em atribuições de tarefa.

Se o administrador da Workfront ativou a variável **Atribuir Funções de Trabalho a entradas de hora manualmente** na área Folhas de horas e preferências de horas e o tempo de registro do usuário no projeto seleciona uma função diferente para associar a esse tempo, a Receita real da tarefa ou projeto sempre é calculada com base na função associada à entrada de hora. Para obter informações sobre como ativar o tempo de registro para uma função de trabalho específica, consulte o artigo [Folha de horas e preferências de hora](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Os seguintes cenários existem ao calcular a receita da tarefa com base no Tipo de receita e na natureza da atribuição da tarefa:

* **O Tipo de Receita da tarefa é Por Hora do Usuário**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Taxa de faturamento por hora</td> 
     <td>Sem atribuição</td> 
     <td>Atribuição de usuário</td> 
     <td>Atribuição de função de trabalho</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taxa de faturamento por hora da Receita Planejada</td> 
     <td>$0.00</td> 
     <td> Se um usuário tiver uma taxa de faturamento em seu perfil, essa taxa será usada para calcular a Receita Planejada. Caso contrário, a taxa de faturamento do sistema de sua função de trabalho principal será usada. <br><p><b>OBSERVAÇÃO</b>  O usuário pode ser atribuído à tarefa com uma de suas funções de trabalho secundárias, mas a taxa da função de trabalho principal é usada aqui.</p></td> 
     <td>A taxa de faturamento do sistema da função de trabalho atribuída à tarefa é usada para calcular a Receita Planejada. </td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taxa de Faturamento por hora para Receita Real</td> 
     <td>Se o usuário que está registrando as horas tiver uma taxa de faturamento em seu perfil, essa taxa será usada. <br>Caso contrário, a taxa de faturamento de sua função de trabalho principal será usada. Se não houver uma taxa de faturamento associada ao usuário ou sua função principal, a Receita Real será de $0,00. <br><p><b>Nota</b>

   Somente as taxas associadas ao usuário que registra a hora são consideradas para o cálculo, mesmo quando outro usuário é atribuído à tarefa.</p></td>
   <td>Se o usuário que está registrando as horas tiver uma taxa de faturamento em seu perfil, essa taxa será usada. <br>Caso contrário, a taxa de faturamento de sua função de trabalho principal será usada. Se não houver uma taxa de faturamento associada ao usuário ou sua função principal, a Receita Real será de $0,00. <br><p><b>Nota</b>

   Somente as taxas associadas ao usuário que registra a hora são consideradas para o cálculo, mesmo quando outro usuário é atribuído à tarefa.</p></td>
   <td>Se o usuário que está registrando as horas tiver uma taxa de faturamento em seu perfil, essa taxa será usada. Caso contrário, a taxa de faturamento de sua função de trabalho principal será usada.<br><p><b>Nota</b>

   Se o tempo de registro do usuário não tiver uma taxa de faturamento associada a ele e ele não tiver uma função de trabalho ou uma taxa de faturamento para sua função de cargo, a taxa da função de trabalho associada à tarefa será usada. Se não houver uma taxa de faturamento para essa função, a receita será $0,00</p></td>
   </tr> 
   </tbody> 
  </table>

* **O Tipo de Receita da tarefa é Função por Hora**

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Taxa de faturamento por hora</td> 
     <td>Sem atribuição</td> 
     <td>Atribuição de usuário</td> 
     <td>Atribuição de função de trabalho</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taxa de faturamento por hora da Receita Planejada</td> 
     <td>$0.00</td> 
     <td>A Workfront observa a função de trabalho que o usuário cumpre na tarefa para calcular a Receita Planejada. <br>Se o usuário não estiver associado a nenhuma função na tarefa, a Receita será de US$ 0,00. </td> 
     <td>A taxa de faturamento da função de trabalho atribuída à tarefa é usada para calcular a Receita Planejada.</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taxa de Faturamento por hora para Receita Real</td> 
     <td>O Workfront usa a taxa de faturamento da função de trabalho principal do usuário que está registrando o tempo. <br>Se o usuário que estiver registrando o horário não tiver nenhuma função de trabalho associada a ele, ou se a função de trabalho principal não tiver uma taxa de faturamento, a Receita Real será de US$ 0,00. </td> 
     <td> Se o usuário que está registrando a hora for atribuído à tarefa, a taxa de faturamento da função de trabalho associada ao usuário na tarefa será usada para calcular a Receita Real. Caso contrário, a taxa de faturamento de sua função de trabalho principal será usada. Se o usuário não tiver nenhuma função de trabalho principal ou se sua função de trabalho principal não tiver taxa de faturamento, a Receita Real será de $0,00. </td> 
     <td>Se uma das funções de trabalho do usuário que está registrando a hora for atribuída à tarefa, essa taxa de função de trabalho será usada. Se a função de trabalho atribuída à tarefa não estiver associada ao usuário registrando a hora, a taxa de faturamento da função principal do usuário será usada para calcular a Receita Real. Se o usuário não tiver uma função de trabalho ou não houver uma taxa associada à função de trabalho primária, a taxa da função de trabalho atribuída à tarefa será usada. </td> 
    </tr> 
   </tbody> 
  </table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Ideal table but does not come across Markdown</p>
<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<col>
<col>
<tbody>
<tr>
<td colspan="3">Revenue Type = User Hourly</td>
<td colspan="4">Revenue Type = Role Hourly</td>
</tr>
<tr>
<td> <p> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
<td> <p><strong>No Assignment</strong> </p> </td>
<td> <p><strong>User Assignment</strong> </p> </td>
<td> <p><strong>Job Role Assignment</strong> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Planned Revenue</strong> </p> </td>
<td> <p>$0.00</p> </td>
<td> <p> If a user has a billing rate in their profile, then that rate is used to calculate Planned Revenue. Otherwise, the system billing rate of their primary job role is used. <br><note type="note">
The user can be assigned to the task with one of their secondary job roles, but the rate of the primary job role is used here instead.
</note></p> </td>
<td> <p> The system billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> </td>
<td> <p>$0.00</p> </td>
<td> <p>Workfront looks at the job role that the user fulfills on the task to calculate the Planned Revenue. <br>If the user is not associated with any role on the task, the Revenue is $0.00. </p> </td>
<td> <p>The billing rate of the job role assigned to the task is used to calculate Planned Revenue. </p> <p> </p> <p> </p> </td>
</tr>
<tr>
<td> <p><strong>Billing per hour rate for Actual Revenue</strong> </p> </td>
<td colspan="2"> <p>If the user logging the hours has a billing rate in their profile, that rate is used. <br>Otherwise, the billing rate of their primary job role is used. If there is no billing rate associated with the user or their primary role, the Actual Revenue is $0.00. <br><note type="note">
Only the rates associated with the user logging the time are taken into account for the calculation, even when another user is assigned to the task.
</note></p> </td>
<td> If the user logging the hours has a billing rate in their profile, that rate is used. Otherwise, the billing rate of their primary job role is used.<br><note type="note">
If the user logging time has no billing rate associated with them, and they do not have a job role or a billing rate for their job role, then the rate from the job role associated with the task is used. If there is no billing rate for this role, the revenue is $0.00
</note></td>
<td> <p>Workfront uses the billing rate of the primary job role of the user logging the time. <br>If the user logging the time has no job role associated with them, or if the primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p> If the user logging the time is assigned to the task, the billing rate of the job role associated with the user on the task is used to calculate the Actual Revenue. Otherwise, the billing rate of their primary job role is used. If the user has no primary job role or if their primary job role has no billing rate, the Actual Revenue is $0.00. </p> </td>
<td> <p>If one of the job roles of the user logging the time is assigned to the task, that job role rate is used. If the job role assigned to the task is not associated with the user logging the time, then the billing rate of the primary role of the user is used to calculate the Actual Revenue. If the user does not have a job role or there is no rate associated with their primary job role, then the rate of the job role assigned to the task is used. </p> </td>
</tr>
</tbody>
</table>
</div>
-->

### Cálculos de receitas para projetos

Você pode rastrear os seguintes tipos de receita para projetos:

* A Receita Planejada de um projeto é calculada pela seguinte fórmula:

   ```
   Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue
   ```

   Para obter informações sobre como a tarefa Receita Planejada é calculada, consulte o [Cálculos de receita para tarefas com base em atribuições de Usuário e Função](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) neste artigo.

* A Receita Real de um projeto é calculada pela seguinte fórmula:

   ```
   Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)
   ```

Para obter informações sobre como a tarefa Receita Real é calculada, consulte o [Cálculos de receita para tarefas com base em atribuições de Usuário e Função](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) neste artigo.

Para a Receita Real associada às horas registradas diretamente no projeto ou aos problemas, o Workfront usa a Taxa de Faturamento do usuário que registra o tempo no projeto. Se o usuário não tiver uma Taxa de Faturamento associada ao perfil, o Workfront usará a Taxa de Faturamento de sua Função de Trabalho Principal. Se ambas as taxas forem zero, a Receita Real associada às horas registradas no projeto ou os problemas serão zero.
