---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Visão geral das atualizações rastreadas pelo sistema
description: O Adobe Workfront captura a atividade que ocorre em determinados objetos registrando informações de status na área [!UICONTROL Atualizações] do objeto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 4448d2fc6d0230ef2f53ad0ea7ae0f10f52fcac4
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Visão geral das atualizações rastreadas pelo sistema

<!-- Audited: 06/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>-->

[!DNL Adobe Workfront] captura a atividade que está ocorrendo em determinados objetos registrando informações de status na seção [!UICONTROL Atualizações] do objeto.

Para obter informações sobre a seção Atualizações, consulte [Visão geral da seção Atualizações](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

A área [!UICONTROL Atualizações] inclui os seguintes tipos de atualizações:

* **Atualizações de usuário:** inseridas manualmente pelos usuários. Também conhecido como comentários, respostas e notas. As atualizações de usuário são exibidas nas guias Comentários e Todas as guias da seção Atualizações de um objeto.

  Para obter mais informações sobre como configurar atualizações de usuários, consulte [Configurar preferências para atualizações de usuários](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![Atualizações](assets/updates-qs-350x125.png)

* **Atualizações do sistema:** feitas automaticamente pelo sistema. Uma atualização do sistema inclui uma breve nota descrevendo que tipo de alteração aconteceu com o item. As atualizações de sistema são exibidas na Atividade do sistema e nas guias All da seção Updates de um objeto.

  Para obter mais informações sobre os feeds de atualização do sistema e como habilitá-los, consulte [Configurar atualizações do sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![Exemplo de atualizações do sistema](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Considerações sobre atualizações rastreadas pelo sistema

As atualizações rastreadas pelo sistema não estão disponíveis para todos os objetos que têm a área Atualizações.

* A área [!UICONTROL Atualizações] está disponível para os seguintes objetos:

   * [!UICONTROL Projeto]
   * [!UICONTROL Tarefa]
   * [!UICONTROL Problema]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Programa]
   * [!UICONTROL Usuário]
   * [!UICONTROL Modelo]
   * [!UICONTROL Modelo de Tarefa]
   * [!UICONTROL Equipe]
   * [!UICONTROL Documento]
   * [!UICONTROL Planilha de horas]
   * [!UICONTROL História]

     Em [!DNL Workfront], uma história é uma tarefa.
   * [!UICONTROL Iteração]
   * [!UICONTROL Meta]

     Nem todos os pacotes do Workfront incluem o Workfront Goals. Para obter informações, consulte [Requisitos para usar as Metas do Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Cartão] em um quadro

     Para obter mais informações sobre atualizações em cartões, consulte [Usar cartões conectados em quadros](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] não rastreia atualizações do sistema para os seguintes objetos:

   * [!UICONTROL Equipe]
   * [!UICONTROL Modelo]
   * [!UICONTROL Modelo de Tarefa]
   * Cartão [!UICONTROL Ad-hoc]
   * [!UICONTROL Iterações]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* As atualizações do usuário são exibidas na guia Comentários e as atualizações do sistema são exibidas na Atividade do sistema e nas guias Todos.

  Para obter uma lista de objetos que não têm a Atividade do Sistema ou as guias Todos, consulte [Visão geral da seção Atualizar](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* Não é possível adicionar uma resposta a uma atualização do sistema. No entanto, quaisquer respostas feitas aos registros de atividade do sistema na experiência de comentários herdada anterior a 11 de abril de 2024 serão preenchidas na guia Atividade do sistema como somente leitura.

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* Os administradores do [!DNL Workfront] podem definir que tipo de alterações o sistema deve rastrear na área [!UICONTROL Atualizações]. Nem todos os objetos que têm uma área [!UICONTROL Atualizações] também têm feeds [!UICONTROL atualizações] configuráveis. Os seguintes objetos têm uma área [!UICONTROL Atualizações] que captura feeds de atualização rastreados pelo sistema, mas não têm feeds de atualização configuráveis:

   * [!UICONTROL Documento]
   * [!UICONTROL Planilha de horas]
   * [!UICONTROL Iteração]
   * [!UICONTROL Meta]


