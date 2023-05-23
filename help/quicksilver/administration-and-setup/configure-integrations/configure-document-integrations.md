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
source-git-commit: 456c7b21835c96912e8974063f7797283dcb4e6d
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# Configurar integrações de documentos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como um [!DNL Adobe Workfront] administrador, você pode configurar integrações de documentos para gerenciar documentos no [!UICONTROL Workfront]. Você também pode configurar [!UICONTROL Workfront] de modo que os documentos sejam armazenados apenas em aplicativos de serviços [!UICONTROL Workfront] próprio. Para obter mais informações, consulte [Atualizar e vincular um documento do [!UICONTROL Workfront] para um provedor de nuvem externo](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Para permitir a comunicação aberta entre [!DNL Workfront Proof] e a variável [!DNL Workfront] lista de permissões servidores, talvez seja necessário adicionar determinados endereços IP ao seu arquivo. Para obter mais informações, consulte [Lista de permissões Configurar o arquivo de pesquisa do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

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
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Integrações compatíveis

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Você pode configurar as seguintes integrações para gerenciar documentos:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   Vincular provas de [!DNL Workfront Proof] permite fazer provas que foram criadas originalmente no [!DNL Workfront Proof] disponível em [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] É necessário um plano ou superior para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos do Workfront.](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   Para obter informações sobre a integração com o [!DNL SharePoint], consulte [Configure o [!DNL SharePoint] integração](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Provedores de documentos em nuvem de terceiros:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >É possível revisar e aprovar documentos vinculados de um provedor de nuvem externo da mesma maneira que você prova e aprova documentos carregados diretamente no [!DNL Workfront].

* Outros provedores de documentos (por meio de integrações de documentos personalizadas).

   A [!UICONTROL Pro] [!DNL Workfront] É necessário um plano ou superior para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [[!DNL Workfront] Planos.](https://www.workfront.com/plans)

Além disso, você pode aprimorar seus [!DNL Workfront] experiência documental com um sistema nativo de Gerenciamento de ativos digitais (DAM) ou com integrações de terceiros DAM. Os administradores devem habilitar esses recursos para que os usuários vinculem o serviço à [!DNL Workfront] conta. Para obter mais informações sobre o Workfront DAM, consulte [Gerenciar documentos com o [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configurar integrações para gerenciar documentos

1. Efetue logon no [!DNL Workfront] como administrador.
1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Provedores de nuvem].**

1. (Opcional) Para documentos armazenados em um aplicativo de serviços de documentos e não em [!DNL Workfront], selecione **[!UICONTROL Impedir que os usuários armazenem documentos no [!DNL Workfront]].**

1. Selecione as integrações que deseja ativar.
1. Clique em **[!UICONTROL Salvar]**.

Se você estiver configurando integrações com o [!DNL Workfront DAM], você pode ativar [!DNL Workfront] para incluir metadados com documentos. Para obter informações sobre o mapeamento de metadados, consulte [Configurar mapeamento de metadados](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurar integrações de documentos personalizadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Uma integração de documento personalizada permite [!DNL Workfront] usuários aos quais vincular arquivos [!DNL Workfront] qualquer sistema, desde que o sistema seja posto em funcionamento com o sistema [!DNL Workfront].

Para disponibilizar a integração personalizada para os usuários, primeiro é necessário criar a integração. Para obter informações sobre como criar integrações a serem usadas com o [!DNL Workfront], consulte [API de webhooks do documento](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Depois que a integração de documentos personalizada for criada, você poderá disponibilizá-la para os usuários do site.

1. Efetue logon no [!DNL Workfront] como administrador.
1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Integração personalizada].**

1. Clique em **[!UICONTROL Adicionar Integração personalizada]**.
1. Especifique as seguintes informações para configurar a integração:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>O nome da integração personalizada. Esse é o nome que os usuários veem ao usar a integração no Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL da API Base] </td> 
      <td>O HTTP básico ou o URL HTTP seguro para chamadas de API. Por exemplo, <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de Autenticação]</td> 
      <td> <p>O método de autenticação a ser usado ao fazer chamadas autorizadas para a API para a integração personalizada.</p> 
       <ul> 
        <li>Se você escolher <strong>[!UICONTROL OAuth]</strong>, continue com a Etapa 6.</li> 
        <li>Se você escolher <strong>[!UICONTROL ChaveAPI]</strong>, continue com a Etapa 7.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se você selecionou **[!UICONTROL OAuth]** autenticação para o **[!UICONTROL Tipo de autenticação]**, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de Autenticação]</td> 
      <td>O URL completo usado para autenticação do usuário. [!DNL Workfront] O navega os usuários para esse endereço como parte do processo de provisionamento do OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Token Endpoint URL]</td> 
      <td>O URL completo da API usado para recuperar tokens OAuth.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ID do Cliente]</td> 
      <td>A ID do cliente OAut para essa integração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Segredo do Cliente]</td> 
      <td>O segredo do cliente OAut para essa integração.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Parâmetros de Solicitação]</td> 
      <td> <p>Especifique valores opcionais a serem anexados à sequência de consulta de cada chamada de API. Por exemplo, access_type=offline.</p> <p>Para adicionar vários parâmetros de solicitação, clique em <strong>+Adicionar parâmetro de solicitação</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >A variável [!DNL Workfront] URI de redirecionamento exibido na parte inferior do [!UICONTROL Integração personalizada] A página lista o URI usado para registrar essa integração com o provedor de documentos externos.

1. (Condicional) Se você selecionou **[!UICONTROL ApiKey]** autenticação para o **[!UICONTROL Tipo de autenticação]**, especifique a chave de API emitida pelo provedor de documentos personalizados.

   [!DNL Workfront] O usa essa chave de API para fazer chamadas de API autorizadas para o provedor de documentos.

1. Clique em **[!UICONTROL Salvar]** para criar a integração.

## Usar integrações de documentos

Para obter informações sobre como os usuários podem usar o [!DNL Workfront DAM], consulte [Gerenciar documentos com o [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Para obter informações sobre como os usuários podem usar provas, consulte [Criar provas](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

Para obter informações sobre como os usuários podem usar integrações de documentos de terceiros depois de configurá-las, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurar [!DNL Workfront] para enviar metadados a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Ao enviar um documento do [!DNL Workfront] para [!DNL Workfront DAM], você também pode enviar informações associadas a esse documento. As informações sobre o documento estão mapeadas para [!DNL Workfront DAM] como metadados.

As informações são mapeadas apenas unidirecionalmente, de [!DNL Workfront] para [!DNL Workfront DAM] e é transferido somente quando o documento é carregado para [!DNL Workfront DAM]. Quaisquer alterações futuras nos campos do Workfront não atualizarão os campos de metadados no [!DNL Workfront DAM] após o documento já ter sido carregado.\
Você pode mapear o mesmo [!DNL Workfront] campo para vários [!DNL Workfront DAM] campos, mas não é possível usar os mesmos [!DNL Workfront DAM] campo para vários [!DNL Workfront] campos.

Se você precisar configurar vários [!DNL Workfront] campos a serem exportados para um [!DNL Workfront DAM] , crie primeiro um campo personalizado calculado em [!DNL Workfront] para exibir todos os campos personalizados individuais de um objeto. Em seguida, mapeie o calculado [!DNL Workfront] campo para um [!DNL Workfront DAM] campo.\
Para obter mais informações sobre campos personalizados calculados, consulte [Adicionar dados calculados a um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

O mapeamento afeta todos os documentos carregados por qualquer usuário do [!DNL Workfront] para [!UICONTROL Workfront] DAM.

Como um [!DNL Workfront] administrador, você deve habilitar [!DNL Workfront DAM] no Workfront antes de mapear os campos para o processo de mapeamento de metadados. Para obter mais informações sobre como habilitar [!DNL Workfront DAM], consulte [Configurar o Workfront para enviar metadados [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

Para configurar [!DNL Workfront] para enviar metadados a [!DNL Workfront DAM]:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Mapeamento de metadados]**.

1. No **[!UICONTROL Selecionar campo de origem para mapeamento]** comece digitando o nome do campo do Workfront para o qual deseja mapear [!DNL Workfront DAM]e, em seguida, selecione-o quando visualizá-lo na lista.
1. No **[!UICONTROL Selecionar campo de destino para mapeamento]**, selecione o [!DNL Workfront DAM] campo que você deseja preencher com as informações na variável [!DNL Workfront] campo.

   >[!NOTE]
   >
   > Todos os documentos enviados para o [!DNL Workfront DAM] por usuários que têm o direito de fazer isso tenham seus metadados atualizados com o [!DNL Workfront] campos mapeados aqui, quando são carregados para [!DNL Workfront DAM].

1. Clique em **[!UICONTROL Adicionar mapeamento]**.

1. Continuar adicionando mais [!UICONTROL Workfront] campos e correspondentes [!DNL Workfront DAM] campos.

### Excluir campos mapeados

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Expandir **[!UICONTROL Documentos]** e, em seguida, clique em **[!UICONTROL Mapeamento de metadados]**.

1. Na lista de campos, selecione qualquer um dos campos que deseja remover do mapeamento de metadados.
1. Clique em **[!UICONTROL Excluir]**.

   Os campos são removidos do mapeamento de metadados e as informações contidas neles não são transferidas para o [!DNL Workfront DAM] com os documentos carregados.
