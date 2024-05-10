---
title: Gerenciar a página de registros
description: É possível editar o layout da visualização de registro e da página no Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: ace194b584601f9edd7862dbd74f639538891370
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Gerenciar a página de registros

{{maestro-important-intro}}

É possível editar o layout da visualização de registro e da página no Adobe Workfront Planning.

A visualização do registro é uma exibição menor da página do registro exibida na exibição de um tipo de registro.

Quando você altera o layout de uma visualização e página de registro, as alterações afetam as caixas de visualização e as páginas de detalhes de todos os registros do mesmo tipo.

Este artigo descreve como alterar o layout e a aparência de uma caixa de visualização de registro ou de uma página de registro. Para obter informações sobre edição de registros, consulte [Editar registros](/help/quicksilver/maestro/records/edit-records.md).

Você deve criar tipos de registro e registros antes de começar a editar páginas de registro.

Para obter informações, consulte os seguintes artigos:

* [Criar tipos de registro](../architecture/create-record-types.md)

* [Criar registros](/help/quicksilver/maestro/records/create-records.md)

## Requisitos de acesso

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
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Novo: Claro ou superior</p>
   Ou
   <p>Atual: trabalho ou superior</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar ou aumentar as permissões de um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerações sobre a edição de páginas de registro

* A reorganização de campos na visualização de registro ou página reorganiza os campos para todos os registros desse tipo e para todos os usuários que acessam esses registros.

* As alterações de exibição feitas na visualização do registro ficam imediatamente visíveis na página de detalhes do registro. As alterações feitas na página de registro também estão visíveis na caixa de visualização do registro.

<!--Replace the first bullet with this when we add sections:

* The following changes affect all the records of the same type and are visible to all users accessing those records: 

   * Rearranging fields
   * Adding or removing sections
-->

* A adição de uma imagem de capa a um registro não faz parte do layout geral da pré-visualização ou página do registro. Você pode adicionar imagens de capa exclusivas a cada registro. Para obter informações, consulte [Adicionar uma imagem da capa a um registro](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

<!--

## Add sections to a record preview or page

You can add sections to a record preview or page, to organize the information by common criteria and make it easier to find. 

Consider the following when adding sections to a record page:

* There is no limit to how many sections you can have on a page (***************IS THIS TRUE???***********)
* You cannot have an empty section. You must have at least one field in a section. 
* You can drag and drop fields from one section to another. 
* When you remove all the fields from a section, the section is automatically deleted and cannot be recovered. 

To add a section to a record preview or page: 

{{step1-to-maestro}}

The workspace that you access last opens. 

1. (Optional) Click the downward-pointing arrow to the right of the workspace name to select the workspace whose records you want to update. 
1. Click a record type card. 

    The record type page opens. 

1. From a view of any type, click the name of a record 

    Or 
    
    From the table table view, click the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of a record name. 
    
    The record's preview opens in the view.

    ![](assets/details-box.png) 

    >[!TIP]
    >
    >You can view the **Open details** icon to the left of the Name field of a record in a table view only when the Name field is a primary field. 

1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) (****************check the icon; they are changing it**********)  in the upper-right corner of the record preview  to open the record's page in a new tab. 

    The record page opens. 

    ![](assets/details-page.png)

1. In the record preview or page, hover over the white space to the left of the fields, then click the **Add section** icon ![](assets/add-section-icon.png) to add a section. 
1. Click inside the section's name and replace **Untitled** with a name, then click Enter. (************has this changed to Untitled section???**********)
1. Start dragging and dropping fields to the new section, as described in the section [Rearrange fields in the record preview or page](#rearrange-fields-in-the-record-preview-or-page) in this article. 

1. (Optional) Hover over the name of a section and click the **More** menu ![](assets/more-menu.png). 

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Optional) Do one of the following to edit the section: 

   * Click **Rename** to rename the section

      >[!TIP]
      >
      > You can rename a section inline, by clicking the name.
   
   * Click **Move up** to move the section up one position 

      Or 
      
      Click **Move down** to move the section down one position.
      All fields in the section move with the section. 

   * Click **Delete** to delete the section. The section is deleted and it cannot be recovered. All users accessing the records of this type will no longer view the deleted section. 

1. Click the downward-pointing arrow to the left of a section name to collapse it, or the right-pointing arrow  to expand it. 
   All sections are expanded by default. 

1. (Optional) Click the **grab** icon ![](assets/grab-icon.png) to the left of a section name, then drag and drop it in a desired spot. 

    The new position of the section updates in both the preview and the page of all records of the same type for all users viewing the records. 

    All changes to sections and field order are saved automatically. 

-->

## Reorganizar campos na visualização ou página do registro

{{step1-to-maestro}}

O espaço de trabalho que você acessa por último é aberto.

1. (Opcional) Clique na seta para baixo à direita do nome do espaço de trabalho para selecionar o espaço de trabalho cujos registros você deseja atualizar.
1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique no nome de um registro

   Ou

   Na exibição de tabela, clique na guia **Abrir detalhes** ícone ![](assets/open-details-icon-in-table-name-field.png) à esquerda do nome de um registro.

   A visualização do registro é aberta na exibição.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >É possível exibir a **Abrir detalhes** Ícone à esquerda do campo Nome de um registro em uma exibição de tabela somente quando o campo Nome é um campo primário.

1. (Opcional) Clique no link **Abrir em nova guia** ícone ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.

   A página de registro é aberta.

   ![](assets/details-page.png)

1. Na visualização ou página do registro, clique na guia **agarrar** ícone ![](assets/grab-icon.png) à esquerda de um nome de campo, arraste e solte-o no ponto desejado. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   A nova posição do campo é atualizada na pré-visualização e na página de todos os registros do mesmo tipo para todos os usuários que visualizam os registros.

   Todas as alterações no layout da visualização do registro ou na página são salvas automaticamente.

