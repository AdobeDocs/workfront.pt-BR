---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar preferências para atualizações de usuário
description: Você pode configurar preferências que acessam determinados recursos quando os usuários adicionam comentários na área [!UICONTROL Atualizações] de um objeto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 1%

---

# Configurar preferências para atualizações de usuário

Você pode configurar preferências que dão aos usuários acesso a determinados recursos ao adicionar comentários na área [!UICONTROL Atualizações] de um objeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
   Ou
   <p>Atual: [!UICONTROL Plano]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td><p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso [!UICONTROL Administrador do Sistema].</p><p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p></td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Permitir que usuários adicionem imagens em atualizações

Por padrão, os usuários não podem adicionar imagens em atualizações. Quando você habilita essa preferência, os usuários podem anexar imagens em atualizações. A preferência se aplica a todas as atualizações em todas as áreas da instância [!DNL Workfront].

>[!NOTE]
>
>* As imagens salvas em atualizações são contadas de acordo com o limite de armazenamento de documentos. Para obter informações, consulte [Verificar limites de armazenamento de documentos](../../../documents/managing-documents/check-document-storage.md).
>* As imagens podem ser acessadas por meio da guia [!UICONTROL Atualizações] em um objeto e também estão disponíveis na área [!UICONTROL Documentos] no [!UICONTROL Menu Principal].
>

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, selecione **[!UICONTROL Interface]** > **[!UICONTROL Feeds de Atualização]**.
1. Selecione a guia **[!UICONTROL Preferências]**.

   ![Preferências do usuário para feeds de atualização](assets/updatefeeds-preferences-350x137.png)

1. Marque a caixa de seleção **[!UICONTROL Permitir que usuários adicionem imagens em atualizações]**.
1. Selecione **[!UICONTROL Salvar]**.

   Quando esta preferência estiver ativada, você poderá desativá-la a qualquer momento. As imagens já postadas nas atualizações permanecerão na área [!UICONTROL Atualizações] do objeto.
