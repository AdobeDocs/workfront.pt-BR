---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Acesso necessário para usar o Planejador de cenários
description: O Planejador de cenários requer uma licença separada da Adobe Workfront e acesso adicional.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: f0f6c2bee98c6cebf8ea9e18bf34262f3c1d6e3a
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Acesso necessário para usar o [!DNL Scenario Planner]

O [!DNL Scenario Planner] requer uma licença adicional. Para obter informações sobre [!DNL Workfront Scenario Planner], consulte [A [!DNL Scenario Planner] visão geral](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Sem o acesso correto ou permissões, talvez você não consiga visualizar a área [!UICONTROL Cenários] de[!DNL  Adobe Workfront] nem gerenciar planos ou iniciativas para sua organização. O gerenciamento de planos e iniciativas inclui sua criação, edição e exclusão.

>[!IMPORTANT]
>
>Ao acessar [!UICONTROL Cenários], você só poderá exibir e gerenciar planos criados. Se quiser permitir que outros usuários exibam ou gerenciem os planos criados, faça o seguinte:
>
>* Enviar um link para seu plano para outros usuários
>* Compartilhar o plano com outros usuários
>
>  Para obter informações sobre como compartilhar um plano, consulte [Compartilhar um plano no [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Quando um usuário é desativado, seus planos não têm proprietário e não podem ser acessados a menos que compartilhados anteriormente com um link.

## Acesso necessário para exibir e usar o [!DNL Adobe Workfront Scenario Planner]

Você deve garantir que todas as condições a seguir sejam atendidas antes de poder acessar o [!DNL Workfront Scenario Planner]:

1. Sua organização deve ter um dos planos da Workfront descritos abaixo.

   Dependendo de você usar o plano novo ou o atual do Workfront, sua organização deve ter um dos seguintes:

   * Para os novos planos, sua organização deve ter um dos seguintes:

      * O plano [!UICONTROL Ultimate] [!DNL Workfront]. O Planejador de cenários está incluído no plano Ultimate.

        Ou

      * O plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront], além da compra de uma licença [!DNL Scenario Planner] separada.

   * Para os planos atuais do Workfront, sua organização deve ter o seguinte:

      * Sua organização deve comprar um plano do [!DNL Workfront] [!UICONTROL Business] ou superior [!DNL Workfront]. Para obter informações sobre os planos [!DNL Workfront], consulte [Planos Workfront](https://workfront.com/plans).

      * Sua organização deve comprar uma licença [!DNL Workfront Scenario Planner], além de uma licença [!DNL Workfront]. Entre em contato com o Representante de Conta do [!DNL Workfront] para saber mais sobre as licenças do [!DNL Workfront Scenario Planner].

1. Você deve ter uma das licenças da Workfront descritas abaixo.

   Dependendo de você usar uma licença nova ou atual, o administrador do [!DNL Workfront] deverá atribuir a você uma licença dos seguintes tipos:

   * Para as novas licenças:
      * [!UICONTROL Padrão]
      * [!UICONTROL Leve]

   * Para as licenças atuais:

      * [!UICONTROL Plano]
      * [!UICONTROL Trabalho]
      * [!UICONTROL Revisão]

   >[!NOTE]
   > 
   >* Ao usar as novas licenças, os usuários com o tipo de licença [!UICONTROL Colaborador] ou [!UICONTROL Externo] não podem acessar o [!DNL Scenario Planner].
   >
   >* Ao usar as licenças atuais, os usuários com um tipo de licença Solicitação ou Externa não podem acessar o Planejador de cenários.

1. O administrador do [!DNL Workfront] deve conceder a você acesso de [!UICONTROL Visualização] ou [!UICONTROL Edição] a [!DNL Scenario Planner] no seu nível de acesso.

   Para obter informações sobre como conceder acesso ao [!DNL Workfront Scenario Planner], consulte [Conceder acesso ao [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Opcional e recomendado) Para exibir ou atualizar informações financeiras para seus planos e iniciativas, o administrador do [!DNL Workfront] também deve conceder a você acesso a [!UICONTROL Dados Financeiros] no seu nível de acesso. Para obter informações sobre como conceder dados financeiros em seu nível de acesso, consulte [Conceder acesso a dados financeiros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Opcional) Se você precisar acessar planos que não criou, um criador de planos deve fornecer as permissões corretas para que o plano possa acessá-lo. Para obter informações sobre as permissões necessárias para acessar planos e iniciativas que você não criou, consulte a seção [Permissões necessárias para acessar planos e iniciativas](#permissions-needed-to-access-plans-and-initiatives) neste artigo.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Acesso necessário para visualizar planos e iniciativas

Além de a empresa adquirir a licença correta para o [!DNL Workfront Scenario Planner], o administrador do [!DNL Workfront] também deve atribuir a você o seguinte acesso e configuração para que você possa exibir o [!DNL Workfront Scenario Planner] e as informações desta área:

* Um nível de acesso com pelo menos [!UICONTROL Visualização] acesso a [!DNL Scenario Planner].

  Para obter informações sobre o nível de acesso a [!DNL Scenario Planner], consulte [Conceder acesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Um nível de acesso com pelo menos [!UICONTROL Exibir] acesso a [!UICONTROL Dados Financeiros] se você também precisar exibir informações financeiras sobre o plano e as iniciativas. Alguns exemplos de informações financeiras são orçamentos, custos ou taxas de função de trabalho.

  Para obter informações sobre o nível de acesso [!UICONTROL Dados Financeiros], consulte [Conceder acesso a dados financeiros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >Os usuários [!UICONTROL Solicitantes] e [!UICONTROL Externos] não têm acesso para exibir o [!DNL Scenario Planner].

* Exibir permissões para o plano. Para obter informações sobre as permissões necessárias para acessar planos e iniciativas que você não criou, consulte a seção [Permissões necessárias para acessar planos e iniciativas](#permissions-needed-to-access-plans-and-initiatives) neste artigo.

## Acesso necessário para gerenciar planos e iniciativas

O administrador do [!DNL Workfront] deve atribuir o seguinte acesso para que você possa gerenciar os planos e suas informações no [!DNL Scenario Planner]:

* Um tipo de licença do [!UICONTROL Plano] ou do [!UICONTROL Trabalho] com acesso de Edição ao [!DNL Scenario Planner] no seu nível de acesso.

  Todos os outros tipos de licença não têm acesso para gerenciar planos.

  Para obter informações sobre como conceder acesso a [!DNL Scenario Planner] a partir do Nível de Acesso, consulte [Conceder acesso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Um tipo de licença do [!UICONTROL Plano] com acesso de [!UICONTROL Edição] aos [!UICONTROL Dados Financeiros] no seu nível de acesso, caso você também precise atualizar informações financeiras sobre o plano.

  Alguns exemplos de informações financeiras que você pode editar são [!UICONTROL Orçamento], [!UICONTROL Benefício Planejado] e [!UICONTROL Custos Fixos].

  >[!TIP]
  >
  >Somente os titulares de licenças do [!UICONTROL Plano] têm acesso de [!UICONTROL Edição] aos [!UICONTROL Dados Financeiros].

  Para obter informações sobre o nível de acesso [!UICONTROL Dados Financeiros], consulte [Conceder acesso a dados financeiros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Gerencie permissões para um plano que você não criou. Para obter informações sobre as permissões necessárias para acessar planos e iniciativas que você não criou, consulte a seção [Permissões necessárias para acessar planos e iniciativas](#permissions-needed-to-access-plans-and-initiatives) neste artigo.

## Permissões necessárias para acessar planos e iniciativas

Os Níveis de Acesso trabalham em conjunto com permissões no [!DNL Workfront] para lhe dar visibilidade dos planos e iniciativas que você não criou. Além de ter o nível de acesso correto para acessar o [!DNL Scenario Planner], você também deve ter as permissões corretas para o plano que deseja exibir ou gerenciar, se não for o criador desses planos.

Por padrão, você tem acesso somente aos planos criados. Para exibir planos criados por outros usuários, eles devem compartilhar os planos com você. Para obter informações sobre planos de compartilhamento, consulte [Compartilhar um plano no [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Se um usuário compartilhar um link para um plano sem também compartilhar o plano, você poderá solicitar permissões para o plano. Para obter informações sobre como solicitar permissões para planos, consulte [Solicitar acesso a um plano no [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

