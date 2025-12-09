---
title: Adicionar uma Página de Registros Conectados a um Registro
description: Você pode exibir informações de registros ou objetos conectados adicionando uma guia de uma página Registros conectados a um registro. Isso adiciona os registros conectados em uma exibição de tabela à guia.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 1%

---


# Adicionar uma página Registros conectados a um registro

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Você pode exibir informações de registros ou objetos conectados adicionando uma guia de uma página Registros conectados a um registro. Isso adiciona os registros conectados em uma exibição de tabela à guia.

Considere o seguinte ao adicionar uma página Registros conectados a um registro:

* Você pode adicionar uma página Registros conectados a um registro depois de conectar tipos de registro ou de objeto ao tipo de registro a partir da exibição de tabela de um tipo de registro.

* É possível adicionar uma página Registros conectados a partir da área de visualização de um registro ou da página do registro.

* As páginas de registros conectados exibem somente os objetos ou registros conectados de um tipo de objeto ou registro em uma exibição de tabela. A página não exibe todos os registros desse tipo.

* Você pode adicionar páginas Registros conectados para os seguintes tipos de registro ou objeto conectados:

   * Tipos de registro do Workfront Planning
   * Projetos, programas, portfólios, grupos ou empresas do Workfront. Você pode visualizar os objetos conectados do Workfront mesmo quando não tem permissões para acessá-los no Workfront.

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
<p>Qualquer Workfront e qualquer pacote do Planning</p>
<p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
<tr>
<td> 
   <p> Produtos adicionais</p> </td> 
   <td> 
   <p> Além do Adobe Workfront, você deve ter o seguinte, se quiser adicionar uma página de registro conectada para objetos dos seguintes aplicativos:</p>
   <ul><li><p>Uma licença do Adobe Experience Manager Assets e uma integração entre o AEM Assets e o Workfront para conectar o AEM Assets aos tipos de registro do Planning.</p>
   <p>Para obter informações, consulte <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront para Experience Manager Assets e Assets Essentials: índice do artigo</a>. </p></li>
   <li><p> Uma licença da Adobe GenStudio for Performance Marketing para conectar tipos de registros com marcas da GenStudio</p>
   <p>Para obter informações, consulte <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started">Introdução ao Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Permissões de objeto</p></td>
   <td>
   <p>Contribuir com ou mais permissões para um espaço de trabalho e tipo de registro </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> 
  </td>
  </tr>   
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Adicionar uma página Registros conectados a um registro

1. Clique no nome do registro para abri-lo a partir de qualquer exibição de uma página do tipo de registro.
1. Clique em **Adicionar página** de uma das seguintes áreas:

   * A janela de visualização do registro
   * A página de detalhes do registro, após clicar no ícone **Abrir em nova guia** ![Abrir detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) no canto superior direito da página de visualização.

   A caixa **Criar página** é aberta.

   ![Adicionar modal da página Registros conectados](assets/add-connection-view-page-modal.png)

1. Adicione o **Nome da página**, clique em **Página de registros conectados** e em **Criar**.

   Uma nova página de registros conectados é adicionada como uma nova guia à página do registro.

   Os registros conectados ao registro atual são exibidos na exibição de tabela.

   >[!TIP]
   >
   >Você deve adicionar registros conectados na área Tabela ou Detalhes de um registro antes de exibi-los em uma página de registros conectados.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   Os primeiros cinco campos dos registros conectados são exibidos por padrão. <!--No lookup fields display by default.-->

   ![Exibição da tabela conectada ao público-alvo nos detalhes da campanha](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Opcional) Procure ou clique no nome de um registro ou tipo de objeto conectado na lista.

1. (Opcional e condicional) Na exibição de tabela da página de registros conectados, siga um destes procedimentos ao exibir registros conectados do Planning ou quaisquer objetos do Workfront, exceto projetos: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Clique no nome de um registro. A página do registro será aberta em uma nova guia.

   * Clique em **Conectar** na parte inferior da exibição de tabela para conectar mais registros e em fora da caixa de conexão para fechá-la. Os novos registros são adicionados automaticamente à tabela.

     Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
   * Edite quaisquer informações dos registros conectados em linha na exibição de tabela.

   * Passe o mouse sobre o nome de um registro conectado, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png)

     Ou

     Selecione um dos registros e clique em uma das seguintes opções na barra azul na parte inferior da lista:

      * **Exibir** para abrir a página de registro em uma nova guia
      * **Copiar link** para copiar um link para a página de registro
      * **Editar miniatura** para abrir a caixa **Gravar miniatura** e editar a imagem de miniatura do registro
      * **Duplicar** para duplicar o registro conectado. O registro duplicado também está conectado ao registro atual.
      * **Insira o registro acima ou abaixo** para adicionar novos registros ao tipo de registro conectado. Os novos registros adicionados aqui também serão conectados ao registro atual. Essa opção não está disponível na barra azul ao selecionar um registro na tabela.
      * **Excluir** para excluir o registro. A exclusão de um registro conectado o exclui de seu tipo de registro e de qualquer lugar onde o registro estiver conectado.

     Para obter informações sobre como editar registros no modo de exibição de tabela, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >É possível selecionar mais de um registro ou objeto para excluí-los.

   * Editar em linha qualquer um dos registros do Planning na tabela na página Registros conectados.

     Todos os outros objetos do Workfront são exibidos em uma exibição de tabela somente leitura e não é possível editá-los.

1. (Opcional e condicional) Na exibição de tabela da página de registros conectados, siga um destes procedimentos ao exibir projetos conectados do Workfront:

   * Clique em **Conectar registros** no canto superior direito da página de registros conectada para conectar projetos existentes.

   Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
   * Editar informações do projeto em linha na tabela.
   * Clique em **Nova linha** para criar um projeto sem um modelo. O novo projeto é conectado ao registro atual imediatamente.

     Para obter mais informações, consulte [Criar objetos do Workfront no Workfront Planning à medida que você os conecta a registros](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * Passe o mouse sobre um projeto e clique no menu **Mais** [Mais menu](assets/more-menu.png)

     Ou

     Selecione um ou mais projetos, observe a barra azul na parte inferior da lista e clique em uma das seguintes opções:

      * **Excluir** para excluir o projeto. A exclusão de um projeto o desconecta do registro e o move para a Lixeira do Workfront.
      * **Desconectar** para desconectar o projeto do registro. Desconectar um projeto o remove e todos os valores de seus campos de pesquisa do registro atual.

1. (Opcional) Clique duas vezes no nome da guia **Página de registros conectados**

   Ou

   Passe o mouse sobre o nome da guia, em seguida, clique em **Mais** ![Mais menu](assets/more-menu.png) e em **Renomear** para renomear para a nova guia Modo de Exibição Conectado.
1. (Opcional) Use qualquer um dos seguintes elementos de exibição na barra de ferramentas de uma página de registro conectada para gerenciar a exibição de tabela:

   * Filtros
   * Ordenar
   * Agrupamento
   * Campos, para exibir, ocultar ou reorganizar campos
   * Altura da linha
   * Pesquisar

   Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Não é possível criar, editar ou excluir campos na exibição de tabela de uma guia de registro conectado.

   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Opcional) Passe o mouse sobre o nome da guia da página Registros conectados, clique em **Mais** ![Mais menu](assets/more-menu.png) e em **Excluir** para remover para a guia.

<!--
<div class="preview">

## Manage multiple views from the connected records page

You can add and manage views from the connected records page of a record. 

1. From the connected records page of a record, click the dropdown menu to the right of the view name, then click **New view** to add a view, then select from the following options: 

   * **Table**. For more information, see [Manage the table view](/help/quicksilver/planning/views/manage-the-table-view.md). 
   * **Timeline**. For more information, see [Manage the timeline view](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendar**. For more information, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md). 

1. (Optional) Hover over the name of a view in the Connected records page, then click the **More** menu ![More menu](assets/more-menu.png), then click one of the following: *************check to make sure these are all possible*********

   * **Rename**
   * **Share**. For more information, see [Share views](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >Sharing views from Connected records pages makes them accessible to users in all areas of Workfront Planning where the view displays. 
   >Also, if a view is shared from any other area of Workfront Planning, it is also available to the same users in Connected records pages. 

   * **Export** 
   * **Duplicate**. For more information, see [Duplicate record views](/help/quicksilver/planning/views/duplicate-record-views.md).

      >[!TIP]
      >
      >Duplicating a view from Connected records pages makes it available in all other areas of Workfornt planning, when viewing the same record types. 

</div> -->