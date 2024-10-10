---
title: Conectar Tipos de Registro
description: Uma maneira de indicar como os tipos de registro individuais se relacionam entre si é conectá-los. Além disso, é possível conectar tipos de registro do Adobe Workfront Planning a tipos de objeto de outros aplicativos para aprimorar a experiência dos usuários e manter o foco em um aplicativo.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 7b5441b2aa17b22f0fd54cfe4921aa5dab2e0461
workflow-type: tm+mt
source-wordcount: '2222'
ht-degree: 1%

---


# Conectar tipos de registro

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

{{planning-important-intro}}

<!--
You can use Adobe Workfront Planning to design fully-customizable workspaces that contain record types needed in your organization. A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Workfront Planning record types with object types from other applications to enhance your users' experience and keep their focus in one application. -->

Você pode conectar tipos de registro uns aos outros ou pode conectar tipos de registro a tipos de objeto de outros aplicativos.

Este artigo descreve como é possível conectar dois tipos de registro do Workfront Planning ou um tipo de registro do Workfront Planning a um objeto de outro aplicativo.

Depois de estabelecer a conexão entre registros ou tipos de objeto, você pode conectar registros individuais uns aos outros e exibir campos do registro vinculado ou tipos de objeto em um registro do Workfront Planning.

Para obter informações gerais sobre tipos de conexão, consulte [Visão geral sobre tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

Para obter informações sobre como conectar registros ou registros a objetos de outros aplicativos, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

Para obter um exemplo de conexão de tipos de registros e registros, consulte [Exemplo de conexão de tipos de registros e registros](/help/quicksilver/planning/architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

Para acessar o Workfront Planning, é necessário ter o seguinte:

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
   <td role="rowheader"><p>Plano de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td> <p>Padrão</p> 
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
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!-- OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p> Adobe Workfront Planning</p>
   <p>To connect Adobe Workfront Planning record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p> 
   <p>Current: Plan</p>
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create.</p>
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

+++


## Conectar tipos de registro

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja conectar,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.
1. Clique no cartão de um tipo de registro para abrir a página do tipo de registro.
1. Clique no ícone **+** no canto superior direito do modo de exibição de tabela e clique na guia **Nova conexão**.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. No campo **Tipo de registro**, procure um tipo de registro ou selecione um dos seguintes:

   * Outro tipo de registro do espaço de trabalho atual

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>
     >[!TIP]
     >
     > 
     >Se você não tiver outros tipos de registro no espaço de trabalho selecionado, a seção espaço de trabalho não será exibida.


   * Um tipo de registro de outro espaço de trabalho que foi configurado para se conectar a outros espaços de trabalho. Para obter informações, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

     >[!TIP]
     >
     >Se não houver tipos de registro configurados para se conectar a partir de outros espaços de trabalho, a seção espaço de trabalho não será exibida.


   * Um **Projeto, Portfolio, Programa, Empresa** ou **Grupo** da seção **Tipos de Objetos do Workfront**.

     ![](assets/workfront-project-connection-selection.png)

   * **Experience Manager Assets** da seção **Adobe Applications**.

     <span class="preview">![](assets/aem-assets-connection-selection.png)</span>

1. Atualize as seguintes informações:

   * **Nome**: o nome do campo conectado, como ele aparecerá na exibição de tabela ou na página de registro do tipo de registro original. Isso cria a coluna de registro vinculado na exibição de tabela do tipo de registro original ou no campo de registro vinculado dos registros originais. Por padrão, o nome do campo é o nome do registro ou objeto ao qual você se conecta.

   >[!TIP]
   >
   >É possível ter várias conexões para o mesmo registro ou tipo de objeto. Se você não editar o nome do campo conectado, o Workfront adicionará um numeral após o nome do registro conectado, para indicar o número de tipos de registros conectados com o mesmo nome.

   * **Descrição**: informações adicionais sobre o campo de registro conectado. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Permitir vários registros**: selecione esta opção para indicar que você permite que os usuários adicionem vários registros quando o campo de tipo de registro vinculado for exibido nos registros originais. É selecionado por padrão.

     Essa opção está disponível somente ao conectar registros de dois espaços de trabalho diferentes ou um registro e um objeto de ativo do Adobe Experience Manager.

     <span class="preview">![](assets/new-connection-allow-multiple-records-box.png)</span>

   * **Tipo de conexão**: selecione uma das seguintes opções para indicar a quantidade de registros aos quais eles podem se conectar e de onde:

      * Muitos para muitos
      * Um para muitos
      * Muitos para um
      * Um para um

     Essa opção está disponível somente ao conectar registros do mesmo espaço de trabalho ou de um registro e um tipo de objeto do Workfront.

     <span class="preview">![](assets/many-to-many-connection-picker.png)</span>

     Para obter mais informações sobre tipos de conexão, consulte [Visão geral sobre tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

   * **Selecionar campos de pesquisa**: selecione esta opção para adicionar campos do tipo de registro selecionado. Os campos de pesquisa são campos associados ao registro ou tipo de objeto ao qual você está vinculando. Vinculá-los exibe informações do registro ou objeto ao qual você está vinculando no registro a partir do qual você está vinculando. É selecionado por padrão.

     >[!TIP]
     >
     > Não é possível adicionar os seguintes tipos de campo como campos de pesquisa:
     >
     >    * Pessoas
     >    * Criado por
     >    * Modificado pela última vez por
     >    * Campos de digitação antecipada do Workfront (incluindo campos como Proprietário do projeto ou Patrocinador do projeto)

1. (Condicional e opcional) Se você selecionou conectar um objeto do Workfront, selecione um **Formulário personalizado** na seção **Vincular somente objetos que correspondam a esses critérios**. Somente objetos que tenham os formulários personalizados selecionados anexados podem ser vinculados ao tipo de registro selecionado. É possível selecionar mais de um formulário.

   >[!NOTE]
   >
   > Você deve criar formulários personalizados no Workfront para os objetos selecionados antes que eles sejam exibidos nesta lista.

1. (Condicional) Se você optou por se conectar ao Experience Manager Assets, selecione um repositório no menu suspenso **Experience Manager repository** na seção **Vincular ativos do repositório a seguir**. Este campo é obrigatório. Somente repositórios aos quais você tem acesso no Experience Manager Assets são exibidos nesse campo.

   >[!NOTE]
   >
   >O administrador do Workfront pode mapear campos do Workfront Planning para campos do Experience Manager Assets por meio do mapeamento de metadados no Workfront. Para obter mais informações, consulte [Configurar o mapeamento de metadados de ativos entre o Adobe Workfront e o Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

1. (Condicional) Se você optou por se conectar ao Experience Manager Assets ou a um tipo de registro do Workfront Planning, selecione uma das seguintes opções na área **Aparência do registro**:

   * <span class="preview">**Nome e imagem**: o nome e a miniatura ou o ícone dos registros conectados serão exibidos no campo de registro conectado. Esta é a opção padrão. </span>
   * <span class="preview">**Nome**: somente o nome dos registros conectados será exibido no campo de registro conectado.</span>
   * <span class="preview">**Imagem**: somente a miniatura ou o ícone dos registros conectados será exibido no campo de registro conectado.</span>

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

1. Clique em **Criar**.

1. (Condicional) Se você selecionou a configuração **Selecionar campo de pesquisa**, a caixa **Adicionar campos de pesquisa** será aberta.

   Clique no ícone **+** para adicionar campos da área **Campos não selecionados**.

   Ou

   Clique no ícone **-** para remover campos da área **Campos selecionados**

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)

   Os valores dos campos conectados são preenchidos automaticamente depois de vincular registros ou objetos.

   >[!IMPORTANT]
   >
   >    Todos os usuários com permissões de Exibição ou superiores ao espaço de trabalho podem exibir as informações nos campos vinculados, independentemente das permissões ou do nível de acesso na aplicação dos tipos de objeto vinculados.


1. (Opcional) Clique em **Ignorar** para ignorar a adição de campos do registro vinculado ou do tipo de objeto. O campo Name ou Primary do registro vinculado é o único campo visível na exibição em tabela do tipo de registro ao qual você está se conectando.

1. (Opcional e condicional) Se você optar por vincular um campo do tipo número, moeda, porcentagem ou data, selecione também um valor agregador para resumir vários valores. Os valores dos campos vinculados são exibidos separados por vírgulas ou como um valor resumido de acordo com o agregador escolhido, quando os usuários selecionam mais de um registro vinculado no campo de registro vinculado.

   Se o campo de pesquisa contiver vários valores que não estão resumidos, considere o seguinte ao usar o campo em classificação ou agrupamento em uma exibição:

   * A classificação é feita pelo primeiro valor

   * Os registros são agrupados por cada combinação exclusiva de valores de campo

   * A exibição da linha do tempo é criada com base no primeiro valor de data

   >[!IMPORTANT]
   >
   >    Você deve selecionar um valor agregador ao adicionar campos de data de pesquisa, se quiser que os campos estejam disponíveis para serem adicionados como Datas inicial e final para as exibições de linha do tempo e calendário. Por exemplo, você pode selecionar o agregador MAX ou MIN para um campo de data de pesquisa.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Os agregadores não estão disponíveis ao conectar tipos de registro ao Experience Manager Assets.

   Selecione entre as seguintes opções:

   * **Nenhum**: exibe os valores provenientes de vários registros separados por vírgulas. Esta é a seleção padrão.
   * **MAX**: exibe o valor mais alto de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **MIN**: exibe o valor mais baixo de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **SOMA**: exibe o total de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **AVG**: exibe a média de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **EXCLUSIVO**: remove as duplicatas dos valores do campo de pesquisa e mostra apenas os valores exclusivos. Isso não está disponível para os seguintes tipos de campo:
      * Parágrafo
      * Caixa de seleção
      * Pessoas

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

1. (Opcional) Use o ícone ![](assets/search-icon.png) de **pesquisa** para procurar um campo.

1. Clique em **Adicionar campos** para salvar as alterações.

   Os seguintes itens são adicionados:

   * Um campo de registro vinculado no tipo de registro a partir do qual você está vinculando. O campo de registro vinculado exibirá registros individuais do tipo de registro vinculado depois que você os adicionar manualmente. Para obter informações sobre como adicionar registros, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md). O nome do campo de registro vinculado é o nome selecionado na etapa 6. <!--accurate-->

   * Um campo (ou campos) vinculado (ou de pesquisa) que exibe informações sobre o registro ou os tipos de objeto vinculados depois de adicionar manualmente os registros ou objetos no campo de registro vinculado. Os campos de pesquisa são criados somente quando a configuração **Selecionar campos de pesquisa** é selecionada ao criar a conexão. Os campos de pesquisa são nomeados automaticamente de acordo com este padrão:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

     Por exemplo, se você vinculou um tipo de registro de Campanha a um tipo de registro de Programa e nomeou o campo &quot;Informações do programa&quot; do registro vinculado ao Programa, então selecionou exibir também o campo Orçamento do programa na exibição de tabela da Campanha, o campo vinculado será automaticamente nomeado como `Budget (from Program information)` na exibição de tabela da campanha.

   * Quando você vincula tipos de registro um ao outro, um campo de registro vinculado também é adicionado ao tipo de registro ao qual você está vinculando. O nome do campo de registro vinculado no tipo de registro vinculado é o nome do tipo de registro que você vincula.

     Por exemplo, se você vincular o tipo de registro &quot;Produto&quot; do tipo de registro &quot;Campanha&quot; e nomear o campo conectado do &quot;Produto vinculado&quot; da Campanha, um campo de registro vinculado &quot;Campanha&quot; será criado para o tipo de registro Produto.

     >[!TIP]
     >
     > Um campo de registro vinculado não é criado para objetos de outro aplicativo para o tipo de registro que você está vinculando no Workfront Planning.

1. (Opcional e condicional) Na exibição da tabela do tipo de registro original ou da tabela do tipo de registro vinculado, clique na seta para baixo no cabeçalho dos campos de registro vinculados e, em seguida, clique em uma das seguintes opções:

   * **Editar campo**: atualize as informações de **Nome** e **Descrição** do campo.
   * **Editar campos de pesquisa**: adicionar ou remover qualquer um dos campos de registro vinculados.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Para adicionar ou remover campos de pesquisa, siga as instruções nas etapas 16 a 17 acima. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Não é possível adicionar campos de pesquisa que pertençam a tipos de registro que você está vinculando a tipos de objeto de outro aplicativo.
   >
   > Por exemplo, não é possível adicionar o campo de pesquisa &quot;Status da campanha&quot; a um projeto do Workfront ao qual você está vinculando nas campanhas.

1. (Opcional) Clique na seta para baixo no cabeçalho de um campo de registro vinculado ou no cabeçalho de um campo de pesquisa do tipo de registro do qual você está vinculando e clique em **Excluir**.

   O campo de registro ou o campo de pesquisa são excluídos. Se você excluir um campo de registro, quaisquer campos de pesquisa associados ao registro vinculado também serão excluídos.
