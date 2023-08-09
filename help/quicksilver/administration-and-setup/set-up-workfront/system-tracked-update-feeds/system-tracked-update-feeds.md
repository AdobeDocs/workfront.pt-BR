---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Atualizações rastreadas pelo sistema
description: O Adobe Workfront captura a atividade que ocorre em determinados objetos registrando informações de status no [!UICONTROL Atualizações] área.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 6%

---

# Atualizações rastreadas pelo sistema

[!DNL Adobe Workfront] captura a atividade que ocorre em determinados objetos registrando informações de status no [!UICONTROL Atualizações] área.

A variável [!UICONTROL Atualizações] inclui os seguintes tipos de atualizações:

* **Atualizações de usuário:** Inserido manualmente por usuários. Também conhecido como comentários, respostas e notas.

  Para obter mais informações sobre a configuração de atualizações de usuários, consulte [Configurar preferências para atualizações de usuário](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Atualizações do sistema:** Automaticamente feito pelo sistema. Uma atualização do sistema inclui uma breve nota descrevendo que tipo de alteração aconteceu com o item.

  Para obter mais informações sobre os feeds de atualização do sistema e como ativá-los, consulte [Configurar atualizações do sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Considerações sobre atualizações rastreadas pelo sistema

* As atualizações rastreadas pelo sistema não estão disponíveis para todos os objetos que têm a área Atualizações. A variável [!UICONTROL Atualizações] está disponível para os seguintes objetos:

   * [!UICONTROL Projeto]
   * [!UICONTROL Tarefa]
   * [!UICONTROL Problema]
   * [!UICONTROL Portfólio]
   * [!UICONTROL Programa]
   * [!UICONTROL Usuário]
   * [!UICONTROL Modelo]
   * [!UICONTROL Modelo de Tarefa]
   * [!UICONTROL Equipe]
   * [!UICONTROL Documento]
   * [!UICONTROL Planilha de horas]
   * [!UICONTROL História]

     Entrada [!DNL Workfront], uma história é uma tarefa.
   * [!UICONTROL Iteração]
   * [!UICONTROL Meta]

     Você deve ter uma licença adicional para ter acesso à [!UICONTROL Metas] área. Para obter informações, consulte [Requisitos para usar as metas do Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Cartão] em um quadro

     Para obter mais informações sobre atualizações em cartões, consulte [Adicionar um cartão ad hoc a um quadro](../../../agile/get-started-with-boards/add-card-to-board.md).


* [!DNL Workfront] O não rastreia nenhuma atualização do sistema para os seguintes objetos:

   * [!UICONTROL Equipe]
   * [!UICONTROL Modelo]
   * [!UICONTROL Modelo de Tarefa]

<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Os usuários podem exibir as atualizações do sistema por padrão ou optar por não exibi-las.

  Para obter informações sobre como desativar a exibição de atualizações do sistema, consulte a seção [Ativar ou desativar atualizações do sistema](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) no artigo [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

  >[!NOTE]
  >
  >No momento, estamos reprojetando a experiência de comentários e o [!UICONTROL Atualizações] área em [!DNL Workfront].
  >
  > Não é possível ocultar atualizações do sistema ao usar a nova experiência de comentários.
  > 
  >Para obter mais informações sobre a nova experiência de comentários, consulte [Nova experiência de comentários](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* O Workfront registra atualizações rastreadas pelo sistema para os seguintes objetos, mas não há opção para desativar a exibição deles:

   * [!UICONTROL Portfólio]
   * [!UICONTROL Programa]
   * [!UICONTROL Iteração]

* [!DNL Workfront] administradores podem definir que tipo de alterações o sistema deve rastrear no [!UICONTROL Atualizações] área. Nem todos os objetos que têm um [!UICONTROL Atualizações] também têm configurações [!UICONTROL atualizar] Feeds. Os seguintes objetos têm um [!UICONTROL Atualizações] área que captura feeds de atualização rastreados pelo sistema, mas não têm feeds de atualização configuráveis:

   * [!UICONTROL Documento]
   * [!UICONTROL Planilha de horas]
   * [!UICONTROL Iteração]

