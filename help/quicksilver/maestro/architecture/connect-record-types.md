---
title: Conectar tipos de registro
description: Uma maneira de indicar como os tipos de registro individuais se relacionam entre si é conectá-los. Além disso, você pode conectar tipos de registro Maestri com tipos de objeto de outros aplicativos para aprimorar a experiência dos usuários e manter o foco em um aplicativo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: 5d8e189f01a52b2d1b605b497ed17737fb0a0924
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Conectar tipos de registro

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode usar o Adobe Maestri para projetar espaços de trabalho totalmente personalizáveis que contenham tipos de registro necessários em sua organização. Uma maneira de indicar como os tipos de registro individuais se relacionam entre si é conectá-los. Além disso, você pode conectar tipos de registro Maestri com tipos de objeto de outros aplicativos para aprimorar a experiência dos usuários e manter o foco em um aplicativo.

Você pode conectar o seguinte:

* Tipos de registro operacional mestre entre si
* Taxonomias maestras umas com as outras
* Tipos e taxonomias de registros operacionais mestre entre si
* Domine os tipos de registros operacionais e taxonomias com tipos de objetos de outras aplicações.

Ao fazer isso, você pode exibir campos do registro vinculado ou tipo de objeto em outro registro Maestro.

Este artigo descreve como você pode conectar dois tipos de registro Maestri ou um tipo de registro Maestri com um objeto de outro aplicativo.

Depois que a conexão entre tipos de registro ou objeto for estabelecida, você poderá conectar registros individuais uns aos outros.

Para obter informações sobre como conectar um registro Maestro a um objeto de outro aplicativo, consulte [Conectar registros](../records/connect-records.md).

Para obter um exemplo de conexão de tipos de registro, consulte [Exemplo de conexão de tipos de registro e registros](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

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
   <p> produto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p><b>Nota</b></p>
   <p>Para conectar tipos de registro Maestri com a Experience Manager Assets, você deve ter uma licença Adobe Experience Manager Assets e a instância da Workfront de sua organização deve ser integrada à Adobe Business Platform ou à Adobe Admin Console. </p>
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
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/grant-access.md">Conceder acesso ao Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>To connect Maestro record types with Experience Manager Assets, you must have an Adobe Experience Manager Assets license and your organization's instance of Workfront must be onboarded to the Adobe Business Platform or the Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Considerações sobre a conexão de tipos de registro

Considere o seguinte:

* Você pode conectar as seguintes entidades no Maestro:

   * Dois tipos de registro operacional
   * Duas taxonomias
   * Um tipo de registro operacional e uma taxonomia
   * Um tipo de registro operacional ou uma taxonomia e um tipo de objeto de outro aplicativo.

* Você pode conectar os seguintes objetos das seguintes aplicações com os tipos de registro Maestri:

   * Adobe Workfront:

      * Projetos
      * Portfólios
      * Programas
      * Empresas
      * Grupos

   * Adobe Experience Manager Assets:

      * Imagens
      * Pastas

     >[!IMPORTANT]
     >
     >Você deve ter uma licença da Adobe Experience Manager Assets e a instância da Workfront de sua organização deve ser integrada à Plataforma de negócios Adobe ou à Adobe Admin Console para conectar os registros Maestri à Adobe Experience Manager Assets.
     >
     >Em caso de dúvidas sobre a integração com a Adobe Admin Console, consulte [Perguntas frequentes sobre a experiência unificada do Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Depois de conectar um tipo de registro com outro tipo de registro ou com um tipo de objeto de outro aplicativo, existem os seguintes cenários:

   * **Quando você conecta dois tipos de registro**: um campo de registro Vinculado é criado no tipo de registro ao qual você está se conectando. Um campo Registro vinculado semelhante é criado no tipo de registro ao qual você está se conectando.

     Por exemplo, se você conectar o tipo de registro &quot;Campanha&quot; ao tipo de registro &quot;Produto&quot;, um campo de registro vinculado chamado &quot;Produto vinculado&quot; será criado no tipo de registro Campanha e um tipo de registro vinculado chamado automaticamente &quot;Campanha&quot; será criado no tipo de registro Produto.

   * **Quando você conecta um tipo de registro a um tipo de objeto de outro aplicativo**: um campo de registro vinculado é criado no tipo de registro ao qual você está se conectando. Nenhum campo de registro vinculado é criado automaticamente no objeto de aplicativo de terceiros.

     Um novo tipo de registro Maestri é criado para o objeto de aplicativo de terceiros somente quando os objetos reais estão conectados aos registros Maestri.

     Para obter mais informações, consulte [Conectar registros](../records/connect-records.md).

   * **Ao adicionar campos de pesquisa a partir do registro ou objeto ao qual você se conecta**: os campos vinculados são adicionados ao registro do qual você está se conectando e exibem os campos de pesquisa selecionados para trazer do registro vinculado para os registros a partir dos quais você está vinculando. Os campos de registro são sempre somente leitura e preenchidos automaticamente com os valores do objeto de terceiros.

     Por exemplo, se você conectar o tipo de registro &quot;Campanha&quot; Maestri com um projeto do Workfront e selecionar trazer o campo Data de conclusão planejada do projeto para o registro Maestri, um campo vinculado chamado Data de conclusão planejada (do projeto) será criado automaticamente para o registro do qual você está vinculando.

* Os campos de registro vinculados são precedidos por um ícone de relacionamento ![](assets/relationship-field-icon.png).

  Os campos vinculados são precedidos por um ícone que identifica o tipo de campo. Por exemplo, ícones que indicam que um campo é um número, um parágrafo ou uma data.

* Depois de criar registros individuais para um tipo de registro, você pode selecionar os registros aos quais se conectar no campo Tipo de registro vinculado. Para obter informações, consulte [Conectar registros](../records/connect-records.md).

## Conectar tipos de registro

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho do qual deseja conectar tipos de registro.
1. Clique no cartão de um tipo de registro para abrir a página do tipo de registro.
1. Clique em **+** no canto superior direito da exibição em tabela, em seguida, clique no **Nova conexão** guia.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. No **Tipo de registro** , pesquise por um tipo de registro ou selecione uma das seguintes opções: <!--is the field name spelled right? lowercase "t"?-->

   * Outro tipo de registro operacional ou uma taxonomia do espaço de trabalho selecionado

     >[!TIP]
     >
     >Somente tipos de registros e taxonomias do espaço de trabalho selecionado estão disponíveis para conexão.
     > 
     >Se você não tiver outros tipos de registro no espaço de trabalho selecionado, o nome do espaço de trabalho não será exibido.

   * A **Projeto, Portfolio, Programa, Empresa** ou **Grupo** do **Tipos de objeto do Workfront** seção.
   * **Experience Manager Assets** do **Aplicativos Adobe** seção.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Atualize as seguintes informações:

   * **Nome**: o nome do campo conectado, como ele aparecerá na exibição de tabela ou na página Detalhes do tipo de registro original. Isso cria a coluna de registro vinculado na exibição de tabela do tipo de registro original ou no campo de registro vinculado dos registros originais. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >É recomendável incluir o nome do registro ao qual você está vinculando no nome do campo de registro conectado para capturar de que tipo de registro o novo campo vem. O nome do registro vinculado não está visível no novo campo de registro vinculado ou em seus campos vinculados.

   * **Descrição**: informações adicionais sobre o campo de registro conectado. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Permitir vários registros**: selecione essa opção para indicar que você permite que os usuários possam adicionar vários registros quando o campo de tipo de registro vinculado for exibido nos registros originais. É selecionado por padrão.
   * **Selecionar campos de pesquisa**: selecione essa opção para adicionar campos do tipo de registro selecionado. É selecionado por padrão.

1. (Condicional e opcional) Se você selecionou conectar um objeto do Workfront, selecione um **Formulário personalizado** do **Vincular somente projetos que correspondam a estes critérios** seção. <!--this needs to be updated for each object when they fix this UI.--> Somente objetos que tenham os formulários personalizados selecionados anexados podem ser vinculados ao tipo de registro Mestre selecionado. É possível selecionar mais de um formulário.

   ![](assets/workfront-project-connection-selection.png)

1. (Condicional) Se você selecionou se conectar ao Experience Manager Assets, selecione um repositório na lista **repositório Experience Manager** menu suspenso no **Vincular ativos do seguinte repositório** seção. Este campo é obrigatório. Somente repositórios aos quais você tem acesso no Experience Manager Assets são exibidos nesse campo.

   ![](assets/aem-assets-connection-selection.png)

1. Clique em **Criar**.

1. (Condicional) Se você selecionou a variável **Selecionar campo de pesquisa** configuração, a variável **Adicionar campos de pesquisa** é aberta.

   Clique em **+** ícone para adicionar campos do **Campos não selecionados** área.

   Ou

   Clique em **-** ícone para remover campos do **Campos selecionados** área

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)


1. (Opcional) Clique em **Ignorar** e não adicione nenhum campo do registro ou objeto vinculado. A variável **Nome** do registro vinculado é o único campo visível na exibição de tabela do registro original.

1. (Opcional e condicional) Se você optar por vincular um campo do tipo número, moeda, porcentagem ou data, selecione também um valor agregador. Os valores dos campos vinculados são exibidos separados por vírgulas ou como um valor agregado de acordo com o agregador escolhido, quando os usuários selecionam mais de um registro vinculado no campo de registro vinculado.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Os agregadores não estão disponíveis ao conectar tipos de registro ao Experience Manager Assets.

   Selecione entre as seguintes opções:

   * **Nenhum**: exibe os valores que vêm de vários registros separados por vírgulas. Esta é a seleção padrão.
   * **MAX**: exibe o valor mais alto de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **MÍN**: exibe o valor mais baixo de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **SOMA**: exibe o total de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.
   * **AVG**: exibe a média de todos os valores que vêm de vários registros selecionados no campo de registro vinculado.

   >[!NOTE]
   >
   >Por exemplo, você pode vincular o registro Product (registro vinculado) do registro Campaign (registro original) e nomeá-lo como &quot;Campo de produto&quot;. Também é possível vincular o campo Budget do registro Product do registro Campaign e chamá-lo de &quot;Product Budget&quot;. Se você tiver permissão para selecionar vários registros no &quot;campo Produto&quot;, poderá selecionar o Produto 1 com um Orçamento de US$ 120.000 e o Produto 2 com um Orçamento de US$ 100.000. Você pode exibir as seguintes informações de Orçamento no campo vinculado do registro original, dependendo do agregador escolhido:
   >
   >* **Nenhum**: US$ 120.000, US$ 100.000
   >* **MAX**: US$ 120.000
   >* **MÍN**: US$ 100.000
   >* **SOMA**: US$ 220.000
   >* **AVG**: US$ 110.000
   >

1. (Opcional) Use o **pesquisa** ícone ![](assets/search-icon.png) para procurar um campo.

1. Clique em **Adicionar campos** para salvar as alterações.

   Os seguintes itens são adicionados:

   * O campo de registro vinculado que exibe os registros do tipo de registro vinculado, depois de adicioná-los manualmente. O nome do campo de registro vinculado é o nome selecionado na etapa 5. <!--accurate-->

   * O(s) campo(s) vinculado(s) que exibe(m) informações dos campos do tipo de registro vinculado depois de adicionar manualmente os registros no campo de registro vinculado. Os campos vinculados são criados somente quando a variável **Selecionar campos de pesquisa** for selecionada ao criar a conexão. Os campos vinculados são nomeados de acordo com este padrão:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * Quando você vincula tipos de registro Maestro um ao outro, um campo de registro vinculado também é adicionado ao tipo de registro ao qual você está vinculando. O nome do campo de registro vinculado no tipo de registro vinculado é o nome do tipo de registro que você vincula.

     Por exemplo, se você vincular o tipo de registro &quot;Produto&quot; do tipo de registro &quot;Campanha&quot; e nomear o campo conectado do &quot;Produto vinculado&quot; da Campanha, um campo de registro vinculado &quot;Campanha&quot; será criado para o tipo de registro Produto.

1. (Opcional) No tipo de registro original ou na exibição de tabela do tipo de registro vinculado, clique na seta para baixo no cabeçalho dos campos de registro vinculados e, em seguida, clique em uma das seguintes opções:

   * **Editar campo**: você só pode atualizar o **Nome** e a variável **Descrição** informações do campo.
   * **Editar campos de pesquisa**: adicione ou remova qualquer um dos campos do registro vinculado.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Para adicionar ou remover campos de pesquisa, siga as instruções nas etapas 9 a 13 acima. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > Não é possível adicionar os campos de pesquisa do registro vinculado ao tipo de registro vinculado que indica um objeto em um aplicativo de terceiros.
   >
   > Por exemplo, não é possível adicionar o campo de pesquisa de um objeto Maestro &quot;Campanha&quot; a partir do campo de registro vinculado &quot;Campanha&quot; exibido no tipo de registro Projeto Maestro ao vincular a projetos Workfront.


1. (Opcional) Clique na seta para baixo no cabeçalho do campo de registro vinculado do tipo de registro que está sendo vinculado e clique em **Excluir**.

   O campo de registro e quaisquer campos de pesquisa vinculados adicionais são excluídos e os campos e suas informações não podem ser recuperados.

   >[!TIP]
   >
   >    O campo de registro vinculado no tipo de registro ao qual você está vinculando não é excluído. <!-- is this still accurate?! -->
