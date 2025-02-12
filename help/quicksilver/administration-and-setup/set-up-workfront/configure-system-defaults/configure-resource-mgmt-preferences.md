---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurar preferências de gerenciamento de recursos
description: Como administrador do  [!DNL Adobe Workfront] , você pode configurar as Preferências de Gerenciamento de Recursos para o seu sistema. Essas preferências do Gerenciamento de recursos determinam como a disponibilidade ou a capacidade do usuário e o FTE são calculados para as  [!DNL Workfront] ferramentas de planejamento e agendamento de recursos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Configurar preferências de [!UICONTROL Gerenciamento de recursos]

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Como administrador do [!DNL Adobe Workfront], você pode configurar as Preferências do [!UICONTROL Gerenciamento de Recursos] para o seu sistema. Essas preferências determinam como a disponibilidade ou a capacidade do FTE ou a hora do usuário são calculadas para as ferramentas de planejamento e agendamento de recursos do [!DNL Workfront].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
   Ou
   <p>Atual: [!UICONTROL Plano]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informações consideradas ao calcular a capacidade de um usuário

Ao calcular a capacidade de um usuário, o Workfront considera as seguintes informações:

* O número de horas agendadas, conforme definido na Agenda do usuário ou na [!UICONTROL Agenda Padrão] do sistema Workfront
* [!UICONTROL Agendar] [!UICONTROL Exceções] (dependendo de qual [!UICONTROL Agendar] é usado, podem ser as exceções do agendamento do usuário ou aquelas associadas ao [!DNL Workfront] [!UICONTROL Agendamento Padrão])
* Tempo de folga do usuário
* O valor do Equivalente de Tempo Integral ([!UICONTROL FTE]) do usuário ou do sistema [!DNL Workfront]. O [!UICONTROL FTE] é igual a 1 quando o usuário trabalha em tempo integral, conforme definido no agendamento.
* O valor de [!UICONTROL Tempo de Trabalho] para o usuário que se refere ao tempo que o usuário gasta no trabalho relacionado ao projeto. Isso não inclui horas extras, como reuniões e treinamento. O [!UICONTROL Tempo de Trabalho] é igual a 1 quando o usuário está disponível para o trabalho o tempo todo, conforme indicado pelo [!UICONTROL FTE] ou pelo agendamento, o que significa que ele não passa nenhum tempo em trabalho não relacionado ao projeto, como reuniões ou treinamentos.


Para obter informações sobre o planejamento e o agendamento de recursos no [!DNL Workfront], consulte [Introdução ao Gerenciamento de Recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configurar preferências de [!UICONTROL Gerenciamento de recursos]

>[!NOTE]
>
>Como essa é uma configuração global, essa seleção afeta todos os cálculos para todo o sistema, para todos os usuários, em todas as ferramentas de gerenciamento de recursos.

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Gerenciamento de recursos]**.
1. Selecione um dos métodos a seguir para calcular a disponibilidade dos usuários em [!DNL Workfront]:

   * **O Agendamento Padrão**: [!DNL Workfront] usa o Agendamento Padrão do sistema e o FTE individual do usuário para calcular as Horas Disponíveis do usuário nas ferramentas de gerenciamento de recursos.

     Para obter mais informações sobre agendamentos, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Para obter mais informações sobre como localizar o valor do [!UICONTROL FTE] do usuário, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     O Workfront calcula as Horas Disponíveis de um usuário usando a seguinte fórmula quando o administrador do Workfront escolhe O [!UICONTROL Calendário Padrão]:


     `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


     >[!INFO]
     >
     >Por exemplo, se o Calendário padrão for 40 horas por semana, o FTE no perfil do usuário será 0,5, o usuário terá 1 hora de Folga em um dia e o [!UICONTROL Tempo de Trabalho] no perfil do usuário será 0,5, o usuário estará disponível para o trabalho real do projeto por 9,5 horas por semana.
     >
     >Se o usuário tiver 1 hora de folga em um dia, suas Horas disponíveis serão calculadas da seguinte maneira:
     >
     >
     >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
    
      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the [!UICONTROL FTE] in the profile of the user is 0.5, the user is available to work for 20 hours a week.
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
      -->



     <!--      
      <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>In the Production environment: (NOTE: this is the old way it was working, before the 22.2 release)</p><p><code>User Available Hours = (Default Schedule Hours - (Schedule Exceptions + Time off hours)) * User FTE value</code></p>      
      <div class="example" data-mc-autonum="<b>Example: </b>">      
      <span class="autonumber"><span><b>Example: </b></span></span>      
      <div>      
      <p>For example, if the Default Schedule is 40 hours a week and the FTE in the profile of the user is 0.5, the user is available to work for 20 hours a week.</p>      
      <p>If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:</p>      
      <p><code>User Daily Available Hours = (40 - 1)* 0.5 = 19.5 hours</code></p>      
      </div>      
      </div></li>      
      -->

   * **O Cronograma do Usuário**: [!DNL Workfront] usa o cronograma do usuário e o [!UICONTROL Cronograma Padrão] do sistema para calcular o valor [!UICONTROL FTE] Disponível do usuário nas ferramentas de gerenciamento de recursos. As Horas Disponíveis são calculadas de acordo apenas com o cronograma do usuário. O valor de [!UICONTROL FTE] do usuário foi ignorado. Esta é a configuração padrão.

     Para obter mais informações sobre agendamentos, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

     Para obter mais informações sobre a [!UICONTROL Agenda] de um usuário, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     >[!NOTE]
     >
     >Se o usuário não estiver associado a um agendamento, as Horas Disponíveis para o usuário serão calculadas usando apenas o [!UICONTROL Agendamento Padrão].

     As Horas disponíveis para o usuário são calculadas pela seguinte fórmula:


     `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


     O [!UICONTROL FTE] Disponível para o usuário é calculado pela seguinte fórmula:


     `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


     >[!INFO]
     >
     >Por exemplo, se o [!UICONTROL Cronograma Padrão] for 40 horas por semana, o cronograma do usuário será 30 horas por semana e o [!UICONTROL Horário de Trabalho] do usuário será 0,5, o [!UICONTROL FTE] do usuário será 0,35.
     >
     >Se o usuário tiver 2 horas de Folga por dia, seu [!UICONTROL FTE] Disponível Semanalmente será calculado da seguinte maneira:
     >
     >
     >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`
     >

     <!--This used to be the calculation before we implemented the Work Time field: 
      

      The Available hours for the user are calculated by the following formula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```  

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week and the schedule of the user is 30 hours a week, the [!UICONTROL FTE] of the user is 0.70.
      >  
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      > 
      >```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```
      -->

1. Clique em **[!UICONTROL Salvar]**.
