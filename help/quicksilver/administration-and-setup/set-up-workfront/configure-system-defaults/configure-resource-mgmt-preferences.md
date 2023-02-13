---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Configurar preferências do Gerenciamento de recursos
description: Como um [!DNL Adobe Workfront] administrador você pode configurar as Preferências de gerenciamento de recursos para seu sistema. Essas preferências de Gerenciamento de recursos determinam como a disponibilidade ou a capacidade do usuário e o FTE são calculados para o [!DNL Workfront] ferramentas de planejamento e agendamento de recursos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7cde2238-cb34-4bee-baba-69d256a3912d
source-git-commit: 80ad604330e8b55037f1607b754cc8bb34f6a3ec
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# Configurar [!UICONTROL Gerenciamento de recursos] preferências

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<!--drafted for Work time field: <span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Como um [!DNL Adobe Workfront] administrador você pode configurar o [!UICONTROL Gerenciamento de recursos] Preferências do seu sistema. Essas preferências determinam como a hora do usuário ou a disponibilidade ou a capacidade do FTE são calculadas para o [!DNL Workfront] ferramentas de planejamento e agendamento de recursos.

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

Você deve ter o seguinte para executar as etapas neste artigo:

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Nível de acesso do Administrador do sistema</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>Nota</b>:

Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

<!--drafted for Work time field: 

## Information taken into account when calculating user's capacity

When calculating a user's capacity, Workfront takes into account the following information:

* The number of scheduled hours, as defined in either the Schedule of the user or the Workfront system's [!UICONTROL Default Schedule]
* [!UICONTROL Schedule] [!UICONTROL Exceptions] (depending on which [!UICONTROL Schedule] is used, it can be the exceptions of the user's schedule, or those associated with the [!DNL Workfront] [!UICONTROL Default Schedule])
* User's time off
* The value of the Full Time Equivalent ([!UICONTROL FTE]) of the user or that of the [!DNL Workfront] system. The [!UICONTROL FTE] equals 1 when the user works full time, as defined in the schedule. 

<!-drafted for Work Time field  

* <span class="preview">The value of [!UICONTROL Work Time] for the user which refers to time that the user spends on project-related work. This does not include overhead time, like meetings and training. The [!UICONTROL Work Time] equals 1 when the user is available for work the entire time as indicated by the [!UICONTROL FTE] or the schedule, which means they don't spend any time in non-project-related work like meetings or trainings.</span>

-->

Para obter informações sobre planejamento e programação de recursos em [!DNL Workfront], consulte [Introdução ao Gerenciamento de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

—>

## Configurar [!UICONTROL Gerenciamento de recursos] preferências

>[!NOTE]
>
>Como essa é uma configuração global, essa seleção afeta todos os cálculos para todo o sistema, para todos os usuários, em todas as ferramentas de gerenciamento de recursos e para todos os Pools de Recursos.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. Clique em **[!UICONTROL Gerenciamento de recursos]**.
1. Selecione um dos métodos a seguir para calcular a disponibilidade dos usuários no [!DNL Workfront]:

   * **O agendamento padrão**: [!DNL Workfront] O usa a Programação padrão do sistema e o FTE individual do usuário para calcular as Horas disponíveis do usuário nas ferramentas de gerenciamento de recursos.

      Para obter mais informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obter mais informações sobre o valor do usuário [!UICONTROL FTE], consulte  [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      O Workfront calcula as Horas Disponíveis de um usuário usando a seguinte fórmula quando o administrador do Workfront escolhe A [!UICONTROL Programação padrão]:

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      ```
      User Available Hours = ([!UICONTROL Default Schedule] Hours - Exceptions) * FTE - Time off hours
      ```

      >[!INFO]
      >
      > Por exemplo, se a variável [!UICONTROL Programação padrão] é de 40 horas por semana e a variável [!UICONTROL FTE] no perfil do usuário é 0,5, ele fica disponível para trabalhar 20 horas por semana.
      >Se o usuário tiver 1 hora de folga por dia, suas Horas disponíveis serão calculadas da seguinte maneira:
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5)] - 1 = 19 hours
      >```
   <!--drafted for Work Time field

      <div class="preview">
      
      In the Preview environment: 

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >For example, if the Default Schedule is 40 hours a week,  the FTE in the profile of the user is 0.5, the user has 1 hour of Time off one day, and the [!UICONTROL Work Time] in the profile of the user is 0.5, the user is available for actual project work for 9.5 hours a week.
      >
      >If the user has 1 hour of Time off one day, their Available Hours will be calculated as follows:
      >
      >```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>

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

   * **O cronograma do usuário**: [!DNL Workfront] O usa o agendamento do usuário e a variável [!UICONTROL Programação padrão] do sistema para calcular o valor de [!UICONTROL FTE] valor do usuário nas ferramentas de gerenciamento de recursos. As Horas disponíveis são calculadas somente de acordo com o agendamento do usuário. O valor da variável [!UICONTROL FTE] do usuário é ignorado. Esta é a configuração padrão.

      Para obter mais informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obter mais informações sobre o [!UICONTROL Agendar], consulte  [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      >[!NOTE]
      >
      >Se o usuário não estiver associado a um agendamento, as Horas Disponíveis para o usuário serão calculadas usando o [!UICONTROL Programação padrão].

      <!--drafted for Work Time field:
      In the Production environment: 
      -->

      Disponível [!UICONTROL FTE] para o usuário é calculado pela seguinte fórmula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - Time off hours) / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Por exemplo, se a variável [!UICONTROL Programação padrão] é de 40 horas por semana e a programação do usuário é de 30 horas por semana, a [!UICONTROL FTE] do usuário é 0,70.
      >  
      >Se o usuário tiver 2 horas de folga por dia, sua Disponibilidade Semanal [!UICONTROL FTE] serão calculadas da seguinte forma:
      > 
      >
      ```
      >User Weekly Available [!UICONTROL FTE] = (30-2) / 40 = 0.70
      >```

      <!--drafted for Work Time field:

      <div class="preview">

      In the Preview environment: 
      
      The Available hours for the user is calculated by the following formula:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Time off hours) * [!UICONTROL Work Time]
      ```    

      The Available [!UICONTROL FTE] for the user is calculated by the following formula:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >For example, if the [!UICONTROL Default Schedule] is 40 hours a week, the schedule of the user is 30 hours a week, and the user's [!UICONTROL Work Time] is 0.5 the [!UICONTROL FTE] of the user is 0.35.
      >
      >If the user has 2 hours of Time off one day, their Weekly Available [!UICONTROL FTE] will be calculated as follows:
      >
      >```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```
      (************ checking this second other with Dev/ Artur - not sure where Exceptions fit in **********)

      </div>
      -->
1. Clique em **[!UICONTROL Salvar]**.
