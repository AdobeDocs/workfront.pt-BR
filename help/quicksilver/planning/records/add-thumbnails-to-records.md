---
title: Adicionar uma miniatura a um registro
description: É possível editar informações de registro no Adobe Workfront Planning e associar cada registro a miniaturas individuais, para torná-las facilmente reconhecíveis.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# Adicionar uma miniatura a um registro

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Você pode associar registros a miniaturas exclusivas no Adobe Workfront Planning para torná-los facilmente reconhecíveis.

Você deve criar tipos de registro antes de começar a criar e editar registros.
Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisitos de acesso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront e qualquer pacote do Planning</p> <p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Contribuir com ou mais permissões para um espaço de trabalho e tipo de registro  </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr>   
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->


## Considerações sobre miniaturas de registro

Para distinguir visualmente entre registros em uma exibição de tabela, você pode associar uma imagem em miniatura exclusiva a cada registro.

Considere o seguinte:

* Uma miniatura é exclusiva de um registro e não se aplica a todos os registros do mesmo tipo.
* Você pode adicionar somente arquivos de imagem como miniaturas.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Você pode adicionar uma imagem em miniatura a registros individuais na exibição de tabela ou na página do registro ou na caixa de pré-visualização.
* O Workfront faz upload de uma imagem em miniatura automaticamente sempre que você cria um registro. Posteriormente, você poderá modificar essa imagem.
* As miniaturas pertencem às informações de registro e são exibidas em áreas onde os registros são exibidos. Por exemplo, as miniaturas são exibidas ao lado das informações de registro nas seguintes áreas:

   * O campo principal de um registro na exibição de tabela
   * A barra de registro na exibição de linha do tempo.
   * Visualização e página dos detalhes do registro.

## Adicionar uma miniatura a um registro

Você pode adicionar uma miniatura das seguintes maneiras:

* [Adicionar uma miniatura a um registro da exibição de tabela](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Adicionar uma miniatura a um registro da página de detalhes](#add-a-thumbnail-to-a-record-from-the-details-page)

### Adicionar uma miniatura a um registro da exibição de tabela

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros deseja adicionar miniaturas e, em seguida, clique no cartão de tipo de registro.

   Isso abre a página do tipo de registro.
1. Selecione uma exibição de tabela no menu suspenso **Exibir**. Todos os registros do tipo selecionado são exibidos em uma tabela.
1. Passe o mouse sobre as informações do campo principal, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Miniatura**.

   ![Gravar mais menu expandido](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   O campo principal é aquele exibido na primeira coluna de uma exibição de tabela. O campo principal é sempre congelado e não pode ser oculto ou realocado. A opção Miniatura não está disponível no menu Mais quando o campo principal é um campo de fórmula.

   A guia **Carregar** é aberta por padrão na caixa **Miniatura do registro**.

   Para obter mais informações sobre como carregar a miniatura, consulte a seção [Adicionar uma miniatura a um registro da página de detalhes](#add-a-thumbnail-to-a-record-from-the-details-page) neste artigo, a partir da Etapa 6. <!--see if this is accurate-->

<!--
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![Upload new image icon](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![Remove image icon](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![Record thumbnail box for gallery](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![More menu](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![Remove image icon](assets/remove-image-icon.png), then click **Save changes**. -->

### Adicionar uma miniatura a um registro da página de detalhes

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros deseja adicionar miniaturas e, em seguida, clique no cartão de tipo de registro.

   Isso abre a página do tipo de registro.
1. Em qualquer exibição, clique em um registro para abri-lo.

   A caixa de visualização de detalhes é exibida.
1. (Opcional) Clique no ícone **Abrir em nova guia** ![Abrir detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) no canto superior direito.

   A página de detalhes do registro é aberta.

1. (Condicional) Na página de visualização ou detalhes do registro, passe o mouse sobre a imagem da miniatura ou o ícone ![Ícone da miniatura do registro na página de detalhes](assets/record-thumbnail-icon-on-details-page.png), passe o mouse sobre o espaço acima do nome do registro e clique em **Adicionar miniatura** ou **Editar miniatura**.

   A guia **Carregar** é aberta por padrão na caixa **Miniatura do registro**.

   ![Gravar caixa de miniatura para carregamento](assets/record-thumbnail-box-for-upload.png)

1. Arraste e solte um arquivo para adicionar como miniatura

   Ou

   Clique em **Procurar imagens** e procure um arquivo de imagem a ser adicionado. O arquivo deve ser salvo no computador.

1. (Opcional) Depois que a imagem for carregada na caixa **Gravar miniatura**, use a ferramenta de dimensionamento para recortar e redimensionar a imagem.
1. (Opcional) Clique no ícone **Carregar nova imagem** ![Carregar nova imagem ícone](assets/upload-new-image-icon.png) para carregar outra imagem.
1. (Opcional) Clique na guia **Galeria** e clique em uma imagem. A galeria de imagens não pode ser modificada.

   ![Gravar caixa de miniatura da galeria](assets/record-thumbnail-box-for-gallery.png)

1. (Opcional) Para remover a miniatura antes de salvá-la, clique no ícone **Remover** ![Ícone Remover imagem](assets/remove-image-icon.png) à direita da imagem.

1. Clique em **Usar imagem** para adicionar a imagem como miniatura.
Isso fecha a caixa **Miniatura do registro**.
A miniatura é exibida nas áreas do Workfront Planning onde o registro é exibido.

   >[!TIP]
   >
   >   Você deve ativar o campo Miniatura na exibição de tabela para exibir miniaturas nesta exibição. Ela está desativada por padrão.

1. (Opcional) Para remover a miniatura depois que ela for salva, clique em um registro em qualquer modo de exibição para abrir a página de detalhes, passe o mouse sobre a imagem de miniatura e clique no ícone de menu **Mais** ![Mais ícone de menu](assets/more-menu.png)> **Remover** ícone ![Remover ícone](assets/remove-image-icon.png). A imagem em miniatura é removida.


<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![More menu](assets/more-menu.png), then click **Thumbnail**. 

   ![Record more menu expanded](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![Record thumbnail box for upload](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->
