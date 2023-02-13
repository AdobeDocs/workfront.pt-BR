---
title: Configurar integrações de documentos
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Configurar integrações de documentos
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# Configurar integrações de documentos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como um [!DNL Adobe Workfront] administrador, você pode configurar integrações de documentos para gerenciar documentos em [!UICONTROL Workfront]. Você também pode configurar [!UICONTROL Workfront] para que os documentos sejam armazenados apenas em aplicativos de serviços de documento e não em [!UICONTROL Workfront] próprio. Para obter mais informações, consulte [Atualizar e vincular um documento de [!UICONTROL Workfront] para um provedor de nuvem externo](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) em [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Para permitir a comunicação aberta entre [!DNL Workfront Proof] e [!DNL Workfront] pode ser necessário adicionar determinados endereços IP à sua lista de permissões. Para obter mais informações, consulte [Configurar a  lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

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
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Integrações compatíveis

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Você pode configurar as seguintes integrações para gerenciar documentos:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   Vincular provas de [!DNL Workfront Proof] O permite fazer provas que foram originalmente criadas em [!DNL Workfront Proof] disponível em [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] É necessário planejar ou superior para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos da Workfront.](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   Para obter informações sobre a integração com o [!DNL SharePoint], consulte [Configure o [!DNL SharePoint] integração](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Fornecedores de documentos em nuvem de terceiros:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >Você pode provar e aprovar documentos vinculados de um provedor de nuvem externo da mesma forma que prova e aprova documentos carregados diretamente no [!DNL Workfront].

* Outros provedores de documento (por meio de integrações de documento personalizadas).

   A [!UICONTROL Pro] [!DNL Workfront] É necessário planejar ou superior para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [[!DNL Workfront] Planos.](https://www.workfront.com/plans)

Além disso, você pode aprimorar o [!DNL Workfront] documentar a experiência com um sistema DAM (Digital Asset Management, gerenciamento de ativos digitais) nativo ou com integrações de DAM de terceiros. Os administradores devem ativar esses recursos para que os usuários vinculem o serviço aos seus [!DNL Workfront] conta. Para obter mais informações sobre o Workfront DAM, consulte [Gerenciar documentos com [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configurar integrações para gerenciar documentos

1. Faça logon em [!DNL Workfront] como administrador.
1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Provedores de nuvem].**

1. (Opcional) Para armazenar documentos em um aplicativo de serviços de documento e não em [!DNL Workfront], selecione **[!UICONTROL Impedir que os usuários armazenem documentos no [!DNL Workfront]].**

1. Selecione as integrações que deseja ativar.
1. Clique em **[!UICONTROL Salvar]**.

Se você estiver configurando integrações com o [!DNL Workfront DAM], você pode ativar [!DNL Workfront] para incluir metadados com documentos. Para obter informações sobre metadados de mapeamento, consulte [Configurar mapeamento de metadados](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurar integrações de documento personalizadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Uma integração de documento personalizado permite [!DNL Workfront] usuários para vincular arquivos em [!DNL Workfront] de praticamente qualquer sistema, desde que o sistema seja feito para funcionar com [!DNL Workfront].

Para disponibilizar a integração personalizada para os usuários, primeiro é necessário criar a integração . Para obter informações sobre como criar integrações a serem usadas com o [!DNL Workfront], consulte [API de Webhooks de documento](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Depois que a integração de documento personalizado for criada, você poderá disponibilizá-la para os usuários do seu site.

1. Faça logon em [!DNL Workfront] como administrador.
1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Integração personalizada].**

1. Clique em **[!UICONTROL Adicionar integração personalizada]**.
1. Especifique as seguintes informações para configurar a integração:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>O nome da integração personalizada. Esse é o nome que os usuários veem ao usar a integração no Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL da API base] </td> 
      <td>O URL HTTP básico ou seguro para chamadas de API. Por exemplo, <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de autenticação]</td> 
      <td> <p>O método de autenticação a ser usado ao fazer chamadas de API autorizadas para a integração personalizada.</p> 
       <ul> 
        <li>Se você escolher <strong>[!UICONTROL OAuth]</strong>, continue com a Etapa 6.</li> 
        <li>Se você escolher <strong>[!UICONTROL ApiKey]</strong>, continue com a Etapa 7.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se você selecionou **[!UICONTROL OAuth]** autenticação para a **[!UICONTROL Tipo de autenticação]**, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de autenticação]</td> 
      <td>O URL completo usado para autenticação de usuário. [!DNL Workfront] navega usuários para esse endereço como parte do processo de provisionamento do OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>O URL completo da API usado para recuperar tokens OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Client ID]</td> 
      <td>A ID do cliente OAut para essa integração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do cliente]</td> 
      <td>O Segredo do Cliente OAut para esta integração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parâmetros da solicitação]</td> 
      <td> <p>Especifique os valores opcionais a serem anexados à sequência de consulta de cada chamada de API. Por exemplo, access_type=offline.</p> <p>Para adicionar vários parâmetros de solicitação, clique em <strong>+Adicionar parâmetro de solicitação</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >O [!DNL Workfront] O URI de redirecionamento que é exibido na parte inferior do [!UICONTROL Integração personalizada] lista o URI usado para registrar essa integração no provedor de documentos externo.

1. (Condicional) Se você selecionou **[!UICONTROL ApiKey]** autenticação para a **[!UICONTROL Tipo de autenticação]**, especifique a chave da API emitida pelo provedor de documento personalizado.

   [!DNL Workfront] O usa essa chave de API para fazer chamadas de API autorizadas para o provedor de documentos.

1. Clique em **[!UICONTROL Salvar]** para criar a integração.

## Usar integrações de documentos

Para obter informações sobre como os usuários podem usar [!DNL Workfront DAM], consulte [Gerenciar documentos com [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Para obter informações sobre como os usuários podem usar provas, consulte [Criar provas](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

Para obter informações sobre como os usuários podem usar integrações de documentos de terceiros depois de configurá-las, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurar [!DNL Workfront] para enviar metadados para [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Ao enviar um documento de [!DNL Workfront] para [!DNL Workfront DAM], você também pode enviar informações associadas a esse documento. As informações sobre o documento estão mapeadas para [!DNL Workfront DAM] como metadados.

As informações são mapeadas apenas de uma maneira, de [!DNL Workfront] para [!DNL Workfront DAM] e é transferido somente quando o documento é carregado para o [!DNL Workfront DAM]. Quaisquer alterações futuras nos campos do Workfront não atualizarão os campos de metadados em [!DNL Workfront DAM] depois que o documento já tiver sido carregado.\
Você pode mapear o mesmo [!DNL Workfront] campo para vários [!DNL Workfront DAM] , mas não é possível usar os mesmos [!DNL Workfront DAM] campo para vários [!DNL Workfront] campos.

Se você precisar configurar vários [!DNL Workfront] campos para exportar para um [!DNL Workfront DAM] primeiro crie um campo personalizado calculado em [!DNL Workfront] para exibir todos os campos personalizados individuais de um objeto. Em seguida, mapeie o [!DNL Workfront] campo para um [!DNL Workfront DAM] campo.\
Para obter mais informações sobre campos personalizados calculados, consulte [Adicionar dados calculados a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

O mapeamento afeta todos os documentos carregados por qualquer usuário do [!DNL Workfront] para [!UICONTROL Workfront] DAM.

Como um [!DNL Workfront] administrador, você deve ativar [!DNL Workfront DAM] no Workfront antes de mapear os campos para o processo de mapeamento de metadados. Para obter mais informações sobre como ativar [!DNL Workfront DAM], consulte [Configure o Workfront para enviar metadados para o [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

Para configurar [!DNL Workfront] para enviar metadados para [!DNL Workfront DAM]:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Mapeamento de metadados]**.

1. No **[!UICONTROL Selecionar campo de origem para mapeamento]** , comece a digitar o nome do campo do Workfront para o qual deseja mapear [!DNL Workfront DAM]e, em seguida, selecione-o ao visualizá-lo na lista.
1. No **[!UICONTROL Selecionar campo de destino para mapeamento]**, selecione o [!DNL Workfront DAM] campo que você deseja preencher com as informações no campo selecionado [!DNL Workfront] campo.

   >[!NOTE]
   >
   > Todos os documentos enviados para [!DNL Workfront DAM] por usuários que têm os direitos de fazer isso, tenham seus metadados atualizados com a variável [!DNL Workfront] campos mapeados aqui, ao fazer upload para [!DNL Workfront DAM].

1. Clique em **[!UICONTROL Adicionar mapeamento]**.

1. Continue adicionando mais [!UICONTROL Workfront] campos e correspondentes [!DNL Workfront DAM] campos.

### Excluir campos mapeados

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Expandir **[!UICONTROL Documentos]**, depois clique em **[!UICONTROL Mapeamento de metadados]**.

1. Na lista de campos, selecione qualquer um dos campos que deseja remover do mapeamento de metadados.
1. Clique em **[!UICONTROL Excluir]**.

   Os campos são removidos do mapeamento de metadados e as informações neles contidas não são transferidas para [!DNL Workfront DAM] com os documentos carregados.
