---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurar a integração do JumpSeat
description: É possível integrar [!DNL JumpSeat] com [!DNL Workfront] para criar orientação personalizada no produto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Configurar a integração do JumpSeat

É possível integrar [!DNL JumpSeat] com [!DNL Workfront] para criar orientação personalizada no produto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>[!UICONTROL Empresa] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Produto</strong></td> 
   <td>Você deve ter um ativo [!DNL JumpSeat] plano.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p> Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Pré-requisitos

Antes de começar, você deve

* Adicionar e ativar [!DNL Workfront] como um aplicativo no [!DNL JumpSeat]. Para obter mais informações, consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configure o [!DNL JumpSeat] integração

Recomendamos configurar um [!DNL JumpSeat] integração em seus ambientes de Pré-visualização e Produção.

>[!TIP]
>
>É necessário adicionar e ativar dois [!DNL Workfront] aplicativos em [!DNL JumpSeat]— um para Visualização e um para Produção. Consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/) para obter mais informações.

Para configurar o [!DNL JumpSeat] integração:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]**.
1. No painel esquerdo, clique em **[!UICONTROL Sistema]** > **[!UICONTROL [!DNL JumpSeat]Integração]**.
1. Insira seu **[!UICONTROL [!DNL JumpSeat]URL]**, que pode ser encontrado no ícone da sua extensão no [!DNL JumpSeat].

   **Exemplo:** [!DNL https]://{mycompanyname}.jumpseat.io

1. Insira o **[!UICONTROL [!DNL JumpSeat]token de integração]**. Você pode encontrar isso no **[!UICONTROL Configuração]** página em [!DNL JumpSeat].

   **Exemplo:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Clique em **[!UICONTROL Testar configuração]**.
1. Escolha se deseja que a integração seja **[!UICONTROL Ativo]** ou **[!UICONTROL Inativo]**.

   >[!IMPORTANT]
   >
   >O teste de configuração executado na etapa 5 deve ser aprovado para ativar a integração.

   ![Página de integração do JumpSeat](assets/jumpseat-integration-page.png)

1. Clique em **[!UICONTROL Salvar]**.

>[!TIP]
>
>Para obter mais informações sobre como configurar o [!DNL JumpSeat] integração, consulte a [!DNL JumpSeat] documentação para [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
