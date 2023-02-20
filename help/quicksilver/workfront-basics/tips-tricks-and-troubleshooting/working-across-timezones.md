---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Trabalhar em vários fusos horários
description: Pode ser útil entender como [!DNL Adobe Workfront] O usa fusos horários para calcular o seguinte - EDITAR ME.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# Trabalhar em vários fusos horários

Pode ser útil entender como [!DNL Adobe Workfront] O usa fusos horários para calcular o seguinte:

* Campos de tempo para objetos
* Tempos em outros [!DNL Workfront] áreas, como emails automatizados do Workfront

## Fusos horários em [!DNL Workfront]

Tempos que você vê em [!DNL Workfront] são baseadas nas configurações de fuso horário para o [!DNL Workfront] e para seu perfil de usuário. Se esses dois fusos horários forem diferentes, você poderá observar discrepâncias de tempo em diferentes áreas e recursos que você usa no [!DNL Workfront].

>[!NOTE]
>
><div class="preview">Em um formulário personalizado anexado a um objeto, as declarações de data e hora em campos personalizados calculados são calculadas e salvas pelo Tempo Universal Coordenado (UTC), não pelas configurações de fuso horário definidas para a instância da sua organização e o perfil do usuário. Os cálculos em um formulário personalizado são gerados e exibidos com base nos fusos horários individuais de cada usuário.</div>




* [A [!DNL Workfront] instância](#your-organization-s-workfront-instance)
* [Seu perfil de usuário](#your-user-profile)

### A [!DNL Workfront] instância {#your-organization-s-workfront-instance}

O fuso horário de sua organização [!DNL Workfront] geralmente é definida para a localização do escritório principal. Isso determina o seguinte:

* O tempo mostrado em emails gerados por [!DNL Workfront]
* O fuso horário de usuários recém-adicionados (antes da variável [!DNL Workfront] o administrador configura um fuso horário diferente para ele com base no local de trabalho)

   Para obter mais informações sobre esses dois exemplos, consulte [Configurar informações básicas para seu sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* O início ou o fim de uma taxa de faturamento sobreposta para um projeto. Para obter mais informações, consulte [Substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Seu perfil de usuário {#your-user-profile}

O fuso horário no seu perfil de usuário deve ser configurado para o local em que você trabalha. Isso determina o seguinte:

* O tempo mostrado em sua saída [!DNL Workfront] mensagens de email
* Tempos de um objeto em que você trabalha, como horários de início e término

   Se usuários em vários fusos horários forem atribuídos a um objeto, [!DNL Workfront] converte os tempos do objeto para todos envolvidos, usando o fuso horário configurado em cada perfil de usuário.

   **Exemplo:** Na zona de horário padrão do leste (EST) onde você trabalha, você define uma tarefa para iniciar às 16:00 e atribuí-la aos usuários que trabalham na zona de horário padrão do Pacífico (PST). Para esses usuários, a hora de início é exibida como 1:00 PM. Se ele fosse exibido como 16h, eles começariam a trabalhar nele com três horas de atraso.

   Se o criador de objeto não observar a diferença entre os fusos horários dos destinatários e fazer os ajustes necessários ao definir horários de objetos, ou se os destinatários não observarem essa diferença, pode ser difícil obter o tempo certo enquanto todos colaboram no objeto.

   **Exemplo:** Você configura uma tarefa de um dia para iniciar às 9h EST, esquecendo que alguns usuários da tarefa funcionam na zona PST. Para eles, a hora de início é 6:00 AM. Como eles não começarão a trabalhar nisso até as 9:00 da hora (meio-dia da hora), a tarefa começa e termina com três horas de atraso.

Para obter informações sobre como configurar seu fuso horário no perfil do usuário, consulte [Definir minhas configurações](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Para obter informações sobre como uma [!DNL Workfront] administrador (ou alguém com [!UICONTROL Editar] acesso aos usuários) pode configurar o fuso horário em um perfil de usuário, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Como você pode facilitar o trabalho dos usuários em vários fusos horários

Você pode ajudar usuários a trabalhar mais facilmente em vários fusos horários de várias maneiras:

* [Usar programações](#use-schedules)
* [Usar campos de tempo calculados em um formulário personalizado](#use-calculated-time-fields-in-a-custom-form)
* [Usar campos de texto em vez de campos de data em um formulário personalizado](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Usar programações {#use-schedules}

[!DNL Workfront] Os administradores criam programações separadas para cada fuso horário em sua organização, para garantir que o trabalho seja agendado adequadamente para todos, onde quer que esteja. Depois que o administrador criar os agendamentos, eles poderão ser associados a determinados projetos e usuários:

* **[!UICONTROL Projetos]**: Um criador de projeto pode selecionar um agendamento para um projeto individual. Isso determina o agendamento das tarefas no projeto, com base no horário de trabalho definido para os fusos horários dos destinatários.
* **[!UICONTROL Usuários]**: A [!DNL Workfront] administrador (ou alguém com [!UICONTROL Editar] acesso aos usuários) pode selecionar um agendamento para usuário individual no perfil do usuário.

   Esse agendamento pode ser diferente de um agendamento de projeto. Por exemplo, quando alguém cria uma tarefa no projeto e ainda não atribuiu ninguém a ela, a tarefa usa o agendamento do projeto. Quando um usuário é atribuído à tarefa, a tarefa usa o agendamento desse usuário.

   Se vários usuários forem atribuídos a uma tarefa, o sistema usará um dos seguintes, conforme configurado nas preferências do projeto em todo o sistema:

   * O fuso horário do agendamento do proprietário principal da tarefa
   * O fuso horário do agendamento do projeto.

   Isso pode fazer com que as datas das tarefas sejam alteradas.

   **Exemplo:** Um usuário EST é atribuído a uma tarefa de um dia agendada para iniciar às 9h PST, que é o meio-dia EST. Como o usuário EST tem apenas 2 horas de trabalho restantes para o dia, a data de conclusão da tarefa se estende por cerca de 6 horas até o dia útil seguinte.

   Para obter informações sobre o [!UICONTROL Preferências do projeto] área de [!UICONTROL Configuração], consulte [Configurar preferências de projeto em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Para obter instruções sobre como atribuir uma agenda a um projeto ou usuário, consulte [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   Para obter informações sobre como o fuso horário configurado em sua programação afeta a distribuição de [!UICONTROL Horas Planejadas] no [!DNL Workload Balancer], consulte [Gerencie alocações de usuários no [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Usar campos de tempo calculados em um formulário personalizado {#use-calculated-time-fields-in-a-custom-form}

Você pode usar uma série de campos personalizados calculados em um formulário personalizado para exibir o tempo atual para os usuários em sua organização, como uma linha de relógios de aeroporto que exibe o tempo em várias cidades. Você poderia criar um campo para cada fuso horário em que seus usuários trabalham, cada um calculando o horário de seu fuso horário.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md), bem como a seção [Campos personalizados de data e hora calculados](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) no artigo [Expressões de dados calculadas](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Usar campos de texto em vez de campos de data em um formulário personalizado {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Se você não quiser [!DNL Workfront] para converter horários configurados para em um objeto para usuários em fusos horários diferentes, é possível usar um campo de texto em um formulário personalizado anexado a um objeto, em vez de um campo de data. Dessa forma, o horário exibe o horário digitado para todos no projeto.

Nesse caso, recomendamos que você lembre os usuários do formulário para calcular a diferença entre o fuso horário e o horário, de modo que possam determinar quando o trabalho deve começar e terminar. Você pode incluir isso nas instruções digitadas para o formulário personalizado ou em uma dica de ferramenta desse campo. Para obter mais informações, consulte [Adicionar um campo personalizado a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
