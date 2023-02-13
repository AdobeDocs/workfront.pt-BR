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
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---

# Configurar [!UICONTROL Gerenciamento de recursos] preferências

<!--Linked to lots of articles for resource planning and LINKED TO CONTEXT SENSITIVE HELP - DO NOT CHANGE OR REMOVE!</p>
Edit the first part, once they add more settings in the Res Management Preferences - right now, only the FTE calculation is the
-->

Como um [!DNL Adobe Workfront] administrador você pode configurar o [!UICONTROL Gerenciamento de recursos] Preferências do seu sistema. Essas preferências determinam como a disponibilidade ou a capacidade do usuário e o FTE são calculados para a variável [!DNL Workfront] ferramentas de planejamento e agendamento de recursos.

Para obter informações sobre planejamento e programação de recursos em [!DNL Workfront], consulte [Introdução ao Gerenciamento de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Requisitos de acesso

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
   <td> <p>Nível de acesso do Administrador do sistema</p> <p>Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar [!UICONTROL Gerenciamento de recursos] preferências

>[!NOTE]
>
>Como essa é uma configuração global, essa seleção afeta todos os cálculos para todo o sistema, para todos os usuários, em todas as ferramentas de gerenciamento de recursos e para todos os Pools de Recursos.

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. Clique em **[!UICONTROL Gerenciamento de recursos]**.
1. Selecione um dos métodos a seguir para calcular a disponibilidade dos usuários no [!DNL Workfront]:

   * **O agendamento padrão**: [!DNL Workfront] O usa a Programação Padrão do sistema e o FTE individual do usuário para calcular as Horas Disponíveis do usuário nas ferramentas de gerenciamento de recursos.\

      Para obter mais informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

      Para obter mais informações sobre o valor do FTE do usuário, consulte  [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

      O Workfront calcula as Horas Disponíveis de um usuário usando a seguinte fórmula quando o administrador do Workfront escolhe A Programação Padrão:

      ```
      User Available Hours = (Default Schedule Hours - Exceptions) * FTE - Time off hours
      ```

      **Exemplo:**\
      Por exemplo, se a Programação padrão for de 40 horas por semana e o FTE no perfil do usuário for de 0,5, o usuário estará disponível para trabalhar 20 horas por semana.

      Se o usuário tiver 1 hora de folga por dia, suas Horas disponíveis serão calculadas da seguinte maneira:

      ```
      User Available Hours = (40 * 0.5) - 1 = 19 hours
      ```

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

   * **O cronograma do usuário**: [!DNL Workfront] O usa o agendamento do usuário e o Agendamento padrão do sistema para calcular o valor FTE disponível do usuário nas ferramentas de gerenciamento de recursos. As Horas disponíveis são calculadas somente de acordo com o agendamento do usuário. O valor do FTE do usuário é ignorado. Esta é a configuração padrão.

      >[!NOTE]
      >
      >Se o usuário não estiver associado a um agendamento, as Horas disponíveis para o usuário serão calculadas usando o Agendamento padrão.

      O FTE disponível para o usuário é calculado pela seguinte fórmula:

      ```
      User Available FTE = (Hours from the Schedule of the User - Time off hours) / Default Schedule Hours
      ```

      **Exemplo:** Por exemplo, se a Programação padrão for de 40 horas por semana e a programação do usuário for de 30 horas por semana, a ETI do usuário será de 0,75.

      Se o usuário tiver 2 horas de Tempo de folga por dia, seu FTE Disponível por Semana será calculado da seguinte maneira:

      ```
      User Weekly Available FTE = (30-2) / 40 = 0.70
      ```

1. Clique em **[!UICONTROL Salvar]**.
