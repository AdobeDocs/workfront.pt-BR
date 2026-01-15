---
title: Excluir campos
description: No Adobe Workfront Planning, é possível excluir campos personalizados que não são mais relevantes.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---



# Excluir campos

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

No Adobe Workfront Planning, é possível criar campos personalizados para armazenar informações sobre registros.

Para obter informações sobre como criar campos personalizados no Workfront Planning, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

É possível excluir campos do Workfront Planning que não são mais relevantes.

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

<p>Para deletar campos de tipos de registro global:</p>
<ul><li><p>Qualquer pacote Workfront e um pacote Planning Plus</p></li>
Ou
<li><p>Qualquer fluxo de trabalho e pacotes do Planning Prime e Ultimate</p></li></ul>

<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões em um espaço de trabalho</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
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
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Considerações sobre a exclusão de campos do Workfront Planning:

* É possível excluir um campo somente na exibição de tabela do tipo de registro.
* Não é possível excluir o campo principal de um registro.
* As informações armazenadas no campo são excluídas e não podem ser recuperadas.
* Quando você exclui um campo de registro conectado, todos os campos de pesquisa conectados também são excluídos do tipo de registro ao qual você se conecta. Os campos de registro conectados dos tipos de registro aos quais você se conecta também são excluídos do registro ao qual você se conecta.

  Por exemplo, ao conectar Campanhas a outro tipo de registro chamado Produto e excluir o campo conectado Produto e o campo de pesquisa Status do Produto da campanha, as seguintes opções são excluídas:

   * O campo Produto conectado da campanha
   * O campo de pesquisa Status do produto da campanha
   * O campo conectado do Campaign do produto

  Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* Não é possível excluir campos de registros globais que foram adicionados a espaços de trabalho secundários a partir de espaços de trabalho secundários.

## Excluir campos

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos campos de registro você deseja deletar.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.

1. Clique no cartão de um tipo de registro.

1. (Condicional) Se ainda não estiver selecionada, clique na guia de uma **exibição de Tabela** na página de tipo de registro.

   Todos os registros existentes associados ao tipo de registro são exibidos nas linhas da exibição de tabela.

1. Localize o campo que deseja excluir nos cabeçalhos da coluna, passe o mouse sobre o cabeçalho da coluna e clique na seta para baixo após o nome do campo.

   ![Menu de seta após o nome do campo no cabeçalho da tabela realçado](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Clique em **Excluir**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Clique em **Excluir** para confirmar.

   Os campos excluídos não podem ser recuperados.

   Dependendo do tipo de campo excluído, o seguinte acontece:

   * Se você excluir um campo que pertence ao registro selecionado, o campo será excluído e não poderá mais ser associado a nenhum registro. Se esse campo for adicionado como um campo de pesquisa em outros registros, esses campos também serão excluídos.
   * Se você excluir um campo de conexão, o campo será excluído do registro selecionado. Além disso, o campo de conexão correspondente de seu registro original também é excluído.
   * Se você excluir um campo de pesquisa que foi adicionado de um registro conectado, o campo será excluído do tipo de registro selecionado, mas permanecerá em seu tipo de registro original.
   * Se você excluir um campo de um tipo de registro global em seu espaço de trabalho principal, ele será excluído de todos os espaços de trabalho em que esse tipo de registro foi adicionado. Não é possível excluir campos de tipos de registro global de seus espaços de trabalho secundários.
