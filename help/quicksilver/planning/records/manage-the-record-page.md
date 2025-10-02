---
title: Gerenciar o layout da página de registro
description: É possível editar o layout da visualização de registro e da página no Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '2458'
ht-degree: 1%

---


# Gerenciar o layout da página de registros

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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

+++ Expanda para visualizar os requisitos de acesso. 

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
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td>
   <td>
<p>Qualquer</p>
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td>
   <td>
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar o Workfront Planning.</p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Standard</p>
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
   <td>
   <p>Permissões do Contribute ou superior para um espaço de trabalho e tipo de registro </a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> 
  </td>
  </tr>
 </tbody>
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


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

Você pode exibir informações de registros ou objetos conectados adicionando uma guia de uma página Registros conectados a um registro.

As informações dos registros conectados podem ser editadas na exibição de tabela. As informações dos objetos conectados de outro aplicativo não são editáveis na exibição de tabela.

Considere o seguinte ao adicionar uma página Registros conectados a um registro:

* Você pode adicionar uma página Registros conectados a um registro depois de conectar tipos de registro ou de objeto ao tipo de registro a partir da exibição de tabela de um tipo de registro.

* No ambiente de Produção, não é possível adicionar uma página Registros conectados a partir da pré-visualização de um registro.

  <span class="preview">Você pode adicionar uma página Registros conectados a partir da visualização de um registro no ambiente Visualização.</span>

* As páginas de registros conectados exibem somente os objetos ou registros conectados de um tipo de objeto ou registro em uma exibição de tabela. A página não exibe todos os registros desse tipo na exibição de tabela.

* Dependendo do ambiente usado, você pode observar o seguinte:

   * No ambiente de Produção, depois de adicionar uma página Registros conectados a um registro, a guia Página fica visível na área de visualização do registro, mas está vazia. Você deve ir para a página inteira para ver a exibição de tabela do registro conectado.
   * <span class="preview">No ambiente de Visualização, a página Registros conectados está visível na área de visualização do registro e na guia do navegador.</span>

* Você pode adicionar páginas Registros conectados para os seguintes tipos de registro ou objeto conectados:

   * Tipos de registro do Workfront Planning
   * Projetos, programas, portfólios, grupos ou empresas do Workfront. Você pode visualizar os objetos conectados do Workfront mesmo quando não tem permissões para acessá-los no Workfront.

  >[!NOTE]
  >
  >   Não é possível adicionar uma página Registros conectados para registros conectados do AEM Assets.

Para adicionar uma página Registros conectados:

1. Clique no nome do registro para abri-lo.
1. Clique em **Adicionar página** de uma das seguintes áreas:

   * <span class="preview">A janela de visualização do registro</span>
   * A página de detalhes do registro, após clicar no ícone **Abrir em nova guia** ![Abrir detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) no canto superior direito da página de visualização.

   A caixa **Criar página** é aberta.

   ![Adicionar modal da página Registros conectados](assets/add-connection-view-page-modal.png)

1. Adicione o **Nome da página**, clique em **Página de registros conectados** e em **Criar**.

   Uma nova guia é adicionada à página do registro.
1. Procure ou clique no nome de um registro ou tipo de objeto conectado na lista.
A exibição de tabela do tipo de registro selecionado é exibida na nova página e os registros conectados são exibidos na exibição de tabela.
Todos os campos do registro conectado são exibidos na exibição de tabela da guia do registro conectado.

   Os primeiros cinco campos da tabela de registro conectada são exibidos por padrão. Nenhum campo de pesquisa é exibido por padrão.

   ![Exibição da tabela conectada ao público-alvo nos detalhes da campanha](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Opcional) Na exibição de tabela dos registros conectados, siga um destes procedimentos:

   * Clique no nome de um registro. A página do registro será aberta em uma nova guia.

     Isso abre a página de visualização do registro. Clique no ícone **Abrir em uma nova guia** ![Abrir em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) no canto superior direito para abrir a página do registro conectado.

   * Clique em **Conectar** para conectar mais registros e em fora da caixa de conexão para fechá-la. Os novos registros são adicionados automaticamente à tabela.
   * Edite qualquer informação dos registros conectados dentro da exibição de tabela.

   * Passe o mouse sobre o nome de um registro conectado, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e, em seguida, clique em uma das seguintes opções:
      * Exibir
      * Copiar link
      * Editar miniatura
      * Duplicar
      * Inserir registro acima ou abaixo
      * Excluir
   * Selecione um dos registros e clique em uma das seguintes opções na barra azul na parte inferior da tela:
      * Exibir
      * Copiar link
      * Editar miniatura
      * Duplicar
      * Excluir. Excluir é a única opção disponível ao selecionar mais de um registro.

     Para obter informações sobre como editar registros no modo de exibição de tabela, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

   * Edite em linha qualquer um dos registros na tabela na página Registros conectados.

     No ambiente de Produção, todos os objetos do Workfront são exibidos em uma exibição de tabela somente leitura e não é possível editá-los.

     <span class="preview">No ambiente de Visualização, você pode editar projetos em linha na página de registros conectados.</span>

1. <span class="preview">(Condicional) Ao visualizar uma lista de projetos conectados, siga um destes procedimentos:</span>

   * <span class="preview">Clique em **Conectar registros** no canto superior direito da página de registro conectada para conectar projetos existentes.</span>
   * <span class="preview">Editar informações do projeto em linha na tabela.</span>
   * <span class="preview">Clique em **Nova linha** para criar um projeto sem um modelo. O novo projeto está conectado ao registro atual imediatamente.</span>

     Para obter mais informações, consulte [Criar objetos do Workfront no Workfront Planning à medida que você os conecta a registros](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * <span class="preview">Passe o mouse sobre um projeto e clique no menu **Mais** [Mais menu](assets/more-menu.png), em seguida, clique em um dos seguintes:</span>
      * <span class="preview">**Excluir** para excluir o projeto. A exclusão de um projeto o desconecta do registro e o move para a Lixeira do Workfront. </span>
      * <span class="preview">**Desconectar** para desconectar o projeto do registro. Desconectar um projeto o remove e todos os valores de seus campos de pesquisa do registro atual. </span>

1. (Opcional) Clique duas vezes no nome da guia da página Registros conectados

   Ou

   Passe o mouse sobre o nome da guia, em seguida, clique em **Mais** ![Mais menu](assets/more-menu.png) e em **Renomear** para renomear para a nova guia Modo de Exibição Conectado.
1. (Opcional) Use qualquer um dos seguintes elementos de exibição na barra de ferramentas para gerenciar a exibição de tabela:

   * Filtros
   * Ordenar
   * Agrupamento
   * Campos, para exibir, ocultar ou reorganizar campos

   Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >   Não é possível criar, editar ou excluir campos na exibição de tabela de uma guia de registro conectado.
   >

1. (Condicional) Para conectar mais registros ou objetos, siga um destes procedimentos:

   * Clique em **Conectar** na parte inferior da tabela para adicionar ou remover registros ou quaisquer objetos do Workfront <span class="preview">exceto projetos.</span>
   * <span class="preview">No ambiente de Visualização, clique em **Conectar registros** no canto superior direito da página de registros conectados para conectar projetos existentes ou clique em **Nova linha** na parte inferior da tabela para criar projetos e conectá-los automaticamente ao registro atual.</span>

   Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
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



