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
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 0%

---

# Configurar [!UICONTROL Gerenciamento de recursos] preferências

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

<span class="preview">As informações destacadas nesta página se referem à funcionalidade ainda não disponível no geral. Está disponível somente no ambiente de Visualização.</span>

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

## Informações tidas em conta ao calcular a capacidade de um usuário

Ao calcular a capacidade de um usuário, a Workfront considera as seguintes informações:

* O número de horas agendadas, conforme definido no Agendamento do usuário ou no do sistema Workfront [!UICONTROL Programação padrão]
* [!UICONTROL Agendar] [!UICONTROL Exceções] (dependendo de [!UICONTROL Agendar] for usada, poderá ser as exceções do agendamento do usuário ou aquelas associadas à variável [!DNL Workfront] [!UICONTROL Programação padrão])
* Tempo limite do usuário
* O valor do Equivalente de Tempo Total ([!UICONTROL FTE]) do usuário ou do [!DNL Workfront] sistema. O [!UICONTROL FTE] é igual a 1 quando o usuário trabalha em tempo integral, conforme definido no cronograma.
<div class="preview">
* O valor de [!UICONTROL Tempo de trabalho] para o usuário que se refere ao tempo que o usuário gasta no trabalho relacionado ao projeto. Isso não inclui tempo de despesas gerais, como reuniões e treinamento. O [!UICONTROL Work Time] é igual a 1 quando o usuário está disponível para trabalhar o tempo todo, conforme indicado pelo [!UICONTROL FTE] ou pelo agendamento, o que significa que ele não gasta tempo em trabalhos não relacionados ao projeto, como reuniões ou treinamentos.
</div>

Para obter informações sobre planejamento e programação de recursos em [!DNL Workfront], consulte [Introdução ao Gerenciamento de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).


## Configurar [!UICONTROL Gerenciamento de recursos] preferências

>[!NOTE]
>
>Como essa é uma configuração global, essa seleção afeta todos os cálculos para todo o sistema, para todos os usuários, em todas as ferramentas de gerenciamento de recursos.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. Clique em **[!UICONTROL Gerenciamento de recursos]**.
1. Selecione um dos métodos a seguir para calcular a disponibilidade dos usuários no [!DNL Workfront]:

   * **O agendamento padrão**: [!DNL Workfront] O usa a Programação padrão do sistema e o FTE individual do usuário para calcular as Horas disponíveis do usuário nas ferramentas de gerenciamento de recursos.

      Para obter mais informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obter mais informações sobre como localizar o valor do [!UICONTROL FTE], consulte  [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      O Workfront calcula as Horas Disponíveis de um usuário usando a seguinte fórmula quando o administrador do Workfront escolhe A [!UICONTROL Programação padrão]:


      No ambiente Produção:

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

      <div class="preview">

      No ambiente de Visualização:

      ```
      User Available Hours = [([!UICONTROL Default Schedule] Hours - [!UICONTROL Exceptions]) * [!UICONTROL FTE] - Time off hours] * Work Time
      ```

      >[!INFO]
      >
      >Por exemplo, se a Programação Padrão for de 40 horas por semana, a FTE no perfil do usuário é de 0,5, o usuário tem 1 hora de Tempo de folga um dia e a variável [!UICONTROL Tempo de trabalho] no perfil do usuário é 0,5, o usuário está disponível para o trabalho real do projeto por 9,5 horas por semana.
      >
      >Se o usuário tiver 1 hora de folga por dia, suas Horas disponíveis serão calculadas da seguinte maneira:
      >
      >
      ```
      >User Available Hours = [(40 - 0) * 0.5) - 1] * 0.5 = 9.5 hours
      >```

      </div>


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
      >Se o usuário não estiver associado a um agendamento, as Horas Disponíveis para o usuário serão calculadas usando somente o [!UICONTROL Programação padrão].

      No ambiente Produção:


      As horas disponíveis para o usuário são calculadas pela seguinte fórmula:

      ```
      User Available Hours = Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours
      ```

      Disponível [!UICONTROL FTE] para o usuário é calculado pela seguinte fórmula:

      ```
      User Available [!UICONTROL FTE] = (Hours from the [!UICONTROL Schedule] of the User - [!UICONTROL Schedule Exceptions] - Time off hours) / [!UICONTROL Default Schedule] hours
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

      <div class="preview">

      No ambiente de Visualização:

      As horas disponíveis para o usuário são calculadas pela seguinte fórmula:

      ```
      User Available Hours = (Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]
      ```

      Disponível [!UICONTROL FTE] para o usuário é calculado pela seguinte fórmula:

      ```
      User Available [!UICONTROL FTE] = [(Hours from the [!UICONTROL Schedule] of the User - Schedule Exceptions - Time off hours) * [!UICONTROL Work Time]] / [!UICONTROL Default Schedule] hours
      ```

      >[!INFO]
      >
      >Por exemplo, se a variável [!UICONTROL Programação padrão] é de 40 horas por semana, a programação do usuário é de 30 horas por semana e a do usuário [!UICONTROL Tempo de trabalho] é 0,5 o valor de [!UICONTROL FTE] do usuário é 0,35.
      >
      >Se o usuário tiver 2 horas de folga por dia, sua Disponibilidade Semanal [!UICONTROL FTE] serão calculadas da seguinte forma:
      >
      >
      ```
      >User Weekly Available FTE = [(30-2) * 0.5] / 40 = 0.35
      >```

      </div>

1. Clique em **[!UICONTROL Salvar]**.
