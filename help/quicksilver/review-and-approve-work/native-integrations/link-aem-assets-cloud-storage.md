---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: Vincular conteúdo e pastas do Experience Manager Assets com o Adobe Cloud Storage
description: Se sua organização usar o armazenamento em nuvem da Adobe, você poderá vincular conteúdo e pastas do Experience Manager Assets a qualquer objeto do Adobe Workfront que ofereça suporte a documentos.
author: Courtney
source-git-commit: 66635b2edc78833ec2d08cef382b39b89238b565
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 7%

---

# Vincular conteúdo e pastas do Experience Manager Assets com o Adobe Cloud Storage

Se sua organização usar o Adobe Cloud Storage, você poderá vincular conteúdo e pastas do Experience Manager Assets ao Workfront. Depois de vinculado, é possível visualizar e gerenciar o conteúdo no Workfront, e quaisquer alterações feitas no conteúdo no Experience Manager Assets serão refletidas no Workfront.

>[!IMPORTANT]
>
>Se sua organização recusar assinar o contrato GenAI Rider, você ainda poderá usar o Supervisor de conteúdo para escolher ativos e pastas no Experience Manager Assets, mas não terá acesso a recursos alimentados por IA, como Pesquisas com IA, sugestões inteligentes ou a análise de resumos de campanha.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou posterior</p> 
   <p>Solicitação ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service e ser adicionado ao produto como um usuário no Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permissões do Experience Manager</td> 
    <td>Você deve ter acesso de gravação à pasta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar:

* O administrador do Workfront deve configurar uma integração do Experience Manager. Para obter mais informações, consulte [Usar o Adobe Experience Manager com a integração do Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* Para usar as sugestões inteligentes ou a funcionalidade dos Resumos de campanha, você deve assinar uma GenAI Rider. Para obter mais informações, consulte [Usar o Supervisor de Conteúdo para acessar conteúdo do AEM em aplicativos do Adobe](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).

## Vincular conteúdo do Experience Manager Assets

Para vincular conteúdo:

1. Vá para o objeto do Workfront ao qual deseja vincular conteúdo.
1. Clique na seção **Documentos** no painel esquerdo.
1. Clique em **Novo** no lado direito da página e em **Arquivos do AEM** para vincular um ativo individual.
   ![Adicionar arquivos AEM à área de documentos](assets/aem-files.png)

1. Com o Supervisor de conteúdo, você pode:

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Pesquisar ativos usando Pesquisas com IA.</strong> Use a pesquisa baseada em IA que entende o significado e a intenção por trás das consultas, oferecendo suporte a vários idiomas, erros de digitação e sinônimos.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">Pesquisa com IA para descoberta de ativos mais inteligente</a>.</td>
      </tr>
      <tr>
         <td><strong>Exibir sugestões inteligentes com base no contexto e na intenção.</strong> Descubra ativos que se alinham às suas necessidades de conteúdo usando as recomendações com reconhecimento de contexto do aplicativo host do Adobe.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Sugestões inteligentes com base no contexto e na intenção</a>.</td>
      </tr>
      <tr>
         <td><strong>Carregue um resumo da campanha para descobrir ativos relevantes.</strong> Faça upload de um documento de resumo da campanha PDF, DOCX ou TXT para que o Supervisor de conteúdo possa analisá-lo e recomendar ativos relevantes.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Resumos da campanha para descobrir ativos relevantes</a>.</td>
      </tr>
      <tr>
         <td><strong>Exiba e selecione representações de ativos do Dynamic Media.</strong> Navegue por representações otimizadas por canal, incluindo predefinições de imagens, Recortes inteligentes e tipos de formato, e aplique modificadores do Dynamic Media para visualizar os ajustes em tempo real.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Representações de ativos do Dynamic Media disponíveis para uso</a>.</td>
      </tr>
      <tr>
         <td><strong>Aplicar modificadores do Dynamic Media a representações.</strong> Adicione modificadores para transformar representações de ativos em tempo real e visualizar os resultados antes de selecionar uma representação para seu aplicativo de host.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Representações de ativos do Dynamic Media disponíveis para uso</a>.</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong>Acessar metadados de ativos.</strong> Revise as propriedades do ativo, como título, descrição, formato, tamanho e outras guias de metadados (Produto, Campanha, Tags) consistentes com a exibição do Assets.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Acessar metadados de ativos consistentes com a exibição do Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtrar ativos usando filtros predefinidos.</strong> Refine os resultados do ativo usando filtros como Tipo de arquivo, Formato de arquivo, Status do ativo, Tamanho do arquivo, Largura da imagem, Altura da imagem, Data de modificação e Data de criação.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Acessar filtros consistentes com a exibição do Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Salvar e reutilizar pesquisas.</strong> Crie pesquisas salvas especificando um termo de pesquisa e opções de filtro, depois reutilize-as no Experience Manager Assets e em outros aplicativos da Adobe.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Acessar e reutilizar pesquisas recentes e salvas</a>.</td>
      </tr>
      <tr>
         <td><strong>Pesquisar ativos entre e dentro de coleções.</strong> Pesquise ativos ou coleções em todas as coleções ou limite a pesquisa a uma coleção específica.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Pesquisar ativos em e dentro de coleções</a>.</td>
      </tr>
   </tbody>
   </table>

   >[!NOTE]
   >
   >O Conteúdo recomendado no Supervisor de Conteúdo usa dados dos itens a seguir para determinar o conteúdo sugerido no Workfront:
   >
   >* Campos de nome e descrição do objeto do Workfront
   >* Campos de formulário personalizados marcados como obrigatórios
   >* Dados de documentos anexados

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## Considerações

* Os fluxos de trabalho de revisão e aprovação não são compatíveis com ativos vinculados do AEM.
* Os campos de metadados são mapeados pela primeira vez quando você envia um ativo do Workfront para o Experience Manager Assets. Se o administrador do Workfront tiver ativado a sincronização de metadados de objeto, os campos permanecerão atualizados se forem alterados em qualquer um dos aplicativos.
