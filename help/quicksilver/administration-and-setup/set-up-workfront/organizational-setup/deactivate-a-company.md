---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desativar ou reativar uma empresa
description: É possível desativar uma empresa que não é mais usada, mantendo todos os dados históricos associados a ela. Se você desativar uma empresa já em uso em algum lugar no sistema, ela continuará a funcionar da mesma forma que sempre funcionou. Ele não é removido ou bloqueado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 479dfb9d-0e47-4790-a33a-336b415fbf6e
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Desativar ou reativar uma empresa

É possível desativar uma empresa que não é mais usada, mantendo todos os dados históricos associados a ela. Se você desativar uma empresa já em uso em algum lugar no sistema, ela continuará a funcionar da mesma forma que sempre funcionou. Ele não é removido ou bloqueado.

## Requisitos de acesso

Você deve ter o seguinte para gerenciar empresas em [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] plano*</p> </td> 
   <td>[!UICONTROL Team] ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator], que permite editar qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>. </p> </li> 
     <li> <p>Acesso administrativo para gerenciar empresas, que permite editar qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </li> 
    </ul> <p><b>NOTA</b>:  
     <ul> 
      <li> <p>Você também pode gerenciar empresas associadas a qualquer grupo ao qual esteja atribuído como administrador de grupo.</p> </li> 
      <li> <p>Para adicionar e remover usuários do sistema [!DNL Workfront], você deve ter um dos seguintes:</p> 
       <ul> 
        <li> <p>O nível de acesso do [!UICONTROL System Administrator]. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>. </p> </li> 
        <li> <p>Em seu nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. Além disso, para a configuração [!UICONTROL Usuários], em [!UICONTROL Ajustar suas configurações] <img src="assets/gear-icon-in-access-levels.png"> , a opção [!UICONTROL Criar] e pelo menos uma das duas opções [!UICONTROL Administrador de Usuário] devem estar habilitadas. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>Se você estiver usando a opção [!UICONTROL Administrador de Usuários (Usuários de Grupo)], deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
       </ul> <p>Para obter informações sobre a configuração Usuários em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber quais configurações de plano, tipo de licença ou nível de acesso você tem, contate o administrador do [!DNL Workfront].

## Desativar ou reativar uma empresa

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito do [!DNL Adobe] Workfront e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Empresas]** ![](assets/companies-icon-left-panel.png).

1. Selecione uma ou mais empresas para desativar ou reativar.
1. Clique em **[!UICONTROL Editar]**.
1. Para uma única empresa, desabilite a opção **[!UICONTROL Está ativo]** para desativá-lo ou habilite a opção para ativá-lo.

   Ou

   Para várias empresas, selecione **[!UICONTROL Não]** no menu suspenso **[!UICONTROL Está ativo]** para desativá-las ou **[!UICONTROL Sim]** para ativá-las.

1. Clique em **[!UICONTROL Salvar alterações]**.
