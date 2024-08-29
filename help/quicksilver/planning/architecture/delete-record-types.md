---
title: Excluir Tipos de Registro
description: É possível excluir tipos de registro quando eles não forem mais relevantes. A exclusão de tipos de registro também exclui todas as informações associadas aos tipos de registro, como seus registros, campos e exibições.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 425c3d3afb892ac83a10bbd36efb4c7d9712c4dc
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 2%

---


# Excluir tipos de registro

{{planning-important-intro}}

É possível excluir tipos de registro quando eles não forem mais relevantes.

No entanto, a exclusão de tipos de registro também exclui todas as informações associadas aos tipos de registro. Para obter mais informações, consulte a seção [Considerações ao excluir tipos de registro](#considerations-when-deleting-record-types) neste artigo.

Para obter informações sobre tipos de registros, consulte [Visão geral sobre tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
   <td><p> Padrão</p>
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
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

OLD: 

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
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## Considerações ao excluir tipos de registro

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Você pode excluir somente tipos de registro de espaços de trabalho para os quais tem permissões de gerenciamento.
* A exclusão de tipos de registro remove as seguintes informações associadas a eles:

   * Todos os registros desse tipo.
   * Todos os campos associados ao tipo de registro.
   * Todas as exibições (incluindo filtros, agrupamentos e critérios de classificação) do tipo de registro.
* O tipo de registro é removido de todos os usuários que acessam o espaço de trabalho.
* Não é possível recuperar tipos de registros excluídos ou suas informações.
* É recomendável recriar os campos e os registros associados ao tipo de registro que você deseja excluir em outro tipo de registro antes de excluí-los.

## Excluir tipos de registro

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja deletar,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de tipo de registro, clique no menu **Mais** e **Excluir**.
   * Clique no cartão do tipo de registro que deseja excluir e, na página de tipo de registro, clique no menu **Mais** ![](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Excluir**.

   ![](assets/permanently-delete-record-type-confirmation.png)

1. Digite **excluir** na caixa de confirmação e clique em **Excluir permanentemente**. Isso não diferencia maiúsculas de minúsculas.

   O tipo de registro selecionado, juntamente com seus campos, registros associados e exibições são excluídos e não podem ser recuperados.
