---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Desativar ou reativar uma empresa
description: É possível desativar uma empresa que não é mais usada enquanto mantém todos os dados históricos associados. Se você desativar uma empresa já em uso em algum lugar do sistema, ela continuará a funcionar como sempre funcionou. Ele não é removido ou bloqueado.
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

É possível desativar uma empresa que não é mais usada enquanto mantém todos os dados históricos associados. Se você desativar uma empresa já em uso em algum lugar do sistema, ela continuará a funcionar como sempre funcionou. Ele não é removido ou bloqueado.

## Requisitos de acesso

Você deve ter o seguinte para gerenciar empresas no [!DNL Workfront]:

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>Um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso do [!UICONTROL System Administrator], que permite a edição de qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p>Acesso administrativo para gerenciar empresas, o que permite editar qualquer empresa no sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </li> 
    </ul> <p><b>Nota</b>:  
     <ul> 
      <li> <p>Também é possível gerenciar empresas associadas a qualquer grupo, onde você está atribuído como administrador de grupo.</p> </li> 
      <li> <p>Para adicionar e remover usuários do [!DNL Workfront] , você deve ter um dos seguintes itens:</p> 
       <ul> 
        <li> <p>O nível de acesso do [!UICONTROL System Administrator]. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
        <li> <p>No nível de acesso, [!UICONTROL Editar] deve ser selecionado para a configuração [!UICONTROL Usuários]. Além disso, para a configuração [!UICONTROL Usuários], em [!UICONTROL Otimizar suas configurações] <img src="assets/gear-icon-in-access-levels.png"> , a opção [!UICONTROL Criar] e pelo menos uma das duas opções do [!UICONTROL User Admin] devem estar habilitadas. </p> <p> <img src="assets/access-req-users.png" style="width: 350;height: 101;"> </p> <p>Se estiver usando a opção [!UICONTROL Administrador de usuário (Usuários de grupo)], você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> </li> 
       </ul> <p>Para obter informações sobre a configuração Usuários em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com seu [!DNL Workfront] administrador.

## Desativar ou reativar uma empresa

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Empresas]** ![](assets/companies-icon-left-panel.png).

1. Selecione uma ou mais empresas para desativar ou reativar.
1. Clique em **[!UICONTROL Editar]**.
1. Para uma única empresa, desative o **[!UICONTROL Está ativo]** para desativá-la ou habilitar a opção para ativá-la.

   Ou

   Para várias empresas, selecione **[!UICONTROL Não]** do **[!UICONTROL Está ativo]** menu suspenso para desativá-los, ou **[!UICONTROL Sim]** para ativá-los.

1. Clique em **[!UICONTROL Salvar alterações]**.
