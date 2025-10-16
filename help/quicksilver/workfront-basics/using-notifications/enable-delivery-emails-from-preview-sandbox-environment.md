---
navigation-topic: notifications
title: Ativar a entrega de emails do ambiente Visualização da sandbox
description: Se você quiser receber notificações por email do ambiente Visualizar sandbox, será necessário habilitar essa funcionalidade nas configurações do usuário enquanto estiver conectado à Visualização.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 770e20cf9e32ac9884f5eb320f7067fcf162c63d
workflow-type: tm+mt
source-wordcount: '463'
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

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença</strong></td> 
   <td> 
   <p>Colaborador ou superior para alterar sua própria configuração</p> <p>Padrão para editar a configuração para outros usuários</p> 
   Ou
   <p> Solicitar ou em um nível superior para alterar sua própria configuração</p> <p>Planejar a edição da configuração para outros usuários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator].</p> </li> 
     <li> <p>Em seu nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. E, para a configuração [!UICONTROL Usuários], em [!UICONTROL Ajustar suas configurações] <img src="assets/gear-icon-in-access-levels.png"> , a opção [!UICONTROL Criar] e pelo menos uma das duas opções [!UICONTROL Administrador de Usuários] devem estar habilitadas. </li> 
     <li>Se você estiver usando a opção [!UICONTROL Administrador de Usuários (Usuários de Grupo)], deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
