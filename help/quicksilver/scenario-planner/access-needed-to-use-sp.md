---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Acesso necessário para usar o Planejador de cenários
description: O Planejador de cenários requer uma licença separada da Adobe Workfront e acesso adicional.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Acesso necessário para usar o [!DNL Scenario Planner]

A variável [!DNL Scenario Planner] exige uma licença adicional. Para obter informações sobre o [!DNL Workfront Scenario Planner], consulte [A variável [!DNL Scenario Planner] visão geral](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Sem acesso ou permissões corretos, talvez você não consiga exibir o [!UICONTROL Cenários] área de[!DNL  Adobe Workfront] nem gerenciar planos ou iniciativas para sua organização. O gerenciamento de planos e iniciativas inclui sua criação, edição e exclusão.

>[!IMPORTANT]
>
>Ao acessar [!UICONTROL Cenários], você só poderá exibir e gerenciar os planos criados. Se quiser permitir que outros usuários exibam ou gerenciem os planos criados, faça o seguinte:
>
>* Enviar um link para seu plano para outros usuários
>* Compartilhar o plano com outros usuários
>
>  Para obter informações sobre o compartilhamento de um plano, consulte [Compartilhar um plano na [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Quando um usuário é desativado, seus planos não têm proprietário e não podem ser acessados a menos que compartilhados anteriormente com um link.

## Acesso necessário para visualizar e usar o [!DNL Adobe Workfront Scenario Planner]

Você deve garantir que as seguintes condições sejam atendidas antes de poder acessar o [!DNL Workfront Scenario Planner]:

<!--drafted for P&P:

* Depending on whether you use the current or the legacy Workfront plans, your organization must have the following:

  * For the current plans:  

    * The [!UICONTROL Ultimate] [!DNL Workfront] plan.

      Or
  
    * The [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] plan, in addition to purchasing a separate [!DNL Scenario Planner] license.

  * For the legacy plans: (indent the bullets below, before the NOTE)

-->

* Sua organização deve comprar um [!DNL Workfront] [!UICONTROL Empresas] ou superior [!DNL Workfront] plano. Para obter informações sobre o [!DNL Workfront] planos, consulte [Planos do Workfront](https://workfront.com/plans).
* Sua organização deve comprar um [!DNL Workfront Scenario Planner] licença, além de uma [!DNL Workfront] licença. Entre em contato com [!DNL Workfront] Representante de conta para saber mais sobre [!DNL Workfront Scenario Planner] licenças.

<!--drafted for P&P: 

* Depending on whether you use the current or legacy licenses, your [!DNL Workfront] administrator must assign you a license of any of the following types: 

  * For the current licenses: 
    * [!UICONTROL Standard]
    * [!UICONTROL Light]

  * For the legacy licenses: (re-indent the licenses below and reword the sentence)

-->



* Seu [!DNL Workfront] o administrador deve atribuir uma licença de qualquer um dos seguintes [!DNL Workfront] tipos:

   * [!UICONTROL Plano]
   * [!UICONTROL Trabalho]
   * [!UICONTROL Revisar]

  >[!NOTE]
  >
  >Usuários com um [!UICONTROL Solicitação] ou [!UICONTROL Externo] o tipo de licença não pode acessar o [!DNL Workfront Scenario Planner].

<!--drafted - replace the note above with this at P&P release: 
  * When using the current licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
  * When using the legacy licenses, users with a Request or External license type cannot access the Scenario Planner. -->

* Seu [!DNL Workfront] o administrador deve fornecer [!UICONTROL Exibir] ou [!UICONTROL Editar] acesso a [!DNL Scenario Planner] no seu nível de acesso.

  Para obter informações sobre a concessão de acesso ao [!DNL Workfront Scenario Planner], consulte [Conceder acesso ao [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* (Opcional e recomendado) Para exibir ou atualizar informações financeiras para seus planos e iniciativas, [!DNL Workfront] o administrador também deve conceder acesso a [!UICONTROL Dados financeiros] no seu nível de acesso. Para obter informações sobre como conceder dados financeiros no seu nível de acesso, consulte [Conceder acesso a dados financeiros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  <!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

* Se você precisar acessar planos que não foram criados, um criador de planos deve fornecer as permissões corretas para que o plano possa acessá-los. Para obter informações sobre as permissões necessárias para acessar planos e iniciativas que você não criou, consulte [Permissões necessárias para acessar planos e iniciativas](#permissions-needed-to-access-plans-and-initiatives) neste artigo.

## Acesso necessário para visualizar planos e iniciativas

Além de sua empresa adquirir a licença correta para o [!DNL Workfront Scenario Planner], seu [!DNL Workfront] administrador também deve atribuir a você o seguinte acesso e configuração para que você possa visualizar o [!DNL Workfront Scenario Planner] e as informações nesta área:

* Um nível de acesso com pelo menos [!UICONTROL Exibir] acesso a [!DNL Scenario Planner].

  Para obter informações sobre o nível de acesso a [!DNL Scenario Planner], consulte [Conceder acesso ao [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Um nível de acesso com pelo menos [!UICONTROL Exibir] acesso a [!UICONTROL Dados financeiros] se você também precisar exibir informações financeiras sobre o plano e as iniciativas. Alguns exemplos de informações financeiras são orçamentos, custos ou taxas de função de trabalho.

  Para obter informações sobre o [!UICONTROL Dados financeiros] nível de acesso, consulte [Conceder acesso a dados financeiros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Solicitantes] e [!UICONTROL Externo] Os usuários não têm acesso a para visualizar as [!DNL Scenario Planner].

* Exibir permissões para o plano. Para obter informações sobre as permissões necessárias para acessar planos e iniciativas que você não criou, consulte [Permissões necessárias para acessar planos e iniciativas](#permissions-needed-to-access-plans-and-initiatives) neste artigo.

## Acesso necessário para gerenciar planos e iniciativas

Seu [!DNL Workfront] o administrador deve atribuir o seguinte acesso para que você possa gerenciar os planos e suas informações na [!DNL Scenario Planner]:

* A [!UICONTROL Plano] ou [!UICONTROL Trabalho] tipo de licença com acesso para Editar ao [!DNL Scenario Planner] no seu nível de acesso.

  Todos os outros tipos de licença não têm acesso para gerenciar planos.

  Para obter informações sobre como conceder acesso a [!DNL Scenario Planner] a partir do Nível de acesso, consulte [Conceder acesso ao [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plano] tipo de licença com [!UICONTROL Editar] acesso a [!UICONTROL Dados financeiros] no seu nível de acesso, se você também precisar atualizar informações financeiras sobre o plano.

  Alguns exemplos de informações financeiras que podem ser editadas são [!UICONTROL Orçamento], [!UICONTROL Benefício Planejado], e [!UICONTROL Custos fixos].

  >[!TIP]
  >
  >Somente [!UICONTROL Plano] os titulares das licenças [!UICONTROL Editar] acesso a [!UICONTROL Dados financeiros].

  Para obter informações sobre o [!UICONTROL Dados financeiros] nível de acesso, consulte [Conceder acesso a dados financeiros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Gerencie permissões para um plano que você não criou. Para obter informações sobre as permissões necessárias para acessar planos e iniciativas que você não criou, consulte [Permissões necessárias para acessar planos e iniciativas](#permissions-needed-to-access-plans-and-initiatives) neste artigo.

## Permissões necessárias para acessar planos e iniciativas

Os Níveis de acesso funcionam em conjunto com as permissões no [!DNL Workfront] para dar visibilidade aos planos e iniciativas que você não criou. Além de ter o nível de acesso correto para acessar o [!DNL Scenario Planner], você também deverá ter as permissões corretas para o plano que deseja exibir ou gerenciar, se não for o criador desses planos.

Por padrão, você tem acesso somente aos planos criados. Para exibir planos criados por outros usuários, eles devem compartilhar os planos com você. Para obter informações sobre planos de compartilhamento, consulte [Compartilhar um plano na [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Se um usuário compartilhar um link para um plano sem também compartilhar o plano, você poderá solicitar permissões para o plano. Para obter informações sobre a solicitação de permissões para planos, consulte [Solicitar acesso a um plano no [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

