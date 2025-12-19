---
title: Adicionar uma Página de Registros Conectados a um Registro
description: Você pode exibir informações de registros ou objetos conectados adicionando uma guia de uma página Registros conectados a um registro. Isso adiciona os registros conectados em uma exibição de tabela à guia.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 66dd7354f3723e266b77cb2f367b09c022e8c95e
workflow-type: tm+mt
source-wordcount: '2745'
ht-degree: 0%

---


# Adicionar uma página Registros conectados a um registro

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Você pode exibir informações de registros ou objetos conectados adicionando uma guia de uma página Registros conectados a um registro no Adobe Workfront Planning. Isso adiciona os registros conectados em uma exibição de tabela à guia.

Considere o seguinte ao adicionar uma página Registros conectados a um registro:

* Você pode adicionar uma página Registros conectados a um registro depois de conectar tipos de registro ou de objeto ao tipo de registro a partir da exibição em tabela.

* É possível adicionar uma página Registros conectados a partir da área de visualização de um registro ou da página do registro.

* <span class="preview">Você só pode ter uma página de registros conectada para um tipo de registro específico.</span>

  <span class="preview">Por exemplo, se você criar uma página de registros conectada para uma campanha e quiser exibir suas Personas conectadas, poderá ter apenas uma página de registros conectada para Personas.</span>

* As páginas de registros conectados exibem somente os objetos ou registros conectados de um tipo de objeto ou registro. A página não exibe todos os registros desse tipo.

* Dependendo do tipo de objeto ou de registro exibido na página de registros conectados, você poderá exibi-los usando as seguintes views:

   * Você pode exibir registros conectados do Planning nas seguintes exibições:
      * Tabela
      * <span class="preview">Linha do tempo</span>
      * <span class="preview">Calendário</span>
   * Você pode exibir projetos conectados do Workfront na exibição de lista.


<!--replace the above bullet with this: 

* You can display the objects in a connected records page in the following types of views:

   * Table
   * <span class="preview">Timeline</span>
   * <span class="preview">Calendar</span>

* <span class="preview">You can create one page per one object or record type. For example, you cannot create two connected record pages for connected projects or tactics.</span>

-->

* Você pode adicionar páginas Registros conectados para os seguintes tipos de registro ou objeto conectados:

   * Tipos de registro do Workfront Planning
   * Projetos Workfront

     Você pode visualizar os projetos conectados do Workfront mesmo quando não tem permissões para acessá-los no Workfront.

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
   <p>Para obter informações, consulte <a href="https://experienceleague.adobe.com/pt-br/docs/genstudio-for-performance-marketing/user-guide/get-started">Introdução ao Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
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

Você deve primeiro conectar tipos de registro a outros tipos de registro ou projetos Workfront antes de adicionar uma página de registros conectada a um registro.

1. Clique no nome do registro para abri-lo a partir de qualquer exibição de uma página do tipo de registro.
1. Clique em **Adicionar página** de uma das seguintes áreas:

   * A janela de visualização do registro
   * A página de detalhes do registro, após clicar no ícone **Abrir em nova guia** ![Abrir detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) no canto superior direito da página de visualização.

   A caixa **Criar página** é aberta.

   ![Adicionar modal da página Registros conectados](assets/add-connection-view-page-modal.png)

1. Adicione o **Nome da página**, clique em **Página de registros conectados** para o **Tipo de página** e clique em **Criar**.
1. (Opcional) Clique no nome de um registro ou tipo de objeto conectado na lista ou procure-o e, em seguida, clique nele quando ele for exibido na lista para criar a página para esse registro ou tipo de objeto.

   >[!TIP]
   >
   ><span class="preview">Você pode criar uma página de registros conectada por tipo de registro. Se um tipo de registro conectado já tiver uma página, ele não será mais exibido como uma opção.</span>


1. (Opcional e condicional) Se mais de um campo conectado do tipo de registro ou objeto para o qual você está criando a página for exibido, clique no campo cujos registros ou objetos você deseja exibir na página de registros conectados da lista **Selecionar campo de referência**.

   ![Selecionar lista de campos de referência](assets/select-reference-field-list-on-connected-records-page.png)

   Uma das seguintes páginas é adicionada à página de registros conectados:

   * A exibição de tabela de um tipo de registro
   * A exibição em lista de um tipo de objeto de projeto

   Os registros ou projetos conectados ao registro atual são exibidos na exibição de tabela ou lista.

   >[!TIP]
   >
   >Você deve adicionar registros conectados na área Tabela ou Detalhes de um registro antes de exibi-los em uma página de registros conectados. Caso contrário, a tabela ou lista estará vazia.

   Os primeiros cinco campos dos registros conectados são exibidos por padrão. <!--No lookup fields display by default.-->

   ![Exibição da tabela conectada ao público-alvo nos detalhes da campanha](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Condicional) Dependendo do tipo de registro exibido na página de registro conectado, siga um destes procedimentos:

   * Gerenciar registros do Planning
Para obter informações, consulte a seção [Gerenciar a página de registros conectados dos registros do Planning](#manage-the-connected-records-page-for-planning-records) neste artigo.
   * Gerenciar projetos do Workfront
Para obter informações, consulte a seção [Gerenciar a página de registros conectados de projetos do Workfront](#manage-the-connected-records-page-for-workfront-projects) neste artigo.

1. (Opcional) Clique duas vezes no nome da guia **Página de registros conectados**

   Ou

   Passe o mouse sobre o nome da guia, em seguida, clique em **Mais** ![Mais menu](assets/more-menu.png) e em **Renomear** para renomear para a nova guia de página de registros conectados.


   <!--1. <span class="preview">(Optional) Click the dropdown menu to the right of the view name, then click **New view** to add a view. For more information, see the section [Manage multiple views from the connected records page](#manage-multiple-views-from-the-connected-records-page) in this article. </span>-->

1. (Opcional) Passe o mouse sobre o nome da guia da página de registros conectados, clique em **Mais** ![Mais menu](assets/more-menu.png) e em **Excluir** para remover para a guia.

### Gerenciar a página de registros conectados para registros do Planning

O gerenciamento da página de registros conectados para registros do Planning difere dependendo do ambiente usado.

#### Gerenciar a página de registros conectados para registros do Planning no ambiente de Produção

Ao criar uma página de registros conectados para registros conectados do Planning no ambiente de Produção, faça o seguinte: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. Vá para uma página de tipo de registro e clique no nome de um registro. Isso abre a página de visualização do registro.
1. Clique na guia de uma página de registros conectados que exibe registros do Planning.
Os registros conectados ao registro selecionado são exibidos na exibição de tabela.
1. Clique em **Conectar** na parte inferior da exibição de tabela para conectar registros existentes, selecione-os na caixa de conexão e clique fora da caixa para fechá-la. Os registros são adicionados automaticamente à tabela e conectados ao registro selecionado. Os registros devem existir antes que você possa adicioná-los.

   Para obter mais informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Edite quaisquer informações dos registros conectados em linha na exibição de tabela.
1. Passe o mouse sobre o nome de um registro conectado, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png)

   Ou

   Selecione um dos registros e clique em uma das seguintes opções na barra azul na parte inferior da lista:

   * **Exibir** para abrir a página de registro em uma nova guia
   * **Copiar link** para copiar um link para a página de registro
   * **Editar miniatura** para abrir a caixa **Gravar miniatura** e editar a imagem de miniatura do registro
   * **Duplicar** para duplicar o registro conectado. O registro duplicado também está conectado ao registro atual.
   * **Insira o registro acima ou abaixo** para adicionar novos registros ao tipo de registro conectado. Os novos registros adicionados aqui também serão conectados ao registro atual. Essa opção não está disponível na barra azul ao selecionar um registro na tabela.
   * **Excluir** para excluir o registro. A exclusão de um registro conectado o exclui de seu tipo de registro e de qualquer lugar onde o registro estiver conectado. Os registros excluídos são movidos para o compartimento **Recentemente excluídos** de seus tipos de registro.

     Para obter informações sobre como editar registros no modo de exibição de tabela, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >É possível selecionar mais de um registro ou objeto para excluí-los.

1. Editar em linha qualquer um dos registros na tabela na página de registros conectados.
1. Use qualquer um dos seguintes elementos de exibição na barra de ferramentas de uma página de registro conectada para gerenciar a exibição de tabela:

   * **Filtros**
   * **Classificar**
   * **Agrupamento**
   * **Campos**, para exibir, ocultar ou reorganizar campos
   * **Altura da linha**
   * **Pesquisa**

   Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Não é possível criar, editar ou excluir campos na exibição de tabela de uma guia de registro conectado.

<div class="preview">

#### Gerenciar a página de registros conectados para registros do Planning no ambiente de Pré-visualização

Ao criar uma página de registros conectados para registros conectados do Planning no ambiente de Visualização, faça o seguinte: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

1. Vá para uma página de tipo de registro e clique no nome de um registro. Isso abre a página de visualização do registro.
1. Clique na guia de uma página de registros conectados que exibe registros do Planning.
Os registros conectados ao registro selecionado são exibidos na exibição de tabela.
1. Clique em **Conectar registros** no canto superior direito da página de registro conectada para conectar registros existentes, selecione-os na caixa de conexão e clique fora da caixa para fechá-la. Os registros são adicionados automaticamente à tabela e conectados ao registro selecionado. Os registros devem existir antes que você possa adicioná-los.

   Para obter mais informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Clique em **Nova linha** na parte inferior da tabela para adicionar novos registros. Os novos registros são conectados automaticamente aos registros selecionados.
1. Edite quaisquer informações dos registros conectados em linha na exibição de tabela.
1. Passe o mouse sobre o nome de um registro conectado, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png)

   Ou

   Selecione um dos registros e clique em uma das seguintes opções na barra azul na parte inferior da lista:

   * **Exibir** para abrir a página de registro em uma nova guia
   * **Copiar link** para copiar um link para a página de registro
   * **Editar miniatura** para abrir a caixa **Gravar miniatura** e editar a imagem de miniatura do registro
   * **Duplicar** para duplicar o registro conectado. O registro duplicado também está conectado ao registro atual.
   * **Insira o registro acima ou abaixo** para adicionar novos registros ao tipo de registro conectado. Os novos registros adicionados aqui também serão conectados ao registro atual. Essa opção não está disponível na barra azul ao selecionar um registro na tabela.
   * **Excluir** para excluir o registro. A exclusão de um registro conectado o exclui de seu tipo de registro e de qualquer lugar onde o registro estiver conectado. Os registros excluídos são movidos para o compartimento **Recentemente excluídos** de seus tipos de registro.

     Para obter informações sobre como editar registros no modo de exibição de tabela, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >É possível selecionar mais de um registro ou objeto para excluí-los.

1. Editar em linha qualquer um dos registros na tabela na página de registros conectados.
1. Use qualquer um dos seguintes elementos de exibição na barra de ferramentas de uma página de registro conectada para gerenciar a exibição de tabela:

   * **Filtros**
   * **Classificar**
   * **Agrupamento**
   * **Campos**, para exibir, ocultar ou reorganizar campos
   * **Altura da linha**
   * **Pesquisa**

   Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >Não é possível criar, editar ou excluir campos na exibição de tabela de uma guia de registro conectado.
1. Clique no menu suspenso modos de exibição e em **Novo modo de exibição** para adicionar um novo modo de exibição à página. Em seguida, faça o seguinte:
   1. Adicione um **Nome da exibição**.
   1. Na área **Tipo de exibição**, selecione um dos seguintes tipos de exibições:

      * Tabela
Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md)
      * Linha do tempo
Para obter informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).
      * Calendário
Para obter informações, consulte [Gerenciar a exibição de calendário](/help/quicksilver/planning/views/manage-the-calendar-view.md).

        Para obter mais informações, consulte a seção [Gerenciar várias exibições da página de registros conectados](#manage-multiple-views-from-the-connected-records-page) neste artigo.

   1. Clique em **Criar**.
Uma nova exibição é adicionada ao menu suspenso de exibições.
   1. (Opcional) Passe o mouse sobre o nome de um modo de exibição criado, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e, em seguida, clique em uma das seguintes opções:
      * **Renomear**, para adicionar um novo nome para o modo de exibição.
      * **Compartilhar**


        Para obter mais informações, consulte [Compartilhar modos de exibição](/help/quicksilver/planning/access/share-views.md).

        >[!NOTE]
        >
        >Não é possível compartilhar uma exibição de Sistema criada pela Workfront.

      * **Excluir**
Para obter informações, consulte [Excluir exibições de registros](/help/quicksilver/planning/views/delete-record-views.md).

        ![](assets/view-more-menu-projects-connected-records-page.png)

</div>


<!--No longer possible: 1. (Optional and conditional) When you create a connected records page for the following Workfront object types:
         * Portfolios
         * Programs
         * Groups
         * Companies
      Do any of the following in the table view of the connected records page: 
      * Click the name of a object. This opens the object's page in a new tab. 
      * Click **Connect** at the bottom of the table view to connect existing objects, select them from the connection box, then click outside the box to close it. The objects are automatically added to the table. The objects must exist before you can add them.
      For more information, see [Connect records](/help/quicksilver/planning/records/connect-records.md).
      * Select one of the objects in the table view, then click one of the following options in the blue bar at the bottom of the list: 
      * **View** to open the record page in a new tab
      * **Copy link** to copy a link to the record page
      * **Disconnect** to disconnect the object from the record you are viewing. 
      TIP      
      You can select more than one record or object to disconnect them.
      -->

### Gerenciar a página de registros conectados de projetos do Workfront

Ao criar uma página de registros conectados para projetos conectados do Workfront, faça o seguinte:

1. Vá para uma página de tipo de registro e clique no nome de um registro. Isso abre a página de visualização do registro.
1. Clique na guia de uma página de registros conectada que exibe projetos Workfront.
Os projetos conectados ao registro selecionado são exibidos na exibição de lista.
1. Clique em **Conectar registros** no canto superior direito da página de registros conectada para conectar projetos existentes.

   Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Editar informações do projeto em linha na tabela.
1. Clique em **Nova linha** para criar um projeto sem um modelo. O novo projeto é automaticamente conectado ao registro atual.

   Para obter mais informações, consulte [Criar objetos do Workfront no Workfront Planning à medida que você os conecta a registros](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
1. Passe o mouse sobre um nome de projeto na lista e clique no menu **Mais** [Mais menu](assets/more-menu.png)

   Ou

   Selecione um ou mais projetos, observe a barra azul na parte inferior da lista e clique em uma das seguintes opções:

   * **Excluir** para excluir o projeto. A exclusão de um projeto o desconecta do registro e o move para a Lixeira do Workfront. Os administradores do Workfront podem recuperar projetos excluídos até 30 dias após a exclusão.
   * **Desconectar** para desconectar o projeto do registro. Desconectar um projeto o remove e todos os valores de seus campos de pesquisa do registro atual.

     >[!TIP]
     >
     >Você pode selecionar mais de um projeto para desconectá-los ou excluí-los.
1. Clique no menu suspenso modos de exibição e em **Novo modo de exibição** para adicionar um novo modo de exibição à página. Em seguida, faça o seguinte:
   1. Adicione um **Nome da exibição**.
   1. Selecione **Lista** na área **Tipo de exibição**.
   1. Clique em **Criar**.
Uma nova exibição em lista é adicionada ao menu suspenso de exibições.

      Para obter mais informações, consulte a seção [Gerenciar várias exibições da página de registros conectados](#manage-multiple-views-from-the-connected-records-page) neste artigo.

   1. (Opcional) Passe o mouse sobre o nome de um modo de exibição criado, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e, em seguida, clique em uma das seguintes opções:
      * **Renomear**, para adicionar um novo nome para o modo de exibição.
      * <span class="preview">**Compartilhar**</span>

        Para obter mais informações, consulte [Compartilhar modos de exibição](/help/quicksilver/planning/access/share-views.md).

        >[!NOTE]
        >
        >Não é possível compartilhar uma exibição de Sistema criada pela Workfront.

      * **Excluir**
Para obter informações, consulte [Excluir exibições de registros](/help/quicksilver/planning/views/delete-record-views.md).

        ![](assets/view-more-menu-projects-connected-records-page.png)

   1. Clique no ícone **Filtro** ![Ícone Filtro](assets/filter-icon.png) e use o filtro para exibir projetos específicos.

      >[!TIP]
      >
      ><span class="preview">Para campos do tipo pessoas, como **Proprietário** ou **Patrocinador**, você pode usar um curinga para mostrar projetos em que o usuário conectado está atribuído a essas funções.</span>
      >
      >![Filtrar com curinga de usuário para a página de registros conectados ao projeto](assets/filter-with-user-wildcard-project-connected-records-page.png)
      >

   1. Clique no ícone **Colunas** ![Colunas](assets/columns-icon.png) para ocultar ou mostrar colunas na lista.
   1. Clique no ícone **+** no canto superior direito do modo de exibição de tabela para adicionar campos existentes à tabela. Os campos devem existir antes que você possa adicioná-los.

      A caixa **Gerenciador de colunas** é aberta. Faça o seguinte:

      1. Procure um campo de objeto existente na coluna **Disponível** e clique em **+** à direita do nome do campo para adicioná-lo à coluna **Selecionado**.

         Os campos selecionados são adicionados à exibição de tabela na página de registros conectados.
      1. Clique em **-** à direita de um campo na coluna **Selecionado** para removê-lo da exibição de tabela.
      1. Clique em **Salvar** para salvar a exibição de tabela da página de registro conectada.


<div class="preview">

## Gerenciar várias exibições na página de registros conectados

Você pode adicionar e gerenciar vários tipos de exibição na página Registros conectados de um registro.

As exibições criadas na página Registros conectados de um tipo de registro estão disponíveis em todo o Workfront Planning onde a página do tipo de registro é exibida. As exibições criadas para o mesmo tipo de registro em qualquer outro lugar no Workfront Planning também podem ser acessadas em todas as páginas de registros conectados desse tipo de registro.

Para gerenciar várias exibições na página registros conectados:

1. Na página de registros conectados de um registro, clique no menu suspenso à direita do nome da exibição e, em seguida, clique em **Nova exibição** para adicionar uma exibição e selecione uma das seguintes opções:

   * **Tabela**. Para obter mais informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).
   * **Linha do tempo**. Para obter mais informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).
   * **Calendário**. Para obter mais informações, consulte [Gerenciar a exibição de calendário](/help/quicksilver/planning/views/manage-the-calendar-view.md).

1. (Opcional) Passe o mouse sobre o nome de um modo de exibição na página Registros conectados, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e, em seguida, clique em um dos seguintes: **&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;*** verifique se todos são possíveis **&#x200B;**&#x200B;**&#x200B;***

   * **Renomear**
   * **Compartilhar**. Para obter mais informações, consulte [Compartilhar modos de exibição](/help/quicksilver/planning/access/share-views.md).

   >[!TIP]
   >
   >O compartilhamento de exibições das páginas de registros Conectados as torna acessíveis aos usuários em todas as áreas do Workfront Planning onde a exibição é exibida.
   >Além disso, se uma exibição for compartilhada de qualquer outra área do Workfront Planning, ela também estará disponível para os mesmos usuários nas páginas Registros conectados.

   * **Exportar**
   * **Duplicar**. Para obter mais informações, consulte [Duplicar exibições de registros](/help/quicksilver/planning/views/duplicate-record-views.md).

     >[!TIP]
     >
     >Duplicar uma exibição das páginas Registros conectados a torna disponível em todas as outras áreas do planejamento do Workfront, ao exibir os mesmos tipos de registro.

</div>