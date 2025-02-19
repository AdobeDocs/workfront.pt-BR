---
navigation-topic: notifications
title: Ativar a entrega de emails do ambiente Visualização da sandbox
description: Se você quiser receber notificações por email do ambiente Visualizar sandbox, será necessário habilitar essa funcionalidade nas configurações do usuário enquanto estiver conectado à Visualização.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# Ativar a entrega de emails do ambiente Visualização da sandbox

O [!UICONTROL Adobe Workfront] desabilita todas as comunicações por email dos ambientes de Pré-visualização e de Atualização Personalizada da Sandbox. Para obter informações sobre o ambiente Visualização da sandbox, consulte [O ambiente Visualização da sandbox da Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Para obter informações sobre o ambiente de Sandbox de atualização personalizada, consulte [O ambiente de Sandbox de atualização personalizada do Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Se você quiser receber as seguintes notificações por email do ambiente Visualização da sandbox, será necessário habilitar essa funcionalidade nas configurações do usuário enquanto estiver conectado à Visualização:

* Notificações por email acionadas por notificações de eventos
* Notificações de lembrete
* Notificações automáticas de lembrete atrasadas ou antecipadas
* Convites por email

Você pode fazer isso para si mesmo ou para qualquer usuário que você tenha acesso para editar. Para obter mais informações sobre o acesso necessário para editar usuários, consulte [Conceder acesso aos usuários](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>O delivery de relatórios e as notificações por push no aplicativo móvel estão sempre desativados para o ambiente Visualização da sandbox. Nem você nem o administrador do [!DNL Workfront] podem habilitar a entrega de relatórios ou notificações por push para o aplicativo móvel quando você acessa o ambiente Visualizar Sandbox.
>
>Para obter informações sobre entregas de relatórios, consulte [Visão geral da entrega de relatórios](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior para alterar sua própria configuração</p> <p>[!UICONTROL Plano] para editar a configuração para outros usuários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator].</p> <p> Para obter informações sobre este nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>. </p> </li> 
     <li> <p>Em seu nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. E, para a configuração [!UICONTROL Usuários], em [!UICONTROL Ajustar suas configurações] <img src="assets/gear-icon-in-access-levels.png"> , a opção [!UICONTROL Criar] e pelo menos uma das duas opções [!UICONTROL Administrador de Usuários] devem estar habilitadas. </p> <p>Se você estiver usando a opção [!UICONTROL Administrador de Usuários (Usuários de Grupo)], deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Para obter informações sobre a configuração [!UICONTROL Usuários] em um nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Ativar a entrega de emails do ambiente Visualização da sandbox

1. Faça logon no ambiente de Pré-visualização da sandbox.
1. Clique na imagem do seu perfil no canto superior direito do [!DNL Adobe Workfront]. Em seguida, clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Ou

   Procure um usuário em [!DNL Workfront] e clique no nome dele. Em seguida, clique no menu **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Ou

   Para vários usuários: Clique no ícone **[!UICONTROL Menu principal]** ![Ícone do menu principal](assets/main-menu-icon.png) no canto superior direito do Workfront e clique no ícone **[!UICONTROL Usuários]** ![Usuário](assets/users-icon-in-main-menu.png).  Em seguida, selecione vários usuários e clique em **[!UICONTROL Editar]**.

1. Clique em **[!UICONTROL Preferências]**.
1. Selecione **[!UICONTROL Receber emails deste ambiente de teste]**.

   >[!NOTE]
   >
   >Essa opção não estará disponível se você estiver em um ambiente de produção.

1. Clique em **[!UICONTROL Salvar alterações]**.
