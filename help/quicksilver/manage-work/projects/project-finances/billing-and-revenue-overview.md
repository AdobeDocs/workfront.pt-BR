---
content-type: overview
product-area: projects
navigation-topic: financials
title: Visão geral de faturamento e receita
description: Como gerente de projeto, você pode usar taxas de faturamento para capturar a receita de seus projetos.
author: Lisa
feature: Work Management
exl-id: 400abcde-e368-4a70-89a9-05027900ab81
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '3691'
ht-degree: 0%

---

# Visão geral de faturamento e receita

<!-- Audited: 1/2024 -->

{{highlighted-preview}}

Como gerente de projeto, você pode usar taxas de faturamento para capturar a receita de seus projetos.

Este artigo descreve o rastreamento da receita de projetos do. A receita é calculada de forma diferente no Relatório de Utilização. Para obter informações sobre cálculos de Receita no Relatório de Utilização, consulte [Exibir informações sobre utilização de recursos](../../../resource-mgmt/resource-utilization/view-utilization-information.md).

## Visão geral das taxas de cobrança

Considere o seguinte ao trabalhar com taxas de faturamento:

* Você precisa de uma licença Plan ou Standard com acesso Edit to Financial Data para gerenciar taxas de faturamento.\
  Para obter mais informações sobre como conceder acesso a Dados Financeiros, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* As taxas de cobrança são quantias de receita por unidade de trabalho associada a funções de trabalho ou usuários.

  Multiplicar as taxas pelas horas gastas no trabalho gera receita para os projetos.

* Depois de estabelecer as taxas de faturamento, é possível rastrear a receita criando registros de faturamento para registrar o que foi ou não faturado.

  >[!TIP]
  >
  >Quando você marca um Registro de cobrança como Faturado, ele nunca pode ser editado. Isso é importante quando suas taxas variam e você deseja bloquear as informações de receita e despesa em seu projeto. Adicioná-lo a um registro de cobrança e marcá-lo como Faturado impede que ele seja atualizado quando as taxas são atualizadas em seu sistema.

  Para obter mais informações sobre como criar registros de cobrança, consulte o artigo [Criar registros de cobrança](../../../manage-work/projects/project-finances/create-billing-records.md).

* Você pode criar taxas de faturamento para usuários, funções de trabalho ou pode ter uma taxa de faturamento única para um projeto ou tarefa.

>[!IMPORTANT]
>
>As taxas que calculam a receita pertencem ao usuário que está registrando o horário ou a suas funções de trabalho.

* [Taxas de Cobrança do Usuário](#user-billing-rates)
* [Taxas de Cobrança de Funções de Trabalho](#job-role-billing-rates)
* [Taxas de Cobrança Fixas para projetos ou tarefas](#fixed-billing-rates-for-projects-or-tasks)
* [Substituir taxas de cobrança](#override-billing-rates)

### Taxas de Cobrança do Usuário {#user-billing-rates}

Como administrador de usuário, ao criar um usuário, você pode associá-lo a Taxas de Faturamento de data efetiva especificando valores para os campos Faturamento por Hora e as datas para as taxas.

Para obter mais informações sobre como criar usuários, consulte o artigo [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

![Editar taxas de cobrança e custo do usuário](assets/edit-user-cost-billing-rate-1.png)

### Taxas de Cobrança de Função de Trabalho {#job-role-billing-rates}

Como administrador do Adobe Workfront, ao criar uma função de trabalho, você pode associá-la a Taxas de cobrança efetivas por data especificando valores para os campos Faturamento por hora e as datas para as taxas.

Você pode definir o valor de uma taxa de cobrança de função de trabalho usando a Moeda base do sistema Workfront ou usando outra moeda personalizada.

Para obter mais informações sobre como criar funções de trabalho e substituir sua moeda, consulte o artigo [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

![Editar taxas de cobrança e custos da função de trabalho](assets/edit-job-role-multiple-billing-rates-new.png)

### Taxas de Cobrança Fixas para projetos ou tarefas {#fixed-billing-rates-for-projects-or-tasks}

Além das taxas horárias de usuário e função de trabalho, você também pode ter as seguintes taxas de faturamento fixas:

* Valor Fixo para o Tipo de Receita por Hora Fixa
* Valor Fixo para o Tipo de Receita Fixa

Para obter mais informações sobre como as taxas de cobrança fixas são usadas para calcular a receita, consulte [Visão Geral dos Tipos de Receita da tarefa](#overview-of-task-revenue-types).

### Substituir taxas de cobrança {#override-billing-rates}

>[!IMPORTANT]
>
>Você pode substituir taxas de faturamento associadas a funções de trabalho. Não é possível substituir taxas de faturamento do usuário ou taxas fixas.

É possível substituir as taxas de faturamento de função de trabalho para:

* Uma Empresa específica

  Para obter mais informações sobre como criar taxas de cobrança de funções de trabalho específicas para uma empresa, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Um projeto específico

  Para obter mais informações sobre como criar taxas de cobrança de função de trabalho específicas para um projeto, consulte o artigo [Visão geral da substituição de Taxas de cobrança de função de trabalho e cálculo de Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Rastrear valores de receita

O Workfront pode rastrear a Receita planejada automaticamente quando as tarefas são criadas com base nas Horas planejadas das tarefas.

Ele também pode rastrear a Receita Real automaticamente quando as Horas Reais são registradas nas tarefas, problemas e no projeto.

A tabela a seguir mostra os tipos de receita associados a tarefas, problemas e projetos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Receita Planejada</td> 
   <td> <p>Para tarefas, essa é a receita associada às Horas planejadas das tarefas. As horas planejadas de todas as tarefas são acumuladas nas horas planejadas do projeto para contribuir no cálculo das horas planejadas do projeto. </p> <p>Para obter mais informações sobre as Horas planejadas no Workfront, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">visão geral das Horas planejadas</a>. </p> <ul><li><p>O Workfront calcula a Receita Planejada para tarefas usando esta fórmula:</p>
   <p><code>Task Planned Revenue = Planned Hours * Billing hourly rate</code><p> <p><strong>OBSERVAÇÃO</strong></br> A taxa horária de cobrança na fórmula considera quaisquer alterações de data de efetivação da taxa.</p> </li><li><p>O Workfront calcula a Receita Planejada para projetos usando a seguinte fórmula:</p> <p><code>Project Planned Revenue = SUM (All tasks Planned Revenue) + Fixed Revenue</code></p>
   <p><b>Nota</b>

<p>A Receita Planejada do projeto exibida na área Detalhes do Projeto e nos relatórios do projeto é diferente da Receita Planejada exibida no relatório de Utilização. </p></li></ul> <p>A Receita Planejada na área Detalhes do Projeto reflete a receita da tarefa associada às Horas Planejadas da tarefa, bem como a Receita Fixa do projeto. A Receita Planejada no Relatório de Utilização exibe a Receita Planejada associada apenas às Horas Planejadas das atribuições de tarefa no projeto. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p>Se o projeto tiver uma tarefa com 10 horas, atribuída a um Consultor com uma taxa horária de US$ 20, e o projeto tiver uma Receita Fixa de US$ 100, o relatório de Utilização exibirá US$ 200 para a Receita Planejada (a Receita Planejada associada às horas na tarefa). A seção Detalhes do Projeto exibe US$ 300 (a Receita Planejada da tarefa e a Receita Fixa do projeto). </p> 
     </div> </p> <p>A Receita Planejada da Tarefa é calculada usando as taxas horárias de Faturamento dos usuários ou funções de trabalho atribuídas às tarefas. O Tipo de receita das tarefas influencia qual taxa (usuário ou função) é usada para calcular a receita planejada. Para obter mais informações, consulte as seguintes seções neste artigo:</p> 
    <ul> 
     <li> <p><a href="#overview-of-task-revenue-types" class="MCXref xref">Visão Geral de Tipos de Receita de tarefa</a> </p> </li> 
     <li> <p><a href="#revenue-calculations-for-tasks-based-on-user-and-role-assignments" class="MCXref xref">Cálculos de receita para tarefas baseadas em atribuições de Usuário e Função</a> </p> </li> 
    </ul> <p>Para obter informações sobre cálculos de Receita Planejada no relatório de Utilização, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações sobre utilização de recursos</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Receita Efetiva*</td> 
   <td> <p>A receita associada às Horas Reais de tarefas, problemas e projetos. </p> <p>Geralmente, o Workfront calcula a Receita Real usando esta fórmula:</p> <p><code>Actual Revenue = Actual Hours * Billing rate</code> </p> <p><strong>OBSERVAÇÃO</strong></br> A taxa horária de cobrança na fórmula considera quaisquer alterações de data de efetivação da taxa.</p> <p>Para obter informações sobre cálculos de Receita Real no Relatório de Utilização, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações sobre utilização de recursos</a>. </p> <p><b>DICA</b>

Não é possível exibir a Receita Efetiva no nível da emissão, mas a receita associada às Horas Efetivas nas emissões contribui para a Receita Efetiva do projeto. </p> </td>
</tr> 
 </tbody> 
</table>

*Para Horas efetivas, as taxas do usuário sempre se referem ao usuário que registra as horas ou às taxas de suas funções de trabalho. Para obter informações sobre quando a Workfront usa as taxas do usuário e quando usa as taxas de suas funções de trabalho, consulte a seção [Cálculos de receita](#revenue-calculations) neste artigo.

<!--Note from the table for Planned Revenue line: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the note below is duplicated in this article: /Content/Resource Mgmt/Resource utilization/view-utilization-information.htm and in the glossary)</p>
    -->

Por exemplo, se uma tarefa com Tipo de Receita por Hora do Usuário for planejada para durar 2 horas e o usuário atribuído a ela tiver uma taxa horária de US$ 30 por hora, a Receita Planejada da tarefa será de US$ 60. Quando a tarefa for concluída, se o usuário registrar apenas 1,5 hora como o tempo real gasto para concluir a tarefa, o valor da receita real será de US$ 45. Se outro usuário que não estiver atribuído à tarefa registrar a hora, a Receita Efetiva será calculada com base nas Taxas de Cobrança desse usuário.

Você pode registrar a receita das seguintes maneiras:

* Definindo o Tipo de Receita de suas tarefas e associando usuários ou funções atribuídos a itens de trabalho com taxas de faturamento. Isso calcula a receita pela quantidade de Horas planejadas ou reais nos itens de trabalho. Você pode ou não definir um limite para o valor máximo cobrado por taxas horárias.\
  Para obter mais informações sobre como especificar o Tipo de Receita de uma tarefa, consulte o artigo [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

* Faturando uma taxa fixa de receita para tarefas ou projetos.\
  Se você tiver tarefas com Receita Fixa, o valor de Receita Fixa será adicionado como a Receita Planejada de uma tarefa ou um projeto, e a Receita Planejada de uma tarefa estará disponível para ser adicionada a um Registro de Faturamento como Receita Fixa.
* Definindo uma taxa de Receita Fixa de faturamento uniforme para um projeto e, em seguida, definindo taxas horárias para as tarefas dentro do projeto. A Workfront adiciona as taxas horárias das tarefas à taxa uniforme do projeto.\
  Por exemplo, um mecânico que utiliza o Workfront poderia informar um custo para as peças como receita fixa para o projeto e, em seguida, faturar por hora o tempo gasto para consertar um carro. Receita fixa em projetos ou tarefas é então realizada na conclusão.

Você também pode marcar suas tarefas como &quot;Não faturável&quot;, caso em que não há nenhuma receita planejada ou real associada a elas.

## Visão Geral dos Tipos de Receita da tarefa {#overview-of-task-revenue-types}

Por padrão, o Tipo de receita de todas as novas tarefas é definido de acordo com as Preferências de tarefas e problemas especificadas pelo seu administrador de grupo ou Workfront.\
Para obter mais informações sobre como definir as preferências de tarefas e problemas para sua instância do Workfront, consulte o artigo [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

O Proprietário do Projeto pode modificar o Tipo de Receita das tarefas e a Receita Fixa dos projetos.\
Para obter mais informações sobre como especificar a Receita Fixa de um projeto, consulte o artigo [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).\
Para obter mais informações sobre como especificar o Tipo de Receita de uma tarefa, consulte o artigo [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

Você pode aplicar os seguintes Tipos de Receita às suas tarefas ou projetos:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Tipo de receita</strong> </p> </th> 
   <th> <p><strong>Descrição</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Receita com Valor Fixo</p> </td> 
   <td> <p>Esse tipo pode ser usado com projetos e tarefas. </p> <p>Ao anexar um modelo a um projeto, a Receita fixa do modelo é adicionada à Receita fixa do projeto. Para obter informações, consulte <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Visão geral de anexar um modelo a um projeto</a>. </p> <p>Para tarefas, independentemente das atribuições de tarefa, a receita na tarefa é sempre calculada usando a Quantia Fixa especificada na tarefa. </p> <p>A Receita fixa das tarefas filho é totalizada na Receita da tarefa pai e, em seguida, na receita do Projeto. Se uma quantia fixa for definida na tarefa pai e/ou no projeto, a quantia será adicionada à receita planejada totalizada a partir de qualquer tarefa filho.</p> <p>A quantidade de receita fixa nas tarefas pode ser incluída em um Registro de cobrança do projeto.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Recurso</p> </td> 
   <td> <p>Este tipo pode ser usado somente para tarefas. </p> <p>A taxa de faturamento definida para um usuário específico multiplicada pelo número de Horas Planejadas para essa tarefa se torna a quantia de Receita Planejada da tarefa. A taxa de cobrança que você definiu para um usuário específico multiplicada pelo número de horas que o usuário registra na tarefa é o valor de Receita Real da tarefa. <br>Por exemplo, ao criar um usuário e definir US$ 20 para o campo Faturamento por Hora, se o usuário enviar 5 horas para uma tarefa na folha de horas, o valor do Faturamento Real da tarefa será de US$ 100.</p>
   <p>Um perfil de usuário pode conter várias taxas de faturamento com datas de efetivação. Por exemplo, a primeira taxa de cobrança de US$ 20 para o usuário termina em 30 de abril de 2023 e a segunda taxa de cobrança de US$ 25 para o usuário começa em 1º de maio de 2023. Se o usuário enviar 2 horas em 28 de abril e 3 horas em 2 de maio para uma tarefa, a quantia de Faturamento Real da tarefa será de US$ 40 + US$ 75 = US$ 115.</p>
   <p><b>DICA</b>

Esse é o Tipo de receita padrão quando você cria uma tarefa.</p> </td>
</tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Perfil</p> </td> 
   <td> <p>Este tipo pode ser usado somente para tarefas.</p> <p>Esse tipo é semelhante a Por hora do usuário, mas usa taxas de função de trabalho em vez de taxas de usuário.</p> <p><strong>OBSERVAÇÃO</strong><br>Uma função de trabalho também pode ter várias taxas de cobrança com datas de efetivação.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Hora do usuário com limite</p> </td> 
   <td> <p>Este tipo pode ser usado somente para tarefas.</p> <p>As tarefas são cobradas por hora, como na Hora do usuário, mas têm uma Quantia máxima que você pode especificar. <br>Por exemplo, se a taxa de cobrança de um usuário for de US$25, mas a Quantia Máxima na tarefa for de US$20 e o usuário fizer o logon em uma hora, a Receita Efetiva na tarefa será de US$20. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Função por hora com limite</p> </td> 
   <td> <p>Este tipo pode ser usado somente para tarefas.</p> <p>Esse tipo é semelhante a Por hora do usuário com Limite, mas usa taxas de função de trabalho em vez de taxas de usuário. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Recurso mais Taxa Fixa</p> </td> 
   <td> <p>Este tipo pode ser usado somente para tarefas. </p> <p>As tarefas são cobradas por hora, como na Hora do usuário, mas têm um Valor fixo que pode ser adicionado à taxa do usuário. O Valor Fixo especificado na tarefa pode ser incluído nos registros de cobrança do projeto. O Valor Fixo não é multiplicado pelas horas na tarefa. Somente a taxa de cobrança do usuário. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor da Hora do Perfil mais Taxa Fixa</p> </td> 
   <td> <p>Este tipo pode ser usado somente para tarefas. </p> <p>As tarefas são cobradas por hora, como na Função de hora em hora, mas têm um valor fixo adicional que pode ser adicionado à taxa de função. O Valor Fixo especificado na tarefa pode ser incluído nos registros de cobrança do projeto. O Valor Fixo não é multiplicado pelas horas na tarefa. Somente a taxa de cobrança da função de trabalho o faz. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Horas por Valor de Hora Fixo</p> </td> 
   <td> <p>Este tipo pode ser usado somente para tarefas.</p> <p>O Valor Máximo ou Fixo que você define para a tarefa multiplicado pelo número de horas informadas na tarefa (independentemente do usuário ou de suas funções de trabalho) é o valor de faturamento.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Não Faturável</p> </td> 
   <td> <p>Este tipo pode ser usado somente para tarefas.</p> <p>Este tipo de receita não afeta a receita. </p> <p>Se um objeto pai tiver essa configuração, as tarefas filho com um tipo de faturamento ainda serão aplicadas normalmente.</p> <p>Quando um usuário sem acesso a dados financeiros ou um usuário sem permissões financeiras em um modelo cria um projeto a partir desse modelo, esse é o Tipo de receita padrão para as tarefas no projeto.</p> <p>Para obter informações sobre acesso a Dados Financeiros, consulte o artigo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso a dados financeiros</a>.<br>Para obter informações sobre permissões financeiras em objetos, consulte o artigo <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral das permissões de compartilhamento em objetos</a>.<br>Para obter informações sobre como criar projetos a partir de modelos, consulte o artigo <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Criar um projeto usando um modelo</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral da Receita para tarefas pai

Se você alterar uma tarefa independente com informações de faturamento nela para um pai, a nova tarefa pai ainda manterá quaisquer informações de faturamento aplicadas anteriormente a ela, juntamente com as horas aplicadas anteriormente. Quaisquer informações de faturamento provenientes de horas registradas nas tarefas filho serão acumuladas como Receita Real para a nova tarefa pai.

A Receita Planejada das tarefas filho também é totalizada na tarefa pai.

## Visão geral de Receita para problemas

Problemas não têm valores de Receita Planejada ou Efetiva, mas podem ter Custo Efetivo.

Se você registrar horas para um problema e usar um tipo de hora marcado como &quot;Contar como receita&quot;, o Workfront calculará um valor de Custo real de acordo com a taxa do usuário que está fazendo logon no tempo. Esse número é adicionado ao Custo Efetivo do projeto. As horas também podem ser incluídas em um registro de cobrança.

Para obter mais informações sobre o rastreamento de custos, consulte o artigo [Rastrear custos](../../../manage-work/projects/project-finances/track-costs.md).

Para obter mais informações sobre tipos de horas, consulte o artigo [Gerenciar tipos de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Cálculos de receita

* [Cálculos de receita para tarefas baseadas em atribuições de Usuário e Função](#revenue-calculations-for-tasks-based-on-user-and-role-assignments)

### Cálculos de receita para tarefas baseadas em atribuições de Usuário e Função {#revenue-calculations-for-tasks-based-on-user-and-role-assignments}

Ao calcular a receita de uma tarefa, considere o seguinte:

* Se um usuário ou uma função de trabalho mostrar uma taxa de US$ 0,00, o Workfront lerá isso como uma quantia válida e multiplicará essa quantia pelo número de horas na tarefa para calcular a receita. Se não quiser mostrar nenhuma receita para suas tarefas, verifique se o campo da taxa de cobrança para seu usuário ou função de trabalho está vazio.
* Quando as taxas de faturamento da função de trabalho são aplicadas, o Workfront usa a taxa de sobreposição no nível do projeto, em vez da taxa de faturamento para essa função definida no nível do sistema sempre que há uma taxa de sobreposição no projeto.
* Para Receita Real, se o usuário ou a função de trabalho tiver várias taxas de faturamento com datas de efetivação, a receita da tarefa será a soma das receitas de cada período no qual o usuário tiver feito o logon. A Receita Planejada é baseada nas horas planejadas para os períodos de tempo.
* No caso de vários atribuídos nas tarefas, os cenários descritos abaixo se aplicam a cada atribuído.

Há uma hierarquia de qual taxa é usada nos cálculos de receita com base nas atribuições de tarefa.

Se o administrador do Workfront habilitou a configuração **Atribuir funções de trabalho a entradas de hora manualmente** na área Preferências de folhas de horas e horas e o tempo de logon do usuário no projeto seleciona uma função diferente para associar a esse tempo, a Receita Efetiva da tarefa ou do projeto sempre é calculada com base na função associada à entrada de horas. Para obter informações sobre como habilitar o tempo de log para uma função de trabalho específica, consulte o artigo [Configurar preferências de horas e folha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Os cenários a seguir existem ao calcular a receita da tarefa com base no Tipo de Receita e na natureza da atribuição da tarefa:

* **O Tipo de Receita da tarefa é de Usuário por Hora**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Taxa por hora de faturamento</td> 
     <td>Nenhuma atribuição</td> 
     <td>Atribuição de usuário</td> 
     <td>Atribuição de funções de trabalho</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taxa por hora de faturamento para Receita Planejada</td> 
     <td>$ 0,00</td> 
     <td> Se um usuário tiver uma taxa de faturamento em seu perfil, essa taxa será usada para calcular a Receita planejada. Caso contrário, será usada a taxa de cobrança do sistema da função de trabalho principal. <br><p><b>OBSERVAÇÃO</b> O usuário pode ser atribuído à tarefa com uma de suas funções de trabalho secundárias, mas a taxa da função de trabalho primária é usada aqui.</p><p>Se a função do usuário tiver sido alterada durante a atribuição, as taxas corretas serão aplicadas quando as finanças do projeto forem recalculadas.</p></td> 
     <td><p><span class="preview">Se um cartão de taxa estiver anexado ao projeto, a Receita Planejada será calculada com base na função de trabalho do cartão de taxa.</span></p> <p><span class="preview">As taxas de cobrança podem ser substituídas no nível do projeto.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taxa por hora de faturamento para Receita Efetiva</td> 
     <td>Se o usuário que registrar as horas tiver uma taxa de faturamento em seu perfil, essa taxa será usada. 
     <br><span class="preview">Quando o horário é registrado para um usuário ou função que tem uma atribuição específica de localização nas atribuições avançadas, a taxa da localização é usada.</span>
     <br>Caso contrário, a taxa de cobrança da função de trabalho principal será usada. Se não houver taxa de faturamento associada ao usuário ou à sua função principal, a Receita real será de US$ 0,00. <br><p><b>Nota</b>

  Somente as taxas associadas ao usuário que registra o tempo são consideradas para o cálculo, mesmo quando outro usuário é atribuído à tarefa.</p></td>
  <td>Se o usuário que registrar as horas tiver uma taxa de faturamento em seu perfil, essa taxa será usada. <br><span class="preview">Quando o horário é registrado para um usuário ou função que tem uma atribuição específica de localização nas atribuições avançadas, a taxa da localização é usada.</span><br>Caso contrário, a taxa de cobrança da função de trabalho principal será usada. Se não houver taxa de faturamento associada ao usuário ou à sua função principal, a Receita real será de US$ 0,00. <br><p><b>Nota</b>

  Somente as taxas associadas ao usuário que registra o tempo são consideradas para o cálculo, mesmo quando outro usuário é atribuído à tarefa.</p></td>
  <td>Se o usuário que registrar as horas tiver uma taxa de faturamento em seu perfil, essa taxa será usada. Caso contrário, a taxa de cobrança da função de trabalho principal será usada.<br><p><b>Nota</b>

  Se o tempo de logon do usuário não tiver uma taxa de faturamento associada a ele e não tiver uma função de trabalho ou uma taxa de faturamento para sua função de trabalho, a taxa da função de trabalho associada à tarefa será usada. Se não houver taxa de cobrança para essa função, a receita será de US$ 0,00</p></td>
  </tr> 
   </tbody> 
  </table>

* **O tipo de receita da tarefa é a função por hora**

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td role="rowheader">Taxa por hora de faturamento</td> 
     <td>Nenhuma atribuição</td> 
     <td>Atribuição de usuário</td> 
     <td>Atribuição de funções de trabalho</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taxa por hora de faturamento para Receita Planejada</td> 
     <td>$ 0,00</td> 
     <td><p>A Workfront analisa a função de trabalho que o usuário desempenha na tarefa para calcular a Receita planejada. <br>Se o usuário não estiver associado a nenhuma função na tarefa, a Receita será de $0,00.</p> <p><strong>OBSERVAÇÃO</strong><br>Se a função do usuário tiver sido alterada durante a atribuição, as taxas corretas serão aplicadas quando as finanças do projeto forem recalculadas.</p> </td> 
     <td><p><span class="preview">Se um cartão de taxa estiver anexado ao projeto, a Receita Planejada será calculada com base na função de trabalho do cartão de taxa.</span></p> <p><span class="preview">As taxas de cobrança podem ser substituídas no nível do projeto.</span></p></td> 
    </tr> 
    <tr> 
     <td role="rowheader">Taxa por hora de faturamento para Receita Efetiva</td> 
     <td>O Workfront usa a taxa de cobrança da função de trabalho principal do usuário que está registrando o tempo. <br><span class="preview">Quando o horário é registrado para um usuário ou função que tem uma atribuição específica de localização nas atribuições avançadas, a taxa da localização é usada.</span> <br>Se o usuário que estiver registrando o horário não tiver uma função de trabalho associada a ele, ou se a função de trabalho principal não tiver uma taxa de cobrança, a Receita Efetiva será de $0,00. </td> 
     <td> Se o usuário que registra a hora estiver atribuído à tarefa, a taxa de cobrança da função de trabalho associada ao usuário na tarefa será usada para calcular a Receita Efetiva. <br><span class="preview">Quando o horário é registrado para um usuário ou função que tem uma atribuição específica de localização nas atribuições avançadas, a taxa da localização é usada.</span> <br>Caso contrário, a taxa de cobrança da função de trabalho principal será usada. Se o usuário não tiver uma função de trabalho principal ou se sua função de trabalho principal não tiver uma taxa de cobrança, a Receita Real será de US$ 0,00. </td> 
     <td>Se uma das funções de trabalho do usuário que está registrando o tempo for atribuída à tarefa, essa taxa de função de trabalho será usada. Se a função de trabalho atribuída à tarefa não estiver associada ao usuário que registra o tempo, a taxa de cobrança da função principal do usuário será usada para calcular a Receita Efetiva. Se o usuário não tiver uma função de trabalho ou se não houver nenhuma taxa associada à função de trabalho principal, a taxa da função de trabalho atribuída à tarefa será usada. </td> 
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

### Cálculos de receita para projetos

Você pode rastrear os seguintes tipos de receita para projetos:

* A receita planejada de um projeto é calculada pela seguinte fórmula:

  `Project Planned Revenue = SUM(Task Planned Revenue)+ Fixed Revenue`

  Para obter informações sobre como a receita planejada da tarefa é calculada, consulte a seção [Cálculos de receita para tarefas baseadas nas atribuições de usuário e função](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) neste artigo.

* A Receita atual de um projeto é calculada pela seguinte fórmula:

  `Project Actual Revenue = SUM (Task Actual Revenue) + (Hours logged for the project x User Billing per Hour Rate) + SUM (Hours logged for the issues x User Billing per Hour rate)`

Para obter informações sobre como a Receita Efetiva da tarefa é calculada, consulte a seção [Cálculos de receita para tarefas baseadas nas atribuições de usuário e função](#revenue-calculations-for-tasks-based-on-user-and-role-assignments) neste artigo.

Para a Receita real associada às horas registradas diretamente no projeto ou aos problemas, o Workfront usa a Taxa de cobrança do usuário que registra o tempo no projeto. Se o usuário não tiver uma Taxa de cobrança associada ao perfil, o Workfront usará a Taxa de cobrança da função de trabalho principal. Se ambas as taxas forem zero, a Receita Real associada às horas registradas no projeto ou aos problemas será zero.
