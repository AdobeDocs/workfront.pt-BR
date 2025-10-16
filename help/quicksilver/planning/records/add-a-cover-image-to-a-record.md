---
title: Adicionar uma imagem da capa a um registro
description: É possível personalizar registros adicionando uma imagem de capa à página de registro no Adobe Workfront Planning, ao editar um registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 0%

---


# Adicionar uma imagem da capa a um registro

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

É possível personalizar registros adicionando uma imagem de capa à página de registro no Adobe Workfront Planning, ao editar um registro.

Para obter informações sobre como editar registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

Você deve criar tipos de registro antes de começar a criar e editar registros.

Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisitos de acesso

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
<ul> 
<li><p>Qualquer Workfront e qualquer pacote do Planning</p></li>
Ou
<li><p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p></li></ul>
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
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
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
   <td><p> Standard</p>
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

## Considerações sobre imagens de capa de página de registro

É possível personalizar a página de um registro adicionando uma imagem de capa a ela.

Considere o seguinte:

* Uma imagem de capa é exclusiva a um registro e não se aplica a todos os registros do mesmo tipo.
* Você pode adicionar somente arquivos de imagem como imagens de capa.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* É possível adicionar uma imagem de capa a registros individuais a partir da pré-visualização do registro em qualquer exibição ou da página do registro.
* Não é possível adicionar imagens de capa a partir de uma visualização de registro.
* O Workfront faz o upload de uma imagem de capa automaticamente toda vez que você cria um registro. Posteriormente, você poderá modificar essa imagem.

## Adicionar uma imagem da capa a um registro

É possível personalizar um registro adicionando uma imagem de capa na parte superior da pré-visualização ou página do registro.

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros você deseja personalizar,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique em um registro

   Ou

   Na exibição de tabela, clique no ícone **Abrir detalhes** ![Ícone Abrir detalhes](assets/open-details-icon-in-table-name-field.png) na primeira coluna.

   A visualização do registro é aberta na exibição.

   ![Caixa de visualização de detalhes](assets/details-box.png)


1. (Opcional) Clique no ícone **Abrir em nova guia**![&#x200B; no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.](assets/open-details-in-a-new-tab-icon.png)<!--check the icon; they are changing it-->

   A página de registro é aberta.

   ![Página de detalhes](assets/details-page.png)

1. Na página de visualização ou detalhes do registro, passe o mouse sobre o espaço acima do nome do registro e clique em **Adicionar capa**.

   Ou

   Passe o mouse sobre uma imagem de capa existente, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Carregar**. <!--check the casing here; I logged a bug for this-->
A caixa **Capa de registro** é aberta na guia **Carregar**.

   ![Caixa de capa de registro para carregamento](assets/record-cover-box-for-upload.png)

1. Clique em **Procurar imagens** e procure uma imagem em seu computador para selecioná-la e adicioná-la.

1. (Opcional) Para remover a imagem antes de salvá-la, clique no **ícone Carregar nova imagem** ![ícone Carregar nova imagem](assets/upload-new-image-icon.png) e carregue uma nova imagem.

1. (Opcional) Clique na guia **Galeria** e clique em uma imagem na galeria de imagens. A galeria de imagens não pode ser modificada.

   ![Caixa de capa de registro para galeria](assets/record-cover-box-for-gallery.png)

1. Clique em **Usar imagem**.

   A imagem é carregada na parte superior da página de visualização ou detalhes do registro e as alterações são salvas automaticamente.

   ![Gravar página com imagem de capa](assets/record-page-with-cover-image.png)

1. (Opcional) Passe o mouse sobre a imagem e clique no menu **Mais** ![Mais menu](assets/more-menu.png), no canto inferior direito da imagem da capa, e siga um destes procedimentos:

   * Clique em **Carregar** se quiser substituir a imagem de capa e repita a Etapa 6 para carregar e salvar uma nova imagem.
   * Clique em **Reposicionar** e use a ferramenta **Reposicionar** ![Ícone da ferramenta Reposicionar](assets/reposition-tool-icon.png) para centralizar a imagem da capa e, em seguida, clique em **Salvar** quando terminar.
   * Clique em **Remover** para remover a imagem da capa.

   O Workfront salva suas alterações automaticamente.
