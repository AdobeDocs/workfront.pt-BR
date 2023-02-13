---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Atualizações controladas pelo sistema
description: O Adobe Workfront captura a atividade que ocorre em determinados objetos, registrando as informações de status no [!UICONTROL Atualizações] área.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# Atualizações controladas pelo sistema

[!DNL Adobe Workfront] captura a atividade que ocorre em determinados objetos, registrando informações de status no [!UICONTROL Atualizações] área.

O [!UICONTROL Atualizações] inclui os seguintes tipos de atualizações:

* **Atualizações do usuário:** Inserido manualmente pelos usuários. Também conhecido como comentários, respostas e observações.

   ![](assets/updates-qs-350x125.png)

* **Atualizações do sistema:** Feito automaticamente pelo sistema. Uma atualização do sistema inclui uma breve nota descrevendo o tipo de mudança que aconteceu com o item.

   <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

Os seguintes objetos podem ter atualizações:

* Projeto
* Tarefa
* Problema
* Portfólio
* Programa
* Usuário
* Modelos
* Tarefas do modelo
* Documentos
* Folhas de horas

Seu [!DNL Workfront] a licença determina se as atualizações do sistema são exibidas por padrão no [!UICONTROL Atualizações] área de objetos. [!DNL Workfront] usuários com uma [!UICONTROL Plano] licença tem atualizações do sistema exibidas na [!UICONTROL Atualizações] por padrão. No entanto, os usuários podem filtrar as atualizações do sistema, conforme descrito na seção [[!UICONTROL Habilitar] ou desative as atualizações do sistema](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) seção em [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Todos os outros [!DNL Workfront] por padrão, as licenças filtram atualizações do sistema.

[!DNL Workfront] os administradores podem definir que tipo de alterações o sistema deve rastrear na variável [!UICONTROL Atualizações] área. Nem todos os objetos têm configuráveis [!UICONTROL atualizar] feeds de status. Os seguintes objetos têm um [!UICONTROL Atualizações] área que captura feeds de atualização rastreados pelo sistema, mas não tem feeds de status de atualização configuráveis:

* Modelos
* Tarefas do modelo
* Documentos
* Folhas de horas

Para obter mais informações sobre feeds de atualização do sistema e como ativá-los, consulte [Configurar atualizações do sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). Para obter mais informações sobre como configurar atualizações de usuários, consulte [Configurar preferências para atualizações do usuário](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
