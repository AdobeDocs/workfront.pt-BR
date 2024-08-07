---
title: Criar tipos de registro
description: Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, você pode criar tipos de registro personalizados que ilustrem os itens de trabalho necessários no ciclo de vida da sua organização.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Criar tipos de registro

{{planning-important-intro}}

Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, você pode criar tipos de registro personalizados que ilustrem os itens relacionados ao trabalho necessários no ciclo de vida da organização.

Para obter mais informações sobre tipos de registros, consulte [Visão geral sobre tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

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
   <td> Adobe Workfront
   </td>
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
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Atual: Plano</p>
   Ou
   <p>Novo: Padrão </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral sobre acesso</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram
</td>
  </tr>
 </tbody>
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações sobre a criação de tipos de registro

* Você pode criar tipos de registro em um espaço de trabalho das seguintes maneiras:

   * Automaticamente:
      * Ao criar um espaço de trabalho usando um modelo.

        Para obter informações, consulte [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

      * Ao importá-los usando um arquivo Excel ou CSV.

        >[!IMPORTANT]
        >
        >Essa funcionalidade está temporariamente desativada desde 21 de março de 2024. Ela será ativada posteriormente.

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->
   * Manualmente:

      * Do zero.

        Este artigo descreve como criar tipos de registro do zero.

* Você pode mover tipos de registro em uma seção e de uma seção de um espaço de trabalho para outra. Não é possível mover tipos de registro de um espaço de trabalho para outro.

## Criar tipos de registro usando um modelo de espaço de trabalho

É possível criar tipos de registro automaticamente ao criar um espaço de trabalho usando um modelo do Workfront Planning. Cada modelo contém tipos de registro de amostra.

Ao criar um espaço de trabalho a partir de um modelo, os tipos de registro são agrupados nas seguintes seções:

* Tipos de registro operacional
* Taxonomias

Você pode adicionar tipos de registro manualmente nas seções Tipos de Registro Operacionais e Taxonomias.

Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

Para obter informações sobre quais tipos de registro são incluídos em cada modelo, consulte [Lista de modelos de espaço de trabalho](/help/quicksilver/planning/architecture/workspace-templates.md).

## Criar um tipo de registro do zero

{{step1-to-planning}}

1. Clique no espaço de trabalho onde deseja criar um tipo de registro,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.
1. (Opcional) Clique em **Adicionar seção** para adicionar uma nova seção ao espaço de trabalho.
1. Clique em **Adicionar tipo de registro**.
1. (Condicional) Ao criar tipos de registro importando um arquivo do Excel ou CSV habilitado, clique em **Do zero**. Caso contrário, a caixa **Adicionar tipo de registro** será aberta.

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Atualize as seguintes informações:

   * Substitua &quot;Tipo de registro sem título&quot; pelo nome do seu tipo de registro futuro. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Descrição**: adicione mais informações sobre o tipo de registro.
   * Selecione uma cor e uma forma para o ícone associado ao tipo de registro. Faça o seguinte:
      * Selecione uma cor para identificar o novo tipo de registro. Esta é a cor do ícone do tipo de registro. O cinza é selecionado por padrão.
      * Selecione um ícone na lista ou comece a digitar o nome de um ícone para descrever o que ele representa e, em seguida, selecione-o quando ele for exibido. Este é o ícone do tipo de registro. Um ícone de arquivo é selecionado por padrão.

1. Clique em **Criar**.

   O cartão de tipo de registro é adicionado à seção e ao espaço de trabalho selecionados.
A Descrição do tipo de registro é exibida no cartão.

   ![](assets/record-type-card-with-description.png)

1. (Opcional) Passe o mouse sobre o cartão de tipo de registro, clique no ícone **Mais** ![](assets/more-menu.png) no canto superior direito e clique em **Editar** para modificar as informações sobre o tipo de registro.
1. (Opcional) Clique no cartão de tipo de registro para abrir a página de tipo de registro.

   ![](assets/operational-record-type-blank.png)

   A página de tipo de registro é exibida na exibição de tabela por padrão. As colunas da tabela são campos associados ao novo tipo de registro. Cada linha é um registro exclusivo que deve ser adicionado.

   >[!TIP]
   >
   >    Se você importar um tipo de registro de um arquivo Excel ou CSV, os registros também serão importados.

   Por padrão, os seguintes campos são exibidos nas colunas de exibição de tabela de um tipo de registro operacional:

   * Nome
   * Descrição
   * Data de início
   * Data Final
   * Status

1. (Opcional) Atualize o nome do tipo de registro no cabeçalho da página

   Ou

   Clique no ícone **Mais** ![](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Editar** para renomeá-lo ou alterar as informações sobre ele. Para obter mais informações, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Opcional) Clique em **+ Novo registro** para adicionar registros do tipo de registro selecionado. Para obter mais informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).
1. (Opcional) Clique no ícone **+** no canto superior direito da tabela para adicionar mais campos ao tipo de registro.

   Para obter mais informações sobre como criar campos, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

1. (Opcional) Clique na seta à esquerda do nome do tipo de registro, no cabeçalho, para voltar ao espaço de trabalho selecionado.

1. (Opcional) No espaço de trabalho, clique e mantenha pressionado um cartão de tipo de registro para arrastar e soltar o tipo de registro em um ponto desejado ou para movê-lo para outra seção.

   As alterações são salvas automaticamente.

   Para obter informações adicionais sobre como adicionar registros, excluir ou editar tipos de registro ou atualizar a exibição na página tipo de registro, consulte os seguintes artigos:

   * [Criar registros](/help/quicksilver/planning/records/create-records.md)
   * [Excluir tipos de registro](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Editar tipos de registro](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md)

## Criar tipos de registro importando um arquivo Excel ou CSV

>[!IMPORTANT]
>
>Essa funcionalidade está temporariamente desativada desde 21 de março de 2024. Ela será ativada posteriormente.

Considere o seguinte ao importar tipos de registro usando um arquivo Excel ou CSV:

* Cada folha do arquivo do Excel se torna um tipo de registro.
* As colunas de cada planilha se tornam os campos associados a cada tipo de registro.
* Os campos são exclusivos para seus respectivos tipos de registro.
* Cada linha em cada planilha se torna um registro exclusivo associado ao respectivo tipo de registro.
* Cada folha do arquivo Excel não deve exceder o seguinte:
   * 50.000 linhas
   * 500 colunas
* O arquivo do Excel não deve ter mais de 5 MB.
* Planilhas vazias não são suportadas.

Para importar tipos de registro usando um arquivo do Excel:

{{step1-to-planning}}

1. Clique no espaço de trabalho onde deseja criar tipos de registro,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.
1. Clique em **Adicionar tipo de registro**.
1. Clique em **Excel/CSV**.
1. Arraste e solte um arquivo Excel ou CSV salvo anteriormente no computador ou clique em **Selecionar um arquivo CSV ou Excel** para procurar um.
1. Clique em **Examine seus dados**.

   A caixa Preview and edit é exibida com as seguintes informações:

   * Os nomes das planilhas ou dos futuros tipos de registros são exibidos no painel esquerdo. Por padrão, o Workfront Planning seleciona um ícone e uma cor para cada novo tipo de registro.
   * A primeira folha ou tipo de registro é selecionado e os nomes dos campos associados a ela são exibidos como cabeçalhos de coluna. O tipo de cada campo é selecionado por padrão.
   * Cada linha representa um novo registro. Somente os primeiros 10 registros são exibidos na caixa Preview and edit.

   ![](assets/preview-and-edit-box.png)

1. (Opcional) Clique no nome de cada planilha no painel esquerdo para revisar as informações que ela contém.

   >[!NOTE]
   >
   >    Planilhas vazias não são suportadas e estão esmaecidas.


1. (Opcional) Clique no menu suspenso **Selecionar planilhas a serem importadas** e desmarque as planilhas que você não deseja importar.

   ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

   As planilhas desmarcadas são exibidas com um plano de fundo cinza.

1. Clique em **Importar** quando estiver pronto para importar o arquivo.

   As seguintes informações são importadas para o Workfront Planning:

   * Novos tipos de registro
   * Novos campos associados a cada tipo de registro
   * Novos registros associados a cada tipo de registro

   Você pode começar a gerenciar campos e registros nas páginas de tipos de registro.

   Todos os usuários com acesso ao Workfront Planning agora podem exibir e editar os tipos de registros importados e suas informações. <!--this will change with permissions-->

<!--## Connect record types with object types from another application

You can connect a record type and an object type from another application. This creates a read-only record type in Workfront Planning that corresponds to the object type in the other application. 

For example, you can create record types by connecting Workfront Planning record types with Workfront projects. As a result, the Workfront project object type is imported into Workfront Planning as a read-only record type. By default, the record type is named "Workfront Project." (********************)has this name changed? Lusine wanted to change it at some point***********)
    
You can import the following objects from the following applications: 

* From Workfront:

    * Projects
    * Portfolios
    * Programs
    * Company
    * Group

For more information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 
-->