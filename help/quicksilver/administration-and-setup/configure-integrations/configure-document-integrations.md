---
title: Configurar integrações de documentos
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Como administrador do Adobe Workfront, você pode configurar integrações de documentos para gerenciar documentos no Workfront.
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 1%

---

# Configurar integrações de documentos

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador do [!DNL Adobe Workfront], você pode configurar integrações de documentos para gerenciar documentos no [!UICONTROL Workfront]. Você também pode configurar o [!UICONTROL Workfront] para que os documentos sejam armazenados somente em aplicativos de serviços de documentos e não no próprio [!UICONTROL Workfront]. Para obter mais informações, consulte [Atualizar e vincular um documento do [!UICONTROL Workfront] a um provedor de nuvem externo](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) em [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>Incluir na lista de permissões Para permitir a comunicação aberta entre os servidores do [!DNL Workfront Proof] e do [!DNL Workfront], talvez seja necessário adicionar determinados endereços IP ao seu arquivo. Incluir na lista de permissões Para obter mais informações, consulte [Configurar o arquivo do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

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
       <p>ou</p>
       <p>Atual: [!UICONTROL Plano]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integrações compatíveis

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Você pode configurar as seguintes integrações para gerenciar documentos:

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  Vincular provas de [!DNL Workfront Proof] permite que você disponibilize provas que foram criadas originalmente em [!DNL Workfront Proof] em [!DNL Workfront]. Para os planos atuais, é necessário um Plano [!UICONTROL Pro] [!DNL Workfront] ou superior para usar este recurso. Para os novos planos, esse recurso está disponível com todos os planos. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos do Workfront](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  Para obter informações sobre a integração com o [!DNL SharePoint], consulte [Configurar a [!DNL SharePoint] integração](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* Provedores de documentos em nuvem de terceiros:

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Unidade Google]

     <!--Quip-->

  >[!TIP]
  >
  >Você pode revisar e aprovar documentos vinculados de um provedor de nuvem externo da mesma forma que prova e aprova documentos carregados diretamente no [!DNL Workfront].

* Outros provedores de documentos (por meio de integrações de documentos personalizadas).

  Para os planos atuais, é necessário um Plano [!UICONTROL Pro] [!DNL Workfront] ou superior para usar este recurso. Para os novos planos, esse recurso está disponível com todos os planos. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos do Workfront](https://www.workfront.com/plans).

Além disso, você pode aprimorar sua experiência com documentos do [!DNL Workfront] com um sistema nativo de Gerenciamento de Ativos Digitais (DAM) ou com integrações de terceiros com o DAM. Os administradores devem habilitar esses recursos para que os usuários vinculem o serviço à sua conta [!DNL Workfront]. Para obter mais informações sobre o Workfront DAM, consulte [Gerenciando documentos com [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## Configurar integrações para gerenciar documentos

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Provedores de Nuvem].**

1. (Opcional) Para armazenar documentos em um aplicativo de serviços de documentos e não em [!DNL Workfront], selecione **[!UICONTROL Impedir Usuários de Armazenar Documentos em [!DNL Workfront]].**

1. Selecione as integrações que deseja ativar.
1. Clique em **[!UICONTROL Salvar]**.

Se você estiver configurando integrações com [!DNL Workfront DAM], é possível habilitar [!DNL Workfront] para incluir metadados com documentos. Para obter informações sobre metadados de mapeamento, consulte [Configurar mapeamento de metadados](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## Configurar integrações de documentos personalizadas

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

Uma integração de documentos personalizada permite que [!DNL Workfront] usuários vinculem arquivos ao [!DNL Workfront] de praticamente qualquer sistema, desde que o sistema tenha sido configurado para funcionar com [!DNL Workfront].

Para disponibilizar a integração personalizada para os usuários, primeiro é necessário criar a integração. Para obter informações sobre como criar integrações a serem usadas com o [!DNL Workfront], consulte a [API de Webhooks de Documentos](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

Depois que a integração de documentos personalizada for criada, você poderá disponibilizá-la para os usuários do site.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Documentos]** > **[!UICONTROL Integração personalizada]**.

1. Clique em **[!UICONTROL Adicionar integração personalizada]**.
1. Insira as seguintes informações para configurar a integração:

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
      <td>O HTTP básico ou o URL HTTP seguro para chamadas de API. Por exemplo, <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de Autenticação]</td> 
      <td> <p>O método de autenticação a ser usado ao fazer chamadas autorizadas para a API para a integração personalizada.</p> 
       <ul> 
        <li>Se você escolher <strong>[!UICONTROL OAuth]</strong>, continue com a Etapa 5.</li> 
        <li>Se você escolher <strong>[!UICONTROL ApiKey]</strong>, continue com a Etapa 6.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se você selecionou a autenticação **[!UICONTROL OAuth]** para o **[!UICONTROL Tipo de Autenticação]**, insira as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL de Autenticação]</td> 
      <td>O URL completo usado para autenticação do usuário. [!DNL Workfront] navega usuários para este endereço como parte do processo de provisionamento do OAuth.</td> 
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
      <td> <p>Insira valores opcionais a serem anexados à sequência de consulta de cada chamada de API. Por exemplo, access_type=offline.</p> <p>Para adicionar vários parâmetros de solicitação, clique em <strong>+Adicionar parâmetro de solicitação</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >O URI de Redirecionamento [!DNL Workfront] exibido na parte inferior da página [!UICONTROL Integração Personalizada] lista o URI usado para registrar essa integração com o provedor de documentos externos.

1. (Condicional) Se você selecionou a autenticação **[!UICONTROL ApiKey]** para o **[!UICONTROL Tipo de Autenticação]**, insira a chave de API emitida pelo provedor de documentos personalizados.

   [!DNL Workfront] usa essa chave de API para fazer chamadas de API autorizadas para o provedor de documentos.

1. Clique em **[!UICONTROL Salvar]** para criar a integração.

## Usar integrações de documentos

Para obter informações sobre como os usuários podem usar o [!DNL Workfront DAM], consulte [Gerenciando Documentos com o  [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

Para obter informações sobre como os usuários podem usar provas, consulte [Criar provas](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

Para obter informações sobre como os usuários podem usar integrações de documentos de terceiros após a configuração, consulte [Vincular documentos de aplicativos externos](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Configurar [!DNL Workfront] para enviar metadados a [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

Ao enviar um documento de [!DNL Workfront] para [!DNL Workfront DAM], você também pode enviar informações associadas a esse documento. As informações sobre o documento estão mapeadas para [!DNL Workfront DAM] como metadados.

As informações são mapeadas apenas unidirecionalmente, de [!DNL Workfront] a [!DNL Workfront DAM] e são transferidas apenas quando o documento é carregado para [!DNL Workfront DAM]. Quaisquer alterações futuras nos campos do Workfront não atualizarão os campos de metadados em [!DNL Workfront DAM] após o documento já ter sido carregado.\
Você pode mapear o mesmo campo [!DNL Workfront] para vários campos [!DNL Workfront DAM], mas não pode usar o mesmo campo [!DNL Workfront DAM] para vários campos [!DNL Workfront].

Se você precisar configurar vários campos [!DNL Workfront] para serem exportados para um campo [!DNL Workfront DAM], primeiro crie um campo personalizado calculado em [!DNL Workfront] para exibir todos os campos personalizados individuais de um objeto. Em seguida, mapeie o campo [!DNL Workfront] calculado para um campo [!DNL Workfront DAM].\
Para obter mais informações sobre campos personalizados calculados, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

O mapeamento afeta todos os documentos carregados por qualquer usuário do DAM [!DNL Workfront] para o [!UICONTROL Workfront].

Como administrador do [!DNL Workfront], você deve habilitar o [!DNL Workfront DAM] no Workfront antes de mapear os campos para o processo de mapeamento de metadados.

Para configurar [!DNL Workfront] para enviar metadados a [!DNL Workfront DAM]:

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Documentos]** > **[!UICONTROL Mapeamento de Metadados]**.

1. No campo **[!UICONTROL Selecionar campo do Source para mapeamento]**, comece digitando o nome do campo do Workfront para o qual deseja mapear [!DNL Workfront DAM] e selecione-o quando o vir na lista.
1. Em **[!UICONTROL Selecionar campo de destino para mapeamento]**, selecione o campo [!DNL Workfront DAM] que deseja preencher com as informações no campo [!DNL Workfront] selecionado.

   >[!NOTE]
   >
   > Todos os documentos enviados para [!DNL Workfront DAM] por usuários com direitos para isso terão seus metadados atualizados com os campos [!DNL Workfront] mapeados aqui, quando forem carregados para [!DNL Workfront DAM].

1. Clique em **[!UICONTROL Adicionar mapeamento]**.

1. Continue adicionando mais campos [!UICONTROL Workfront] e os campos [!DNL Workfront DAM] correspondentes.

### Excluir campos mapeados

{{step-1-to-setup}}

1. Expanda **[!UICONTROL Documentos]** e clique em **[!UICONTROL Mapeamento de Metadados]**.

1. Na lista de campos, selecione qualquer um dos campos que deseja remover do mapeamento de metadados.
1. Clique em **[!UICONTROL Excluir]**.

   Os campos são removidos do mapeamento de metadados e as informações contidas neles não são transferidas para [!DNL Workfront DAM] com os documentos carregados.
