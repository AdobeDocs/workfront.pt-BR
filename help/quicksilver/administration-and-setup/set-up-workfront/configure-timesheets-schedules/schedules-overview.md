---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: user,schedule
navigation-topic: configure-timesheets-and-schedules
title: Visão geral de cronogramas
description: Você pode definir sua semana de trabalho usando programações. Você pode associar um agendamento a um usuário ou projeto. Isso permite [!DNL Adobe Workfront] calcular linhas do tempo e disponibilidade de usuários. Para obter instruções, consulte Criar um agendamento.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Visão geral dos cronogramas

<!-- Audited: 1/2024 -->

Você pode definir sua semana de trabalho usando cronogramas e associar um cronograma a um usuário ou projeto. Isso permite que [!DNL Adobe Workfront] calcule linhas do tempo e a disponibilidade do usuário. Para obter instruções, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Leve em consideração o seguinte ao trabalhar com programações no Workfront:

* O administrador [!DNL Workfront] identifica as horas de operação da organização em um agendamento.

  Da mesma forma, um administrador de grupo pode identificar as horas de operação de um agendamento administrado por um grupo gerenciado por ele. Para obter mais informações sobre administradores de grupo, consulte [Administradores de grupo](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Por exemplo, uma programação pode ser definida como: de segunda a sexta-feira, das 8h às 17h, com um intervalo de uma hora para almoço.

* [!DNL Workfront] usa o agendamento para determinar quando o dia de trabalho começa e termina.

  Isso não impede que um usuário trabalhe ou conclua o trabalho em [!DNL Workfront] fora do horário comercial normal. Geralmente, não é necessário criar uma nova programação ou uma exceção de programação para se concentrar no trabalho planejado à noite.

  Da mesma forma, sua organização pode ter horários de chegada flexíveis para o seu dia de trabalho. Você pode ter um conjunto de funcionários que chega às 8h e outro conjunto que chega às 9h. Não é necessário criar programações exclusivas para cada grupo, se os grupos tiverem programações semelhantes ou idênticas. Mas se os grupos tiverem cronogramas drasticamente diferentes, os usuários deverão ser associados a cronogramas únicos. Um funcionário entende se uma atribuição deve ser concluída às 17:00, isso significa que o trabalho deve ser concluído até o final do dia útil, independentemente do horário em que ele chega ao trabalho.

* Recomendamos que você crie agendas separadas para cada fuso horário associado à organização.

  Você pode atribuir um fuso horário específico para cada agendamento para garantir que o trabalho seja agendado corretamente para usuários que trabalham em fusos horários diferentes.

* O Cronograma Padrão [!DNL Workfront] é usado em cálculos de cronograma quando usuários ou projetos não estão associados a um cronograma.

  A Agenda Padrão vem com o sistema [!DNL Workfront] e não pode ser excluída a menos que seja substituída por uma nova agenda criada por você.

* Além de calcular as linhas do tempo, [!DNL Workfront] usa cronogramas para calcular a disponibilidade dos usuários.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] usa o usuário ou o agendamento do projeto para determinar a disponibilidade de recursos no Planejador de Recursos. O cronograma usado depende do que o administrador do [!DNL Workfront] selecionou para a configuração [!UICONTROL Calcular Disponibilidade de Recursos Usando]. Para obter informações sobre as configurações de Gerenciamento de Recursos, consulte [Configurar preferências de Gerenciamento de Recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Hierarquia de programações

Se uma tarefa for atribuída a um usuário associado a um agendamento e residir em um projeto associado a um segundo agendamento, você terá pelo menos dois agendamentos que poderiam ser aplicados potencialmente aos seus cálculos de linha do tempo.

>[!IMPORTANT]
>
>[!DNL Workfront] usa o agendamento de um usuário somente quando a configuração [!UICONTROL Calcular Disponibilidade de Recursos Usando] está definida como [!UICONTROL O Agendamento do Usuário] na área [!UICONTROL Gerenciamento de Recursos] da [!UICONTROL Instalação]. Para obter informações sobre como a configuração [!UICONTROL Calcular Disponibilidade de Recursos Usando] afeta qual agendamento é usado para o Gerenciamento de Recursos, consulte [Configurar preferências de Gerenciamento de Recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

A ordem em que as programações são usadas pelo sistema quando existe mais de uma é:

* Quando um usuário é atribuído a uma tarefa, [!DNL Workfront] usa o cronograma do usuário para calcular a linha do tempo da tarefa. Isso também inclui o tempo pessoal do usuário. O cronograma do projeto é ignorado.

  Para obter mais informações sobre tempo pessoal, consulte [Configurar tempo pessoal](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* Quando vários usuários são atribuídos a uma tarefa e os usuários têm agendamentos diferentes durante o período da tarefa, [!DNL Workfront] usa um dos seguintes agendamentos, conforme definido na área [!UICONTROL Preferências do Projeto] da [!UICONTROL Instalação]:

   * A programação do usuário designado como Principal Designado
   * A programação associada ao projeto.

     Para obter mais informações sobre preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Se o usuário atribuído à tarefa não tiver cronograma, ou a tarefa for atribuída apenas a uma função de trabalho, uma equipe ou não for atribuída, [!DNL Workfront] usará o cronograma do projeto para os cálculos da linha do tempo.
* Se o usuário atribuído à tarefa não tiver cronograma, ou a tarefa for atribuída somente a uma função de trabalho, uma equipe ou não for atribuída, e o projeto não tiver cronograma, então [!DNL Workfront] usa o cronograma no sistema designado como Cronograma Padrão para cálculos de cronograma.

  ![](assets/default-schedule.png)

## Collaboration em [!DNL Workfront] em fusos horários

Para obter informações sobre como usar agendas para ajudar usuários a colaborar no [!DNL Workfront] entre fusos horários, consulte [Trabalhando entre fusos horários](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
