---
title: Criar registros
description: Ao usar o Adobe Workfront Planning, um registro é uma instância de um tipo de registro. Você pode criar registros exclusivos para cada tipo de registro no Workfront Planning adicionando-os manualmente à exibição de tabela, importando-os de uma lista, duplicando-os ou criando-os conforme você os conecta a outros registros.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '1450'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Criar registros

{{planning-important-intro}}

No Adobe Workfront Planning, um registro é uma instância de um tipo de registro.

Você pode criar registros seguindo um destes procedimentos:

* Adicionar registros da página de tipo de registro na exibição de tabela
* Copiar e colar uma lista de registros de uma lista externa
* Duplicar registros de uma exibição de tabela
* Criar registros ao conectá-los a partir de outros registros
* Crie-os enviando um formulário de solicitação para um tipo de registro

Este artigo descreve como criar registros.

Para obter informações sobre o gerenciamento de registros nas exibições de tabela ou linha do tempo, consulte os seguintes artigos:

* [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Gerenciar a exibição de linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

Para acessar o Workfront Planning, é necessário ter o seguinte:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Plano de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, consulte <a href="https://business.adobe.com/products/workfront/pricing.html">Preços e pacotes do Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td> Padrão
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p> 
   <p>Edite o acesso no Workfront para os tipos de objeto que deseja criar (projetos e portfólios) à medida que os registros são conectados a eles. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Gerencie permissões no espaço de trabalho ao qual deseja adicionar registros. </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   <p>Gerencie permissões para objetos do Workfront (portfólios) para adicionar objetos secundários (projetos).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD info: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p>  
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements for Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++

## Criar registros adicionando-os a um tipo de registro em uma tabela de tipo de registro

Você pode criar registros na exibição de tabela de uma página do tipo de registro.

Para obter informações sobre como editar informações de registro, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.
Todos os registros do tipo selecionado são exibidos na visualização.

1. (Condicional) Dependendo da exibição exibida, siga um destes procedimentos:

   * Na exibição de tabela:

      * Clique em **Novo registro** na última linha da tabela

      * Clique em **Shift + Enter** no teclado a partir de qualquer coluna ou linha da tabela. Isso adiciona uma linha vazia sob o registro do qual você começa.
      * Passe o mouse sobre o campo principal de um registro, clique no menu **Mais** ![](assets/more-menu.png) à direita do campo e clique em **Inserir registro acima** ou **Inserir registro abaixo**.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * Em qualquer modo de exibição:

      * Clique em **Novo registro** no canto superior direito da página. A caixa de visualização do registro é aberta.

     O Workfront faz o upload de uma miniatura e de uma imagem de capa automaticamente para cada novo registro. Posteriormente, você poderá modificar essas imagens. Para obter informações, consulte os seguintes artigos:

      * [Adicionar uma imagem da capa a um registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Comece digitando informações sobre o novo registro nos campos que você vê na caixa de visualização.

   >[!NOTE]
   >
   >  * Não há campos obrigatórios para registros. No entanto, recomendamos adicionar informações para o campo principal de um registro, pois é útil identificar registros ao vincular registros uns aos outros. Para obter mais informações sobre campos primários, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md) e [Visão geral do campo primário](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Os campos que se referem a outros tipos de registro ou campos calculados são campos somente leitura.

1. (Condicional) Ao adicionar registros à tabela, continue adicionando informações em cada linha e clique em **Inserir** no teclado para salvar as alterações.

   Ou

   Clique no nome do novo registro ou no ícone ![](assets/open-details-icon-in-table-name-field.png) de **Abrir detalhes** à esquerda do nome do registro. Uma visualização com as informações detalhadas do registro é aberta na tabela.

   >[!TIP]
   >
   >Você pode acessar o ícone **Abrir Detalhes** somente a partir do campo de nome do registro quando o campo Nome for um campo primário.

1. Iniciar edição das informações do registro na visualização do registro. O Workfront salva suas alterações automaticamente.
1. (Opcional) Clique no ícone ![](assets/open-details-in-a-new-tab-icon.png) de **Abrir em nova guia** no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia. Continuar editando o registro na página de registro. Para obter informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

1. (Opcional) Use os seguintes atalhos de teclado para desfazer ou refazer a adição de novos registros ou suas informações ao adicioná-los na exibição de tabela:

   * CTRL + Z (⌘ + Z para Mac) para desfazer uma alteração
   * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer uma alteração

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## Criar registros copiando e colando-os de uma lista externa

1. Comece a criar registros na exibição Tabela, conforme descrito na seção [Criar registros adicionando-os manualmente a um tipo de registro](#create-records-by-manually-adding-them-to-a-record-type) neste artigo.

   Certifique-se de que a exibição de tabela tenha as colunas (ou os campos) que você deseja preencher com as novas informações de registro.

1. Clique em **Novo &lt; Nome do tipo de registro >** na última linha da tabela para adicionar quantas linhas novas à tabela você desejar que seus novos registros sejam.

   Por exemplo, adicione 10 linhas à exibição de tabela se desejar colar as informações de 10 novos registros de outro aplicativo.

1. Em outro aplicativo, crie uma lista de registros que deseja importar.

   Por exemplo, você pode usar uma planilha do Excel para criar sua lista.

   A lista deve conter informações em formato de tabela.

   >[!TIP]
   >
   > As colunas da lista devem conter informações para os campos existentes no Workfront.
   >
   > Certifique-se de que você tenha os campos desejados já criados no Workfront e que as informações na sua planilha sejam exibidas no formato correto que corresponda ao de cada campo no Workfront.

1. Em outro aplicativo, selecione várias linhas e colunas e cole as informações na exibição de tabela do tipo de registro, começando com o primeiro novo registro.

   As informações a seguir são importadas na área do Workfront Planning:

   * As linhas contêm os novos registros
   * As colunas preenchem informações para os campos dos registros.

## Criar registros duplicando-os

Para obter informações sobre duplicação de registros, consulte [Duplicar registros](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

## Criar registros ao conectá-los

É possível criar registros ou objetos Workfront ao conectá-los a partir de outros registros.

Você deve ter as seguintes opções antes de adicionar novos registros ou objetos do Workfront, conectando-os a partir de registros existentes:

* Tipos de registro conectados. Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
* Registros conectados. Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
* O acesso e as permissões corretos no Workfront Planning e no Workfront, conforme descrito na seção [Requisitos de acesso](#access-requirements) deste artigo.

>[!NOTE]
>
>A criação de projetos e portfólios do Workfront à medida que você os conecta aos registros do Workfront Planning é semelhante à criação de registros do Planning à medida que você os conecta a outros registros.

Para criar registros ao conectá-los a partir de outros registros:

1. Comece a conectar os registros do Workfront Planning, conforme descrito no artigo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. (Condicional) Se não conseguir localizar um registro ao tentar adicioná-lo do campo de registro conectado de outro registro, procure um registro e clique em **+ Adicionar**. O botão **+ Adicionar** é seguido pelo nome do tipo de registro do qual você está se conectando.

   ![](assets/add-button-to-create-records-in-context-highlighted.png)

   O registro é criado e adicionado ao campo de registro conectado.
1. (Opcional) Vá para a exibição de tabela do tipo de registro cujo registro você criou. Um novo registro é exibido na última linha da exibição.
1. (Opcional) Comece a adicionar informações para o novo registro na exibição de tabela
Ou
Clique no nome para abrir a página de detalhes e adicionar informações lá.

## Criar registros enviando um formulário de solicitação para um tipo de registro

Depois que alguém criar um formulário de solicitação para um tipo de registro e compartilhar um vínculo a ele com você, você poderá submeter uma solicitação que criará um registro para esse tipo de registro.

Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Tanto os usuários do Workfront quanto os usuários externos à sua organização podem enviar solicitações para tipos de registro do Planning e criar registros, se tiverem um link para o formulário de solicitação.

Para obter informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).