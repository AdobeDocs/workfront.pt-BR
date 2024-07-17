---
title: Configurar o mapeamento de metadados
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
source-wordcount: '616'
ht-degree: 1%

---

# Configurar o mapeamento de metadados

Os metadados são informações descritivas associadas a um documento. Você pode configurar o [!DNL Adobe Workfront] para incluir metadados com documentos enviados para aplicativos do [!DNL Workfront].

## Requisitos de acesso

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
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront]. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sobre [!DNL Workfront] metadados

Os metadados para documentos em [!DNL Workfront] podem incluir informações como nome do projeto relacionado, descrição da tarefa ou Data de Conclusão Planejada. Como administrador do [!DNL Workfront], você pode configurar o [!DNL Workfront] para incluir metadados com documentos enviados de [!DNL Workfront] para os seguintes aplicativos [!DNL Workfront]:

* [!DNL Workfront DAM]

Antes que os metadados possam ser enviados com documentos, você deve primeiro especificar ou mapear os metadados que deseja incluir. Você pode mapear qualquer campo usado em [!DNL Workfront]. Depois de configurar o mapeamento de metadados, todos os documentos carregados em um aplicativo [!DNL Workfront] incluirão os metadados mapeados.

Quando um usuário envia um documento de [!DNL Workfront] para um aplicativo [!DNL Workfront], os metadados mapeados são transferidos ao longo do documento. Embora a versão do documento no aplicativo [!DNL Workfront] esteja vinculada a [!DNL Workfront], as alterações feitas nos metadados do documento em [!DNL Workfront] não são refletidas nos metadados do documento no aplicativo [!DNL Workfront]. Se um campo mapeado em [!DNL Workfront] for alterado, você deverá enviar uma nova versão do documento com os metadados atualizados para o aplicativo [!DNL Workfront].

>[!NOTE]
>
>Você pode mapear metadados somente em uma direção: de [!DNL Workfront] a [!DNL Workfront DAM]. Os metadados de documentos vinculados a [!DNL Workfront] a partir de [!DNL Workfront DAM] não podem ser transferidos para o Workfront.

Você pode mapear o mesmo campo [!DNL Workfront] para vários campos de metadados em [!DNL Workfront DAM], mas não pode usar um campo de metadados em nenhum desses aplicativos para vários campos de metadados [!DNL Workfront].

Para configurar vários campos [!DNL Workfront] para serem exportados para um campo de metadados em um aplicativo [!DNL Workfront], primeiro crie um campo personalizado calculado em [!DNL Workfront] para exibir todos os campos personalizados individuais de um objeto. Em seguida, mapeie o campo [!DNL Workfront] calculado para um campo de metadados no aplicativo [!DNL Workfront]. Para obter mais informações sobre campos personalizados calculados, consulte [Adicionar dados calculados a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

Antes de mapear campos para o processo de mapeamento de metadados, você deve habilitar o aplicativo em [!DNL Workfront]. Para obter mais informações, consulte [Configurar integrações de documentos](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## Configurar [!DNL Workfront] para enviar metadados

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Mapeamento de Metadados]**.

   ![](assets/metadata-mapping.png)

1. Na caixa **[!UICONTROL Selecionar campo do Source para mapeamento]**, comece a digitar o nome do campo do Workfront para o qual deseja mapear [!DNL Workfront DAM] e selecione-o ao vê-lo na lista.
1. Na caixa **[!UICONTROL Selecionar campo de destino para mapeamento]**, selecione o campo que deseja preencher com as informações no campo [!DNL Workfront] selecionado.

1. Clique em **[!UICONTROL Adicionar mapeamento]**.

   O campo mapeado é exibido nos campos mapeados listados na parte inferior da página.

1. Repita as etapas 5 e 6 até adicionar todos os campos [!DNL Workfront] desejados e seus campos [!DNL Workfront DAM] correspondentes.

## Excluir campos mapeados

1. Faça logon em [!DNL Workfront] como administrador.
1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Mapeamento de Metadados]**.

1. Na lista de campos mapeados, selecione os campos que deseja remover do mapeamento de metadados.
1. Clique em **[!UICONTROL Excluir]**.

   Os campos designados não são mais mapeados. Agora, quando um usuário envia um documento de [!DNL Workfront] para [!DNL Workfront DAM], os metadados contidos nos campos excluídos não são transferidos com o documento.

   Um documento enviado antes da exclusão dos campos mapeados retém os metadados originais enviados com ele, incluindo os metadados dos campos excluídos.
