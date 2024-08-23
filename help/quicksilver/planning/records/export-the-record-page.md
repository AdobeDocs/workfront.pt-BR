---
title: Exportar a página de registro
description: Você pode exportar a página de visualização ou de detalhes do registro para o Word.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 61cad7dc76ba04ea84ff0bd5052182f040f7b4d9
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 1%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--update the miniTOC and TOC when you make this public-->

# Exportar os detalhes de um registro

Para colaborar de forma mais eficiente com outras pessoas que talvez não tenham uma conta do Workfront, é possível exportar os detalhes de um registro para um documento do Word e compartilhá-lo com elas.

<!--replace the above with this, when we release export to PDF:

To collaborate more efficiently with others that might not have a Workfront account, you can export a record's details to a file and share it with them.-->

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
   <td> <p>Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Exibir ou aumentar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD:

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
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
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

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Considerações sobre a exportação de detalhes de um registro:

* Você pode exportar os detalhes de um registro para um documento do Word.

<!--replace the first bullet with this, when it's possible:

* You can export a record's details to the following file formats:

    * Word
    * PDF -->

* É possível exportar a página Detalhes da página de um registro. Não é possível exportar a guia Connections.

* O arquivo exportado preserva o layout da página de registro, incluindo a miniatura e as imagens de capa.

## Exportar os detalhes de um registro

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos em cartões.

1. Clique em um cartão de tipo de registro.
A página de tipo de registro é aberta e todos os registros desse tipo são exibidos.

1. Em qualquer exibição, clique no nome de um registro.

   A caixa de visualização do registro é aberta.

1. (Opcional) Clique no ícone ![](assets/open-details-in-a-new-tab-icon.png) de **Abrir em nova guia** para abrir a página do registro.

1. Escolha a guia **Detalhes**. A guia Detalhes deve ser aberta por padrão.

1. Clique no ícone **Exportar** ![](assets/export-icon-in-record-details-page.png) na visualização ou na página do registro.

   Um arquivo do Word (.docx) é baixado e salvo no computador.

   ![](assets/exported-word-file.png)

1. (Opcional) Vá para o arquivo baixado, abra-o e edite-o ou compartilhe-o com outras pessoas.