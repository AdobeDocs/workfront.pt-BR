---
title: Gerenciar o layout da página de registro
description: É possível editar o layout da visualização de registro e da página no Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '2262'
ht-degree: 0%

---


# Gerenciar o layout da página de registros

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

É possível editar o layout da visualização de registro e da página no Adobe Workfront Planning.

A visualização do registro é uma exibição menor da página do registro exibida na exibição de um tipo de registro.

Quando você altera o layout de uma visualização e página de registro, as alterações afetam as caixas de visualização e as páginas de detalhes de todos os registros do mesmo tipo.

Este artigo descreve como alterar o layout e a aparência de uma caixa de visualização de registro ou de uma página de registro. Para obter informações sobre como editar registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

Você deve criar tipos de registro e registros antes de começar a editar páginas de registro.

Para obter informações, consulte os seguintes artigos:

* [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md)

* [Criar registros](/help/quicksilver/planning/records/create-records.md)

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
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
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
<p>Any</p>
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
   <td>
   <p>Standard</p>
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
   <td>
   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->

## Considerações sobre a edição de páginas de registro

* Por padrão, os detalhes e as páginas de visualização de um registro exibem todos os campos associados ao registro.

* Não é possível adicionar novos campos a um registro na página de visualização ou de detalhes. Você deve adicionar novos campos na exibição de tabela para exibi-los nas páginas de visualização e detalhes.

* É possível adicionar seções a uma visualização de registro ou página de detalhes para organizar as informações por critérios comuns e facilitar a localização.

* As alterações a seguir afetam todos os registros do mesmo tipo e são visíveis para todos os usuários que acessam esses registros:

   * Reorganização de campos
   * Adição ou remoção de seções

* As alterações de exibição feitas na visualização do registro ficam imediatamente visíveis na página de detalhes do registro. As alterações feitas na página de registro também estão visíveis na caixa de visualização do registro.

* Adicionar uma imagem de capa ou uma miniatura a um registro não faz parte do layout geral da pré-visualização ou página do registro. É possível adicionar imagens de capa ou miniaturas exclusivas a cada registro. Para obter informações, consulte [Adicionar uma imagem de capa a um registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) e [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Adicionar seções a uma visualização ou página de registro

Considere o seguinte ao adicionar seções a uma página de registro:

* Não há limite para quantas seções você pode ter em uma página.
* Você não pode ter uma seção vazia. Você deve ter pelo menos um campo em uma seção.
* Você pode arrastar e soltar campos de uma seção para outra. Para obter mais informações, consulte a seção [Reorganizar campos na página de visualização ou detalhes do registro](#rearrange-fields-in-the-record-preview-or-details-page) neste artigo.
* Ao remover todos os campos de uma seção, ela é automaticamente excluída e não pode ser recuperada.

Para adicionar uma seção a uma visualização de registro ou página:

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique no nome de um registro

   Ou

   Na exibição de tabela, clique no ícone **Abrir detalhes** ![Ícone Abrir detalhes no campo de nome de tabela](assets/open-details-icon-in-table-name-field.png) na primeira coluna.

   A visualização do registro é aberta na exibição.

   ![Caixa Detalhes](assets/details-box.png)

1. (Opcional) Clique no ícone **Abrir em nova guia** ![Abrir detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.

   A página de registro é aberta. A guia Detalhes é aberta por padrão.

   ![Página de detalhes](assets/details-page.png)

1. Na guia **Detalhes** da visualização ou página do registro, passe o mouse sobre o espaço em branco à esquerda dos campos e clique no ícone **Adicionar seção** ícone ![Adicionar seção](assets/add-section-icon.png) para adicionar uma seção.
1. Clique dentro do nome da seção e substitua **Seção sem título** por um nome e clique em Enter. Os campos exibidos abaixo da seção fazem parte automaticamente da nova seção.
1. Comece a arrastar e soltar campos na nova seção, conforme descrito na seção [Reorganizar campos na página de visualização de registro ou de detalhes](#rearrange-fields-in-the-record-preview-or-details-page) deste artigo.

1. (Opcional) Passe o mouse sobre o nome de uma seção e clique no menu **Mais** ![Mais menu](assets/more-menu.png).

   ![Mais opções de menu para a seção na página de registro](assets/more-menu-options-for-section-on-record-page.png)
1. (Opcional) Siga um destes procedimentos para editar a seção:

   * Clique em **Renomear** para renomear a seção

     >[!TIP]
     >
     > É possível renomear uma seção em linha clicando no nome.

   * Clique em **Mover para cima** para mover a seção uma posição para cima

     Ou

     Clique em **Mover para baixo** para mover a seção uma posição para baixo.
Todos os campos na seção se movem com a seção.

   * Clique em **Excluir** para excluir a seção. A seção é excluída e não pode ser recuperada. Todos os usuários que acessarem os registros desse tipo não visualizarão mais a seção excluída.

1. Clique na seta apontando para baixo à esquerda do nome de uma seção para recolhê-la ou na seta apontando para a direita para expandi-la.
Todas as seções são expandidas por padrão.

1. (Opcional) Clique no ícone de **captura** ![ícone de captura](assets/grab-icon.png) à esquerda do nome de uma seção e arraste-o e solte-o no local desejado.

   A nova posição da seção atualiza na pré-visualização e na página de todos os registros do mesmo tipo para todos os usuários que visualizam os registros.

   Todas as alterações nas seções e na ordem dos campos são salvas automaticamente.

1. (Opcional) Clique no menu **Exportar** ![ícone Exportar na página de detalhes do registro](assets/export-icon-in-record-details-page.png) para exportar a guia Detalhes para um arquivo do Word ou PDF. Para obter mais informações, consulte [Exportar os detalhes de um registro](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Opcional) Clique na guia **Conexões** ao lado da guia **Detalhes**. Talvez seja necessário clicar em **Mais** antes da guia **Conexões**.

   Todos os registros ou objetos conectados ao registro selecionado são exibidos sob os nomes do tipo de registro ou do aplicativo ao qual pertencem.

   ![Guia Conexões em registro no Workfront Planning](assets/connections-tab-on-record-in-workfront-planning.png)

1. (Opcional) Selecione a configuração **Mostrar todos os registros** no canto superior direito da guia Conexões. Todos os tipos de registros conectados são exibidos, incluindo aqueles que ainda não têm nenhum registro conectado. Por padrão, a opção é desmarcada e os tipos de registro sem registros conectados são ocultos.

1. (Opcional) Clique em **Conectar** para adicionar mais registros aos tipos de registros conectados. Para obter mais informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

1. (Opcional) Passe o mouse sobre um cartão de registro, em seguida, clique no ícone de desconectar registro **-** e clique em **Desconectar**. <!--this is copied to the Manage the Planning page in Workfront article; update in both articles-->
As seguintes situações ocorrem:
   * O registro não está mais conectado ao objeto Workfront.
   * O objeto Workfront também é removido do campo conectado do registro do Workfront Planning.
   * Os valores dos campos de pesquisa do Workfront conectados ao registro do Planning também são excluídos.

## Reorganizar campos na guia Detalhes do registro

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique no nome de um registro

   Ou

   Na exibição de tabela, clique no ícone **Abrir detalhes** ![Ícone Abrir detalhes no campo de nome de tabela](assets/open-details-icon-in-table-name-field.png) na primeira coluna.

   A visualização do registro é aberta na exibição.

   ![Caixa Detalhes](assets/details-box.png)

1. (Opcional) Clique no ícone **Abrir em nova guia** ![Abrir caixa de detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.

   A guia **Detalhes** do registro é aberta por padrão.

   ![Página de detalhes](assets/details-page.png)

1. Na guia **Detalhes** do registro, clique no ícone **Capturar** ![Ícone Capturar](assets/grab-icon.png) à esquerda de um nome de campo e arraste-o e solte-o no local desejado.

   >[!TIP]
   >
   >Você pode arrastar e soltar campos em outra seção.
   >Você deve ter pelo menos um campo em uma seção.
   >

   A nova posição do campo é atualizada na pré-visualização e na página de todos os registros do mesmo tipo para todos os usuários que visualizam os registros.

   Todas as alterações no layout da visualização do registro ou na página são salvas automaticamente.

## Adicionar uma página Registros conectados a um registro

Você pode exibir informações de registros ou objetos conectados adicionando uma guia de uma página Registros conectados a um registro. Isso adiciona os registros conectados em uma exibição de tabela à guia.

Considere o seguinte ao adicionar uma página Registros conectados a um registro:

* Você pode adicionar uma página Registros conectados a um registro depois de conectar tipos de registro ou de objeto ao tipo de registro a partir da exibição de tabela de um tipo de registro.

* É possível adicionar uma página Registros conectados a partir da área de visualização de um registro ou da página do registro.

* As páginas de registros conectados exibem somente os objetos ou registros conectados de um tipo de objeto ou registro em uma exibição de tabela. A página não exibe todos os registros desse tipo.

* Você pode adicionar páginas Registros conectados para os seguintes tipos de registro ou objeto conectados:

   * Tipos de registro do Workfront Planning
   * Projetos, programas, portfólios, grupos ou empresas do Workfront. Você pode visualizar os objetos conectados do Workfront mesmo quando não tem permissões para acessá-los no Workfront.

  >[!NOTE]
  >
  > Não é possível adicionar uma página Registros conectados para registros conectados do AEM Assets.

Para adicionar uma página Registros conectados:

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
         >Você pode selecionar mais de um registro ou objeto para excluí-los.
     
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

1. (Opcional) Passe o mouse sobre o nome da guia da página Registros conectados, clique em **Mais** ![Mais menu](assets/more-menu.png) e em **Excluir** para remover para a guia.

<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



