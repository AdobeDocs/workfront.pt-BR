---
navigation-topic: notifications
title: Ativar a entrega de emails do ambiente Preview Sandbox
description: Se quiser receber notificações por email do ambiente Preview Sandbox, ative essa funcionalidade nas configurações do usuário enquanto estiver conectado à Visualização.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Ativar a entrega de emails do ambiente Preview Sandbox

[!UICONTROL Adobe Workfront] desativa todas as comunicações por email dos ambientes Preview e Custom Refresh Sandbox. Para obter informações sobre o ambiente Preview Sandbox, consulte [O Ambiente de sandbox de visualização do Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Para obter informações sobre o ambiente Sandbox de atualização personalizada, consulte [O ambiente Sandbox de atualização personalizada do Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Se desejar receber as seguintes notificações por email do ambiente Preview Sandbox, ative essa funcionalidade nas configurações do usuário enquanto estiver conectado à Visualização:

* Notificações por email acionadas por notificações de evento
* Notificações de lembrete
* Notificações de lembrete atrasadas ou antecipadas automáticas
* Convites por email

Você pode fazer isso sozinho ou para qualquer usuário que tenha acesso para editar. Para obter mais informações sobre o acesso necessário para editar usuários, consulte [Conceder acesso aos usuários](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>A entrega de relatórios e as notificações por push no aplicativo móvel ficam sempre desativadas no ambiente de sandbox de visualização. Nem você nem o [!DNL Workfront] o administrador pode ativar o delivery de relatórios ou notificações por push para o aplicativo móvel ao acessar o ambiente Preview Sandbox .
>
>Para obter informações sobre deliveries de relatórios, consulte [Visão geral da entrega de relatórios](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior para alterar sua própria configuração</p> <p>[!UICONTROL Plan] para editar a configuração para outros usuários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Você deve ter uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator].</p> <p> Para obter informações sobre esse nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p>No nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. E, para a configuração [!UICONTROL Usuários], em [!UICONTROL Otimizar suas configurações] <img src="assets/gear-icon-in-access-levels.png"> , a opção [!UICONTROL Criar] e pelo menos uma das duas opções do [!UICONTROL User Admin] devem estar habilitadas. </p> <p>Se estiver usando a opção [!UICONTROL Administrador de usuário (Usuários de grupo)], você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Para obter informações sobre a configuração [!UICONTROL Usuários] em um nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Ativar a entrega de emails do ambiente Preview Sandbox

1. Faça logon no ambiente Preview Sandbox .
1. Clique na imagem do perfil no canto superior direito de [!DNL Adobe Workfront]. Em seguida, clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Ou

   Pesquisar por um usuário em [!DNL Workfront] e clique no nome. Em seguida, clique no botão **[!UICONTROL Mais]** e selecione **[!UICONTROL Editar]**.

   Ou

   Para vários usuários: Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **[!UICONTROL Usuários]** ![](assets/users-icon-in-main-menu.png).  Em seguida, selecione vários usuários e clique em **[!UICONTROL Editar]**.

1. Clique em **[!UICONTROL Preferências]**.
1. Selecionar **[!UICONTROL Receber emails deste ambiente de teste]**.

   >[!NOTE]
   >
   >Essa opção não estará disponível se você estiver em um ambiente de produção.

1. Clique em **[!UICONTROL Salvar alterações]**.
