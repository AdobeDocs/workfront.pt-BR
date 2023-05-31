---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Trabalhar em fusos horários
description: Pode ser útil compreender como [!DNL Adobe Workfront] O usa fusos horários para calcular campos de tempo para objetos e horários em outras áreas, como emails.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# Trabalhar em fusos horários

Pode ser útil compreender como [!DNL Adobe Workfront] O usa fusos horários para calcular o seguinte:

* Campos de tempo para objetos
* Horas em outras [!DNL Workfront] áreas, como emails automatizados do Workfront

## Fusos horários em [!DNL Workfront]

Vezes que você vê em [!DNL Workfront] são baseados nas configurações de fuso horário da sua organização [!DNL Workfront] instância e para seu perfil de usuário. Se esses dois fusos horários forem diferentes, você poderá ver discrepâncias de tempo em diferentes áreas e recursos que usa no [!DNL Workfront].

>[!NOTE]
>
>Em um formulário personalizado anexado a um objeto, os demonstrativos de data e hora em campos personalizados calculados são calculados e salvos pelo Tempo universal coordenado (UTC), não pelas configurações de fuso horário definidas para a instância da organização e o perfil do usuário. Os cálculos em um formulário personalizado são gerados e exibidos com base nos fusos horários individuais de cada usuário.

* [Da sua organização [!DNL Workfront] instância](#your-organization-s-workfront-instance)
* [Seu perfil de usuário](#your-user-profile)

### Da sua organização [!DNL Workfront] instância {#your-organization-s-workfront-instance}

O fuso horário de sua organização [!DNL Workfront] geralmente, a instância é definida para a localização do escritório principal. Isso determina o seguinte:

* O tempo mostrado nos emails gerados por [!DNL Workfront]
* O fuso horário dos usuários recém-adicionados (antes da variável [!DNL Workfront] o administrador configura um fuso horário diferente para eles com base no local em que trabalham)

   Para obter mais informações sobre esses dois exemplos, consulte [Configurar informações básicas do seu sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* O início ou o fim de uma taxa de cobrança substituída para um projeto. Para obter mais informações, consulte [Substituir Taxas de Cobrança de Função de Trabalho no nível do projeto](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Seu perfil de usuário {#your-user-profile}

O fuso horário em seu perfil de usuário deve ser configurado para o local onde você trabalha. Isso determina o seguinte:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Horários para um objeto no qual você trabalha, como horário de início e término

   Se usuários em vários fusos horários forem atribuídos a um objeto, [!DNL Workfront] converte as horas do objeto para todos envolvidos, usando o fuso horário configurado em cada perfil de usuário.

   **Exemplo:** Na zona Horário Padrão da Costa Leste (EST) onde você trabalha, você define uma tarefa para começar às 16h e a atribui aos usuários que trabalham na zona Horário Padrão do Pacífico (PST). Para esses usuários, a hora de início é exibida como 13h. Se fosse exibido como 16h, começariam a trabalhar nele com três horas de atraso.

   Se o criador do objeto não observar a diferença entre os fusos horários dos atribuídos e fizer os ajustes necessários ao definir os tempos do objeto, ou se os atribuídos não observarem essa diferença, pode ser difícil obter o tempo correto enquanto todos colaboram no objeto.

   **Exemplo:** Você configura uma tarefa de um dia para começar às 9h EST, esquecendo que alguns usuários na tarefa trabalham na zona PST. Para eles, a hora de início é 6:00. Como eles não começarão a trabalhar nisso até às 9:00 da hora (meio-dia, horário de vocês), a tarefa começa e termina com três horas de atraso.

Para obter informações sobre como configurar o fuso horário no perfil do usuário, consulte [Definir minhas configurações](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Para obter informações sobre como uma [!DNL Workfront] administrador (ou alguém com [!UICONTROL Editar] aos usuários) puder configurar o fuso horário em um perfil de usuário, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Como você pode facilitar para os usuários trabalharem em fusos horários

Você pode ajudar os usuários a trabalharem mais facilmente em vários fusos horários de várias maneiras:

* [Usar agendas](#use-schedules)
* [Usar campos de tempo calculado em um formulário personalizado](#use-calculated-time-fields-in-a-custom-form)
* [Usar campos de texto em vez de campos de data em um formulário personalizado](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Usar agendas {#use-schedules}

[!DNL Workfront] os administradores criam programações separadas para cada fuso horário na organização para garantir que o trabalho seja agendado adequadamente para todos, onde quer que estejam. Depois que o administrador cria os cronogramas, eles podem ser associados a determinados projetos e usuários:

* **[!UICONTROL Projetos]**: um criador de projeto pode selecionar um agendamento para um projeto individual. Isso determina o agendamento das tarefas no projeto, com base nas horas de trabalho definidas para os fusos horários dos atribuídos.
* **[!UICONTROL Usuários]**: A [!DNL Workfront] administrador (ou alguém com [!UICONTROL Editar] acesso a usuários) podem selecionar um agendamento para usuários individuais no perfil do usuário.

   Este cronograma pode ser diferente de um cronograma de projeto. Por exemplo, quando alguém cria uma tarefa no projeto e ainda não atribuiu ninguém a ela, a tarefa usa o cronograma do projeto. Quando um usuário é atribuído à tarefa, ela usa o agendamento desse usuário.

   Se vários usuários forem atribuídos a uma tarefa, o sistema usará um dos seguintes, conforme configurado nas preferências do projeto do sistema geral:

   * O fuso horário do agendamento do proprietário principal da tarefa
   * O fuso horário para o agendamento do projeto.

   Isso pode fazer com que as datas das tarefas mudem.

   **Exemplo:** Um usuário EST é atribuído a uma tarefa de um dia agendada para iniciar às 9h00 PST, que é meio-dia EST. Como o usuário EST tem apenas 2 horas de trabalho restantes para o dia, a data de conclusão da tarefa se estende por cerca de 6 horas no próximo dia útil.

   Para obter informações sobre o [!UICONTROL Preferências do projeto] área de [!UICONTROL Configuração], consulte [Configurar preferências de projeto em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Para obter instruções sobre como atribuir um agendamento a um projeto ou usuário, consulte [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   Para obter informações sobre como o fuso horário configurado no seu agendamento afeta a distribuição de [!UICONTROL Horas planejadas] no [!UICONTROL Balanceador de carga de trabalho], consulte [Gerenciar alocações de usuários no [!UICONTROL Balanceador de carga de trabalho]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Usar campos de tempo calculado em um formulário personalizado {#use-calculated-time-fields-in-a-custom-form}

Você pode usar uma série de campos personalizados calculados em um formulário personalizado para exibir a hora atual dos usuários em sua organização, como uma linha de relógios do aeroporto exibindo a hora em várias cidades. Você pode criar um campo para cada um dos fusos horários em que seus usuários trabalham, cada um calculando o horário para seu fuso horário.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md), bem como a seção [Campos personalizados calculados de data e hora](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) no artigo [Expressões de dados calculadas](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Usar campos de texto em vez de campos de data em um formulário personalizado {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Se você não quiser [!DNL Workfront] para converter as horas configuradas para o em um objeto para usuários em diferentes fusos horários, é possível usar um campo de texto em um formulário personalizado anexado a um objeto, em vez de um campo de data. Dessa forma, o horário exibe o horário digitado para todos no projeto.

Se você fizer isso, recomendamos lembrar os usuários do formulário de calcular a diferença entre o fuso horário deles e o seu para que eles possam determinar quando o trabalho deve começar e terminar. Você pode incluir isso nas instruções digitadas para o formulário personalizado ou em uma dica de ferramenta para esse campo. Para obter mais informações, consulte [Adicionar um campo personalizado a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
