---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurar preferências de gerenciamento de recursos
description: Como um [!DNL Adobe Workfront] administrador, você pode configurar as Preferências de Gerenciamento de Recursos para o seu sistema. Essas preferências do Gerenciamento de recursos determinam como a disponibilidade ou a capacidade do usuário e o FTE são calculados para o [!DNL Workfront] ferramentas de planejamento e programação de recursos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Configurar [!UICONTROL Gerenciamento de recursos] preferências

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Como um [!DNL Adobe Workfront] administrador, você pode configurar o [!UICONTROL Gerenciamento de recursos] Preferências para o seu sistema. Essas preferências determinam como a disponibilidade ou capacidade de FTE ou hora do usuário é calculada para a variável [!DNL Workfront] ferramentas de planejamento e programação de recursos.

## Requisitos de acesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td>
   <p>Current license: [!UICONTROL Standard]</p>
   
   Or
   
   <p>Legacy license: [!UICONTROL Plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System Administrator access level</p> <p>For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p><b>NOTE</b>: 
   
   If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Nível de acesso do administrador do sistema</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> <p><b>Nota</b>:

Se você ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Informações consideradas ao calcular a capacidade de um usuário

Ao calcular a capacidade de um usuário, o Workfront considera as seguintes informações:

* O número de horas agendadas, conforme definido no Cronograma do usuário ou no do sistema do Workfront [!UICONTROL Agendamento Padrão]
* [!UICONTROL Agendar] [!UICONTROL Exceções] (dependendo de qual [!UICONTROL Agendar] for usado, poderá ser as exceções do agendamento do usuário ou aquelas associadas ao [!DNL Workfront] [!UICONTROL Agendamento Padrão])
* Tempo de folga do usuário
* O valor do Equivalente de Tempo Integral ([!UICONTROL FTE]do utilizador ou do utilizador [!DNL Workfront] sistema. A variável [!UICONTROL FTE] é igual a 1 quando o usuário trabalha em tempo integral, conforme definido no agendamento.
* O valor de [!UICONTROL Horário de trabalho] para o usuário que se refere ao tempo que o usuário gasta no trabalho relacionado ao projeto. Isso não inclui horas extras, como reuniões e treinamento. A variável [!UICONTROL Horário de trabalho] é igual a 1 quando o usuário está disponível para trabalhar o tempo todo, conforme indicado pela variável [!UICONTROL FTE] ou a programação, o que significa que eles não gastam tempo em trabalhos não relacionados a projetos, como reuniões ou treinamentos.


Para obter informações sobre planejamento e programação de recursos no [!DNL Workfront], consulte [Introdução ao gerenciamento de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configurar [!UICONTROL Gerenciamento de recursos] preferências

>[!NOTE]
>
>Como essa é uma configuração global, essa seleção afeta todos os cálculos para todo o sistema, para todos os usuários, em todas as ferramentas de gerenciamento de recursos.

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. Clique em **[!UICONTROL Gerenciamento de recursos]**.
1. Selecione um dos métodos a seguir para calcular a disponibilidade de usuários no [!DNL Workfront]:

   * **O calendário padrão**: [!DNL Workfront] O usa o Cronograma Padrão do sistema e o FTE individual do usuário para calcular as Horas Disponíveis do usuário nas ferramentas de gerenciamento de recursos.

      Para obter mais informações sobre cronogramas, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obter mais informações sobre como localizar o valor do [!UICONTROL FTE], consulte  [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      O Workfront calcula as Horas disponíveis de um usuário usando a seguinte fórmula quando o administrador do Workfront escolhe A [!UICONTROL Agendamento Padrão]:


      `User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * [!UICONTROL Work Time]`


      >[!INFO]
      >
      >Por exemplo, se o Cronograma padrão for 40 horas por semana, o FTE no perfil do usuário será 0,5, o usuário terá 1 hora de Folga em um dia e a variável [!UICONTROL Horário de trabalho] no perfil do usuário é 0,5, o usuário está disponível para o trabalho real do projeto por 9,5 horas por semana.
      >
      >Se o usuário tiver 1 hora de folga em um dia, suas Horas disponíveis serão calculadas da seguinte maneira:
      >
      >
      >`User Available Hours = [((40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours`

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

   * **O Cronograma do Usuário**: [!DNL Workfront] O usa o agendamento do usuário, bem como a variável [!UICONTROL Agendamento Padrão] do sistema para calcular o Valor [!UICONTROL FTE] valor do usuário nas ferramentas de gerenciamento de recursos. As Horas Disponíveis são calculadas de acordo apenas com o cronograma do usuário. O valor de [!UICONTROL FTE] do usuário é ignorado. Esta é a configuração padrão.

      Para obter mais informações sobre cronogramas, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obter mais informações sobre o [!UICONTROL Agendar], consulte  [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Se o usuário não estiver associado a um agendamento, as Horas Disponíveis para o usuário serão calculadas usando apenas o [!UICONTROL Agendamento Padrão].

      As Horas disponíveis para o usuário são calculadas pela seguinte fórmula:


      `User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]`


      O Disponível [!UICONTROL FTE] para o usuário é calculada pela seguinte fórmula:


      `User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours`


      >[!INFO]
      >
      >Por exemplo, se a variável [!UICONTROL Agendamento Padrão] é de 40 horas por semana, a programação do usuário é de 30 horas por semana e a [!UICONTROL Horário de trabalho] é 0,5 o [!UICONTROL FTE] do usuário é 0,35.
      >
      >Se o usuário tiver 2 horas de Folga por dia, a variável Semanal Disponível [!UICONTROL FTE] será calculada da seguinte forma:
      >
      >
      >`User Weekly Available [!UICONTROL FTE] = [(30-2) * 0.5] / 40 = 0.35`

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
