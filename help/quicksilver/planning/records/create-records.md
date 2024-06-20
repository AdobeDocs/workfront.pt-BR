---
title: Criar registros
description: Ao usar o Adobe Workfront Planning, um registro é uma instância de um tipo de registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 7882b67578cd5b8792ce582ebab118c8993c9214
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Criar registros

{{planning-important-intro}}

No Adobe Workfront Planning, um registro é uma instância de um tipo de registro.

Você pode criar registros seguindo um destes procedimentos:

* Criá-los manualmente para tipos de registro
* Criar registros copiando e colando informações de uma lista externa.

Este artigo descreve como criar registros. Para obter informações sobre o gerenciamento de registros nas exibições de tabela ou linha do tempo, consulte os seguintes artigos:

* [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Gerenciar a exibição de linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
<p>Sua organização deve estar inscrita no estágio de acesso antecipado do Workfront Planning </p>
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
   <td> <p>Não há controles de acesso para o Adobe Workfront Planning </p>  
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
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/planning/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Criar registros adicionando-os manualmente a um tipo de registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Você pode criar registros na exibição de tabela de uma página do tipo de registro.

Para obter informações sobre edição de informações de registro, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.
Todos os registros do tipo selecionado são exibidos na visualização.

1. (Condicional) Dependendo da exibição exibida, siga um destes procedimentos:

   * Na exibição de tabela:

      * Clique em **Novo registro** na última linha da tabela

      * Clique em **Shift + Enter** no teclado a partir de qualquer coluna ou linha da tabela. Isso adiciona uma linha vazia.

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * Em qualquer modo de exibição:

      * Clique em **Novo registro** no canto superior direito da página. A caixa de visualização do registro é aberta.

     O Workfront faz o upload de uma miniatura e de uma imagem de capa automaticamente para cada novo registro. Posteriormente, você poderá modificar essas imagens. Para obter informações, consulte os seguintes artigos:

      * [Adicionar uma imagem da capa a um registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Comece digitando informações sobre o novo registro nos campos que você vê na caixa de visualização.

   >[!NOTE]
   >
   >  * Não há campos obrigatórios para registros. No entanto, recomendamos adicionar informações para o campo principal de um registro, pois é útil identificar registros ao vincular registros uns aos outros. Para obter mais informações sobre campos primários, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md) e [Visão geral do campo principal](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Os campos que se referem a outros tipos de registro ou campos calculados são campos somente leitura.

1. (Condicional) Ao adicionar registros na tabela, continue adicionando informações em cada linha e clique em **Enter** no teclado para salvar as alterações.

   Ou

   Clique no nome do novo registro ou na **Abrir detalhes** ícone ![](assets/open-details-icon-in-table-name-field.png) à esquerda do nome do registro. Uma visualização com as informações detalhadas do registro é aberta na tabela.

   >[!TIP]
   >
   >Você pode acessar o **Abrir detalhes** ícone somente do campo name do registro quando o campo Name é um campo primário.

1. Iniciar edição das informações do registro na visualização do registro. O Workfront salva suas alterações automaticamente.
1. (Opcional) Clique no link **Abrir em nova guia** ícone ![](assets/open-details-in-a-new-tab-icon.png) no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia. Continuar editando o registro na página de registro. Para obter informações, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

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

   As informações a seguir são importadas na área do Workfront Planning:

   * As linhas contêm os novos registros
   * As colunas preenchem informações para os campos dos registros.
