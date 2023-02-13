---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: usuário,agendar
navigation-topic: configure-timesheets-and-schedules
title: Visão geral dos agendamentos
description: Você pode definir sua semana de trabalho usando agendamentos. Você pode associar um agendamento a um usuário ou projeto. Isso permite [!DNL Adobe Workfront] para calcular linhas do tempo e disponibilidade do usuário. Para obter instruções, consulte Criar um agendamento.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Visão geral dos agendamentos

Você pode definir sua semana de trabalho usando agendamentos e associar uma agenda a um usuário ou projeto. Isso permite [!DNL Adobe Workfront] para calcular linhas do tempo e disponibilidade do usuário. Para obter instruções, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Considere o seguinte ao trabalhar com programações no Workfront:

* O [!DNL Workfront] O administrador identifica as horas de operação da organização em um agendamento.

   Da mesma forma, um administrador de grupo pode identificar as horas de operação de um agendamento administrado por um grupo que gerencia.

   Para obter mais informações sobre administradores de grupo, consulte [Administradores do grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

   Por exemplo, um agendamento pode ser definido como: De segunda a sexta-feira, das 8h às 17h, com uma hora de pausa para almoço.

* [!DNL Workfront] O usa o agendamento para determinar quando o dia de trabalho começa e termina.

   Isso não impede que um usuário trabalhe ou conclua o trabalho no [!DNL Workfront] fora do horário comercial normal. Geralmente, não é necessário criar um novo agendamento ou uma exceção de agendamento para se concentrar no trabalho planejado à noite.

   Da mesma forma, sua organização pode ter horários flexíveis de chegada para seu dia de trabalho. Você pode ter um conjunto de funcionários que chega às 8h e outro que chega às 9h. Não é necessário criar programações exclusivas para cada grupo, se os grupos tiverem programações semelhantes ou idênticas. Mas se os grupos tiverem programações drasticamente diferentes, seus usuários deverão estar associados a programações exclusivas. Um funcionário entende se uma atribuição deve ser concluída às 17:00 horas, o que significa que o trabalho deve ser feito até ao fim do dia útil, independentemente do horário em que entre para trabalhar.

* Recomendamos que você crie programações separadas para cada fuso horário associado à organização.

   Você pode atribuir um fuso horário específico para cada programação para garantir que o trabalho seja agendado adequadamente para usuários que trabalham em fusos horários diferentes.

* O [!DNL Workfront] A Programação padrão é usada em cálculos de linha do tempo quando usuários ou projetos não estão associados a uma programação.

   O agendamento padrão vem com seu [!DNL Workfront] e não pode ser excluído, a menos que seja substituído por um novo agendamento criado por você.

* Além de calcular as linhas do tempo, [!DNL Workfront] O usa programações para calcular a disponibilidade do usuário.

   >[!IMPORTANT]
   >
   >[!DNL Workfront] O usa o usuário ou o agendamento do projeto para determinar a disponibilidade dos recursos no Planejador de Recursos. O agendamento usado depende do [!DNL Workfront] administrador selecionado para a [!UICONTROL Calcule a disponibilidade de recursos usando] configuração. Para obter informações sobre as configurações de Gerenciamento de Recursos, consulte [Configurar preferências do Gerenciamento de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Hierarquia de agendamentos

Se uma tarefa for atribuída a um usuário associado a uma programação e residir em um projeto associado a uma segunda programação, você terá pelo menos 2 programações que poderão ser aplicadas aos cálculos da linha do tempo.

>[!IMPORTANT]
>
>[!DNL Workfront] usa o agendamento de um usuário somente quando a variável [!UICONTROL Calcule a disponibilidade de recursos usando] está definida como [!UICONTROL O cronograma do usuário] no [!UICONTROL Gerenciamento de recursos] área de [!UICONTROL Configuração]. Para obter informações sobre como a variável [!UICONTROL Calcule a disponibilidade de recursos usando] a configuração afeta qual programação é usada para o Gerenciamento de Recursos, consulte [Configurar preferências do Gerenciamento de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

A ordem em que as programações são usadas pelo sistema quando existe mais de uma é:

* Quando um usuário é atribuído a uma tarefa, [!DNL Workfront] O usa o agendamento do usuário para calcular a linha do tempo da tarefa. Isso também inclui o horário pessoal do usuário. O agendamento do projeto é ignorado.

   Para obter mais informações sobre tempo pessoal, consulte [Configurar tempo de folga pessoal em [!DNL Adobe Workfront]](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Quando vários usuários são atribuídos a uma tarefa e os usuários têm agendamentos diferentes durante o período da tarefa, [!DNL Workfront] O usa uma das programações a seguir, conforme definido no [!UICONTROL Preferências do projeto] área de [!UICONTROL Configuração]:

   * O agendamento do usuário designado como o Destinatário Principal
   * O agendamento associado ao projeto.

      Para obter mais informações sobre as preferências do projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se o usuário atribuído à tarefa não tiver agendamento ou a tarefa estiver atribuída somente a uma função de trabalho, uma equipe ou não estiver atribuída, [!DNL Workfront] O usa a programação do projeto para os cálculos da linha do tempo.
* Se o usuário atribuído à tarefa não tiver agendamento, ou a tarefa for atribuída somente a uma função de trabalho, uma equipe ou estiver desatribuída e o projeto não tiver agendamento, [!DNL Workfront] O usa a programação no sistema designado como Programação padrão para cálculos de linha do tempo.

   ![](assets/default-schedule.png)

## Colaboração em [!DNL Workfront] em fusos horários

Para obter informações sobre como usar agendamentos para ajudar usuários a colaborar em [!DNL Workfront] em todos os fusos horários, consulte [Trabalhar em vários fusos horários](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
