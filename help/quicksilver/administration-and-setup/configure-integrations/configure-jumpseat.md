---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurar a integração do JumpSeat
description: É possível integrar [!DNL JumpSeat] com [!DNL Workfront] para criar orientação personalizada no produto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# Configurar a integração do JumpSeat

É possível integrar [!DNL JumpSeat] com [!DNL Workfront] para criar orientação personalizada no produto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Produto</strong></td> 
   <td>Você deve ter um [!DNL JumpSeat] plano.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p> Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Antes de começar, você deve

* Adicionar e ativar [!DNL Workfront] como um pedido de [!DNL JumpSeat]. Para obter mais informações, consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configure o [!DNL JumpSeat] integração

Recomendamos configurar um [!DNL JumpSeat] integração em seus ambientes de Visualização e Produção.

>[!TIP]
>
>Você precisa adicionar e ativar dois [!DNL Workfront] de [!DNL JumpSeat]—um para Pré-visualização e outro para Produção. Consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/) para obter mais informações.

Para configurar o [!DNL JumpSeat] integração:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]**.
1. No painel esquerdo, clique em **[!UICONTROL Sistema]** > **[!UICONTROL [!DNL JumpSeat]Integração]**.
1. Insira seu **[!UICONTROL [!DNL JumpSeat]URL]**.

   **Exemplo:** [!DNL https]://{mycompanyname}.jumpsat.io

1. Insira o **[!UICONTROL [!DNL JumpSeat]token de integração]**. Você pode encontrar isso no **[!UICONTROL Configuração]** em [!DNL JumpSeat].

   **Exemplo:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Clique em **[!UICONTROL Testar configuração]**.
1. Escolha se deseja que a integração seja **[!UICONTROL Ativo]** ou **[!UICONTROL Inativo]**.

   >[!IMPORTANT]
   >
   >O teste de configuração executado na etapa 5 deve ser bem-sucedido para ativar a integração.

   ![Página Integração do JumpSeat](assets/jumpseat-integration-page.png)

1. Clique em **[!UICONTROL Salvar]**.
