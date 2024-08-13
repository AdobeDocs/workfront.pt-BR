---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Criar um Cronograma
description: Você pode definir as semanas de trabalho dos usuários com cronogramas. Você pode associar um agendamento a um usuário ou projeto. Isso permite [!DNL Workfront] calcular linhas do tempo e disponibilidade de usuários.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 0%

---

# Criar um agendamento

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

Como administrador [!DNL Adobe Workfront], você pode definir sua semana de trabalho com cronogramas. Você pode associar um agendamento a um usuário ou projeto. Isso permite que [!DNL Workfront] calcule linhas do tempo e a disponibilidade do usuário.

Quando você tem usuários que trabalham em fusos horários diferentes, criar um agendamento em cada um dos fusos horários e associá-lo a esses usuários garante que seu trabalho seja registrado em [!DNL Workfront] em tempo real e que sua disponibilidade seja sempre precisa de acordo com quando eles trabalham.

Para obter informações sobre como associar agendas a usuários e projetos, consulte [Editar perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) e [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Os administradores de grupo também podem criar agendamentos associados aos grupos que gerenciam. Para obter mais informações, consulte [Criar e modificar as agendas de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

Para obter informações sobre como usar agendas para ajudar usuários a colaborar no [!DNL Workfront] entre fusos horários, consulte [Trabalhando entre fusos horários](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

Para obter informações sobre como os agendamentos são usados no planejamento de recursos, consulte [Visão geral dos agendamentos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) e [Visão geral do Planejador de recursos](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

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
       <p>Ou</p>
       <p>Atual: [!UICONTROL Plano]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um agendamento

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Agendamentos]**.
1. Clique em **[!UICONTROL Novo Calendário]**.
1. Insira um nome para o agendamento.
1. (Opcional) Selecione **[!UICONTROL Agendamento padrão]** para identificar este agendamento como seu padrão.

   Você deve ter pelo menos um agendamento em [!DNL Workfront]. Se você tiver apenas uma, ela será designada como a programação padrão.

   Você pode ter mais de um agendamento, mas só pode ter um agendamento padrão.

   >[!NOTE]
   >
   >Você não pode designar um agendamento como o agendamento padrão se for um administrador de grupo. Somente um administrador do [!DNL Workfront] pode designar um agendamento como padrão para o sistema.

   ![Novo agendamento](assets/new-schedule.png)

1. Na guia **[!UICONTROL Agendar]**, selecione um agendamento diário arrastando o contorno azul entre os blocos de horas para realçá-los.

   Recomendamos que você selecione 8 blocos de uma hora durante um período de 9 horas. Isso acomoda para almoço ou outros intervalos.

   ![Blocos de tempo em um agendamento](assets/new-schedule-with-exceptions.png)

1. Na guia **[!UICONTROL Detalhes]**, insira as seguintes informações:

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Grupo com Acesso de Administração]</td>
     <td><p>Selecione o grupo cujos administradores têm permissão para editar este agendamento.</p>
     <p><b>IMPORTANTE</b>:</p>
      <ul>
       <li>
       <p>Se você for um administrador de grupo que cria um agendamento, esse campo será obrigatório.</p>
       <p>Como administrador de grupo, você só poderá criar um agendamento se ele for designado para um grupo ou subgrupo para o qual você foi designado como administrador.</p>
       <p>Se você gerenciar apenas um grupo, esse grupo será selecionado nesse campo, por padrão.</p>
       <p>Se você gerenciar vários grupos, deverá selecionar um grupo nesse campo antes de salvar o agendamento.</p></li>
       <li>Se você for um administrador [!DNL Workfront] criando um agendamento, este campo será opcional. Quando você cria um agendamento sem associá-lo a um grupo, ele é salvo como um agendamento no nível do sistema e não pode ser gerenciado por um administrador de grupo de nenhum grupo.
       <p>Os cronogramas atribuídos a contas ou projetos estão visíveis para todos os usuários que podem editar esses objetos. Isso ocorre para programações de nível de sistema e de grupo.</p>
       </li>
       <p>A especificação de um Grupo com Acesso de Administração para um agendamento não atribui o agendamento aos usuários do grupo; ela só permite que os administradores do grupo editem, excluam e copiem o agendamento.</p>
       <p>Os administradores de grupo não podem editar, excluir ou copiar agendamentos no nível do sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Grupos com Acesso de Exibição]</td>
     <td><p>Selecione os grupos com acesso à [!UICONTROL View] que podem ver esse agendamento.</p>
     <p>Somente os usuários nos grupos especificados aqui podem encontrar o agendamento no menu suspenso quando estão atribuindo-o a usuários ou projetos.</p></tr>
    <tr>
     <td>[!UICONTROL Fuso Horário]</td>
     <td><p>Selecione o fuso horário para o agendamento.</p>
     <p>Se você associar o agendamento a um usuário, recomendamos que o fuso horário do agendamento corresponda ao do usuário. Para obter informações sobre fusos horários do usuário, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de usuário.
     </td>
    </tr>
   </table>


1. Na guia **[!UICONTROL Exceções]**, especifique as exceções ao agendamento.

   As exceções são dias inteiros ou meio que precisam ser excluídos da programação, como feriados ou eventos da empresa.

   >[!NOTE]
   >
   >Se você já souber quais são as exceções de programação recorrentes, poderá definir as exceções de programação para muitos anos no futuro.

   Dias inteiros ou parciais podem ser excluídos da programação de trabalho. Clique na data para selecioná-la como uma exceção e selecione o campo **[!UICONTROL Todo o dia]** para indicar se a exceção é um dia inteiro ou não.

   ![Exceção de dia inteiro](assets/schedule-adding-an-all-day-exception.png)

1. Informe a hora inicial e final para as exceções de dias parciais.

   ![Exceção de dia parcial](assets/partial-day-exception-on-schedules.png)

1. Clique em **[!UICONTROL Salvar]** e em **[!UICONTROL Salvar] Alterações**.

1. (Opcional) Associe o agendamento a um usuário.

   Para obter informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. (Opcional) Associe o agendamento a um projeto.

   Para obter informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).
