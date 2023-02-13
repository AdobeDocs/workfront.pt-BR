---
product-area: projects
navigation-topic: financials
title: Visão Geral das Taxas de Faturamento da Função do Trabalho e cálculo da Receita em um projeto
description: Você pode usar as taxas de faturamento para calcular a receita em seus projetos quando você as multiplica pelas horas gastas no projeto. Para obter mais informações sobre taxas de faturamento e receita, consulte o artigo Visão geral de faturamento e receita.
author: Alina
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '3644'
ht-degree: 0%

---

# Visão Geral das Taxas de Faturamento da Função do Trabalho e cálculo da Receita em um projeto

Você pode usar as taxas de faturamento para calcular a receita em seus projetos quando você as multiplica pelas horas gastas no projeto. Para obter mais informações sobre taxas de faturamento e receita, consulte o artigo [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because the only procedure here was moved to a different article.&nbsp;This stays as an overview)</p>
<h2>Access requirements</h2>
<p>You must have the following access to perform the steps in this article:</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Adobe Workfront plan*</td>
<td> <p>Any</p> </td>
</tr>
<tr>
<td role="rowheader">Adobe Workfront license*</td>
<td> <p>Plan </p> </td>
</tr>
<tr>
<td role="rowheader">Access level configurations*</td>
<td> <p>Edit access to Projects and Financial&nbsp;Data</p> <note type="note">
If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see
<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.
</note> </td>
</tr>
<tr>
<td role="rowheader">Object permissions</td>
<td> <p>Manage permissions to the project with permissions to Manage Finance</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td>
</tr>
</tbody>
</table>
<p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p>
</div>
-->

## Visão Geral das Taxas de Faturamento da Função de Trabalho e Tipos de Receita por Hora

Como administrador do Adobe Workfront, você pode associar taxas de faturamento a usuários e funções de trabalho.\
Para obter mais informações sobre como criar usuários e associá-los às taxas de faturamento, consulte o artigo [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Para obter mais informações sobre como criar funções de cargo e associá-las a taxas de faturamento, consulte o artigo [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

As taxas de faturamento associadas aos usuários não podem ser substituídas.

As taxas de faturamento associadas às funções de jobs podem ser substituídas no nível da empresa ou do projeto.

Para calcular a receita em projetos com base nas taxas de faturamento das funções de cargo, a variável **Tipo de receita** das tarefas dos projetos deve ser uma das seguintes:

* Horas por Valor da Hora do Perfil
* Horas por Valor da Hora do Perfil, com Teto
* Função por hora mais fixa

Para obter mais informações sobre **Tipo de receita** e taxas de faturamento, consulte [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## A hierarquia da Taxa de Faturamento se sobrepõe ao calcular a Receita

Uma função de trabalho pode ter uma taxa de faturamento associada a ela das seguintes maneiras:

* Como administrador do Workfront, você pode definir a taxa de faturamento no nível do sistema associada a uma função de cargo ao criar essa função de trabalho.\
   Para obter mais informações sobre a criação de funções de job, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Como administrador do Workfront, você pode definir a taxa de faturamento no nível da empresa para a mesma função de trabalho ao criar uma empresa.\
   Quando a Workfront calcula a receita dos projetos associados a essa empresa, a taxa de faturamento da empresa é usada quando a função é atribuída às tarefas, em vez da taxa de faturamento no nível do sistema para essa função de trabalho.\
   As taxas de função de trabalho alteradas no nível da empresa afetarão todos os projetos associados a essa empresa.

   >[!NOTE]
   >
   >Se você precisar atualizar a taxa de faturamento da Empresa, a taxa no projeto não será atualizada automaticamente. Você deve remover a Empresa do projeto, atualizar a taxa para a Empresa e, em seguida, reanexar a Empresa ao projeto, antes que a nova taxa da Empresa entre em vigor no projeto. Para obter instruções sobre como anexar uma empresa a um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

   Para obter mais informações sobre como criar taxas de faturamento de função de cargo específicas para uma empresa, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Como administrador do Workfront, você pode ativar uma opção ao editar um projeto para aplicar alterações nas taxas de faturamento da empresa ao projeto quando os usuários recalcular manualmente as finanças do projeto.\
   Para obter mais informações, consulte [Substituir as taxas de faturamento no nível do projeto por taxas de faturamento no nível da empresa](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

* Como gerente de projeto, você pode definir a taxa de faturamento para a mesma função de trabalho no nível do projeto.\
   As taxas de função de trabalho alteradas no projeto afetarão somente esse projeto.

   Para obter informações sobre a substituição de taxas de função para o projeto, consulte [Substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Se uma função de cargo estiver associada a uma taxa de faturamento no nível do sistema, no nível da Empresa e no nível do projeto, o Workfront calculará a receita das tarefas usando a taxa de faturamento da função de cargo no nível do projeto, quando usar as taxas de função de cargo. A receita de todas as tarefas é acumulada até a receita do projeto.

## Substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto

Como gerente de projeto, você pode especificar a taxa de faturamento de uma função de cargo em um projeto específico. Essa taxa de faturamento no nível do projeto substitui a taxa de faturamento no nível do sistema para essa função de trabalho. O Workfront usa a taxa de faturamento no nível do projeto da função de trabalho para calcular a receita, em vez de usar a taxa de faturamento no nível do sistema.

Para obter informações sobre como substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto, consulte [Substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Para obter mais informações sobre qual função de cargo é usada para calcular a receita no projeto, consulte a seção &quot;Cálculos de receita para tarefas com base em atribuições de usuário e função&quot; em [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>No caso da Receita Real, as taxas de faturamento aplicadas às horas adicionadas a um Registro de Faturamento que está marcado como Faturado não devem ser afetadas pelas substituições da taxa de faturamento que ocorrem após o Registro de Faturamento ter sido faturado.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted and linked above to the stand-alone article for overriding billing rates on projects.)</p>
<p>You can override the billing rate of a job role on a project in the following ways:</p>
<ul>
<li>One time, by selecting a new rate for the job role.<br>The new rate is used for the entire duration of the project, to calculate revenue. </li>
</ul>
<ul>
<li>Several times, by selecting several new rates for specific date ranges. <br>A different rate can be used during each specified date range.</li>
</ul>
<p>To override a billing rate for a project:</p>
<ol>
<li value="1">Go to the project you want to override billing rates for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Billing Rates</strong> in the left panel. You might have to first click <strong>Show More</strong>. </p> </li>
<li value="3"> <p>Click <strong>Add Billing Rate</strong> > <strong>New Billing Rate</strong>.</p> <p>The New Billing Rate box opens</p> <p> <img src="assets/override-billing-rate-on-project-nwe-350x310.png" style="width: 350;height: 310;"> </p> <p> <br>The <strong>Default Billing Rate</strong> field displays the system-level rate for this job role.</p> </li>
<li value="4">In the <strong>Job Role</strong> field, select the job role you want to change the billing rate for.<br></li>
<li value="5">In the <strong>Billing Rates 1</strong> field, enter the one time billing rate override, then click <strong>Save</strong> to override the billing rate one time, <br>Or Click <strong>Add Rate</strong> to add more billing rate overrides.</li>
<li value="6">(Conditional) If you are adding more than one billing rate override, specify the following information:<br>- <strong>Billing Rates 1</strong>: the value of the Billing Rate from the beginning of the project to the first date of the first override. This is typically the same amount as the <strong>Default Rate</strong>.<br>- <strong>Start Date</strong>: this is the date when the Default Rate ends.<br>- <strong>End Date</strong>: the date when the new billing rate override ends. <br>Workfront applies the override job role rate to the hours that occur during the time frames specified when calculating revenue on the project.<br>There should be no gaps between the time frames of two override rates. The <strong>Start Date</strong> of an override rate should be the day immediately following the <strong>End Date</strong> of the previous override date.<br><note type="note">
You cannot specify a
<strong>Start Date</strong> for the first override rate, nor an
<strong>End Date</strong> for the last override rate. We recommend that you use the Default Rate for the first override rate.
<br>Workfront assumes that the first override rate is applied for all hours with a date older than the
<strong>End Date</strong> of the first override, and that the last override rate is applied for all hours with a date newer than the
<strong>Start Date</strong> of the last override.
<br>If an hour is logged before the Planned Start Date of the project the very first billing rate is used.
<br>If an hour is logged after the Planned Completion Date of the project the very last billing rate is used.
</note><br></li>
<li value="7">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Visão geral da seção Taxas de Faturamento de um projeto

Depois de especificar as taxas de faturamento de substituição para as funções de job associadas ao projeto, você pode ver todas as funções de job e suas substituições na **Taxas de Faturamento** do projeto.

Observe as seguintes informações na lista de **Taxas de Faturamento**:

* [Agrupamento de Função de Trabalho](#job-role-grouping)
* [Valor da Taxa de Faturamento do Projeto](#project-billing-rate-value)
* [Valor padrão da Taxa de Faturamento](#default-billing-rate-value)
* [Valor da Taxa de Faturamento da Empresa](#company-billing-rate-value)
* [Vários valores e cronogramas da Taxa de Faturamento](#multiple-billing-rate-values-and-timeframes)

### Agrupamento de Função de Trabalho {#job-role-grouping}

As taxas de faturamento são agrupadas na variável **Taxas de Faturamento** por suas respectivas funções.

### Valor da Taxa de Faturamento do Projeto {#project-billing-rate-value}

Na linha de agrupamento correspondente a uma função de cargo, observe a taxa de faturamento dessa função de cargo no nível do projeto na **Taxa de Faturamento do Projeto** coluna. Se a função de trabalho tiver várias taxas de substituição, a taxa de substituição correspondente à data atual será exibida na linha de agrupamento na **Taxa de Faturamento do Projeto** coluna.

### Valor padrão da Taxa de Faturamento {#default-billing-rate-value}

Na linha de agrupamento de uma função de cargo, observe a taxa de faturamento dessa função de cargo no nível do sistema na **Taxa de Faturamento Padrão** coluna.

>[!NOTE]
>
>Se houver taxas de faturamento do projeto para uma função de cargo, a variável **Taxa de Faturamento Padrão** nunca é aplicada para calcular a Receita do projeto. Somente a variável **Taxas de Faturamento do Projeto** são aplicadas para calcular a Receita.

### Valor da Taxa de Faturamento da Empresa {#company-billing-rate-value}

Na linha de agrupamento de uma função de cargo, observe a taxa de faturamento dessa função de cargo no nível da empresa na **Taxa de Faturamento da Empresa** coluna. Isso significa que há uma empresa associada a esse projeto e essa função de trabalho tem uma taxa de faturamento diferente para essa empresa. A taxa de faturamento da empresa é exibida, mesmo se for igual à taxa do projeto.

>[!NOTE]
>
>Se houver taxas de faturamento do projeto para uma função de cargo, a variável **Taxa de Faturamento da Empresa** nunca é aplicada para calcular a receita do projeto. Somente a variável **Taxas de Faturamento do Projeto** são aplicadas para calcular a receita.

### Vários valores e cronogramas da Taxa de Faturamento {#multiple-billing-rate-values-and-timeframes}

Se você tiver várias taxas de faturamento de substituição para uma função de cargo específica, elas serão listadas no agrupamento dessa função de cargo. Usando a edição em linha, você pode alterar as taxas de substituição e a variável **Iniciar** **Data** e **Data final** das taxas de faturamento de sobreposição nesta guia.

>[!NOTE]
>
>Não é possível especificar uma **Data inicial** para a primeira taxa de substituição e não é possível especificar um **Data final** para a última taxa de substituição. A Workfront parte do princípio que a primeira taxa de substituição é aplicada para todas as horas com uma data anterior à data **Data final** da primeira substituição e que a última taxa de substituição é aplicada para todas as horas com uma data mais recente que a **Data inicial** da última substituição.\
>Se uma hora for registrada antes da Data inicial planejada do projeto, a primeira taxa de faturamento será usada.\
>Se uma hora for registrada após a Data de conclusão planejada do projeto, a última taxa de faturamento será usada.

## Calcular Receita Planejada

* [Calcular Receita Planejada com base em uma sobreposição de Taxa de Faturamento única](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Calcular Receita Planejada com base em várias sobreposições da Taxa de Faturamento](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Distribuição de Horas Planejadas durante a Duração de uma tarefa](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calcular Receita Planejada com base em uma sobreposição de Taxa de Faturamento única {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Considere o seguinte ao calcular a Receita Planejada com base em uma sobreposição de taxa de Faturamento única:

* Quando a variável **Tipo de receita** de uma tarefa **Função por hora**, o Workfront multiplica as Horas Planejadas de uma tarefa pela taxa de faturamento da função de trabalho associada à tarefa para calcular a Receita Planejada na tarefa.

* Quando a taxa de faturamento da função de trabalho tiver sido substituída no nível do projeto, o Workfront usará a taxa de sobreposição do projeto para calcular a Receita Planejada.
* Quando uma tarefa tem várias atribuições, a Receita Planejada é calculada multiplicando a taxa de faturamento da função de trabalho de cada atribuição e sua respectiva alocação de Hora Planejada.

>[!NOTE]
>
>As Horas Planejadas por atribuição não são as mesmas que as Horas Planejadas para a tarefa, no caso de várias atribuições.

Para obter mais informações sobre qual função de cargo é usada para calcular a Receita Planejada, consulte a seção &quot;Noções Gerais de Cálculos de Receita para Tarefas com Base em Atribuições de Usuário e Função&quot; no artigo [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calcular Receita Planejada com base em várias sobreposições da Taxa de Faturamento {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Considere o seguinte ao calcular a Receita Planejada com base em várias substituições da Taxa de Faturamento:

* Quando a variável **Tipo de receita** de uma tarefa **Função por hora**, o Workfront multiplica as Horas Planejadas de uma tarefa pela taxa de faturamento da função de trabalho associada à tarefa para calcular a Receita Planejada na tarefa.

   Para obter mais informações sobre qual função de cargo é usada para calcular a Receita Planejada, consulte a seção &quot;Noções Gerais de Cálculos de Receita para Tarefas com Base em Atribuições de Usuário e Função&quot; no artigo [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* No caso de várias substituições da taxa de faturamento, a taxa pela qual as Horas Planejadas são multiplicadas muda durante a duração de uma tarefa. Por padrão, o Workfront distribui as Horas Planejadas uniformemente na duração de uma tarefa, alocando um número igual de horas para cada dia da tarefa. Ao calcular **Receita planejada** para uma tarefa, o Workfront multiplica a Hora Planejada por Dia pela taxa de faturamento desse dia. No caso de várias taxas de faturação, essa taxa pode ser diferente todos os dias.

   Por exemplo, você tem uma tarefa com uma Função por hora **Tipo de receita**. A tarefa tem uma duração de 5 dias e um valor de Horas Planejadas de 40 horas. As Horas Planejadas por Dia são de 8 horas. Atribua uma função de trabalho do Gerenciador de Projetos à tarefa e substitua a taxa de faturamento dessa função de trabalho pelos últimos 3 dias da tarefa, de modo que você terá uma taxa de faturamento de Taxa 1 para os primeiros dois dias e Taxa 2 para os 3 dias restantes da tarefa para esta função de cargo.

   A fórmula que calcula a **Receita planejada** desta tarefa está:

   ```
   Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
   ```

Para obter mais informações sobre como encontrar o valor de Horas Planejadas por Dia no Workfront, consulte a seção [Distribuição de Horas Planejadas durante a Duração de uma tarefa](#distribution-of-planned-hours-across-the-duration-of-a-task) neste artigo.

>[!NOTE]
>
>Se você tiver vários destinatários na tarefa, a quantidade de Horas Planejadas será distribuída primeiro para cada destinatário e, em seguida, para cada dia durante a duração da tarefa. Nesse caso, a Receita Planejada será calculada levando em conta a quantidade de horas diárias de cada destinatário e a taxa de faturamento de cada função de cargo que pode mudar durante a duração da tarefa, no caso de várias taxas de faturamento.

### Distribuição de Horas Planejadas durante a Duração de uma tarefa {#distribution-of-planned-hours-across-the-duration-of-a-task}

Considere o seguinte ao entender a distribuição de Horas Planejadas na Duração de uma tarefa:

* Por padrão, o Workfront distribui as Horas Planejadas uniformemente na Duração de uma tarefa, alocando um número igual de Horas Planejadas para cada dia da tarefa, com base na disponibilidade do agendamento do projeto.

   Para obter mais informações sobre como entender a distribuição de Horas Planejadas durante a Duração de uma tarefa, consulte a seção &quot;Como entender a distribuição de horas planejadas durante a duração de uma tarefa&quot; no artigo [Visão geral das Horas Planejadas](../../../manage-work/tasks/task-information/planned-hours.md).

   >[!NOTE]
   >
   >As Horas Planejadas por Dia são a alocação de Horas Planejadas para cada dia durante a Duração da tarefa. Se a tarefa tiver uma atribuição, esse número também representará as Horas Planejadas por Dia por atribuição. Se a tarefa tiver várias atribuições, as Horas Planejadas por Dia por atribuição serão diferentes das Horas Planejadas por Dia para a tarefa. Não há representação visual no Workfront para as Horas Planejadas por Dia por atribuição, para tarefas com várias atribuições.
   >
   >
   >As Horas Planejadas por Dia são multiplicadas pela taxa de faturamento da função de trabalho atribuída à tarefa para esse dia para calcular a Receita Planejada por Dia para essa tarefa. Uma soma de todas as Receitas Planejadas diárias calculadas dessa forma é igual à Receita Planejada para essa tarefa.

## Calcular Receita Real

* [Calcular a Receita Real com base em uma sobreposição da Taxa de Faturamento única](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calcular a receita real com base em várias sobreposições da taxa de faturamento](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calcular a Receita Real com base em uma sobreposição da Taxa de Faturamento única {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Considere o seguinte ao calcular a Receita Real com base em uma sobreposição de Taxa de Faturamento única:

* Quando a variável **Tipo de receita** de uma tarefa **Função por hora**, o Workfront multiplica a variável **Horas reais** de uma tarefa pela taxa de faturamento da função de trabalho associada à tarefa a ser calculada **Receita real** na tarefa. Horas reais são horas registradas diretamente na tarefa.

   Para obter mais informações sobre qual função de trabalho é usada para calcular **Receita real**, consulte a seção &quot;Como entender cálculos de receita para tarefas com base em atribuições de usuário e função&quot; no artigo [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Se a taxa de faturamento da função de trabalho tiver sido substituída no nível do projeto, o Workfront usará a taxa de substituição do projeto para calcular a Receita Real. Quando você substitui a taxa de faturamento da função de trabalho no projeto, a variável **Receita real** do projeto é recalculado automaticamente usando a nova taxa ajustada.

   Para obter informações sobre a substituição de taxas de função para o projeto, consulte [Substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Se desejar manter as horas em que você já fez logon no projeto antes de sobrepor a taxa de faturamento original faturada na taxa original, você deve incluí-las em um **Registro de Faturamento** e você deve marcar o **Registro de Faturamento** as **Faturado**. Caso contrário, a variável **Receita real** das horas registradas antes da substituição da taxa de faturamento do projeto, o será recalculado usando a nova taxa quando as finanças dos projetos forem recalculadas.\
>Para obter mais informações sobre como incluir horas em um registro de faturamento e marcá-lo como **Faturado**, consulte o artigo [Criar registros de faturamento](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calcular a receita real com base em várias sobreposições da taxa de faturamento {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Considere o seguinte ao calcular a Receita Real com base em várias substituições da Taxa de Faturamento:

* Quando a variável **Tipo de receita** de uma tarefa **Função por hora**, o Workfront multiplica a variável **Horas reais** na tarefa com a taxa de faturamento das funções de job atribuídas à tarefa para calcular **Receita real** na tarefa. Horas reais são horas registradas diretamente na tarefa.

* No caso de várias substituições de taxa de faturamento, a taxa pela qual a variável **Horas reais** são multiplicadas para calcular a variável **Receita real** pode mudar durante a duração de uma tarefa. O Workfront usa a taxa de faturamento da função de trabalho cujo período corresponde ao período **Data de entrada** das horas registradas para a tarefa calcular **Receita Real.**

   Por exemplo, uma tarefa tem a variável **Tipo de receita** de **Função por hora** e é atribuído à função de trabalho do Gerenciador de Projetos. Substitua a taxa de faturamento desta função de cargo pela Taxa 1 para as datas entre 19 de junho e 25 de junho. A partir de 26 de junho, substitua a taxa de faturamento pela Taxa 2. Registre 2 horas para 20 de junho e 3 horas para 28 de junho.

   A Workfront calcula a variável **Receita real** para esta tarefa usando a seguinte fórmula:

   ```
   Actual Revenue = 2 * Rate 1 + 3 * Rate 2
   ```

   Para obter mais informações sobre qual função de trabalho é usada para calcular **Receita real**, consulte a seção &quot;Como entender cálculos de receita para tarefas com base em atribuições de usuário e função&quot; no artigo [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## O impacto dos Fusos Horários ao calcular a Receita com base em várias Taxas de Faturamento

Os usuários podem ver diferentes Horas Planejadas por Dia de outros usuários, se houver diferenças de fuso horário entre eles e outras entidades no Workfront. Os seguintes cenários podem distorcer as informações de Horas Planejadas por Dia para um usuário do que outro usuário vê:

* Os dois usuários podem ter seus computadores definidos para dois fusos horários diferentes
* Os dois perfis de usuário no Workfront podem ser definidos como dois fusos horários diferentes
* O fuso horário associado ao perfil do usuário pode ser diferente do fuso horário do sistema no Workfront
* O fuso horário associado ao perfil do usuário pode ser diferente do Fuso horário do agendamento do projeto.

Nesses casos, o número de Horas Planejadas por Dia pode ser diferente entre dois usuários que não compartilham as mesmas configurações para fusos horários. Eles também verão números diferentes da Receita planejada ao usar várias substituições de taxa de faturamento em um projeto.

* [Calcular a receita planejada para usuários em fusos horários diferentes](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calcular a receita real para usuários em fusos horários diferentes](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calcular a receita planejada para usuários em fusos horários diferentes {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Se você tiver usuários em fusos horários diferentes trabalhando nos mesmos projetos, recomendamos que você não altere as substituições da taxa de faturamento para seus projetos durante a semana. Isso pode exibir uma quantidade incorreta da Receita planejada para o seu projeto, como resultado de diferenças de hora entre os fusos horários na programação dos usuários e o fuso horário do sistema Workfront . A maioria dos agendamentos permite que os fins de semana sejam excluídos dos cálculos de Horas Planejadas. Se uma alteração ocorrer na substituição da taxa de faturamento de uma função de trabalho, é melhor que ocorra durante um fim de semana do que no meio de uma semana em que possa coincidir com o meio da Duração de uma tarefa.

Considere o seguinte ao calcular a Receita Planejada para usuários em fusos horários diferentes:

* Para tarefas que têm um **Tipo de receita** de **Função por hora** e são atribuídas a funções de tarefa, **Receita planejada** é calculada multiplicando o **Horas Planejadas** de uma tarefa pela taxa de faturamento da função de trabalho.

* O **Horas Planejadas** são distribuídos uniformemente na variável **Duração** da tarefa.

* O **Duração** é o período de tempo entre o **Início planejado** **Data** e **Data de Conclusão Planejada** da tarefa. Porque a variável **Data de início planejada** e **Data de Conclusão Planejada** das tarefas podem diferir dependendo dos fusos horários dos usuários que visualizam a tarefa, a quantidade de Horas Planejadas por Dia pode ser diferente para dois usuários em dois fusos horários diferentes.

* A quantidade de Horas Planejadas por Dia não altera a Receita Planejada de um projeto se a taxa de faturamento da função de trabalho não for alterada ou se houver apenas uma sobreposição de taxa de faturamento. Nesse caso, mesmo que dois usuários de dois fusos horários diferentes vejam Horas planejadas diferentes por dia, a Receita planejada geral do projeto é idêntica entre os dois usuários.

   No entanto, no caso de várias substituições da taxa de faturação, o valor global **Receita planejada** do projeto pode parecer diferente para dois usuários em dois fusos horários diferentes, pois depende da quantidade de Horas Planejadas por Dia (que pode ser diferente para os dois usuários) e da substituição da taxa de faturamento (que pode ser diferente para o mesmo dia, quando cada usuário está olhando para a tarefa em seu próprio fuso horário).

* A exatidão **Receita planejada** amount é o acessado pelo usuário que tem o mesmo fuso horário que o Fuso horário de sua instância do Workfront. O administrador do Workfront define o Fuso horário do Workfront na área Informações do cliente do sistema.\
   Para obter mais informações sobre como definir o Fuso Horário de seu sistema, consulte o artigo [Configurar informações básicas para seu sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calcular a receita real para usuários em fusos horários diferentes {#calculate-actual-revenue-for-users-in-different-time-zones}

Considere o seguinte ao calcular a Receita Real para usuários em fusos horários diferentes:

* Quando a variável **Tipo de receita** de uma tarefa **Função por hora**, o Workfront multiplica a variável **Horas reais** na tarefa com a taxa de faturamento das funções de job atribuídas à tarefa para calcular o valor de **Receita real**. Horas reais são horas registradas diretamente na tarefa.

* No caso de várias substituições de taxa de faturamento, o Workfront usa a taxa de faturamento da função de trabalho cujo período corresponde ao período **Data de entrada** das horas registradas para a tarefa calcular **Receita real**.

* Como não há carimbo de data e hora no **Data de entrada** de horas registradas e não houver carimbo de data e hora nos intervalos de data de várias substituições de taxa de faturamento, **Receita real** os cálculos não são afetados pelo Fuso horário associado aos usuários.

Para obter mais informações sobre qual função de trabalho é usada para calcular **Receita real**, consulte a seção &quot;Como entender cálculos de receita para tarefas com base em atribuições de usuário e função&quot; no artigo [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Recalcular as finanças do projeto

As finanças são calculadas em um projeto conforme as alterações ocorrem nas horas registradas para o projeto.

Se as taxas forem alteradas durante a vida de um projeto, você poderá recalcular manualmente os custos e as receitas do projeto, usando a opção Recalcular Financiamento em um projeto. Além disso, algumas ações acionam um recálculo automático.

Para obter mais informações sobre o recálculo das finanças do projeto, consulte o artigo [Recalcular as finanças do projeto](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Adicionar uma nova Taxa de Faturamento usando a API

Para adicionar uma nova taxa de faturamento para uma função de trabalho usando a API, execute um *setRatesForRole* ação para **Rate** usando o *método PUT*.
A ação e os campos de data na **Rate** estão disponíveis na API versão 8.0. Se você já tiver várias taxas de faturamento definidas para uma função de trabalho em um projeto e quiser adicionar uma nova taxa de faturamento para ele com um novo intervalo de datas, deverá incluir a taxa existente e a taxa a ser adicionada na mesma chamada de API. É semelhante à forma como você atualiza coleções em objetos.

A chamada de API a seguir é um exemplo em que **attachmentID** é **ID do projeto** do projeto ao qual você está adicionando a taxa e **RoleID** é **ID da Função da Tarefa** para o qual você está adicionando a nova taxa de faturamento.<pre>{</pre><pre>&quot;attachmentID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachmentObjCode&quot;: &quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df00014148cda5136d4b79d09&quot;, </pre><pre>&quot;Taxas&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;2017-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Para obter mais informações sobre como usar a API do Workfront, consulte o artigo [Noções básicas da API](https://experience.workfront.com/s/article/API-Basics-638808549).
