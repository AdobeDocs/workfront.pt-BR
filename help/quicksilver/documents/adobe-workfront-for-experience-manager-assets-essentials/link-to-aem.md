---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Vincular conteúdo e pastas com o Supervisor de conteúdo viabilizado pelo Experience Manager Assets
description: Você pode usar o Supervisor de Conteúdo para vincular conteúdo ou pastas do Experience Manager Assets a qualquer objeto do Adobe Workfront que suporte documentos. O Content Advisor traz detecção inteligente e sensível ao contexto diretamente para o Workfront, ajudando você a encontrar rapidamente conteúdo relevante e aprovado.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 5%

---

# Vincular conteúdo e pastas ao Supervisor de conteúdo do Experience Manager Assets

O Content Advisor traz detecção inteligente e sensível ao contexto diretamente para o Workfront, ajudando você a encontrar rapidamente conteúdo relevante e aprovado com base no contexto. Com recursos como sugestões inteligentes, representações do Dynamic Media e metadados de ativos detalhados, ele permite avaliar e reutilizar o conteúdo com eficiência sem sair do Workfront, acelerando a criação de conteúdo e mantendo a consistência da marca.

Você pode usar o Supervisor de Conteúdo para vincular conteúdo e pastas do Experience Manager Assets ao Workfront. Depois de vinculado, é possível visualizar e gerenciar o conteúdo no Workfront, e quaisquer alterações feitas no conteúdo no Experience Manager Assets serão refletidas no Workfront.

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
   <td>Você deve ter o Experience Manager as a Cloud Service ou o Assets Essentials e deve ser adicionado ao produto como usuário na Admin Console.</td> 
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

* O administrador do Workfront deve configurar uma integração do Experience Manager. Para obter mais informações, consulte [Configurar a integração do Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

* Para usar as sugestões inteligentes ou a funcionalidade dos Resumos de campanha, você deve assinar uma GenAI Rider. Para obter mais informações, consulte [Usar o Supervisor de Conteúdo para acessar conteúdo do AEM em aplicativos do Adobe](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).



## Vincular conteúdo do Experience Manager Assets com o Supervisor de conteúdo

Agora você pode usar o Supervisor de Conteúdo para vincular conteúdo do Experience Manager Assets diretamente no Workfront. O Supervisor de conteúdo não está disponível para o Assets Essentials.

Para vincular conteúdo:

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Selecione **Adicionar novo** e depois selecione a integração do Experience Manager que o administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, talvez ele não mencione especificamente o Experience Manager Assets.

1. Com o Supervisor de conteúdo, você pode:


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Pesquise por ativos usando Pesquisas com IA.</strong> Use a pesquisa habilitada por IA que entenda o significado e a intenção por trás das consultas, oferecendo suporte a vários idiomas, erros de digitação e sinônimos.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">Pesquisa com IA para descoberta de ativos mais inteligente</a>.</td>
      </tr>
      <tr>
         <td><strong>Exiba sugestões inteligentes com base no contexto e na intenção.</strong> Descubra ativos que se alinham às suas necessidades de conteúdo usando as recomendações com reconhecimento de contexto do aplicativo host Adobe.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Sugestões inteligentes com base no contexto e na intenção</a>.</td>
      </tr>
      <tr>
         <td><strong>Carregue um resumo da campanha para descobrir ativos relevantes.</strong> Carregue um documento de resumo da campanha do PDF, DOCX ou TXT para que o Supervisor de Conteúdo possa analisá-lo e recomendar ativos relevantes.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Resumos da campanha para descobrir ativos relevantes</a>.</td>
      </tr>
      <tr>
         <td><strong>Exiba e selecione representações de ativos do Dynamic Media.</strong> Navegue por representações otimizadas por canal, incluindo predefinições de imagens, Recortes inteligentes e tipos de formato, e aplique modificadores do Dynamic Media para visualizar os ajustes em tempo real.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Representações de ativos do Dynamic Media disponíveis para uso</a>.</td>
      </tr>
      <tr>
         <td><strong>Aplicar modificadores do Dynamic Media a representações.</strong> Adicione modificadores para transformar representações de ativos em tempo real e visualize os resultados antes de selecionar uma representação para seu aplicativo host.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Representações de ativos do Dynamic Media disponíveis para uso</a>.</td>
      </tr>
      <tr>
         <td><strong>Descubra e procure os Fragmentos de conteúdo.</strong> Pesquise por fragmentos de conteúdo, visualize visualizações de miniaturas em tempo real, verifique o status (Rascunho, Modificado ou Publicado) e inspecione propriedades, referências e variações detalhadas.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Descoberta de fragmentos de conteúdo</a>.</td>
      </tr>
      <tr>
         <td><strong>Acessar metadados de ativos.</strong> Examine as propriedades do ativo, como título, descrição, formato, tamanho e outras guias de metadados (Produto, Campanha, Marcas) compatíveis com o modo de exibição do Assets.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Acessar metadados de ativos consistentes com a exibição do Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtre ativos usando filtros predefinidos.</strong> Refine os resultados do ativo usando filtros como Tipo de Arquivo, Formato de Arquivo, Status do Ativo, Tamanho do Arquivo, Largura da Imagem, Altura da Imagem, Data de Modificação e Data de Criação.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Acessar filtros consistentes com a exibição do Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Salve e reutilize pesquisas.</strong> Crie pesquisas salvas especificando um termo de pesquisa e opções de filtro, e depois reutilize-as no Experience Manager Assets e em outros aplicativos da Adobe.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Acessar e reutilizar pesquisas recentes e salvas</a>.</td>
      </tr>
      <tr>
         <td><strong>Pesquise por ativos nas coleções e dentro delas.</strong> Pesquise ativos ou coleções em todas as coleções ou limite a pesquisa a uma coleção específica.</td>
         <td>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Pesquisar ativos em e dentro de coleções</a>.</td>
      </tr>
   </tbody>
   </table>


### Vincular uma nova versão do Experience Manager Assets com o Supervisor de conteúdo

Você pode obter novo conteúdo do Experience Manager Assets ou do Assets Essentials e adicioná-lo a um ativo existente como uma nova versão. Se o documento já estiver vinculado e uma nova versão for adicionada ao Experience Manager Assets ou ao Assets Essentials, a nova versão será exibida automaticamente no Workfront.

Para vincular uma nova versão:

1. Vá para a área **Documentos** no Workfront onde deseja adicionar o documento.
1. Selecione o ativo que deseja substituir por uma nova versão. Não é possível criar uma nova versão de um ativo em uma pasta vinculada.
1. Selecione **Adicionar novo** > **Versão** e selecione a integração do Experience Manager que seu administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, talvez ele não mencione especificamente o Experience Manager Assets.

1. Selecione o conteúdo que deseja vincular:

   * Selecione a guia Assets para procurar ativos, pastas ou coleções no Experience Manager Assets ou no Assets Essentials.

     ![Consultor de conteúdo](assets/content-advisor-full.png)

   * Os fragmentos de conteúdo não são compatíveis com versões. Se você selecionar um fragmento de conteúdo, a nova versão substituirá o fragmento de conteúdo existente em vez de criar uma nova versão.

1. Clique em **Selecionar**.

## Vincular uma pasta do Experience Manager Assets com o Supervisor de conteúdo

As permissões para visualizar ativos individuais dentro de uma pasta dependem das permissões do Experience Manager Assets.

Para vincular uma pasta:

1. Vá para a área **Documentos** no Workfront onde deseja colocar a pasta.
1. Selecione **Adicionar novo** e depois selecione a integração do Experience Manager que o administrador configurou.

   >[!NOTE]
   >
   >O administrador do Workfront pode escolher qualquer nome para essa integração, portanto, talvez ele não mencione especificamente o Experience Manager Assets.

1. Clique em **Assets** > **Arquivos e pastas**.

1. Clique no ícone **Filtro** e, na seção **Tipo de ativo**, escolha **Pastas**.

1. Selecione a pasta que deseja vincular.

1. Clique em **Selecionar**.

## Considerações

* A funcionalidade Supervisor de conteúdo não está disponível para objetos que usam o Adobe Enterprise Storage. Se sua organização usar o Adobe Enterprise Storage, você ainda poderá vincular ativos e pastas do Experience Manager Assets ou do Assets Essentials, mas não terá acesso aos recursos do Supervisor de conteúdo, como Pesquisas com IA, sugestões inteligentes ou representações do Dynamic Media. Para obter mais informações, consulte [Usar o Adobe Experience Manager com a integração do Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* A funcionalidade Supervisor de conteúdo não está disponível para o Assets Essentials. Para vincular ativos e pastas do Assets Essentials, consulte [Vincular ativos e pastas do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md).

* Os campos de metadados são mapeados pela primeira vez quando você envia um ativo do Workfront para o Experience Manager Assets. Se o administrador do Workfront tiver ativado a sincronização de metadados de objeto, os campos permanecerão atualizados se forem alterados em qualquer um dos aplicativos.
