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
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 6%

---

# Configurar a integração do JumpSeat

É possível integrar o [!DNL JumpSeat] ao [!DNL Workfront] para criar orientação personalizada no produto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table>
  <tr>
   <td>Pacote do Adobe Workfront
   </td>
    <p>Workflow Ultimate</p>
   <td> <p>Prime ou Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Licenças do Adobe Workfront
   </td>
   <td>Standard
   <p>Plano</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>Produto
   </td>
   <td>Você deve ter um plano [!DNL JumpSeat] ativo.
   </td>
  </tr>
   <tr>
   <td>Configurações de nível de acesso
   </td>
   <td>Você deve ser um administrador [!DNL Workfront].
   </td>
  </tr>
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar, você deve

* Adicionar e ativar [!DNL Workfront] como um aplicativo em [!DNL JumpSeat]. Para obter mais informações, consulte [Como Adicionar Ou Excluir Um Aplicativo](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>Se você estiver na Experiência Unificada do Adobe, deverá usar a seguinte URL do Aplicativo: `.workfront.adobe.com`.



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

>>

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
