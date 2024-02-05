---
title: Criar tipos de registro operacional
description: Os tipos de registros são os tipos de objetos do Adobe Maestro. No Maestri, você pode criar tipos de registro personalizados que ilustram os itens de trabalho necessários no ciclo de vida da organização.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '1189'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Criar tipos de registro operacional

{{maestro-important-intro}}

Os tipos de registros são os tipos de objetos do Adobe Maestro. No Maestri, você pode criar tipos de registro personalizados que ilustram os itens relacionados ao trabalho necessários no ciclo de vida da organização.

Os tipos de registro podem ser um dos seguintes:

* **Tipos de registro operacional**
* **Taxonomias**

Para obter mais informações sobre os tipos de registros do Maestro, consulte [Visão geral dos tipos de registro e taxonomias](../architecture/overview-of-record-types-and-taxonomies.md).

A criação de tipos de registros operacionais é semelhante à criação de tipos de registros de taxonomia. Este artigo descreve como criar tipos de registros operacionais.

Para obter informações sobre como criar taxonomias, consulte [Criar tipos de registro de taxonomia](../architecture/create-a-taxonomy.md).

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
   </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
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
   <td> <p>Não há controles de nível de acesso para o Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Maestri no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações sobre a criação de tipos de registro

* Você pode criar tipos de registro em um espaço de trabalho das seguintes maneiras:

   * Automaticamente:
      * Ao criar um espaço de trabalho usando um modelo.

        Para obter informações, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).
      * Ao importá-los usando um arquivo Excel ou CSV. Isso não está disponível para tipos de registro de taxonomia.
     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a Maestro record. This creates a read-only record type in Maestro which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/maestro/architecture/connect-record-types.md).
        For information about connecting objects with Maestro records, see [Connect records](/help/quicksilver/maestro/records/connect-records.md). -->
   * Manualmente:

      * Do zero.

## Criar tipos de registro usando um modelo de espaço de trabalho

É possível criar tipos de registro automaticamente ao criar um espaço de trabalho usando um modelo. Cada modelo Maestri contém exemplos de tipos de registros operacionais e taxonomia.

Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture/create-workspaces.md).

Para obter informações sobre quais tipos de registro são incluídos em cada modelo, consulte [Lista de modelos do espaço de trabalho](../architecture/workspace-templates.md).

## Criar um tipo de registro do zero

Este artigo descreve como criar tipos de registros operacionais do zero. A criação de tipos de registros operacionais do zero é semelhante à criação de taxonomias.

Para obter mais informações sobre taxonomias, consulte [Criar uma taxonomia](../architecture/create-a-taxonomy.md).

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho para o qual deseja criar tipos de registro.
1. Clique em **Adicionar tipo de registro**.
1. (Condicional) Se você estiver criando um tipo de registro operacional, clique em **Do zero**. Essa opção não está disponível ao criar taxonomias.

   A caixa Adicionar tipo de registro é aberta.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Atualize as seguintes informações:

   * **Nome do tipo de registro**: substitua &quot;Tipo de registro operacional sem título&quot; pelo nome do seu tipo de registro futuro.
   * **Aparência**: Defina a cor e a forma do ícone associado ao tipo de registro. Faça o seguinte:
      * Selecione uma cor para identificar o novo tipo de registro. Esta é a cor do ícone do tipo de registro. O cinza é selecionado por padrão.
      * Selecione um ícone na lista ou comece a digitar o nome de um ícone para descrever o que ele representa e, em seguida, selecione-o quando ele for exibido. Este é o ícone do tipo de registro. Um ícone de arquivo é selecionado por padrão.

1. Clique fora da **Adicionar tipo de registro** para salvar o tipo de registro.

   O cartão de tipo de registro é adicionado ao espaço de trabalho selecionado.
O número de campos que o tipo de registro contém é exibido no cartão.
1. (Opcional) Clique no cartão de tipo de registro para abrir a página de tipo de registro.

   ![](assets/operational-record-type-blank.png)

   A página de tipo de registro é exibida na exibição Tabela por padrão. As colunas da tabela são campos associados ao novo tipo de registro. Cada linha é um registro exclusivo que deve ser adicionado.

   Por padrão, os seguintes campos são exibidos nas colunas de exibição de tabela de um tipo de registro operacional:

   * Nome

     O campo Nome é o único campo criado automaticamente para taxonomias.
   * Descrição
   * Data de início
   * Data Final
   * Status

1. (Opcional) Atualizar o nome do tipo de registro no cabeçalho da página

   Ou

   Clique em **Mais** ícone ![](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Renomear** para renomeá-la.

1. (Opcional) Clique em **+ Novo registro** para adicionar registros do tipo selecionado. Para obter mais informações, consulte [Criar registros](../records/create-records.md).
1. (Opcional) Clique no link **+** ícone no canto superior direito da tabela para adicionar mais campos ao tipo de registro.

   Para obter mais informações sobre a criação de campos, consulte [Criar campos](../fields/create-fields.md).

1. (Opcional) Clique na seta à esquerda do nome do tipo de registro para voltar ao espaço de trabalho selecionado.

   O cartão de tipo de registro exibe o número de campos e conexões que o tipo de registro contém.

   ![](assets/campaign-card-with-fields-and-connections-highlighted.png)

   Para obter informações adicionais sobre como adicionar registros, excluir ou editar tipos de registro ou atualizar a exibição na página tipo de registro, consulte os seguintes artigos:

   * [Criar registros](../records/create-records.md)
   * [Excluir tipos de registro](../architecture/delete-record-types.md)
   * [Editar tipos de registro](../architecture/edit-record-types.md)
   * [Gerenciar exibições de registro](../views/manage-record-views.md)

## Criar tipos de registro importando um arquivo Excel ou CSV

Considere o seguinte ao importar tipos de registro usando um arquivo Excel ou CSV:

* Cada folha do arquivo Excel torna-se um tipo de registro no Maestro.
* As colunas de cada planilha se tornam os campos associados a cada tipo de registro.
* Os campos são exclusivos para seus respectivos tipos de registro.
* Cada linha em cada planilha se torna um registro exclusivo associado ao respectivo tipo de registro.
* Cada folha do arquivo Excel não deve exceder o seguinte:
   * 10.000 linhas
   * 500 colunas
* O arquivo do Excel não deve ter mais de 5 MB.
* Planilhas vazias não são suportadas.

Para importar tipos de registro usando um arquivo do Excel:

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho para o qual deseja criar tipos de registro.
1. Clique em **Adicionar tipo de registro**.
1. (Condicional) Se você estiver criando um tipo de registro operacional, clique em **Excel/CSV**.

   >[!NOTE]
   >
   >    Essa opção não está disponível ao criar tipos de registro de taxonomia.

1. Arraste e solte um arquivo Excel ou CSV salvo anteriormente no computador ou clique em **Selecione um arquivo CSV ou do Excel** para procurar um.
1. Clique em **Revise seus dados**.

   A caixa Preview and edit é exibida com as seguintes informações:

   * Os nomes das planilhas ou dos futuros tipos de registros são exibidos no painel esquerdo. Por padrão, o Maestro seleciona um ícone e uma cor para cada novo tipo de registro.
   * A primeira folha ou tipo de registro é selecionado e os nomes dos campos associados a ela são exibidos como cabeçalhos de coluna. O tipo de cada campo é selecionado por padrão.
   * Cada linha representa um novo registro. Somente os primeiros 10 registros são exibidos na caixa Preview and edit.

   ![](assets/preview-and-edit-box.png)

1. (Opcional) Clique no nome de cada planilha no painel esquerdo para revisar as informações que ela contém.

   >[!NOTE]
   >
   >    Planilhas vazias não são suportadas e estão esmaecidas.


1. (Opcional) Clique no link **Selecionar planilhas para importar** e desmarque as planilhas que não deseja importar.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   As planilhas desmarcadas são exibidas com um plano de fundo cinza.

1. Clique em **Importar** quando estiver pronto para importar o arquivo.

   As seguintes informações são importadas para o Maestri:

   * Novos tipos de registro
   * Novos campos associados a cada tipo de registro
   * Novos registros associados a cada tipo de registro

   Você pode começar a gerenciar campos e registros nas páginas de tipos de registro.

   Todos os que têm acesso ao Maestro agora podem visualizar e editar os tipos de registros importados e suas informações. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a Maestro record type and an object type from another application. This creates a read-only record type in Maestro that corresponds to the object type in the other application. 

For example, you can create record types by connecting Maestro record types with Workfront projects. As a result, the Workfront project object type is imported into Maestro as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](../architecture/connect-record-types.md). 
-->