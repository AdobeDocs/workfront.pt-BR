---
title: Conectar Tipos de Registro
description: Uma maneira de indicar como os tipos de registro individuais se relacionam entre si é conectá-los. Além disso, é possível conectar tipos de registro do Adobe Workfront Planning a tipos de objeto de outros aplicativos para aprimorar a experiência dos usuários e manter o foco em um aplicativo.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 98ef4a4f0a30dc90956132cb715393a29170d715
workflow-type: tm+mt
source-wordcount: '2853'
ht-degree: 1%

---


<!--keep the 30 fields limit in yellow till Jan 2026; also the global record type cross-workspace capability information-->

# Conectar tipos de registro

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Você pode conectar tipos de registro uns aos outros ou pode conectar tipos de registro a tipos de objeto de outros aplicativos.

A conexão de tipos de registro é útil quando há vários tipos de objetos de trabalho que afetam uns aos outros. Por exemplo, você pode trabalhar com campanhas do e cada campanha pode atender a várias marcas. Para indicar esse relacionamento, você pode conectar campanhas a marcas. Isso cria um campo de conexão para Marcas no registro da campanha.

Além disso, o trabalho para cada campanha pode ser planejado em vários projetos no Workfront. Para indicar isso, você pode conectar as campanhas aos projetos relevantes. Isso cria um campo de conexão para Projetos no registro da campanha.

Depois que os campos de conexão forem criados, será possível conectar registros individuais entre os dois tipos de registro ou objeto.

>[!NOTE]
>
><span class="preview">Você pode ter até 30 campos de conexão para um tipo de registro.</span>

Este artigo descreve como é possível conectar dois tipos de registro do Workfront Planning ou um tipo de registro do Workfront Planning a um objeto de outro aplicativo.

Depois de estabelecer a conexão entre registros ou tipos de objeto, um campo de conexão é adicionado a um tipo de registro do Planning. No campo de conexão, é possível conectar registros individuais uns aos outros e exibir campos do registro vinculado ou tipos de objeto em um registro do Workfront Planning.

Para obter informações gerais sobre tipos de conexão, consulte [Visão geral sobre tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Para obter informações sobre como conectar registros ou registros a objetos de outros aplicativos, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

Para obter um exemplo de conexão de tipos de registros e registros, consulte [Exemplo de conexão de tipos de registros e registros](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->


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
<p>Para conectar tipos de registro do mesmo espaço de trabalho: </p>
<ul> 
<li><p>Qualquer Workfront e qualquer pacote do Planning</p></li>
<li><p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</li></ul>

<p>Para conectar tipos de registro de espaços de trabalho diferentes:</p>

<ul> 
<li><p>Qualquer Workfront e qualquer pacote do Planning</p></li>
<li><p>Qualquer fluxo de trabalho e um pacote do Planning Prime ou Ultimate</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
<tr> 
<td> 
   <p> Produtos adicionais</p> </td> 
   <td> 
   <p> Além do Adobe Workfront, você deve ter o seguinte, se quiser conectar tipos de registro a objetos dos seguintes aplicativos:</p>
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
   <td>   <p>Gerenciar permissões em um espaço de trabalho</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
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
   <li><p> Adobe Workfront Planning<p></li>
   <li><p> Adobe Experience Manager Assets, if you want to connect AEM assets with Planning record types<p>
   <p>You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront for Experience Manager Assets and Assets Essentials: article index</a>. </p>
   </li>
   </ul></td> 
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
   <td> <p>Standard</p> 
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p></td> 
  </tr> 
 
</tbody> 
</table> -->

## Conectar tipos de registro

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja conectar,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.
1. Clique no cartão de um tipo de registro para abrir a página do tipo de registro.
1. Clique no ícone **+** no canto superior direito do modo de exibição de tabela e clique na guia **Nova conexão**.

   ![Nova guia de conexão com opções do Workfront AEM](assets/new-connection-tab-with-workfront-aem-options-no-buttons.png)

1. Procure um tipo de registro ou selecione um dos seguintes:

   * Um tipo de registro do espaço de trabalho atual

     ![Seletor de conexão de seleção múltipla para o tipo de registro do mesmo espaço de trabalho](assets/multi-select-connection-picker-record-type.png)

     >[!TIP]
     >
     > 
     >Se você não tiver outros tipos de registro no espaço de trabalho selecionado, a seção espaço de trabalho não será exibida.

   * Um tipo de registro de outro espaço de trabalho que foi configurado para se conectar a outros espaços de trabalho.

     >[!TIP]
     >
     >A configuração **Permitir conexão com este tipo de registro em outros espaços de trabalho** deve ser habilitada para um tipo de registro nas **Configurações avançadas** <span class="preview">ou na guia **Configurações entre espaços de trabalho**</span> da caixa **Editar tipo de registro**, para que um tipo de registro seja acessível de outros espaços de trabalho. Se não houver tipos de registro configurados para se conectar a partir de outros espaços de trabalho, a seção espaço de trabalho não será exibida.
     >
     >Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). <!--update screen shot at production-->
     >
     >![Guia de configurações avançadas da caixa Editar tipo de registro](assets/edit-record-type-box-advanced-settings-tab.png)

     <!--Old:
        [!TIP]
        The **Allow connecting to this record type in other workspaces** setting must be enabled for a record type in the **Advanced settings** tab of the **Edit record type** box, for a record type to be accessible from other workspaces. If there are no record types that are configured to connect from other workspaces, the workspace section does not display.
        ![Edit record type box advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)
        -->

   Para obter informações, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

   * Um **Projeto, Portfolio, Programa, Empresa** ou **Grupo** da seção **Tipos de Objeto do Workfront**.

     ![Seleção de conexão do projeto Workfront](assets/multi-select-connection-picker-project.png)

   * **Experience Manager Assets** da seção **Aplicativos Adobe**.

     ![Seleção de conexão do AEM Assets](assets/aem-assets-connection-selection.png)

     Uma guia Nova conexão é aberta para o registro ou tipo de objeto selecionado.

   * Uma **Marca** da Adobe GenStudio for Performance Marketing da seção **Adobe GenStudio**

     ![Seleção de conexão de Marca da GenStudio](assets/brand-genstudio-connection-selection.png)

1. Atualize o campo **Nome** com o nome do novo campo conectado, como ele aparecerá na exibição de tabela ou na página de registro do tipo de registro original. Isso cria a coluna (ou campo) de registro conectado na exibição de tabela do tipo de registro original. Por padrão, o nome do campo é o nome do registro ou objeto ao qual você se conecta.

   >[!TIP]
   >
   >É possível ter várias conexões para o mesmo registro ou tipo de objeto. Se você não editar o nome do campo conectado, o Workfront adicionará um numeral após o nome do registro conectado, para indicar o número de tipos de registros conectados com o mesmo nome.

1. Atualize o campo **Descrição** adicionando informações sobre o campo de registro conectado. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
1. (Condicional) Ao conectar tipos de registro de dois espaços de trabalho diferentes, um tipo de registro e um objeto de ativo do Adobe Experience Manager ou um tipo de registro e uma Marca da GenStudio, selecione a opção **Permitir vários registros**. Ao selecioná-lo, você indica que permite que os usuários adicionem vários registros quando o campo de tipo de registro conectado é exibido nos registros originais. É selecionado por padrão.

   ![Nova conexão com o tipo de registro de outro espaço de trabalho](assets/new-connection-allow-multiple-records-box.png)

1. (Condicional) Ao conectar tipos de registro do mesmo espaço de trabalho ou de um tipo de registro do Planning a um tipo de objeto do Workfront, selecione uma das seguintes opções:

   * **Multisseleção**: selecione esta opção para permitir que um registro do tipo de registro atual se conecte a vários registros do tipo de registro de conexão.
   * **Seleção única**: selecione esta opção para permitir que um registro do tipo de registro atual se conecte a um registro do tipo de registro de conexão.

1. Selecione o **Criar campo correspondente no tipo de registro vinculado**. Quando selecionado, um campo de conexão é criado no tipo de registro ao qual você está conectado, além do campo de conexão adicionado ao tipo de registro atual. Essa opção está desativada por padrão.

   >[!TIP]
   >
   >* Além do <span class="preview">limite de 30 campos de conexão para um tipo de registro</span>, há um limite de 500 campos para um tipo de registro. Recomendamos manter essa configuração desativada, especialmente para tipos de registros taxonômicos, para evitar atingir esse limite.
   >
   >* <span class="preview">Selecionar o **Criar campo correspondente no tipo de registro vinculado** é um pré-requisito para a criação de hierarquias.</span>

1. (Condicional) Se você habilitou **Criar campo correspondente no tipo de registro vinculado**, escolha entre as seguintes opções para indicar a quantidade de registros aos quais os usuários podem se conectar e de:

   * Muitos para muitos
   * Um para muitos
   * Muitos para um
   * Um para um

   Para obter mais informações sobre tipos de conexão, consulte [Visão geral sobre tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   >[!NOTE]
   >
   >Se você selecionar Um para muitos ou Um para um para o tipo de conexão e quiser conectar um registro ou um objeto que já esteja conectado em outro lugar, você receberá um aviso de que a conexão novamente o removerá da conexão original. Você pode permitir a remoção ou selecionar outro registro.

1. (Condicional e opcional) Ao selecionar a conexão de um objeto do Workfront, escolha um **Formulário personalizado** na seção **Vincular somente objetos que correspondam a esses critérios**. Somente objetos que tenham os formulários personalizados selecionados anexados podem ser vinculados ao tipo de registro selecionado. É possível selecionar mais de um formulário.

   >[!NOTE]
   >
   > Você deve criar formulários personalizados no Workfront para os objetos selecionados antes que eles sejam exibidos nesta lista.

1. (Condicional) Ao se conectar ao Experience Manager Assets, escolha um repositório no menu suspenso **Repositório do Experience Manager** na seção **Vincular ativos do repositório a seguir**. Este campo é obrigatório. Somente repositórios aos quais você tem acesso no Experience Manager Assets são exibidos nesse campo.

   >[!NOTE]
   >
   >O administrador do Workfront pode mapear campos do Workfront Planning para campos do Experience Manager Assets por meio do mapeamento de metadados no Workfront. Para obter mais informações, consulte [Configurar o mapeamento de metadados de ativos entre o Adobe Workfront e o Experience Manager Assets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


1. (Condicional) Ao se conectar ao Experience Manager Assets, a um tipo de registro do Workfront Planning ou a uma Marca GenStudio, escolha uma das seguintes opções na área **Aparência do registro**:

   * **Nome e imagem**: o nome e a miniatura ou o ícone dos registros conectados serão exibidos no campo de registro conectado. Esta é a opção padrão.
   * **Nome**: somente o nome dos registros conectados será exibido no campo de registro conectado.
   * **Imagem**: somente a miniatura ou o ícone dos registros conectados será exibido no campo de registro conectado.

   Os registros sem uma imagem em miniatura exibem o ícone de tipo de registro. Um exemplo de como os registros conectados serão exibidos é exibido na área **Aparência do registro**.

   >[!NOTE]
   >
   >* Quando você permite que vários registros sejam vinculados, exibir somente a miniatura pode economizar espaço em áreas menores, como visualizações de registros.
   >
   >* O nome de um registro é o campo principal do registro. Para obter mais informações, consulte [Visão geral do campo principal](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >* A seleção da aparência de um registro não está disponível ao selecionar tipos de objeto do Workfront.
   >
   >* O que você seleciona na área Aparência do registro determina como os registros são exibidos em conexões em todos os locais do sistema, incluindo todas as exibições e páginas de detalhes.

1. Selecione os **Selecionar campos de pesquisa** para adicionar campos do tipo de registro ao qual você está se conectando. Os campos de pesquisa são campos associados ao registro ou tipo de objeto ao qual você está vinculando. Vinculá-los exibe informações do registro ou objeto ao qual você está vinculando no registro a partir do qual você está vinculando. É selecionado por padrão.

   >[!TIP]
   >
   >* Não é possível adicionar campos de digitação antecipada do Workfront (incluindo campos como Proprietário do projeto ou Patrocinador do projeto) como campos de pesquisa.
   >
   >* As informações do campo de data dos objetos do Workfront são exibidas no formato de 24 horas no Workfront Planning, independentemente de como são exibidas no Workfront.
   >
   >   Por exemplo, se a Data de Início Planejada de um projeto for exibida como 3:00 PM no Workfront, ela será exibida como 15:00 no Workfront Planning em um campo de pesquisa importado.

1. Clique em **Criar**.

1. (Condicional) Se você selecionou a configuração **Selecionar campo de pesquisa**, a caixa **Adicionar campos de pesquisa** será aberta.

   Clique no ícone **+** para adicionar campos da área **Campos não selecionados**.

   Ou

   Clique no ícone **-** para remover campos da área **Campos selecionados**

   ![Adicionar campos de pesquisa para outra caixa de tipo de registro](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Os valores dos campos conectados são preenchidos automaticamente depois de vincular registros ou objetos.

   >[!IMPORTANT]
   >
   >    Todos os usuários com permissões de Exibição ou superiores ao espaço de trabalho podem exibir as informações nos campos vinculados, independentemente das permissões ou do nível de acesso na aplicação dos tipos de objeto vinculados.

1. (Opcional) Clique em **Ignorar** para ignorar a adição de campos do registro vinculado ou do tipo de objeto. O campo Name ou Primary do registro vinculado é o único campo visível na exibição em tabela do tipo de registro ao qual você está se conectando.

1. Escolha um agregador para os campos de pesquisa adicionados.

   >[!NOTE]
   >
   >Não é possível adicionar agregadores para os seguintes tipos de campo:
   >
   >    * Parágrafo
   >    * Caixa de seleção

   Os valores dos campos vinculados são exibidos separados por vírgulas ou como um valor resumido de acordo com o agregador escolhido, quando os usuários selecionam mais de um registro vinculado no campo de registro vinculado.

   Se o campo de pesquisa contiver vários valores que não estão resumidos, considere o seguinte ao usar o campo em classificação ou agrupamento em uma exibição:

   * A classificação é feita pelo primeiro valor

   * Os registros são agrupados por cada combinação exclusiva de valores de campo

   * A exibição da linha do tempo é criada com base no primeiro valor de data do tipo de registro conectado, quando exibida na exibição

   >[!IMPORTANT]
   >
   > Você deve selecionar um valor agregador ao adicionar campos de data de pesquisa, se quiser que os campos estejam disponíveis para serem adicionados como Datas inicial e final para as exibições de linha do tempo e calendário. Por exemplo, você pode selecionar o agregador MAX ou MIN para um campo de data de pesquisa.

   ![Lista suspensa de agregadores para o campo de número vinculado](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Os agregadores não estão disponíveis ao conectar tipos de registro ao seguinte:
   >* Experience Manager Assets
   >* Marcas GenStudio.
   >

   Selecione entre as seguintes opções:

   * **Nenhum**: exibe os valores provenientes de vários registros separados por vírgulas. Esta é a seleção padrão.
   * **MAX**: exibe o valor mais alto de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **MIN**: exibe o valor mais baixo de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **SOMA**: exibe o total de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **AVG**: exibe a média de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **EXCLUSIVO**: remove as duplicatas dos valores do campo de pesquisa e mostra apenas os valores exclusivos. Isso não está disponível para os seguintes tipos de campo:
      * Parágrafo
      * Caixa de seleção
      * People

   >[!NOTE]
   >
   >Por exemplo, você pode vincular o registro Product (registro vinculado) do registro Campaign (registro original) e nomeá-lo como &quot;Campo de produto&quot;. Também é possível vincular o campo Budget do registro Product do registro Campaign e chamá-lo de &quot;Product Budget&quot;. Se você tiver permissão para selecionar vários registros no &quot;campo Produto&quot;, poderá selecionar o Produto 1 com um Orçamento de US$ 100.000 e o Produto 2 com um Orçamento de US$ 110.000, e o Produto 3 com um Orçamento de US$ 100.000. Você pode exibir as seguintes informações de Orçamento no campo vinculado do registro original, dependendo do agregador escolhido:
   >
   >* **Nenhum**: $100.000, $110.000, $100.000
   >* **MAX**: $110.000
   >* **MIN**: $100.000
   >* **SOMA**: $310.000
   >* **MÉDIA**: $103.000,33
   >* **ÚNICO**: $100.000
   >

1. (Opcional) Use o **ícone de pesquisa** ![ícone de pesquisa](assets/search-icon.png) para procurar um campo.

1. Clique em **Adicionar campos** para salvar as alterações.

   Os seguintes itens são adicionados:

   * Um campo de registro vinculado no tipo de registro a partir do qual você está vinculando. O campo de registro vinculado exibirá registros individuais do tipo de registro vinculado depois que você os adicionar manualmente. Para obter informações sobre como adicionar registros, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md). O nome do campo de registro vinculado é o nome selecionado na etapa 6. <!--accurate-->

   * Um campo (ou campos) vinculado (ou de pesquisa) que exibe informações sobre o registro ou os tipos de objeto vinculados depois de adicionar manualmente os registros ou objetos no campo de registro vinculado. Os campos de pesquisa são criados somente quando a configuração **Selecionar campos de pesquisa** é selecionada ao criar a conexão. Os campos de pesquisa são nomeados automaticamente de acordo com este padrão:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Por exemplo, se você vinculou um tipo de registro de Campanha a um tipo de registro de Programa e nomeou o campo &quot;Informações do programa&quot; do registro vinculado ao Programa, então selecionou exibir também o campo Orçamento do programa na exibição de tabela da Campanha, o campo vinculado será automaticamente nomeado como `Budget (from Program information)` na exibição de tabela da campanha.

   * Ao vincular tipos de registro uns aos outros, um campo de registro vinculado também é adicionado ao tipo de registro ao qual você está vinculando, somente quando você habilita a configuração **Criar campo correspondente no tipo de registro vinculado**. O nome do campo de registro vinculado no tipo de registro vinculado é o nome do tipo de registro que você vincula.

     Por exemplo, se você vincular o tipo de registro &quot;Produto&quot; do tipo de registro &quot;Campanha&quot; e nomear o campo conectado do &quot;Produto vinculado&quot; da Campanha, um campo de registro vinculado &quot;Campanha&quot; será criado para o tipo de registro Produto.

     >[!TIP]
     >
     > Um campo de registro vinculado não é criado para objetos de outro aplicativo em seus respectivos aplicativos.
     >Recomendamos não criar links para tipos de registros taxonômicos, pois há um limite de 500 campos, <span class="preview"> além do limite de 30 campos conectados</span> para cada tipo de registro.

   <!--see the span preview text in the TIP above; it might not show up in green-->

1. (Opcional e condicional) Na exibição da tabela do tipo de registro original ou da tabela do tipo de registro vinculado, clique na seta para baixo no cabeçalho dos campos de registro vinculados e, em seguida, clique em uma das seguintes opções:

   * **Editar campo**: atualize as informações de **Nome** e **Descrição** do campo.
   * **Editar campos de pesquisa**: adicionar ou remover qualquer um dos campos de registro vinculados.

   ![Menu suspenso Editar campo e campos de pesquisa na coluna da tabela](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Para adicionar ou remover campos de pesquisa, siga as instruções nas etapas 16 a 17 acima. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Não é possível adicionar campos de pesquisa que pertençam a tipos de registro que você está vinculando a tipos de objeto de outro aplicativo.
   >
   > Por exemplo, não é possível adicionar o campo de pesquisa &quot;Status da campanha&quot; a um projeto do Workfront ao qual você está vinculando nas campanhas.

1. (Opcional) Clique na seta para baixo no cabeçalho de um campo de registro vinculado ou no cabeçalho de um campo de pesquisa do tipo de registro do qual você está vinculando e clique em **Excluir**.

   O campo de registro ou o campo de pesquisa são excluídos. Se você excluir um campo de registro, quaisquer campos de pesquisa associados ao registro vinculado também serão excluídos.
