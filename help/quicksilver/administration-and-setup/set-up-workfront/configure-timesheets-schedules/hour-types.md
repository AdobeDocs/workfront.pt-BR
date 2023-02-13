---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gerenciar tipos de hora
description: Você pode associar tipos de hora às entradas de hora. Os tipos de horas são rótulos que você usa para definir suas entradas de hora.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Gerenciar tipos de hora

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Você pode associar tipos de hora às entradas de hora. Os tipos de horas são rótulos que você usa para definir suas entradas de hora.

Há dois conjuntos de tipos de hora:

* **Tipos de horas específicas do projeto**: Este é o momento em que os projetos, as tarefas e os problemas estão conectados. Tipos de hora específicos do projeto podem ser associados a entradas de hora em qualquer lugar do [!DNL Adobe Workfront] onde você pode registrar o tempo dos projetos, tarefas e problemas.

   Ao fazer logon [!DNL Workfront], os tipos de hora específicos do projeto que estão disponíveis dependem das opções de configuração definidas nos níveis do sistema, do projeto e do usuário.

   Os seguintes tipos de hora padrão específicos do projeto estão sempre disponíveis:

   * Tempo em Projeto
   * Tempo em Tarefa
   * Tempo em Problema

   O [!DNL Workfront] O administrador determina quais tipos de hora específicos do projeto são disponibilizados, conforme descrito em [Definir os tipos de hora e a disponibilidade das folhas de horas](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >Se você ativar tipos de horas específicos do projeto no [!DNL Workfront] , pelo menos uma hora específica do projeto deve estar ativada em cada projeto no sistema. Não é possível ativar um tipo de hora específico do projeto no nível do sistema e não há tipos de hora específicos do projeto disponíveis no nível do projeto.

* **Tipos de hora gerais**: As horas gerais não podem ser associadas a um projeto, tarefa ou problema e são registradas diretamente em uma folha de ponto. Para obter mais informações sobre tempo de registro, consulte [Tempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).

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

## Tipos de hora incorporados

O Workfront vem com um conjunto de tipos de hora incorporados. Esses tipos de hora não podem ser editados e não podem ser ocultos.

Os tipos de hora que vêm com [!DNL Workfront] são:

* **[!UICONTROL Hora de Doença]**: Um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema.
* **[!UICONTROL Hora de Férias]**: Um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema.
* **[!UICONTROL Despesas gerais]**: Um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. No entanto, pode contar como receita no processo de planejamento do projeto.
* **[!UICONTROL Hora do projeto]**: Um tipo de hora geral que pode ser associado somente a entradas de hora em um projeto.
* **[!UICONTROL Hora da Tarefa]**: Um tipo de hora geral que pode ser associado somente a entradas de hora em uma tarefa.
* **[!UICONTROL Hora de emissão]**: um tipo de hora geral que pode ser associado apenas a entradas de hora em um problema.

## Criar tipos de hora

Como um [!DNL Workfront] administrador, você pode criar novos tipos de hora para sua organização nos níveis do sistema e do projeto. Depois de criar tipos de hora nos níveis do sistema e do projeto, os usuários podem definir quais tipos de hora estarão disponíveis para projetos e usuários específicos. Para obter mais informações, consulte o [Definir os tipos de hora e a disponibilidade das folhas de horas](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Para criar novos tipos de hora:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Folha de Horas e Horas]** > **[!UICONTROL Tipos de hora]**.

1. Clique em **[!UICONTROL Novo tipo de hora].**
1. Especifique as seguintes informações no **[!UICONTROL Novo tipo de hora]** formulário:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Dê um nome ao novo tipo de hora que seja facilmente reconhecível no sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Adicione uma descrição para o tipo de hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Escopo]</td> 
      <td> <p>Defina se o tipo de hora é um tipo de hora geral ou específico do projeto, selecionando o escopo correto no menu suspenso.</p> <p>Os tipos de hora gerais são visíveis apenas nas folhas de horas e não podem ser associados a projetos, tarefas ou problemas.</p> <p><b>IMPORTANTE</b>: Se você tiver um Tipo de hora personalizado que seja [!UICONTROL Específico do projeto] e alterá-lo para [!UICONTROL Geral], todas as tarefas, ocorrências e horas do projeto existentes serão definidas com os tipos padrão do sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Contar Como Receita]</td> 
      <td>Selecione essa opção se desejar que a entrada de hora associada a esse tipo de hora afete seus cálculos de receita.</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Contar como Receita]**: Selecione essa opção se desejar que a entrada de hora associada a esse tipo de hora afete seus cálculos de receita.

1. Clique em **[!UICONTROL Criar tipo de hora].**

## Desativar tipos de hora

Se os tipos de hora se tornarem obsoletos e você não quiser mais que os usuários associem suas entradas de hora a eles, é possível desativar os tipos de hora.

Desativar tipos de hora oculta os tipos de hora de qualquer lugar em [!DNL Workfront] onde os tipos de hora estão visíveis.

Para desativar um tipo de hora:

1. Clique em **[!UICONTROL Configuração]** próximo do canto superior direito de [!DNL Adobe Workfront] na Barra de Navegação Global.

1. Expandir **[!UICONTROL Folha de Horas e Preferências de Horas]**, depois clique em **[!UICONTROL Tipos de hora]**.

1. Selecione o tipo de hora que deseja desativar.

1. Clique em **[!UICONTROL Desativar]**.
