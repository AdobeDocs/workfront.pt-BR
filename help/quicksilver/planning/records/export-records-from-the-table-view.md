---
title: Exportar Registros da Exibição de Tabela
description: É possível exportar registros e suas informações da exibição de tabela para um arquivo CSV ou do Excel.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 1%

---

# Exportar registros da exibição de tabela

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Você pode exportar registros e suas informações da exibição de tabela para um arquivo Excel ou CSV no Adobe Workfront Planning.

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
<p>Qualquer Workfront e qualquer pacote do Planning</p> <p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Leve ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Exibir permissões ou mais altas para um espaço de trabalho e um tipo de registro</p>   
   <p>Exibir ou ter permissões mais altas para uma exibição</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> Os usuários com uma licença Light ou Contributor devem receber um modelo de layout que inclua o Planning.
   <p>Usuários padrão e Administradores do sistema têm as áreas do Planning habilitadas por padrão.</p></div></li></ul>
</td>
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
   <td><p> Light or higher </p>
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
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


## Exportar registros da exibição de tabela

Considere o seguinte ao exportar a exibição de tabela:

* As informações exportadas para um arquivo do Excel preservam os filtros, agrupamentos e classificações aplicados à exibição de tabela no Workfront Planning. Os agrupamentos não estão visíveis no arquivo CSV.

* Miniaturas e cores de linha personalizadas não são suportadas em arquivos exportados.

* Somente os campos tornados visíveis na interface do Workfront são exportados. Campos ocultos não são exportados.

Para exportar informações da exibição de tabela ou de um tipo de registro:

1. Vá para uma página de tipo de registro e clique em uma guia de exibição de tabela.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o nome da guia de exibição de tabela, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome da exibição e clique em **Exportar**.

   ![Mais menus em um modo de exibição](assets/view-more-menu-with-duplicate-option.png)

   * Clique em **Compartilhar** > **Exportar a exibição atual**. Essa opção está disponível somente quando você exibe a exibição de tabela.

   ![Botão Compartilhar com tipo de registro e opções de compartilhamento de exibição](assets/share-button-with-record-type-and-view-sharing-options.png)

1. Selecione um dos seguintes formatos:

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >Não é possível exportar informações da exibição de tabela quando você exibe uma exibição diferente na tela. Você deve exibir a exibição de tabela que deseja exportar para acessar a opção Exportar no menu Mais.

   O arquivo é baixado no computador.

1. (Opcional) Vá para a pasta de downloads no seu computador e localize o arquivo baixado.

   O nome do arquivo exportado segue o seguinte formato:

   `Name of the view - name of the record type`

   Por exemplo, uma exibição de tabela para o tipo de registro Campanhas gera um arquivo chamado `Table view - Campaigns`.

   O arquivo exibe as seguintes informações:

   * Os cabeçalhos de coluna são realçados em preto no arquivo do Excel
   * Todos os campos visíveis na interface do Workfront, classificados e filtrados pelos mesmos critérios
   * Os agrupamentos são preservados no arquivo do Excel

   Agora é possível compartilhar os arquivos exportados com outras pessoas ou anexá-los a qualquer comunicação.

</div>
