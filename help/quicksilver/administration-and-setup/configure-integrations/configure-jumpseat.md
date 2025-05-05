---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Configurar a integração do JumpSeat
description: É possível integrar o [!DNL JumpSeat] com o [!DNL Workfront] para criar orientação personalizada no produto.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 01b7eb79028eb3fe47f988a31cb62ace31bba3f1
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 4%

---

# Configurar a integração do JumpSeat

É possível integrar o [!DNL JumpSeat] ao [!DNL Workfront] para criar orientação personalizada no produto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Empresa] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Você deve ter um plano [!DNL JumpSeat] ativo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p> Você deve ser um administrador [!DNL Workfront]. Para obter informações sobre administradores do [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

+++

## Pré-requisitos

Antes de começar, você deve

* Adicionar e ativar [!DNL Workfront] como um aplicativo em [!DNL JumpSeat]. Para obter mais informações, consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>Se você estiver no Adobe Unified Experience, deverá usar a seguinte URL do Aplicativo: `.workfront.adobe.com`.



## Configurar a integração do [!DNL JumpSeat]

Recomendamos configurar uma integração do [!DNL JumpSeat] nos ambientes de Pré-visualização e Produção.

>[!TIP]
>
>Você precisa adicionar e ativar dois aplicativos separados do [!DNL Workfront] no [!DNL JumpSeat], um para Pré-visualização e outro para Produção. Consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/) para obter mais informações.

Para configurar a integração do [!DNL JumpSeat]:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Sistema]** > **[!UICONTROL [!DNL JumpSeat]Integração]**.
1. Insira a URL **[!UICONTROL [!DNL JumpSeat]]**, que pode ser encontrada no ícone da sua extensão em [!DNL JumpSeat].

>[!BEGINSHADEBOX]

**Exemplo:**

https://{mycompanyname}.jumpseat.io

&#x200B;>>

>[!ENDSHADEBOX]

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
