---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Criar um agendamento
description: Você pode definir as semanas de trabalho dos usuários usando agendamentos. Você pode associar um agendamento a um usuário ou projeto. Isso permite [!DNL Workfront] para calcular linhas do tempo e disponibilidade do usuário.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Criar um agendamento

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Como um [!DNL Adobe Workfront] administrador, você pode definir sua semana de trabalho usando agendamentos. Você pode associar um agendamento a um usuário ou projeto. Isso permite [!DNL Workfront] para calcular linhas do tempo e disponibilidade do usuário.

Quando você tem usuários que trabalham em fusos horários diferentes, criar uma programação em cada um dos fusos horários e associá-la a esses usuários garante que seu trabalho seja registrado em [!DNL Workfront] em tempo real e que sua disponibilidade é sempre precisa de acordo com quando trabalham.

Para obter informações sobre como associar agendamentos a usuários e projetos, consulte os seguintes artigos:

* [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
* [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md)

Os administradores de grupo também podem criar agendamentos associados aos grupos que gerenciam. Para obter mais informações, consulte [Criar e modificar agendamentos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Para obter informações sobre como usar agendamentos para ajudar usuários a colaborar em [!DNL Workfront] em todos os fusos horários, consulte [Trabalhar em vários fusos horários](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano da [!UICONTROL Adobe Workfront]</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar um agendamento

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. Clique em **[!UICONTROL Agendamentos]**.
1. Clique em **[!UICONTROL Novo agendamento]**.
1. Especifique um nome para o agendamento.
1. (Opcional) Selecione **[!UICONTROL Programação padrão]** para identificar essa programação como padrão.

   Você pode ter mais de uma programação em [!DNL Workfront], mas você só pode ter uma programação padrão.

   Você deve ter pelo menos uma programação em [!DNL Workfront]. Se você tiver apenas um, ele será designado como a programação padrão.

   >[!NOTE]
   >
   >Não é possível designar um agendamento como padrão se você for um administrador de grupo. Somente um [!DNL Workfront] O administrador pode designar um agendamento como padrão para o sistema.

   ![](assets/new-schedule.png)

1. No **[!UICONTROL Agendar]** selecione uma programação diária arrastando o contorno azul entre blocos de hora para destacá-los.

   Recomendamos que você selecione 8 blocos de uma hora em um período de 9 horas. Isso se acomoda para almoço ou outras pausas.

   ![](assets/new-schedule-with-exceptions.png)

1. No **[!UICONTROL Detalhes]** , especifique as seguintes informações:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Grupo com acesso de administração]</td>
     <td><p>Indique o grupo cujos administradores têm permissão para editar este agendamento.</p>
     <p><b>IMPORTANTE</b>:</p>
      <ul>
       <li>
       <p>Se você for um administrador de grupo criando uma programação, este campo será obrigatório.</p>
       <p>Como administrador de grupo, você só poderá criar um agendamento se ele for designado para um grupo ou subgrupo para o qual você foi designado como administrador.</p>
       <p>Se você gerenciar apenas um grupo, esse grupo será selecionado nesse campo, por padrão.</p>
       <p>Se você gerenciar vários grupos, é necessário selecionar um grupo nesse campo antes de salvar o agendamento.</p></li>
       <li>Se você for um [!DNL Workfront] administrador criando um agendamento, este campo é opcional. Ao criar um agendamento sem associá-lo a um grupo, ele é salvo como um agendamento no nível do sistema e não pode ser gerenciado por um administrador de grupo de qualquer grupo.
       <p>Os agendamentos atribuídos a contas ou projetos ficam visíveis para todos os usuários que podem editar esses objetos. Isso é verdadeiro para programações de nível de sistema e de grupo.</p>
       </li>
       <p>Especificar um Grupo com Acesso de Administração para um agendamento não atribui o agendamento aos usuários do grupo; ela permite somente que os administradores de grupo no grupo editem, excluam e copiem o agendamento.</p>
       <p>Os administradores de grupo não podem editar, excluir ou copiar agendamentos no nível do sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Grupos com acesso de exibição]</td>
     <td><p>Selecione os grupos com acesso à [!UICONTROL View] para os quais este agendamento está visível.</p>
     <p>Somente os usuários nos grupos especificados aqui podem encontrar o agendamento no menu suspenso quando estiverem atribuindo a ela usuários ou projetos.</p></tr>
    <tr>
     <td>[!UICONTROL Fuso horário]</td>
     <td><p>Selecione o fuso horário de sua programação.</p>
     <p>Se você associar a programação a um usuário, recomendamos que o Fuso Horário da programação corresponda ao do usuário.Para obter informações sobre os fusos horários do usuário, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edite o perfil de um usuário.
     </td>
    </tr>
   </table>


1. No **[!UICONTROL Exceções]** , especifique as exceções para o agendamento.

   As exceções são dias completos ou meio que precisam ser excluídos da programação, como feriados ou eventos da empresa.

   >[!NOTE]
   >
   >Se você já sabe quais são as exceções de programação recorrente, poderá definir as exceções de programação para muitos anos no futuro.

   Dias completos ou parciais podem ser excluídos da programação de trabalho. Clique na data para selecioná-la como uma exceção e selecione a variável **[!UICONTROL O dia todo]** para indicar se a exceção é um dia completo ou não.

   ![](assets/schedule-adding-an-all-day-exception.png)

1. Especifique a hora de início e fim para as exceções de dia parcial.

   ![parcial-dia-exceção-nos-agendamentos.png](assets/partial-day-exception-on-schedules.png)

1. Clique em **[!UICONTROL Salvar]**, depois clique em **[!UICONTROL Salvar] Alterações**.

1. (Opcional) Associe o agendamento a um usuário.

   Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Opcional) Associe o agendamento a um projeto.

   Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).
