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
source-git-commit: d76ab0e165d280f84718b52cc72a9b4c152a0897
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Atualizações rastreadas pelo sistema

{{highlighted-preview}}

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] captura a atividade que ocorre em determinados objetos registrando informações de status no [!UICONTROL Atualizações] área.

A variável [!UICONTROL Atualizações] inclui os seguintes tipos de atualizações:

* **Atualizações de usuário:** Inserido manualmente por usuários. Também conhecido como comentários, respostas e notas.

  Para obter mais informações sobre a configuração de atualizações de usuários, consulte [Configurar preferências para atualizações de usuário](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Atualizações do sistema:** Automaticamente feito pelo sistema. Uma atualização do sistema inclui uma breve nota descrevendo que tipo de alteração aconteceu com o item.

  Para obter mais informações sobre os feeds de atualização do sistema e como ativá-los, consulte [Configurar atualizações do sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Considerações sobre atualizações rastreadas pelo sistema

As atualizações rastreadas pelo sistema não estão disponíveis para todos os objetos que têm a área Atualizações.

* A variável [!UICONTROL Atualizações] está disponível para os seguintes objetos:

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
   * [!UICONTROL Story]

     Entrada [!DNL Workfront], uma história é uma tarefa.
   * [!UICONTROL Iteração]
   * [!UICONTROL Meta]

     Você deve ter uma licença adicional para ter acesso à [!UICONTROL Metas] área. Para obter informações, consulte [Requisitos para usar as metas do Workfront](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Cartão] em um quadro

     Para obter mais informações sobre atualizações em cartões, consulte [Usar placas conectadas em placas](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] O não rastreia atualizações do sistema para os seguintes objetos:

   * [!UICONTROL Equipe]
   * [!UICONTROL Modelo]
   * [!UICONTROL Modelo de Tarefa]
   * Ad-hoc [!UICONTROL Cartão]
   * [!UICONTROL Iterações]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Veja a seguir as diferenças entre a experiência de comentários nova e herdada:

   * Ao usar a nova experiência de comentários, as atualizações do usuário são exibidas na guia Comentários e as atualizações do sistema são exibidas na guia Atividade do sistema.

     Para obter mais informações sobre a nova experiência de comentários, consulte [Nova experiência de comentários](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * <span class="preview">Ao usar a nova experiência de comentários, os usuários não podem adicionar um comentário a uma atualização do sistema. No entanto, todas as respostas feitas aos registros de atividade do sistema na experiência de comentários herdada são preenchidas na guia Atividade do sistema como somente leitura na nova experiência de comentários.</span>
   * Ao usar a experiência de comentários herdada, as atualizações do sistema e do usuário são exibidas em um feed contínuo.

   * Ao usar a experiência de comentários herdada, os usuários podem visualizar as atualizações do sistema por padrão ou optar por não exibi-las. Não é possível desativar as atualizações do sistema ao usar a nova experiência de comentários.

     Para obter informações sobre como desativar a exibição de atualizações do sistema, consulte a seção [Ativar ou desativar atualizações do sistema](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) no artigo [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* O Workfront registra atualizações rastreadas pelo sistema para os seguintes objetos, mas não há opção para desativar a exibição deles:

   * [!UICONTROL Portfolio]
   * [!UICONTROL Programa]
   * [!UICONTROL Iteração]

* [!DNL Workfront] administradores podem definir que tipo de alterações o sistema deve rastrear no [!UICONTROL Atualizações] área. Nem todos os objetos que têm um [!UICONTROL Atualizações] também têm configurações [!UICONTROL atualizar] Feeds. Os seguintes objetos têm um [!UICONTROL Atualizações] área que captura feeds de atualização rastreados pelo sistema, mas não têm feeds de atualização configuráveis:

   * [!UICONTROL Documento]
   * [!UICONTROL Planilha de horas]
   * [!UICONTROL Iteração]
   * [!UICONTROL Meta]


