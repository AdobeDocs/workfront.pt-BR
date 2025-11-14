---
product-area: projects
navigation-topic: financials
title: Visão geral da substituição de taxas de cobrança de função de trabalho e do cálculo da receita em um projeto
description: É possível usar as taxas de faturamento para calcular a receita dos projetos quando você as multiplica pelas horas gastas no projeto. Para obter mais informações sobre taxas de faturamento e receita, consulte o artigo Visão geral de faturamento e receita.
author: Lisa
feature: Work Management
exl-id: 63ba6758-ba62-48b4-89f4-d784e32a1bfa
source-git-commit: 01a80f6140650ca12aaee14115f79449dcfa2a18
workflow-type: tm+mt
source-wordcount: '3859'
ht-degree: 0%

---

# Visão geral da substituição de Taxas de cobrança de função de trabalho e do cálculo de Receita em um projeto

{{highlighted-preview}}

É possível usar as taxas de faturamento para calcular a receita dos projetos quando você as multiplica pelas horas gastas no projeto. Para obter mais informações sobre taxas de cobrança e receita, consulte o artigo [Visão Geral de Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Visão Geral das Taxas de Faturamento de Função de Trabalho e Tipos de Receita por Hora de Função

Como administrador do Adobe Workfront, você pode associar taxas de faturamento a usuários e funções de trabalho.\
Para obter mais informações sobre como criar usuários e associá-los a taxas de cobrança, consulte o artigo [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md). Para obter mais informações sobre como criar funções de trabalho e associá-las a taxas de cobrança, consulte o artigo [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Taxas de cobrança associadas a usuários não podem ser substituídas.

As taxas de cobrança associadas a funções de trabalho podem ser substituídas no nível da empresa ou do projeto.

Para calcular a receita em projetos com base nas taxas de cobrança de funções de trabalho, o **Tipo de receita** das tarefas nos projetos deve ser um dos seguintes:

* Horas por Valor da Hora do Perfil
* Horas por Valor da Hora do Perfil, com Teto
* Horas por Valor da Hora do Perfil mais Taxa Fixa

Para obter mais informações sobre **Tipo de receita** e taxas de cobrança, consulte [Visão geral de cobrança e receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Hierarquia de sobreposições de Taxa de Cobrança ao calcular Receita

Uma função de trabalho pode ter uma taxa de cobrança associada a ela das seguintes maneiras:

* Como administrador do Workfront, você pode definir a taxa de cobrança no nível do sistema associada a uma função de trabalho ao criar essa função de trabalho.\
  Para obter mais informações sobre como criar funções de trabalho, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* Como administrador do Workfront, você pode definir a taxa de cobrança no nível da empresa para a mesma função de trabalho ao criar uma empresa.\
  Quando a Workfront calcula a receita para os projetos associados a esta empresa, a taxa de cobrança da empresa é usada quando a função é atribuída a tarefas, em vez da taxa de cobrança no nível do sistema para esta função de trabalho.\
  As taxas de função de trabalho alteradas no nível da empresa afetarão todos os projetos associados a essa empresa.

  >[!NOTE]
  >
  >Se você precisar atualizar a taxa de cobrança da Empresa, a taxa no projeto não será atualizada automaticamente. Você deve remover a Empresa do projeto, atualizar a taxa para a Empresa e, em seguida, reanexar a Empresa ao projeto, antes que a nova taxa da Empresa entre em vigor no projeto. Para obter instruções sobre como anexar uma Empresa a um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

  Para obter mais informações sobre como criar taxas de cobrança de funções de trabalho específicas para uma empresa, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* Como administrador do Workfront, você pode ativar uma opção ao editar um projeto para aplicar alterações nas taxas de cobrança no nível da empresa ao projeto quando os usuários recalcularem manualmente as finanças do projeto.\
  Para obter mais informações, consulte [Substituir taxas de cobrança no nível do projeto por taxas de cobrança no nível da empresa](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

<div class="preview">

* Como administrador do Workfront, você pode definir cartões de taxa com várias taxas de cobrança por função, com base no local e na data. Quando um cartão de taxa é anexado a um projeto, todas as funções (por local, se locais forem usados) e suas taxas de cobrança associadas são adicionadas à seção taxas de cobrança do projeto. Anexar um cartão de taxa substitui todas as taxas de faturamento existentes no projeto.

  Para obter mais informações, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md) e [Anexar um cartão de taxa a um projeto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

</div>

* Como gerente de projeto, você pode definir a taxa de faturamento para a mesma função de trabalho no nível do projeto.\
  As taxas de função de trabalho alteradas no projeto afetarão somente esse projeto.

  Para obter informações sobre substituição de taxas de função para o projeto, consulte [Substituir taxas de cobrança de função de trabalho no nível do projeto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!IMPORTANT]
>
>Se uma função de trabalho estiver associada a uma taxa de faturamento no nível do sistema, no nível da Empresa e no nível do projeto, o Workfront calculará a receita das tarefas usando a taxa de faturamento da função de trabalho no nível do projeto, quando usar as taxas da função de trabalho. A receita de todas as tarefas totaliza a receita do projeto.

## Substituir Taxas de Cobrança de Função de Trabalho no nível do projeto

Como gerente de projeto, você pode especificar a taxa de faturamento de uma função de trabalho em um projeto específico. Essa taxa de cobrança no nível do projeto substitui a taxa de cobrança no nível do sistema para essa função de trabalho. O Workfront usa a taxa de cobrança no nível do projeto da função de trabalho para calcular a receita, em vez de usar a taxa de cobrança no nível do sistema.

<span class="preview">Você também pode anexar um cartão de taxa ao projeto, o que importará as taxas de cobrança da função de trabalho do cartão de taxa para o projeto.</span>

Para obter informações sobre como substituir as Taxas de Cobrança de Função de Trabalho no nível do projeto, consulte [Substituir Taxas de Cobrança de Função de Trabalho no nível do projeto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

Para obter mais informações sobre qual função de trabalho é usada para calcular a receita no projeto, consulte a seção &quot;Cálculos de receita para tarefas baseadas em atribuições de usuário e função&quot; em [Visão geral de faturamento e receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md). <span class="preview">Para obter informações sobre como anexar um cartão de taxa a um projeto, consulte [Anexar um cartão de taxa a um projeto](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).</span>

>[!NOTE]
>
>No caso da receita real, as taxas de cobrança aplicadas a horas que são adicionadas a um registro de cobrança que está marcado como faturado não devem ser afetadas por sobreposições de taxa de cobrança que ocorrem após o registro de cobrança ter sido faturado.

## Visão Geral da seção Taxas de Faturamento de um projeto

Depois de especificar as taxas de cobrança de substituição para as funções de trabalho associadas ao projeto, você pode ver todas as funções de trabalho e suas substituições na guia **Taxas de Cobrança** do projeto.

Observe as seguintes informações na lista de **Taxas de cobrança**:

* [Agrupamento de Funções de Trabalho](#job-role-grouping)
* [Valor da Taxa de Cobrança do Projeto](#project-billing-rate-value)
* [Valor padrão da taxa de cobrança](#default-billing-rate-value)
* [Valor da taxa de cobrança da empresa](#company-billing-rate-value)
* [Vários valores de Taxa de Cobrança e cronogramas](#multiple-billing-rate-values-and-timeframes)

### Agrupamento de funções de trabalho {#job-role-grouping}

As taxas de cobrança são agrupadas na área **Taxas de Cobrança** por suas respectivas funções de trabalho. <span class="preview">Se um cartão de taxa estiver anexado ao projeto, as funções de trabalho também serão agrupadas por cartão de taxa. Se os locais forem aplicados às funções de trabalho, o nome do local será incluído como parte do nome da função de trabalho. Você pode ter a mesma função de trabalho listada para vários locais.</span>

### Valor da Taxa de Cobrança do Projeto {#project-billing-rate-value}

Na linha de agrupamento correspondente a uma função de trabalho, observe a taxa de cobrança dessa função de trabalho no nível do projeto na coluna **Taxa de Cobrança do Projeto**. Se a função de trabalho tiver várias taxas de substituição, a taxa de substituição correspondente à data atual será exibida na linha de agrupamento na coluna **Taxa de Cobrança do Projeto**.

### Valor da taxa de cobrança padrão {#default-billing-rate-value}

Na linha de agrupamento de uma função de trabalho, observe a taxa de cobrança dessa função de trabalho no nível do sistema na coluna **Taxa de Cobrança Padrão**.

>[!NOTE]
>
>Se houver taxas de cobrança do projeto para uma função de trabalho, a **Taxa de Cobrança Padrão** nunca será aplicada ao cálculo da Receita para o projeto. Somente as **Taxas de Cobrança do Projeto** são aplicadas para calcular a Receita.

### Valor da taxa de cobrança da empresa {#company-billing-rate-value}

Na linha de agrupamento de uma função de trabalho, observe a taxa de cobrança dessa função de trabalho no nível da empresa na coluna **Taxa de Cobrança da Empresa**. Isso significa que há uma empresa associada a este projeto e essa função de trabalho tem uma taxa de cobrança diferente para essa empresa. A taxa de faturamento da empresa é exibida, mesmo que seja a mesma da taxa do projeto.

>[!NOTE]
>
><span class="preview">Quando um cartão de taxa é anexado ao projeto, as **Taxas de Cobrança da Empresa** não são importadas nas taxas de cobrança. Os cálculos são baseados nas taxas de ficha ou nas taxas da empresa para as funções de trabalho.</span>
>
>Se houver taxas de cobrança do projeto para uma função de trabalho, a **Taxa de Cobrança da Empresa** nunca será aplicada ao cálculo da receita para o projeto. Somente as **Taxas de Cobrança do Projeto** são aplicadas para calcular a receita.

### Vários valores de Taxa de Cobrança e cronogramas {#multiple-billing-rate-values-and-timeframes}

Se você tiver várias taxas de faturamento de sobreposição para uma função de trabalho específica, elas serão listadas no agrupamento dessa função de trabalho. Usando a edição em linha, você pode alterar as taxas de substituição e a **Data de início****Data** e a **Data de término** das taxas de cobrança de substituição nesta guia.

>[!NOTE]
>
>Você não pode especificar uma **Data de Início** para a primeira taxa de substituição e não pode especificar uma **Data de Término** para a última taxa de substituição. A Workfront presume que a primeira taxa de substituição é aplicada para todas as horas com uma data anterior à **Data final** da primeira substituição e que a última taxa de substituição é aplicada para todas as horas com uma data posterior à **Data inicial** da última substituição.\
>Se uma hora for registrada antes da Data de início planejada do projeto, a primeira taxa de cobrança será usada.\
>Se uma hora for registrada depois da Data de conclusão planejada do projeto, a última taxa de cobrança será usada.

## Calcular Receita Planejada

* [Calcular receita planejada com base em uma substituição de taxa de cobrança única](#calculate-planned-revenue-based-on-a-one-time-billing-rate-override)
* [Calcular receita planejada com base em várias substituições de taxa de cobrança](#calculate-planned-revenue-based-on-multiple-billing-rate-overrides)
* [Distribuição de horas planejadas na duração de uma tarefa](#distribution-of-planned-hours-across-the-duration-of-a-task)

### Calcular Receita Planejada com base em uma substituição de Taxa de Faturamento única {#calculate-planned-revenue-based-on-a-one-time-billing-rate-override}

Considere o seguinte ao calcular a Receita Planejada com base em uma substituição de taxa de Faturamento ocasional:

* Quando o **Tipo de Receita** de uma tarefa é **Função por Hora**, a Workfront multiplica as Horas Planejadas de uma tarefa pela taxa de cobrança da função de trabalho associada à tarefa para calcular a Receita Planejada na tarefa.

* Quando a taxa de faturamento da função de trabalho for substituída no nível do projeto, o Workfront usará a taxa de substituição do projeto para calcular a Receita Planejada.
* Quando uma tarefa tem várias atribuições, a Receita Planejada é calculada multiplicando-se a taxa de faturamento da função de trabalho de cada atribuição e sua respectiva alocação de Hora Planejada.

>[!NOTE]
>
>As Horas Planejadas por atribuição não são as mesmas que as Horas Planejadas para a tarefa, no caso de várias atribuições.

Para obter mais informações sobre qual função de trabalho é usada para calcular a Receita Planejada, consulte a seção &quot;Understanding Revenue Calculations for Tasks Based on User and Role Assignments&quot; no artigo [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

### Calcular Receita Planejada com base em várias sobreposições de Taxa de Faturamento {#calculate-planned-revenue-based-on-multiple-billing-rate-overrides}

Considere o seguinte ao calcular a Receita Planejada com base em várias sobreposições de Taxa de Faturamento:

* Quando o **Tipo de Receita** de uma tarefa é **Função por Hora**, a Workfront multiplica as Horas Planejadas de uma tarefa pela taxa de cobrança da função de trabalho associada à tarefa para calcular a Receita Planejada na tarefa.

  Para obter mais informações sobre qual função de trabalho é usada para calcular a Receita Planejada, consulte a seção &quot;Understanding Revenue Calculations for Tasks Based on User and Role Assignments&quot; no artigo [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* No caso de várias sobreposições de taxa de faturamento, a taxa pela qual as Horas Planejadas são multiplicadas é alterada durante a duração de uma tarefa. Por padrão, o Workfront distribui as Horas planejadas uniformemente pela duração de uma tarefa, alocando um número igual de horas para cada dia da tarefa. Ao calcular a **Receita planejada** para uma tarefa, o Workfront multiplica a Hora planejada por dia pela taxa de cobrança desse dia. No caso de várias taxas de cobrança, essa taxa pode ser diferente todos os dias.

  Por exemplo, você tem uma tarefa com uma Função por hora **Tipo de receita**. A tarefa tem uma duração de 5 dias e um valor de Planned Hours de 40 horas. O Trabalho necessário por dia é de 8 horas. Atribua uma função de trabalho de Gerente de Projeto à tarefa e substitua a taxa de faturamento dessa função de trabalho para os últimos 3 dias da tarefa. Dessa forma, você terá uma taxa de faturamento de Taxa 1 para os primeiros dois dias e uma taxa de faturamento de Taxa 2 para os 3 dias restantes da tarefa para essa função de trabalho.

  A fórmula que calcula a **Receita Planejada** desta tarefa é:

  ```
  Planned Revenue = (Rate 1) * (Planned Hours for Day 1) + (Rate 1) * (Planned hours for Day 2) + (Rate 2) * (Planned hours for Day 3) + (Rate 2) * (Planned hours for Day 4) + (Rate 2) * (Planned hours for Day 5)
  ```

Para obter mais informações sobre como localizar o valor de Horas planejadas por dia no Workfront, consulte a seção [Distribuição de horas planejadas pela duração de uma tarefa](#distribution-of-planned-hours-across-the-duration-of-a-task) neste artigo.

>[!NOTE]
>
>Se houver vários designados na tarefa, a quantidade de Horas planejadas será distribuída primeiro a cada designado e, em seguida, a cada dia durante a duração da tarefa. Nesse caso, a receita planejada será calculada levando em conta a quantidade de horas diárias para cada destinatário e a taxa de cobrança de cada função de trabalho que pode mudar durante a duração da tarefa, no caso de várias taxas de cobrança.

### Distribuição de horas planejadas na duração de uma tarefa {#distribution-of-planned-hours-across-the-duration-of-a-task}

Considere o seguinte ao entender a distribuição de Horas Planejadas pela Duração de uma tarefa:

* Por padrão, o Workfront distribui as Horas planejadas uniformemente pela Duração de uma tarefa, alocando um número igual de Horas planejadas para cada dia da tarefa, com base na disponibilidade do agendamento do projeto.

  Para obter mais informações sobre como entender a distribuição de Horas Planejadas durante a duração de uma tarefa, consulte a seção &quot;Como entender a distribuição de Horas Planejadas durante a duração de uma tarefa&quot; no artigo [visão geral sobre Horas Planejadas](../../../manage-work/tasks/task-information/planned-hours.md).

  >[!NOTE]
  >
  >As horas planejadas por dia são a alocação das horas planejadas para cada dia durante a duração da tarefa. Se a tarefa tiver uma atribuição, esse número também representará as Horas Planejadas por Dia por atribuição. Se a tarefa tiver várias atribuições, as Horas Planejadas por Dia por atribuição serão diferentes das Horas Planejadas por Dia para a tarefa. Não há representação visual no Workfront para as Horas planejadas por dia por atribuição, para tarefas com várias atribuições.
  >
  >
  >As Horas Planejadas por Dia são multiplicadas pela taxa de faturamento da função de trabalho atribuída à tarefa para esse dia, a fim de calcular a Receita Planejada por Dia para essa tarefa. Uma soma de todas as Receitas planejadas diárias calculadas dessa forma é igual à Receita planejada para essa tarefa.

## Calcular Receita Real

* [Calcular a Receita Efetiva com base em uma substituição da Taxa de Cobrança única](#calculate-actual-revenue-based-on-a-one-time-billing-rate-override)
* [Calcular Receita Efetiva com base em várias sobreposições de Taxa de Faturamento](#calculate-actual-revenue-based-on-multiple-billing-rate-overrides)

### Calcular Receita Efetiva com base em uma substituição de Taxa de Faturamento ocasional {#calculate-actual-revenue-based-on-a-one-time-billing-rate-override}

Considere o seguinte ao calcular a Receita Real com base em uma sobreposição de Taxa de Faturamento ocasional:

* Quando o **Tipo de Receita** de uma tarefa é **Função por Hora**, a Workfront multiplica as **Horas Efetivas** de uma tarefa pela taxa de cobrança da função de trabalho associada à tarefa para calcular a **Receita Efetiva** na tarefa. Horas efetivas são horas registradas diretamente na tarefa.

  Para obter mais informações sobre qual função de trabalho é usada para calcular **Receita Efetiva**, consulte a seção &quot;Entendendo os Cálculos de Receita para Tarefas com Base nas Atribuições de Usuário e Função&quot; no artigo [Visão Geral de Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

* Se a taxa de faturamento da função de trabalho tiver sido substituída no nível do projeto, o Workfront usará a taxa de substituição do projeto para calcular a Receita Efetiva. Quando você substitui a taxa de cobrança da função de trabalho no projeto, a **Receita Efetiva** do projeto é recalculada automaticamente usando a nova taxa ajustada.

  Para obter informações sobre substituição de taxas de função para o projeto, consulte [Substituir taxas de cobrança de função de trabalho no nível do projeto](../../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

>[!NOTE]
>
>Para manter as horas nas quais você já fez logon no projeto antes de substituir a taxa de cobrança original cobrada pela taxa original, você deve incluí-las em um **Registro de cobrança** e deve marcar o **Registro de cobrança** como **Faturado**. Caso contrário, a **Receita Efetiva** das horas registradas antes da taxa de cobrança ser substituída para o projeto será recalculada usando a nova taxa quando as finanças dos projetos forem recalculadas.\
>Para obter mais informações sobre como incluir horas em um registro de cobrança e marcá-lo como **Faturado**, consulte o artigo [Criar registros de cobrança](../../../manage-work/projects/project-finances/create-billing-records.md).

### Calcular Receita Efetiva com base em várias sobreposições de Taxa de Faturamento {#calculate-actual-revenue-based-on-multiple-billing-rate-overrides}

Considere o seguinte ao calcular a Receita Real com base em várias sobreposições de Taxa de Faturamento:

* Quando o **Tipo de Receita** de uma tarefa é **Função por Hora**, a Workfront multiplica as **Horas Efetivas** na tarefa pela taxa de cobrança das funções de trabalho atribuídas à tarefa para calcular a **Receita Efetiva** na tarefa. Horas efetivas são horas registradas diretamente na tarefa.

* No caso de várias substituições de taxa de cobrança, a taxa pela qual as **Horas Efetivas** são multiplicadas para calcular a **Receita Efetiva** pode mudar durante a duração de uma tarefa. A Workfront usa a taxa de cobrança da função de trabalho cujo período corresponde à **Data de Entrada** das horas registradas para a tarefa para calcular **Receita Efetiva.**

  Por exemplo, uma tarefa tem o **Tipo de Receita** de **Função por Hora** e está atribuída à função de trabalho de Gerente de Projetos. Substitua a taxa de cobrança desta função de trabalho pela Taxa 1 para as datas entre 19 de junho e 25 de junho. A partir de 26 de junho, substitua a taxa de cobrança pela Taxa 2. Registre 2 horas para 20 de junho e 3 horas para 28 de junho.

  A Workfront calcula a **Receita Efetiva** para essa tarefa usando a seguinte fórmula:

  ```
  Actual Revenue = 2 * Rate 1 + 3 * Rate 2
  ```

  Para obter mais informações sobre qual função de trabalho é usada para calcular **Receita Efetiva**, consulte a seção &quot;Entendendo os Cálculos de Receita para Tarefas com Base nas Atribuições de Usuário e Função&quot; no artigo [Visão Geral de Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## O impacto dos fusos horários ao calcular a receita com base em várias taxas de cobrança

Os usuários podem ver Horas planejadas por dia diferentes das de outros usuários, se ocorrerem diferenças de fuso horário entre eles e outras entidades no Workfront. Os cenários a seguir podem distorcer as informações de Horas planejadas por dia para um usuário do que outro usuário vê:

* Os dois usuários podem ter seus computadores definidos para dois fusos horários diferentes
* Os dois perfis de usuário no Workfront podem ser definidos como dois fusos horários diferentes
* O fuso horário associado ao perfil do usuário pode ser diferente do Fuso horário do sistema no Workfront
* O fuso horário associado ao perfil do usuário pode ser diferente do fuso horário do agendamento do projeto.

Nesses casos, o número de Horas planejadas por dia pode ser diferente entre dois usuários que não compartilham as mesmas configurações para fusos horários. Eles também verão diferentes números de receita planejada ao usar várias sobreposições de taxa de faturamento em um projeto.

* [Calcular a receita planejada para usuários em diferentes fusos horários](#calculate-planned-revenue-for-users-in-different-time-zones)
* [Calcular a receita atual para usuários em diferentes fusos horários](#calculate-actual-revenue-for-users-in-different-time-zones)

### Calcular a receita planejada para usuários em diferentes fusos horários {#calculate-planned-revenue-for-users-in-different-time-zones}

>[!NOTE]
>
>Se você tiver usuários em fusos horários diferentes trabalhando nos mesmos projetos, recomendamos que você não altere as substituições da taxa de cobrança para seus projetos durante a semana. Isso pode exibir uma quantidade incorreta de receita planejada para o seu projeto, como resultado das diferenças de hora entre os fusos horários na programação dos usuários e o fuso horário do sistema Workfront. A maioria das programações permite que os finais de semana sejam excluídos dos cálculos de Horas planejadas. Se ocorrer uma alteração na substituição da taxa de cobrança de uma função de trabalho, é melhor que isso ocorra durante um fim de semana do que no meio de uma semana, quando poderia coincidir com o meio da Duração de uma tarefa.

Considere o seguinte ao calcular a Receita Planejada para usuários em diferentes Fusos Horários:

* Para tarefas que têm um **Tipo de Receita** de **Função por Hora** e são atribuídas a funções de trabalho, a **Receita Planejada** é calculada multiplicando-se as **Horas Planejadas** de uma tarefa pela taxa de cobrança da função de trabalho.

* As **Horas Planejadas** são distribuídas uniformemente pela **Duração** da tarefa.

* A **Duração** é o período entre o **Início Planejado** **Data** e a **Data de Conclusão Planejada** da tarefa. Como a **Data de Início Planejada** e a **Data de Conclusão Planejada** das tarefas podem diferir dependendo dos fusos horários dos usuários que visualizam a tarefa, a quantidade de Horas Planejadas por Dia pode ser diferente para dois usuários em dois fusos horários diferentes.

* O valor de Horas planejadas por dia não altera a Receita planejada de um projeto se a taxa de faturamento da função de trabalho não for alterada ou quando houver apenas uma sobreposição de taxa de faturamento. Nesse caso, mesmo que dois usuários de dois fusos horários diferentes vejam Horas planejadas por dia diferentes, a Receita planejada geral do projeto é idêntica entre os dois usuários.

  No entanto, no caso de várias substituições de taxa de cobrança, a **receita planejada** geral do projeto pode parecer diferente para dois usuários em dois fusos horários diferentes, pois depende da quantidade de horas planejadas por dia (que pode ser diferente para os dois usuários) e da substituição da taxa de cobrança (que pode ser diferente para o mesmo dia, quando cada usuário está olhando a tarefa em seu próprio fuso horário).

* O valor preciso de **Receita planejada** é o visto pelo usuário que tem o mesmo fuso horário da sua instância do Workfront. O administrador do Workfront define o Fuso horário do Workfront na área Informações do cliente do sistema.\
  Para obter mais informações sobre como definir o Fuso Horário do seu sistema, consulte o artigo [Configurar informações básicas do seu sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### Calcular a receita atual para usuários em diferentes fusos horários {#calculate-actual-revenue-for-users-in-different-time-zones}

Considere o seguinte ao calcular a Receita Real para usuários em diferentes Fusos Horários:

* Quando o **Tipo de Receita** de uma tarefa é **Função por Hora**, a Workfront multiplica as **Horas Efetivas** na tarefa pela taxa de cobrança das funções de trabalho atribuídas à tarefa para calcular a **Receita Efetiva**. Horas efetivas são horas registradas diretamente na tarefa.

* No caso de várias substituições de taxa de cobrança, a Workfront usa a taxa de cobrança da função de trabalho cujo período corresponde à **Data de Entrada** das horas registradas para a tarefa para calcular **Receita Efetiva**.

* Como não há carimbo de data/hora na **Data de Entrada** das horas registradas e não há carimbo de data/hora nos intervalos de datas de várias substituições de taxa de cobrança, os cálculos de **Receita Efetiva** não são afetados pelo Fuso Horário associado aos usuários.

Para obter mais informações sobre qual função de trabalho é usada para calcular **Receita Efetiva**, consulte a seção &quot;Entendendo os Cálculos de Receita para Tarefas com Base nas Atribuições de Usuário e Função&quot; no artigo [Visão Geral de Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Recalcular as finanças do projeto

As finanças são calculadas em um projeto à medida que ocorrem alterações nas horas registradas para o projeto.

Se as taxas forem alteradas durante a vida útil de um projeto, você poderá recalcular custos e receitas manualmente, usando a opção Recalcular Finanças em um projeto. Além disso, algumas ações acionam um recálculo automático.

Para obter mais informações sobre como recalcular as finanças do projeto, consulte o artigo [Recalcular as finanças do projeto](../../../manage-work/projects/project-finances/recalculate-project-finances.md).

## Adicionar uma nova taxa de cobrança usando a API

Para adicionar uma nova taxa de cobrança para uma função de trabalho usando a API, execute uma ação *setRatesForRole* para o objeto **Rate** usando o *método PUT*.
Os campos de ação e data no objeto **Rate** estão disponíveis na API versão 8.0.
Se você já tiver várias taxas de cobrança definidas para uma função de trabalho em um projeto e quiser adicionar uma nova taxa de cobrança para ele com um novo intervalo de datas, será necessário incluir a taxa existente e a taxa a ser adicionada na mesma chamada de API. É semelhante à forma como as coleções são atualizadas em objetos.

A chamada de API a seguir é um exemplo em que **attachableID** é a **ID do Projeto** do projeto em que você está adicionando a taxa de cobrança e **RoleID** é a **ID de Função do Trabalho** para a qual você está adicionando a nova taxa de cobrança.<pre>{</pre><pre>&quot;attachableID&quot;:&quot;593f01500000557d75fdd4fdfcc624f2&quot;,</pre><pre>&quot;attachableObjCode&quot;:&quot;PROJ&quot;,</pre><pre>&quot;roleID&quot;:&quot;544820df000014148cda5136d4b79d09&quot;, </pre><pre>&quot;taxas&quot;:[</pre><pre>         {&quot;rateValue&quot;:&quot;0.00&quot;,&quot;startDate&quot;:null,&quot;endDate&quot;:&quot;06-06-11&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;45.00&quot;,&quot;startDate&quot;:&quot;2017-06-12&quot;,&quot;endDate&quot;:&quot;2017-06-17&quot;},</pre><pre>         {&quot;rateValue&quot;:&quot;95.00&quot;,&quot;startDate&quot;:&quot;2017-06-21&quot;,&quot;endDate&quot;:null}</pre><pre>]</pre><pre>}</pre>Para obter mais informações sobre como usar a API do Workfront, consulte o artigo [Noções básicas sobre API](https://experience.workfront.com/s/article/API-Basics-638808549).
