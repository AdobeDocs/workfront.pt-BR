---
title: Gerenciar o layout da página de registro
description: É possível editar o layout da visualização de registro e da página no Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: bddd0dcd2263bd65420a17e4b9cc74336877719f
workflow-type: tm+mt
source-wordcount: '1916'
ht-degree: 0%

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

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

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
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Padrão</p>
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
   <p>Contribuir com ou mais permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal e a área Planejamento para projetos, portfólios e programas. </p> Para obter mais informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral sobre acesso ao Adobe Planning</a>. </p>  </p>  
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

   <div class="preview">

   ![Caixa Detalhes](assets/details-box.png)

   </div>

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

   <div class="preview">

   ![Caixa Detalhes](assets/details-box.png)

   </div>

1. (Opcional) Clique no ícone **Abrir em nova guia** ![Abrir caixa de detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.

   A guia **Detalhes** do registro é aberta por padrão.

   <div class="preview">

   ![Página de detalhes](assets/details-page.png)

   </div>

1. Na guia **Detalhes** do registro, clique no ícone **Capturar** ![Ícone Capturar](assets/grab-icon.png) à esquerda de um nome de campo e arraste-o e solte-o no local desejado.

   >[!TIP]
   >
   >Você pode arrastar e soltar campos em outra seção.
   >Você deve ter pelo menos um campo em uma seção.
   >

   A nova posição do campo é atualizada na pré-visualização e na página de todos os registros do mesmo tipo para todos os usuários que visualizam os registros.

   Todas as alterações no layout da visualização do registro ou na página são salvas automaticamente.

## Adicionar uma página de exibição de conexão à página de um registro

<!--suggested a new name for this type of page: "Connected records details" - check to see if this changed-->

Considere o seguinte ao adicionar uma exibição de Conexão à página de um registro:

* Você pode adicionar uma página de exibição de conexão à página de um registro.

* Não é possível adicionar uma página de exibição de conexão à área de visualização de um registro.

* As páginas de exibição de conexão exibem uma página de registro conectada na exibição de tabela. A exibição de tabela é somente leitura. <!--more views might be added in the future-->

* É possível adicionar uma página de exibição de conexão para cada tipo de registro conectado.  <!--edit this when we can remove fields from this page-->

* Depois de adicionar uma página Exibição de conexão à página de um registro, a guia Página fica visível na área de visualização do registro. Você deve ir para a página inteira para ver a exibição de tabela do registro conectado. <!--this might have changed? check and take disclaimer out-->

Para adicionar uma página de exibição de conexão:

1. Em uma exibição de página de registro, clique no nome de um registro para abri-lo e no ícone **Abrir em nova guia** ![Abrir detalhes em um novo ícone de guia](assets/open-details-in-a-new-tab-icon.png) no canto superior direito da página de visualização.
1. Clique em **Adicionar página** > **Exibição de conexão**.

   ![Adicionar modal da página de exibição de conexão](assets/add-connection-view-page-modal.png)
1. Adicione o **Nome da página**, clique em **Modo de exibição de conexão** e em **Criar**.

   Uma nova guia é adicionada à página do registro.
1. Pesquise ou clique no nome de um registro ou tipo de objeto conectado na lista.
A exibição de tabela do tipo de registro selecionado é exibida e os registros conectados são exibidos na exibição de tabela.
Todos os campos do registro conectado são exibidos na exibição de tabela da guia do registro conectado.

   <span class="preview">Ao acessar o Workfront Planning no ambiente de Visualização, os primeiros cinco campos da tabela de registro conectada são exibidos por padrão. Nenhum campo de pesquisa é exibido por padrão.</span>

   A exibição de tabela é somente leitura.

   <!--replace screen shot below when additional capabilities come to the table view - Fields, etc-->

   <div class="preview">

   ![Exibição da tabela conectada ao público-alvo nos detalhes da campanha](assets/audience-connected-table-view-under-campaign-details-page.png)

   </div>

1. (Opcional) Clique duas vezes no nome da guia

   Ou

   Passe o mouse sobre o nome da guia, em seguida, clique em **Mais** ![Mais menu](assets/more-menu.png) e em **Renomear** para renomear para a nova guia Modo de Exibição Conectado.
1. (Opcional) Use qualquer um dos seguintes elementos de exibição na barra de ferramentas para gerenciar a exibição de tabela:

   * Filtros
   * Ordenar
   * Agrupamento
   * <span class="preview">Campos, para exibir, ocultar ou reorganizar campos</span>

   <!--Add to the list above from the list below - and condition these for Preview only: Hide fields, rearrange fields-->

   Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >   Não é possível executar nenhuma das ações a seguir na exibição de tabela da guia de um registro conectado:
   >
   >   * Ocultar ou reorganizar campos. <span class="preview">Você pode ocultar e reorganizar campos no ambiente de Visualização.</span>
   >   * Criar, editar ou excluir campos
   >

1. <span class="preview">Clique em **Conectar** para adicionar ou remover registros. Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md)</span>
1. (Opcional) Passe o mouse sobre o nome da guia Exibição de conexão, clique em **Mais** ![Mais menu](assets/more-menu.png) e em **Excluir** para remover para a nova guia Exibição conectada.




<!--
## Add a Brief page to a record's page

You can add a Brief page to the record's preview or pages. 

Brief pages contain the same information as the Details tab, in a read-only format. <!--edit this when we can remove fields from this page-->

<!--
1. From a record's page view, click the name of a record to open its preview or page.
1. Click **Add page** > **Brief**. 
1. Add the **Page name**, then click **Create**. 
-->



