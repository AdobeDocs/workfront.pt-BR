---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Criar um agendamento
description: Você pode definir as semanas de trabalho dos usuários usando agendamentos. Você pode associar um agendamento a um usuário ou projeto. Isso permite [!DNL Workfront] para calcular as linhas do tempo e a disponibilidade dos usuários.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 3aad2a3d9ad32313cb14670965bc3ad05ab215d3
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Criar um agendamento

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Como um [!DNL Adobe Workfront] administrador, você pode definir sua semana de trabalho usando agendamentos. Você pode associar um agendamento a um usuário ou projeto. Isso permite [!DNL Workfront] para calcular as linhas do tempo e a disponibilidade dos usuários.

Quando você tem usuários que trabalham em fusos horários diferentes, criar um agendamento em cada um dos fusos horários e associá-lo a esses usuários garante que o trabalho deles seja registrado no [!DNL Workfront] em tempo real e que sua disponibilidade seja sempre precisa de acordo com o horário em que trabalham.

Para obter informações sobre como associar cronogramas a usuários e projetos, consulte os seguintes artigos:

* [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md)

Os administradores de grupo também podem criar agendamentos associados aos grupos que gerenciam. Para obter mais informações, consulte [Criar e modificar as agendas de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Para obter informações sobre como usar as agendas para ajudar os usuários a colaborar no [!DNL Workfront] em fusos horários, consulte [Trabalhar em fusos horários](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Para obter informações sobre como as programações são usadas no planejamento de recursos, consulte [Visão geral dos cronogramas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) e [Visão geral do Planejador de recursos](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano do [!UICONTROL Adobe Workfront]</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar um agendamento

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront e clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. Clique em **[!UICONTROL Agendamentos]**.
1. Clique em **[!UICONTROL Nova programação]**.
1. Especifique um nome para o agendamento.
1. (Opcional) Selecione **[!UICONTROL Agendamento Padrão]** para identificar esse cronograma como padrão.

   Você pode ter mais de um cronograma em [!DNL Workfront], mas você só pode ter um agendamento padrão.

   Você deve ter pelo menos uma programação em [!DNL Workfront]. Se você tiver apenas uma, ela será designada como a programação padrão.

   >[!NOTE]
   >
   >Você não pode designar um agendamento como o agendamento padrão se for um administrador de grupo. Somente um [!DNL Workfront] administrador pode designar um agendamento como padrão para o sistema.

   ![](assets/new-schedule.png)

1. No **[!UICONTROL Agendar]** , selecione um agendamento diário arrastando o contorno azul pelos blocos de horas para realçá-los.

   Recomendamos que você selecione 8 blocos de uma hora durante um período de 9 horas. Isso acomoda para almoço ou outros intervalos.

   ![](assets/new-schedule-with-exceptions.png)

1. No **[!UICONTROL Detalhes]** especifique as seguintes informações:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Grupo com Acesso de Administração]</td>
     <td><p>Indique o grupo cujos administradores têm permissão para editar este agendamento.</p>
     <p><b>IMPORTANTE</b>:</p>
      <ul>
       <li>
       <p>Se você for um administrador de grupo que cria um agendamento, esse campo será obrigatório.</p>
       <p>Como administrador de grupo, você só poderá criar um agendamento se ele for designado para um grupo ou subgrupo para o qual você foi designado como administrador.</p>
       <p>Se você gerenciar apenas um grupo, esse grupo será selecionado nesse campo, por padrão.</p>
       <p>Se você gerenciar vários grupos, deverá selecionar um grupo nesse campo antes de salvar o agendamento.</p></li>
       <li>Se você é um [!DNL Workfront] administrador que cria um agendamento, esse campo é opcional. Quando você cria um agendamento sem associá-lo a um grupo, ele é salvo como um agendamento no nível do sistema e não pode ser gerenciado por um administrador de grupo de nenhum grupo.
       <p>Os cronogramas atribuídos a contas ou projetos estão visíveis para todos os usuários que podem editar esses objetos. Isso ocorre para programações de nível de sistema e de grupo.</p>
       </li>
       <p>A especificação de um Grupo com Acesso de Administração para um agendamento não atribui o agendamento aos usuários do grupo; ela só permite que os administradores do grupo editem, excluam e copiem o agendamento.</p>
       <p>Os administradores de grupo não podem editar, excluir ou copiar agendamentos no nível do sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Grupos com Acesso de Exibição]</td>
     <td><p>Selecione os grupos com acesso à [!UICONTROL View] para os quais este agendamento está visível.</p>
     <p>Somente os usuários nos grupos especificados aqui podem encontrar o agendamento no menu suspenso quando estão atribuindo-o a usuários ou projetos.</p></tr>
    <tr>
     <td>[!UICONTROL Fuso Horário]</td>
     <td><p>Selecione o fuso horário para seu cronograma.</p>
     <p>Se você associar o agendamento a um usuário, recomendamos que o Fuso Horário do agendamento corresponda ao do usuário. Para obter informações sobre os fusos horários do usuário, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário.
     </td>
    </tr>
   </table>


1. No **[!UICONTROL Exceções]** especifique as exceções para a programação.

   As exceções são dias inteiros ou meio que precisam ser excluídos da programação, como feriados ou eventos da empresa.

   >[!NOTE]
   >
   >Se você já souber quais são as exceções de programação recorrentes, poderá definir as exceções de programação para muitos anos no futuro.

   Dias inteiros ou parciais podem ser excluídos da programação de trabalho. Clique na data para selecioná-la como uma exceção e selecione a variável **[!UICONTROL O dia todo]** para indicar se a exceção é um dia inteiro ou não.

   ![](assets/schedule-adding-an-all-day-exception.png)

1. Especifique a hora de início e término para as exceções de dias parciais.

   ![partial-day-exception-on-schedule.png](assets/partial-day-exception-on-schedules.png)

1. Clique em **[!UICONTROL Salvar]** e, em seguida, clique em **[!UICONTROL Salvar] Alterações**.

1. (Opcional) Associe o agendamento a um usuário.

   Para obter informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Opcional) Associe o agendamento a um projeto.

   Para obter informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).
