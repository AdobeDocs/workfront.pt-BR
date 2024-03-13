---
title: Criar registros
description: Ao usar os recursos de planejamento do Adobe Workfront, um registro é uma instância de um tipo de registro. Você deve criar tipos de registro antes de criar registros individuais. Criar registros de taxonomia é idêntico à criação de registros operacionais.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Criar registros

{{maestro-important-intro}}

Nos recursos de planejamento do Adobe Workfront, um registro é uma instância de um tipo de registro.

Você pode ter os seguintes tipos de registros:

* **Registros operacionais**: elas representam objetos relacionados ao trabalho. Por exemplo, para um registro operacional chamado &quot;Campanha&quot;, é possível nomear registros como &quot;Informativo mensal&quot; ou &quot;Vendas de verão&quot;.
* **Registros de taxonomia**: eles representam atributos que podem ser associados a registros operacionais. Por exemplo, para um tipo de registro de taxonomia chamado &quot;Canal&quot;, é possível nomear taxonomias como &quot;Email&quot;, &quot;Mídia social&quot; ou &quot;Publicidade&quot;.

A criação de registros operacionais é idêntica à criação de registros de taxonomia.

Você pode criar registros seguindo um destes procedimentos:

* Criá-los manualmente para tipos de registro
  <!-- not possible anymore: * Connect them to records from other applications-->
* Criar registros copiando e colando informações de uma lista externa.

Este artigo descreve como criar registros. Para obter informações sobre o gerenciamento de registros nas exibições de tabela ou linha do tempo, consulte os seguintes artigos:

* [Gerenciar a exibição de tabela](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [Gerenciar a exibição de linha do tempo](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
<p>Sua organização deve estar inscrita no programa beta fechado de recursos de planejamento do Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
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
   <td> <p>Não há controles de acesso para os recursos de planejamento do Adobe Workfront </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Contribuir com permissões ou mais altas para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Maestri no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Criar registros adicionando-os manualmente a um tipo de registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Você pode criar registros na exibição de tabela de uma página do tipo de registro.

Para obter informações sobre edição de informações de registro, consulte [Editar registros](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

O espaço de trabalho acessado pela última vez é aberto por padrão. Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).
1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](../architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.
Todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. (Condicional) Se a página do tipo de registro não abrir na exibição de tabela, clique no link **Exibir** e selecione um existente **Visualização em tabela** ![](assets/table-view-icon.png) ou clique em **Criar visualização > Tabela** para criar uma visualização de tabela.

<!--Replace the above with this when we release the tabbed views: 
1. (Conditional) If the record type page does not open in the table view, click the tab of a table view, or click **+ View** to create a table view. -->

1. Para adicionar novos registros, clique em **Novo registro** na última linha da tabela

   Ou

   Clique em **Shift + Enter** no teclado a partir de qualquer coluna ou linha da tabela. Isso adiciona uma linha vazia.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Comece a digitar informações na nova linha sobre o novo registro.

   >[!NOTE]
   >
   >  * Não há campos obrigatórios para registros. No entanto, recomendamos adicionar um Nome para o registro, pois é útil identificar registros ao vincular registros uns aos outros.
   >
   >  * Os campos que se referem a outros tipos de registro ou campos calculados são campos somente leitura.

1. Continue adicionando informações em cada linha e clique em **Enter** no teclado para salvar as alterações.

<!--Or 
    
    Click the new record's name or the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of the record name. The **Details** box opens in the table. 

      >[!TIP]
      >
      >    You can access the Details box only from the name field of the record when the Name field is a primary field. 

  1. Start editing the record's information in the Details box. Workfront automatically saves your changes. 
  1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the Details box to open the record's **Details** page in a new tab. Continue editing the record on the Details page.
    -->

1. (Opcional) Use os seguintes atalhos de teclado para desfazer ou refazer a adição de novos registros:

   * CTRL + Z (⌘ + Z para Mac) para desfazer uma alteração
   * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer uma alteração

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## Criar registros copiando e colando informações de uma lista externa

1. Comece a criar registros na exibição Tabela, conforme descrito na seção [Criar registros adicionando-os manualmente a um tipo de registro](#create-records-by-manually-adding-them-to-a-record-type) neste artigo.

   Certifique-se de que a exibição de tabela tenha as colunas (ou os campos) que você deseja preencher com as novas informações de registro.

1. Clique em **Novo &lt; Nome do tipo de registro >** na última linha da tabela para adicionar quantas linhas novas desejar aos novos registros.

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

   As informações a seguir são importadas na área de recursos do Workfront Planning:

   * As linhas contêm os novos registros
   * As colunas preenchem informações para os campos dos registros.
