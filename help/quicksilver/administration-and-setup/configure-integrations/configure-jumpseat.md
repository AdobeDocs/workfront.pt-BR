---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurar a integração do JumpSeat
description: É possível integrar o [!DNL JumpSeat] com o [!DNL Workfront] para criar orientação personalizada no produto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Configurar a integração do JumpSeat

É possível integrar o [!DNL JumpSeat] ao [!DNL Workfront] para criar orientação personalizada no produto.

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
   <td>Você deve ter um plano [!DNL JumpSeat] ativo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p> Você deve ser um administrador [!DNL Workfront]. Para obter informações sobre administradores do [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

Antes de começar, você deve

* Adicionar e ativar [!DNL Workfront] como um aplicativo em [!DNL JumpSeat]. Para obter mais informações, consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/).

## Configurar a integração do [!DNL JumpSeat]

Recomendamos configurar uma integração do [!DNL JumpSeat] nos ambientes de Pré-visualização e Produção.

>[!TIP]
>
>Você precisa adicionar e ativar dois aplicativos separados do [!DNL Workfront] no [!DNL JumpSeat], um para Pré-visualização e outro para Produção. Consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/) para obter mais informações.

Para configurar a integração do [!DNL JumpSeat]:

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Instalação]**.
1. No painel esquerdo, clique em **[!UICONTROL Sistema]** > **[!UICONTROL [!DNL JumpSeat]Integração]**.
1. Insira a URL **[!UICONTROL [!DNL JumpSeat]]**, que pode ser encontrada no ícone da sua extensão em [!DNL JumpSeat].

   **Exemplo:** [!DNL https]://{mycompanyname}.jumpseat.io

1. Insira o token de integração **[!UICONTROL [!DNL JumpSeat]]**. Você pode encontrar isso na página **[!UICONTROL Configuração]** em [!DNL JumpSeat].

   **Exemplo:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Clique em **[!UICONTROL Testar configuração]**.
1. Escolha se deseja que a integração seja **[!UICONTROL Ativa]** ou **[!UICONTROL Inativa]**.

   >[!IMPORTANT]
   >
   >O teste de configuração executado na etapa 5 deve ser aprovado para ativar a integração.

   ![Página de integração do JumpSeat](assets/jumpseat-integration-page.png)

1. Clique em **[!UICONTROL Salvar]**.

>[!TIP]
>
>Para obter mais informações sobre como configurar a integração do [!DNL JumpSeat], consulte a documentação do [!DNL JumpSeat] para o [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
