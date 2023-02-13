---
title: Configurar mapeamento de metadados
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Os metadados são informações descritivas associadas a um documento. Você pode configurar [!DNL Adobe Workfront] para incluir metadados com documentos enviados para [!DNL Workfront] aplicativos.
author: Caroline
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 7cf4787d-7cff-489e-bd5b-69db3ff09f6e
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Configurar mapeamento de metadados

Os metadados são informações descritivas associadas a um documento. Você pode configurar [!DNL Adobe Workfront] para incluir metadados com documentos enviados para [!DNL Workfront] aplicativos.

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
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sobre [!DNL Workfront] metadados

Metadados para documentos em [!DNL Workfront] pode incluir informações como o nome do projeto relacionado, a descrição da tarefa ou a Data de Conclusão Planejada. Como um [!DNL Workfront] administrador, você pode configurar [!DNL Workfront] para incluir metadados com documentos enviados de [!DNL Workfront] para [!DNL Workfront] Aplicativos:

* [!DNL Workfront DAM]

Para que os metadados possam ser enviados com documentos, você deve primeiro especificar ou mapear os metadados que deseja incluir. Você pode mapear qualquer campo usado em [!DNL Workfront]. Depois de configurar o mapeamento de metadados, todos os documentos carregados em um [!DNL Workfront] o aplicativo incluirá os metadados mapeados.

Quando um usuário envia um documento de [!DNL Workfront] para [!DNL Workfront] , os metadados mapeados são transferidos ao longo do documento. Enquanto a versão do documento na [!DNL Workfront] o aplicativo está vinculado a [!DNL Workfront], alterações feitas nos metadados do documento em [!DNL Workfront] não são refletidas nos metadados do documento no [!DNL Workfront] aplicativo. Se um campo mapeado em [!DNL Workfront] for alterado, você deverá enviar uma nova versão do documento com os metadados atualizados para o [!DNL Workfront] aplicativo.

>[!NOTE]
>
>Você pode mapear metadados somente em uma direção: from [!DNL Workfront] para [!DNL Workfront DAM]. Metadados para documentos vinculados a [!DNL Workfront] from [!DNL Workfront DAM] não pode ser transferido para o Workfront.

Você pode mapear o mesmo [!DNL Workfront] para vários campos de metadados em [!DNL Workfront DAM], mas não é possível usar um campo de metadados em nenhum desses aplicativos para vários [!DNL Workfront] campos de metadados.

Para configurar vários [!DNL Workfront] campos a serem exportados para um campo de metadados em uma [!DNL Workfront] primeiro crie um campo personalizado calculado em [!DNL Workfront] para exibir todos os campos personalizados individuais de um objeto. Em seguida, mapeie o [!DNL Workfront] para um campo de metadados na [!DNL Workfront] aplicativo. Para obter mais informações sobre campos personalizados calculados, consulte [Adicionar dados calculados a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Antes de mapear campos para o processo de mapeamento de metadados, você deve habilitar o aplicativo em [!DNL Workfront]. Para obter mais informações, consulte [Configurar integrações de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configurar [!DNL Workfront] para enviar metadados

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Mapeamento de metadados]**.

   ![](assets/metadata-mapping.png)

1. No **[!UICONTROL Selecionar campo de origem para mapeamento]** , comece a digitar o nome do campo do Workfront para o qual deseja mapear [!DNL Workfront DAM]e, em seguida, selecione-o ao visualizá-lo na lista.
1. No **[!UICONTROL Selecionar campo de destino para mapeamento]** , selecione o campo que deseja preencher com as informações no campo selecionado [!DNL Workfront] campo.

1. Clique em **[!UICONTROL Adicionar mapeamento]**.

   O campo mapeado é exibido nos campos mapeados listados na parte inferior da página.

1. Repita as Etapas 5 e 6 até adicionar todas as etapas desejadas [!DNL Workfront] campos e seus correspondentes [!DNL Workfront DAM] campos.

## Excluir campos mapeados

1. Faça logon em [!DNL Workfront] como administrador.
1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Mapeamento de metadados]**.

1. Na lista de campos mapeados, selecione os campos que deseja remover do mapeamento de metadados.
1. Clique em **[!UICONTROL Excluir]**.

   Os campos designados não são mais mapeados. Agora, quando um usuário envia um documento de [!DNL Workfront] para [!DNL Workfront DAM], os metadados contidos nos campos excluídos não são transferidos com o documento.

   Um documento enviado antes da exclusão dos campos mapeados retém os metadados originais enviados com ele, incluindo os metadados dos campos excluídos.
