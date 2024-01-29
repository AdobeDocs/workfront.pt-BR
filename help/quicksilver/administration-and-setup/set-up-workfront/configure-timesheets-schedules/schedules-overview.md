---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: user,schedule
navigation-topic: configure-timesheets-and-schedules
title: Visão geral dos cronogramas
description: Você pode definir sua semana de trabalho usando programações. Você pode associar um agendamento a um usuário ou projeto. Isso permite [!DNL Adobe Workfront] para calcular as linhas do tempo e a disponibilidade dos usuários. Para obter instruções, consulte Criar um agendamento.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Visão geral dos cronogramas

<!-- Audited: 1/2024 -->

Você pode definir sua semana de trabalho usando cronogramas e associar um cronograma a um usuário ou projeto. Isso permite [!DNL Adobe Workfront] para calcular as linhas do tempo e a disponibilidade dos usuários. Para obter instruções, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Leve em consideração o seguinte ao trabalhar com programações no Workfront:

* A variável [!DNL Workfront] o administrador identifica as horas de operação da organização em uma programação.

  Da mesma forma, um administrador de grupo pode identificar as horas de operação de um agendamento administrado por um grupo gerenciado por ele. Para obter mais informações sobre administradores de grupo, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Por exemplo, uma programação pode ser definida como: de segunda a sexta-feira, das 8h às 17h, com um intervalo de uma hora para almoço.

* [!DNL Workfront] O usa o cronograma para determinar quando o dia de trabalho começa e termina.

  Isso não impede que um usuário trabalhe ou conclua um trabalho no [!DNL Workfront] fora do horário comercial normal. Geralmente, não é necessário criar uma nova programação ou uma exceção de programação para se concentrar no trabalho planejado à noite.

  Da mesma forma, sua organização pode ter horários de chegada flexíveis para o seu dia de trabalho. Você pode ter um conjunto de funcionários que chega às 8h e outro conjunto que chega às 9h. Não é necessário criar programações exclusivas para cada grupo, se os grupos tiverem programações semelhantes ou idênticas. Mas se os grupos tiverem cronogramas drasticamente diferentes, os usuários deverão ser associados a cronogramas únicos. Um funcionário entende se uma atribuição deve ser concluída às 17:00, isso significa que o trabalho deve ser concluído até o final do dia útil, independentemente do horário em que ele chega ao trabalho.

* Recomendamos que você crie agendas separadas para cada fuso horário associado à organização.

  Você pode atribuir um fuso horário específico para cada agendamento para garantir que o trabalho seja agendado corretamente para usuários que trabalham em fusos horários diferentes.

* A variável [!DNL Workfront] O Cronograma padrão é usado em cálculos de cronograma quando usuários ou projetos não estão associados a um cronograma.

  O Cronograma Padrão vem com seu [!DNL Workfront] e não podem ser excluídos, a menos que sejam substituídos por um novo agendamento criado por você.

* Além de calcular linhas do tempo, [!DNL Workfront] O usa agendamentos para calcular a disponibilidade do usuário.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] O usa o usuário ou o agendamento do projeto para determinar a disponibilidade de recursos no Planejador de recursos. Qual cronograma é usado depende do que o [!DNL Workfront] administrador selecionado para o [!UICONTROL Calcular Disponibilidade de Recursos Usando] configuração. Para obter informações sobre as configurações de Gerenciamento de recursos, consulte [Configurar preferências de gerenciamento de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Hierarquia de programações

Se uma tarefa for atribuída a um usuário associado a um agendamento e residir em um projeto associado a um segundo agendamento, você terá pelo menos dois agendamentos que poderiam ser aplicados potencialmente aos seus cálculos de linha do tempo.

>[!IMPORTANT]
>
>[!DNL Workfront] O usa o agendamento de um usuário somente quando a variável [!UICONTROL Calcular Disponibilidade de Recursos Usando] está definida como [!UICONTROL O Cronograma do Usuário] no [!UICONTROL Gerenciamento de recursos] área de [!UICONTROL Configuração]. Para obter informações sobre como a variável [!UICONTROL Calcular Disponibilidade de Recursos Usando] que a configuração afeta qual programação é usada para o Gerenciamento de recursos, consulte [Configurar preferências de gerenciamento de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

A ordem em que as programações são usadas pelo sistema quando existe mais de uma é:

* Quando um usuário é atribuído a uma tarefa, [!DNL Workfront] O usa o cronograma do usuário para calcular a linha do tempo da tarefa. Isso também inclui o tempo pessoal do usuário. O cronograma do projeto é ignorado.

  Para obter mais informações sobre o tempo pessoal, consulte [Configurar folga pessoal](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Quando vários usuários são atribuídos a uma tarefa e os usuários têm agendamentos diferentes durante o período da tarefa, [!DNL Workfront] O usa uma das seguintes programações, conforme definido na [!UICONTROL Preferências do projeto] área de [!UICONTROL Configuração]:

   * A programação do usuário designado como Principal Designado
   * A programação associada ao projeto.

     Para obter mais informações sobre preferências de projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se o usuário atribuído à tarefa não tiver agendamento ou a tarefa for atribuída somente a uma função de trabalho, a uma equipe ou não estiver atribuída, [!DNL Workfront] usa a agenda do projeto para os cálculos da linha do tempo.
* Se o usuário atribuído à tarefa não tiver agendamento ou a tarefa for atribuída somente a uma função de trabalho, a uma equipe ou não estiver atribuída, e o projeto não tiver agendamento, [!DNL Workfront] O usa a programação no sistema designada como a Programação Padrão para cálculos de cronograma.

  ![](assets/default-schedule.png)

## Colaboração em [!DNL Workfront] em fusos horários

Para obter informações sobre como usar as agendas para ajudar os usuários a colaborar no [!DNL Workfront] em fusos horários, consulte [Trabalhar em fusos horários](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
