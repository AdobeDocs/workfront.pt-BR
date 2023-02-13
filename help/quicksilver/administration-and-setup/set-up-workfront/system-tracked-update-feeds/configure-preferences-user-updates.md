---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar preferências para atualizações do usuário
description: É possível configurar preferências que acessam determinados recursos quando usuários adicionam comentários em um objeto [!UICONTROL Atualizações] área.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Configurar preferências para atualizações do usuário

É possível configurar preferências que dão aos usuários acesso a determinados recursos ao adicionar comentários em um objeto [!UICONTROL Atualizações] área.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, é necessário o nível de acesso [!UICONTROL System Administrator].</p><p>Para executá-los para um grupo, você deve ser um gerente desse grupo.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Permitir que usuários adicionem imagens em atualizações

Por padrão, os usuários não podem adicionar imagens em atualizações. Ao ativar essa preferência, os usuários poderão anexar imagens em atualizações. A preferência se aplica a todas as atualizações em todas as áreas de sua [!DNL Workfront] instância.

>[!NOTE]
>
>* As imagens salvas em atualizações contam no limite de armazenamento de documentos. Para obter mais informações, consulte [Verificar limites de armazenamento do documento](../../../documents/managing-documents/check-document-storage.md).
>* As imagens só podem ser acessadas por meio da variável [!UICONTROL Atualizações] em um objeto e não estão disponíveis na variável [!UICONTROL Documentos] guia .
>




1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, selecione **[!UICONTROL Interface]** > **[!UICONTROL Atualizar feeds]**.
1. Selecione o **[!UICONTROL Preferências]** guia .

   ![Preferências do usuário para feeds de atualização](assets/updatefeeds-preferences-350x137.png)

1. Selecione o **[!UICONTROL Permitir que usuários adicionem imagens em atualizações]** caixa de seleção.
1. Selecionar **[!UICONTROL Salvar]**.

   Quando essa preferência estiver ativada, você pode desativá-la a qualquer momento. Todas as imagens já publicadas nas atualizações permanecerão no [!UICONTROL Atualizações] no objeto.
