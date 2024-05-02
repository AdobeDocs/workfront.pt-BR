---
title: Adicionar uma miniatura a um registro
description: É possível editar informações de registro no Adobe Workfront Planning e associar cada registro a miniaturas individuais, para torná-las facilmente reconhecíveis.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Adicionar uma miniatura a um registro

{{maestro-important-intro}}

Você pode associar registros a miniaturas exclusivas no Adobe Workfront Planning para torná-los facilmente reconhecíveis.

Você deve criar tipos de registro antes de começar a criar e editar registros.
Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

## Requisitos de acesso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta de Planejamento do Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Contribuir com permissões ou mais altas para um espaço de trabalho </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td>  <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> <p>Para obter informações, consulte <a href="/help/quicksilver/maestro/access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Considerações sobre miniaturas de registro

Para distinguir visualmente entre registros em uma exibição de tabela, você pode associar uma imagem em miniatura exclusiva a cada registro.

Considere o seguinte:

* Você pode adicionar somente arquivos de imagem como miniaturas.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Você pode adicionar uma imagem em miniatura a registros individuais na exibição de tabela.
* As miniaturas pertencem às informações de registro e são exibidas em exibições nas quais os registros são exibidos. Por exemplo, as miniaturas são exibidas ao lado das informações de registro nas seguintes áreas:

   * O campo principal de um registro na exibição de tabela
   * A barra de registro na exibição de linha do tempo.
* Não é possível adicionar miniaturas de registro da página do registro ou de outro tipo de visualização.
* As miniaturas não são exibidas na página do registro.

## Adicionar uma miniatura a um registro

{{step1-to-maestro}}

1. Selecione o espaço de trabalho cujos registros deseja adicionar miniaturas e clique no cartão de tipo de registro.

   Isso abre a página do tipo de registro.
1. Selecione uma exibição de tabela na **Exibir** menu suspenso. Todos os registros do tipo selecionado são exibidos em uma tabela.
1. Passe o mouse sobre as informações do campo principal, clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Miniatura**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   O campo principal é aquele exibido na primeira coluna de uma exibição de tabela. O campo principal é sempre congelado e não pode ser oculto ou realocado.

   A variável **Miniatura de registro** é aberta.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. No **Carregar** arraste e solte um arquivo para adicionar como miniatura ou clique em **Selecione para fazer upload** e procure um arquivo de imagem para adicionar. O arquivo deve ser salvo no computador.
1. (Opcional) Use a ferramenta de dimensionamento para cortar e redimensionar a imagem.
1. Clique em **Usar imagem** para adicionar a imagem como miniatura.
Isso fecha o **Miniatura de registro** caixa.
1. (Condicional) Se você tiver pelo menos permissões do Contribute para a exibição de tabela, clique em **Campos** no canto superior direito da exibição em tabela.
1. Selecione o **Miniatura** para exibir a miniatura. Essa opção é desmarcada por padrão.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   A miniatura é exibida à esquerda do valor do campo principal.
1. (Opcional e condicional) Se você não tiver permissões do Contribute ou superiores para a exibição, selecione uma nova exibição na **Exibir** ou crie uma visualização.
1. (Opcional) Para remover a miniatura, passe o mouse sobre o campo principal e clique no link **Mais** menu ![](assets/more-menu.png)> **Miniatura** > o **Remover** ícone ![](assets/remove-image-icon.png)e, em seguida, clique em **Salvar alterações**.

<!--
Replace the section above with the following when we release generate thumbnails:

## Add a thumbnail to a record

You can add a thumbnail to a record in the following ways:

* Upload a file from your computer
* Generate an image with a prompt

### Upload a thumbnail to a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Upload** tab, and drag and drop a file to add as a thumbnail
   Or
   Click **Select to upload**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) Use the sizing tool to crop and resize the image.
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
1. (Conditional) If you have at least Contribute permissions to the table view, click **Fields** in the upper-right corner of the table view. 
1. Select the **Thumbnail** toggle to display the thumbnail. This is deselected by default. 

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   The thumbnail displays to the left of the primary field value. 
1. (Optional and conditional) If you do not have Contribute or higher permissions to the view, select a new view from the **View** drop-down menu, or create a view. 
1. (Optional) To remove the thumbnail, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**.

### Generate a thumbnail for a record

{{step1-to-maestro}}

1. Select the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->