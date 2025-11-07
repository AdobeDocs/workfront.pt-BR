---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Trabalhar em fusos horários
description: Pode ser útil entender como o  [!DNL Adobe Workfront] usa fusos horários para calcular campos de tempo para objetos e horários em outras áreas, como emails.
feature: Get Started with Workfront
author: Becky
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# Trabalhar em fusos horários

<!-- Audited: 2/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Pode ser útil entender como o [!DNL Adobe Workfront] usa fusos horários para calcular o seguinte:

* Campos de tempo para objetos
* Tempos em outras áreas do [!DNL Workfront], como emails automatizados do Workfront

>[!WARNING]
>
>Se você não conseguir encontrar o fuso horário exato na lista que fornecemos, encontre o fuso horário mais próximo do seu e atualize-o para a sua instância.
>
>Além disso, considere que um fuso horário semelhante pode não corresponder perfeitamente ao seu.
>
>Por exemplo, alguns países ou territórios podem observar o Horário de verão, mas seu país pode não observar. Talvez seja necessário ajustar os fusos horários do sistema de acordo com essas alterações, se necessário.


## Fusos horários em [!DNL Workfront]

Os horários que você vê no [!DNL Workfront] são baseados nas configurações de fuso horário da instância [!DNL Workfront] da sua organização e do seu perfil de usuário. Se esses dois fusos horários forem diferentes, você poderá ver discrepâncias de tempo em diferentes áreas e recursos que você usa no [!DNL Workfront].

>[!NOTE]
>
>Em um formulário personalizado anexado a um objeto, os demonstrativos de data e hora em campos personalizados calculados são calculados e salvos pelo Tempo universal coordenado (UTC), não pelas configurações de fuso horário definidas para a instância da organização e o perfil do usuário. Os cálculos em um formulário personalizado são gerados e exibidos com base nos fusos horários individuais de cada usuário.

* [Instância  [!DNL Workfront]  da sua organização](#your-organization-s-workfront-instance)
* [Seu perfil de usuário](#your-user-profile)

### Instância [!DNL Workfront] da sua organização {#your-organization-s-workfront-instance}

O fuso horário da instância [!DNL Workfront] de sua organização geralmente é definido para a localização do escritório principal. Isso determina o seguinte:

* O tempo mostrado nos emails gerados por [!DNL Workfront]
* O fuso horário para usuários recém-adicionados (antes do administrador do [!DNL Workfront] configurar um fuso horário diferente para eles com base no local em que trabalham)

  Para obter mais informações sobre esses dois exemplos, consulte [Configurar informações básicas do sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* O início ou o fim de uma taxa de cobrança substituída para um projeto. Para obter mais informações, consulte [Substituir taxas de cobrança de função de trabalho no nível do projeto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Seu perfil de usuário {#your-user-profile}

O campo Fuso horário no perfil do usuário controla a hora mostrada nas mensagens de email de saída.

O fuso horário também afeta o que é exibido em um relatório de calendário PTO.

Para obter informações sobre como configurar o fuso horário no seu perfil de usuário, consulte [Configurar minhas configurações](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Para obter informações sobre como um administrador do [!DNL Workfront] (ou alguém com acesso de [!UICONTROL Edição] aos usuários) pode configurar o fuso horário em um perfil de usuário, consulte [Editar perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

### Fuso horário do seu navegador

O fuso horário no navegador deve ser configurado para o local em que você trabalha. Isso determina o seguinte:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Horários para um objeto no qual você trabalha, como horário de início e término.

  Se usuários em vários fusos horários forem atribuídos a um objeto, o [!DNL Workfront] converterá os horários do objeto para todos os envolvidos, usando o fuso horário configurado no navegador de cada usuário.

  **EXEMPLO**
Na zona Horário Padrão da Costa Leste (EST) onde você trabalha, você define uma tarefa para começar às 16h20 e a atribui aos usuários que trabalham na zona Horário Padrão do Pacífico (PST). :00 Para esses usuários, a hora de início é exibida como 1:00 PM. Se fosse exibido como 4:00 PM, eles começariam a trabalhar nele com três horas de atraso.

  Se o criador do objeto não souber a diferença entre os fusos horários dos atribuídos e não fizer os ajustes necessários ao definir os tempos do objeto, ou se os atribuídos não souberem essa diferença, pode ser difícil obter o tempo correto enquanto todos colaboram no objeto.

  **EXEMPLO**

  Você configura uma tarefa de um dia para começar às 9:00 AM EST, esquecendo que alguns usuários na tarefa trabalham na zona PST. Para eles, a hora de início é 6:00 AM. Como eles não começarão a trabalhar nela até o dia 9:00 de cada vez (meio-dia, horário local), a tarefa será iniciada e finalizada com três horas de atraso.

A configuração do fuso horário é diferente entre os navegadores. Para obter mais informações, consulte a documentação de cada navegador ou informações de ajuda.

## Como você pode facilitar para os usuários trabalharem em fusos horários

Você pode ajudar os usuários a trabalharem mais facilmente em vários fusos horários de várias maneiras:

* [Usar agendas](#use-schedules)
* [Usar campos de tempo calculado em um formulário personalizado](#use-calculated-time-fields-in-a-custom-form)
* [Usar campos de texto em vez de campos de data em um formulário personalizado](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Usar agendas {#use-schedules}

Os administradores do [!DNL Workfront] criam cronogramas separados para cada fuso horário da sua organização para garantir que o trabalho seja agendado adequadamente para todos, onde quer que estejam. Depois que o administrador cria os cronogramas, eles podem ser associados a determinados projetos e usuários:

* **[!UICONTROL Projetos]**: o criador de um projeto pode selecionar um agendamento para um projeto individual. Isso determina o agendamento das tarefas no projeto, com base nas horas de trabalho definidas para os fusos horários dos atribuídos.
* **[!UICONTROL Usuários]**: Um administrador do [!DNL Workfront] (ou alguém com acesso de [!UICONTROL Edição] aos usuários) pode selecionar um agendamento para um usuário individual no perfil do usuário.

  Este cronograma pode ser diferente de um cronograma de projeto. Por exemplo, quando alguém cria uma tarefa no projeto e ainda não atribuiu ninguém a ela, a tarefa usa o cronograma do projeto. Quando um usuário é atribuído à tarefa, ela usa o agendamento desse usuário.

  Se vários usuários forem atribuídos a uma tarefa, o sistema usará um dos seguintes, conforme configurado nas preferências do projeto do sistema ou do grupo:

   * O fuso horário do agendamento do proprietário principal da tarefa
   * O fuso horário para o agendamento do projeto.

  Se um usuário for atribuído a uma tarefa, o sistema usará um dos seguintes, conforme configurado nas preferências do projeto do sistema ou do grupo:

   * O fuso horário do agendamento do destinatário da tarefa
   * O fuso horário para o agendamento do projeto.

  Isso pode fazer com que as datas das tarefas mudem.

>[!BEGINSHADEBOX]

**EXEMPLO:**
Um usuário EST é atribuído a uma tarefa de um dia agendada para iniciar às 9:00 AM PST, que é meio-dia EST. Como o usuário EST tem apenas 2 horas de trabalho restantes para o dia, a data de conclusão da tarefa se estende por cerca de 6 horas no próximo dia útil.


>[!ENDSHADEBOX]

Para obter informações sobre a área [!UICONTROL Preferências do Projeto] da [!UICONTROL Instalação], consulte [Configurar preferências de projeto do sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Para obter instruções sobre como atribuir uma agenda a um projeto ou usuário, consulte [Criar uma agenda](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Para obter informações sobre como o fuso horário configurado em seu agendamento afeta a distribuição de [!UICONTROL Horas planejadas] no [!UICONTROL Balanceador de carga de trabalho], consulte [Gerenciar alocações de usuários no [!UICONTROL Balanceador de carga de trabalho]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Usar campos de tempo calculado em um formulário personalizado {#use-calculated-time-fields-in-a-custom-form}

Você pode usar uma série de campos personalizados calculados em um formulário personalizado para exibir a hora atual dos usuários em sua organização, como uma linha de relógios do aeroporto exibindo a hora em várias cidades. Você pode criar um campo para cada um dos fusos horários em que seus usuários trabalham, cada um calculando o horário para seu fuso horário.

Para obter mais informações, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md), bem como a seção [Campos personalizados calculados de data e hora](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) no artigo [Visão geral das expressões de dados calculados](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Usar campos de texto em vez de campos de data em um formulário personalizado {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Se você não quiser que o [!DNL Workfront] converta horas configuradas em um objeto para usuários em diferentes fusos horários, poderá usar um campo de texto em um formulário personalizado anexado a um objeto, em vez de um campo de data. Dessa forma, o horário exibe o horário digitado para todos no projeto.

Se você fizer isso, recomendamos lembrar os usuários do formulário de calcular a diferença entre o fuso horário deles e o seu para que eles possam determinar quando o trabalho deve começar e terminar. Você pode incluir isso nas instruções digitadas para o formulário personalizado ou em uma dica de ferramenta para esse campo. Para obter mais informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
