---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Acesso Necessário para Usar o Planejador de cenários
description: O Planejador de cenários requer uma licença separada da Adobe Workfront e acesso adicional.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 1b06589a705cf218239ff1273b865c05e4ceb96f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Acesso necessário para usar o [!DNL Scenario Planner]

<!--Audited: 04/2024-->

<!--The [!DNL Scenario Planner] has additional license requirements. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).-->

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Sem o acesso correto ou permissões, talvez você não consiga visualizar a área [!UICONTROL Cenários] de[!DNL &#x200B; Adobe Workfront] nem gerenciar planos ou iniciativas para sua organização. O gerenciamento de planos e iniciativas inclui sua criação, edição e exclusão.

## Acesso necessário para exibir e usar o [!DNL Adobe Workfront Scenario Planner]

Você deve garantir que todas as condições a seguir sejam atendidas antes de poder acessar o [!DNL Workfront Scenario Planner]:

1. Sua organização deve ter um pacote do Workfront Ultimate.

   O Planejador de cenários não está disponível para pacotes de fluxo de trabalho do Workfront.

   Fale com o representante de conta da Workfront se estiver renovando o Workfront e se quiser manter o Planejador de cenários.

   Se você for um novo cliente, o Planejador de cenários não estará mais disponível para compra.

   <!--Old: 
    Depending on whether you use the new or the current Workfront plan, your organization must have one of the following:
    * For the new plans, your organization must have the  [!UICONTROL Ultimate] [!DNL Workfront] plan. The Scenario Planner is included only in the [!UICONTROL Ultimate] plan. 
    * For the current Workfront plans, your organization must have both of the following: 
      * Your organization must purchase a [!DNL Workfront] [!UICONTROL Business] or higher [!DNL Workfront] plan. 
      
      * Your organization must purchase a [!DNL Workfront Scenario Planner] license, in addition to a [!DNL Workfront] license. Contact your [!DNL Workfront] Account Representative to learn about [!DNL Workfront Scenario Planner] licenses. -->

1. Você deve ter uma das seguintes licenças da Workfront:

   * [!UICONTROL Leve] ou superior
   * [!UICONTROL Revisor] ou superior

   <!--Old: 
      * For the current licenses: 
        * [!UICONTROL Plan]
        * [!UICONTROL Work]
        * [!UICONTROL Review]-->
   <!--Old: 
      >[!NOTE]
      > 
      >* When using the new licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
      >
      >* When using the current licenses, users with a Request or External license type cannot access the Scenario Planner. -->

1. O administrador do [!DNL Workfront] deve conceder a você acesso de [!UICONTROL Visualização] ou [!UICONTROL Edição] a [!DNL Scenario Planner] no seu nível de acesso.

   Para obter informações sobre como conceder acesso ao [!DNL Workfront Scenario Planner], consulte [Conceder acesso ao [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Opcional e recomendado) Para exibir ou atualizar informações financeiras para seus planos e iniciativas, o administrador do [!DNL Workfront] também deve conceder a você acesso a [!UICONTROL Dados Financeiros] no seu nível de acesso. Para obter informações sobre como conceder dados financeiros em seu nível de acesso, consulte [Conceder acesso a dados financeiros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).


<!--1. (Optional) If you need to access plans you didn't create, a plan creator must give you the correct permissions to their plan to access it. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.-->

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

<!--Repetitive from above?? 

## Access needed to view plans and initiatives

In addition to your company acquiring the correct license for the [!DNL Workfront Scenario Planner], your [!DNL Workfront] administrator must also assign you the following access and setup so you can view the [!DNL Workfront Scenario Planner] and the information in this area:

* An access level with at least [!UICONTROL View] access to [!DNL Scenario Planner].

  For information about the access level to [!DNL Scenario Planner], see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* An access level with at least [!UICONTROL View] access to [!UICONTROL Financial Data] if you need to also view financial information about the plan and the initiatives. Some examples of financial information are budgets, costs, or job role rates.

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] and [!UICONTROL External] Users do not have access to view the [!DNL Scenario Planner].

* View permissions to the plan. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

## Access needed to manage plans and initiatives

Your [!DNL Workfront] administrator must assign you the following access so you can manage plans and their information in the [!DNL Scenario Planner]:

* A [!UICONTROL Plan] or [!UICONTROL Work] license type with Edit access to the [!DNL Scenario Planner] in your access level.

  All other license types do not have access to manage plans.

  For information about granting access to [!DNL Scenario Planner] from the Access Level, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] license type with [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level, if you need to also update financial information about the plan.

  Some examples of financial information that you can edit are [!UICONTROL Budget], [!UICONTROL Planned Benefit], and [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Only [!UICONTROL Plan] license holders have [!UICONTROL Edit] access to [!UICONTROL Financial Data].

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Manage permissions to a plan that you didn't create. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

-->

## Permissões necessárias para acessar planos e iniciativas

Os Níveis de Acesso trabalham em conjunto com permissões no [!DNL Workfront] para lhe dar visibilidade dos planos e iniciativas que você não criou. Além de ter o nível de acesso correto para acessar o [!DNL Scenario Planner], você também deve ter as permissões corretas para os planos que deseja exibir ou gerenciar, se não for o criador desses planos.

Todos os usuários, incluindo administradores do sistema, têm acesso somente aos planos que criaram.

Para exibir planos criados por outros usuários, eles devem compartilhar seus planos com você das seguintes maneiras:

* Compartilhe o plano com você

  Para obter informações sobre planos de compartilhamento, consulte [Compartilhar um plano no [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

* Enviar um link para um plano que eles criaram

  Se um usuário compartilhar um link para um plano sem também compartilhar o plano, você poderá solicitar permissões para o plano. Para obter informações sobre como solicitar permissões para planos, consulte [Solicitar acesso a um plano no [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

>[!NOTE]
>
>Quando um usuário é desativado, seus planos não têm proprietário e não podem ser acessados a menos que compartilhados anteriormente com um link.


