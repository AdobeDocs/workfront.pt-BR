---
filename: change-date-format-chrome
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Alterar o formato de datas em  [!DNL Adobe Workfront]
description: Para alterar o formato de data para as datas em [!DNL Adobe Workfront] você deve alterar as configurações de idioma no seu navegador.
feature: Get Started with Workfront
exl-id: 9fac92fb-e3d1-4537-b324-4b35447cef28
source-git-commit: 7ad3fbcfa5be5074016f399560cca509d81f4714
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Alterar o formato de datas em [!DNL Adobe Workfront]

<!--this article used to be called "Change the date format in Adobe Workfront when using Chrome". The team decieded to make it more generic and hide the steps. Also see drafted content below-->

>[!IMPORTANT]
>
> As informações neste artigo se aplicam apenas a organizações que ainda não foram integradas à Experiência unificada do Adobe.
> Se sua organização foi integrada à Experiência unificada do Adobe, sua preferência de data é controlada pela preferência de idioma definida no shell unificado do Adobe. A configuração de idioma padrão e, portanto, a configuração de data padrão, é `en-US`.

Você pode alterar o formato de datas em [!DNL Adobe Workfront], como [!UICONTROL Data de Conclusão Planejada], [!UICONTROL Data de Conclusão Efetiva] ou [!UICONTROL Data de Conclusão Projetada].

Por exemplo, você pode alterar o formato de data de _DD/MM/AAAA_ para _MM/DD/AAAA_ ou vice-versa.
Ou você pode alterar o formato de data de _MM/DD/AA_ para _Mon DD, AAAA_.

Você pode alterar os formatos de data no Workfront das seguintes maneiras, dependendo das alterações que deseja ver e de onde gostaria de ver as alterações.

* Para alterar todos os formatos de data para todas as páginas em [!DNL Workfront] de acordo com sua localização e idioma, você deve alterar as configurações de idioma no seu navegador.

  Por exemplo, se o idioma padrão do navegador estiver definido como *[!UICONTROL inglês (Estados Unidos)]*, as datas serão exibidas nos seguintes formatos:

   * DD/MM/AAAA
   * DD seg., AAAA

  Para alterar as configurações de idioma no [!DNL Chrome] ou em qualquer outro navegador, você deve modificar as configurações desse navegador. As etapas para modificar as configurações de um navegador variam de um navegador para outro. Consulte as áreas [!UICONTROL Ajuda], [!UICONTROL Preferências] ou [!UICONTROL Configurações] do seu navegador para saber como modificar suas configurações.

* Para alterar o formato de datas somente em relatórios e modos de exibição, atualize a configuração [!UICONTROL Formato do Campo] na área [!UICONTROL Opções Avançadas] de uma coluna ao criar o relatório ou o modo de exibição. Isso não modifica o formato de data de acordo com o local ou idioma. Ele modifica o formato de datas no contexto do mesmo local ou idioma.

  ![](assets/field-format-in-advanced-options-of-a-view-highlighted.png)

  Para obter mais informações, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Para alterar o formato de datas em todas as notificações por email de saída para toda a organização, você deve atualizar a configuração [!UICONTROL Local de Email Padrão] na área [!UICONTROL Informações do Cliente] da [!UICONTROL Configuração].

  ![](assets/default-email-locale-field.png)

  Para obter mais informações, consulte [Configurar informações básicas do sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Para alterar o formato de todas as datas em todas as notificações por email de saída para um único usuário, você deve atualizar a configuração [!UICONTROL Local de email] na caixa [!UICONTROL Editar pessoa], ao editar o perfil de um usuário.

  ![](assets/email-locale-for-user-profile-highlighted.png)

  Para obter mais informações, consulte [Editar perfil de usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--drafted because we should not document steps for a third-party application

To change your language settings in Chrome:

1. Click the 3-dots in the top right corner of your Chrome interface, then click **Settings**.
1. On the left area of the Settings page, expand **Advanced**, then click **Languages**.  
   Or  
   Search for *language*&nbsp;at the top of the Settings page, then click **Languages**.

1. In the **Language** list, locate the language and region that use your preferred date format.

   **Example:** If you speak English and you want the date format to be MM/DD/YYYY, you would select **English (United States)**. If you speak English and you want the date format to be DD/MM/YYY, you would select **English (United Kingdom)**.

1. (Conditional) If the language and region you want to use are not visible in the list, click **Add languages** to add it to the list.
1. Click the 3-dot menu next to the language and region you want to use, then click **Move to the top**.
1. Return to the Workfront interface, then refresh the page.  
   The date format is now updated in projects and other areas of Workfront that use MM/DD/YYYY or DD/MM/YYYY format when displaying dates.

   -->
