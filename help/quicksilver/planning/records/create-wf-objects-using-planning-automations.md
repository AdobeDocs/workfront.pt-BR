---
title: Criar Objetos Workfront Usando Automações de Registro do Adobe Workfront Planning
description: Você pode configurar automações no Adobe Workfront Planning que, quando ativadas, criam objetos no Workfront ou registros no Workfront Planning. Os objetos e registros criados são conectados automaticamente aos registros existentes do Planning. Este artigo descreve como gerenciar automações, incluindo como editá-las, desativá-las, excluí-las e acioná-las para criar objetos e registros.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '2218'
ht-degree: 2%

---

# Criar objetos usando automações de registro do Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Você pode configurar automações no Adobe Workfront Planning que, quando ativadas, criam objetos no Workfront ou registros no Workfront Planning quando acionadas a partir de um registro do Planning. Os objetos ou registros criados são conectados automaticamente aos registros dos quais você está acionando a automação.

Você pode configurar e ativar a automação na página do tipo de registro no Workfront Planning. O objeto conectado criado é colocado no campo conectado do tipo de registro a partir do qual a automação é executada.

Por exemplo, você pode criar uma automação que use uma campanha do Workfront Planning e crie um projeto no Workfront para rastrear o progresso dessa campanha. O projeto seria conectado à campanha do Workfront Planning no campo Connected Project da campanha.

Para obter mais informações sobre registros conectados, consulte [Visão geral dos registros conectados](/help/quicksilver/planning/records/connected-records-overview.md).

Você pode criar o seguinte usando automações no Workfront Planning:

* Um ou vários projetos
* Um grupo
* Um programa
* Um portfólio
* Um projeto
* Registro A

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

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
<p>Qualquer </p> 
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
   <td> Padrão
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p> 
   <p>Edite o acesso com acesso para Criar objetos no Workfront para os tipos de objeto que você deseja criar (projetos, portfólios, programas). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Gerencie permissões no espaço de trabalho para criar automações. </p>
   <p>Contribute ou aumente as permissões para o espaço de trabalho <span class="preview">e para o tipo de registro</span> onde você deseja criar o objeto usando as automações existentes. </p>  
   <p>Gerencie permissões para objetos do Workfront (portfólios) para adicionar objetos secundários (programas ou projetos).</p>
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>No ambiente de Produção, todos os usuários, inclusive os Administradores do Sistema, devem ser atribuídos a um modelo de layout que inclua o Planning.</p>
<p><span class="preview">No ambiente de Pré-visualização, os usuários do Standard e os administradores do sistema têm o Planning habilitado por padrão.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerações sobre a criação de objetos e registros usando uma automação

* O nome do objeto ou registro criado por uma automação é igual ao nome do registro a partir do qual você o cria, ao criar um único objeto.

* Ao criar vários projetos, eles são nomeados automaticamente de acordo com o seguinte padrão:

  `[ Name of the record ] Name of the field choice`

  Para obter mais informações, consulte a seção [Usar uma automação do Workfront Planning para criar um objeto ou um registro](#use-a-workfront-planning-automation-to-create-an-object-or-a-record) neste artigo.

* Novos objetos ou registros não substituem os existentes no mesmo campo. Acionar a mesma automação várias vezes para o mesmo registro adiciona os novos objetos ou registros no mesmo campo conectado do registro original, além dos criados antes.

<!--hide this for now; they are trying to remove this limitation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->

## Configurar uma automação no Workfront Planning

Você deve configurar uma automação para um tipo de registro no Workfront Planning antes de usá-la para criar objetos.

{{step1-to-planning}}

1. Clique em um cartão de tipo de registro e no nome de um registro.

   A página de tipo de registro é aberta.
1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Gerenciar automações**.

   A lista de automações disponíveis para o tipo de registro selecionado é aberta.

1. Clique em **Nova automação** no canto superior direito da tela. A caixa **Nova automação** é aberta.
1. Atualize os seguintes campos:

   * Substitua **Automação sem título** pelo texto que você deseja que apareça no botão de automação. Os usuários clicarão nesse botão ao usar a automação para criar um objeto do Workfront ou um registro do Planning.
   * **Descrição**: adicione uma descrição para identificar a finalidade da automação.
1. Clique em **Salvar**.
A página de detalhes da automação é aberta.

1. Na página de detalhes da automação, atualize os seguintes campos na seção **Triggers**:

   * **Acionador**: selecione a ação que acionará a automação. Por exemplo, selecione **Botão, clique**. <!--update this step with a list of all possible triggers; right now only Button click is available-->

1. Atualizar os seguintes campos na seção **Ações**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Ações**: selecione a ação que você deseja que o Workfront execute ao acionar a automação. Este campo é obrigatório.
Selecione uma das seguintes ações:

      * Criar vários projetos
      * Criar um único projeto
      * Criar um projeto
      * Criar registro
      * Criar programa
      * Criar portfólio
      * Criar grupo

     >[!TIP]
     >
     >Depois de salvar a automação, não é mais possível alterar a ação selecionada nesse campo.

1. (Condicional) Dependendo da ação selecionada, atualize os seguintes campos:

   * **Criar um único projeto**: <!--replace to the left: Create a single project-->
      * **Campo conectado onde o projeto é criado**: este é o campo conectado onde o novo projeto será exibido. Este campo é obrigatório.
      * **Modelo de projeto**: selecione um modelo de projeto que a Workfront usará para criar o projeto.

   * Criar vários projetos:
      * **Campo conectado onde o projeto é criado**: este é o campo conectado onde o novo projeto será exibido. Este campo é obrigatório.
      * **Campo cujas opções criarão os registros**: escolha um campo de seleção única ou múltipla do tipo de registro selecionado. O Workfront cria um projeto para cada opção de campo atualmente selecionada no registro de onde você aciona a automação.

     >[!TIP]
     >
     >Um projeto é criado apenas para as opções atualmente selecionadas no campo de seleção múltipla ou única do registro a partir do qual você está executando a automação, e não para todas as opções possíveis para esse campo.
     >

      * **Usar o mesmo modelo**: selecione esta opção para usar o mesmo modelo para cada novo projeto. Se a opção estiver desmarcada, selecione um **Modelo de projeto** para cada escolha de campo.
      * **Modelo de projeto**: se você selecionou a opção **Usar o mesmo modelo**, selecione um modelo de projeto que a Workfront usará para criar os projetos.

   * **Criar portfólio**:
      * **Campo conectado onde o portfólio é criado**: este é o campo conectado onde o novo portfólio será exibido. Este campo é obrigatório.
      * **Formulário personalizado para anexar ao novo portfólio**: selecione um formulário personalizado para anexar ao novo portfólio. Você deve criar um formulário personalizado do portfólio antes de selecioná-lo.
   * **Criar programa**:
      * **Campo conectado onde o programa é criado**: este é o campo conectado onde o novo programa será exibido. Este campo é obrigatório.
      * **Portfólio de programas**: selecione um portfólio onde o novo programa será adicionado. Este campo é obrigatório.
      * **Formulário personalizado para anexar ao novo programa**: selecione um formulário personalizado para anexar ao novo programa. Você deve criar um formulário personalizado de programa antes de selecioná-lo.
   * **Criar grupo**:
      * **Campo conectado onde o grupo é criado**: este é o campo conectado onde o novo grupo será exibido. Este campo é obrigatório.
      * **Formulário personalizado para anexar ao novo grupo**: selecione um formulário personalizado para anexar ao novo programa. Você deve criar um formulário personalizado de programa antes de selecioná-lo.
   * **Criar registro**:
      * **Tipo de registro**: selecione o tipo de registro que deseja criar.

        A subseção **Settings** é exibida. Atualize os seguintes campos na subseção **Configurações**:

         * **Campo no tipo de registro conectado onde o registro atual será exibido**: este é o campo conectado no tipo de registro selecionado para a ação onde o registro atual será exibido.

        Por exemplo, se estiver criando uma automação para que as campanhas conectem registros de Produto do, esse será o campo conectado no tipo de registro de Produto em que as campanhas serão exibidas, depois que os produtos forem criados usando a automação.

        Este campo é obrigatório.

        <!--submitted a change in functionality and UI text for this - revise??-->
Na área **Mapear campos**, atualize as seguintes informações:

         * **Transferir de**: selecione campos do tipo de registro para o qual a automação é criada para mapeá-los para os campos do tipo de registro conectado.
         * **Transferir para**: selecione campos do registro recém-criado que serão preenchidos com informações do registro a partir do qual você está executando a automação.

        >[!TIP]
        >
        >* Os tipos de campo do tipo de registro original devem corresponder aos tipos de campo do tipo de registro recém-criado.
        >* Se você não escolher nenhum campo, os nomes dos novos registros serão **Registro sem título**.

1. (Opcional e condicional) Se você optou por criar um registro, clique em **Adicionar campos** para mapear campos de pesquisa adicionais de um registro para outro.
1. (Condicional) Se não houver campos de conexão entre o tipo de registro original e o tipo de registro selecionado no campo **Tipo de registro**, clique em **Adicionar campo conectado**.

   ![Configuração de automação para criar um registro](assets/automation-setup-create-record.png)

   Os dois campos a seguir são criados:

   * Um novo campo de conexão chamado **Registro conectado** é criado para o tipo de registro indicado no campo **Tipo de registro**.
   * Um novo campo de conexão com o mesmo nome que o indicado no campo **Tipo de registro** é criado para o tipo de registro para o qual você está configurando a automação.

     Por exemplo, se você estiver configurando uma automação para que o Campaigns crie automaticamente outro tipo de registro chamado Marcas e clicar em **Adicionar campo conectado**, os seguintes campos serão criados:

      * O campo de conexão **Registro conectado** foi criado para o tipo de registro **Marcas**.
      * O campo de conexão **Marcas** é criado para o tipo de registro **Campanhas**.

1. (Opcional) Se não houver campos de conexão entre o tipo de registro original e o objeto do Workfront selecionado na área Ações, clique em **Adicionar campo conectado**.

   ![Configuração de automação para criar vários projetos](assets/automation-setup-create-multiple-projects.png)

   Os itens a seguir são criados:

   * Um novo campo de conexão chamado **Conectado &lt; nome do objeto Workfront >** é criado para o tipo de registro para o qual você criou a automação. Por exemplo, um campo **Projeto conectado** é criado para o tipo de registro para o qual você está criando a automação, quando você opta por criar projetos automaticamente.
   * Um novo cartão de tipo de registro é adicionado à seção Planejamento de um projeto do Workfront, no Workfront, com o nome do tipo de registro para o qual você está configurando a automação.

1. Clique em **Salvar** no canto superior direito da página de detalhes de automação.

   A automação é exibida na lista de automações e está disponível para uso em registros.

## Gerenciar automações existentes

{{step1-to-planning}}

1. Clique em um cartão de tipo de registro e no nome de um registro.

   A página de tipo de registro é aberta.
1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Gerenciar automações**.

   A lista de automações disponíveis para o tipo de registro selecionado é aberta.

1. (Opcional) Para editar, desativar ou excluir uma automação, siga um destes procedimentos:

   1. Na lista de automações, passe o mouse sobre o nome de uma automação salva e clique no menu **Mais** ![Mais menu](assets/more-menu.png).

   1. Clique em **Editar** para atualizar as seguintes informações:

      * Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome da automação e clique em **Editar** para alterar o nome da automação.
      * Qualquer campo na automação, exceto o campo **Ações**.

        >[!TIP]
        >
        >Não é possível alterar a ação originalmente selecionada para uma automação.


   1. Clique em **Desabilitar** para remover a automação da exibição de tabela do registro e impedir que os usuários a utilizem para criar registros ou objetos.

      Os registros que foram criados usando uma automação desativada permanecem conectados ao registro selecionado originalmente.

      Para torná-lo disponível novamente, clique novamente no menu **Mais**, no menu ![Mais](assets/more-menu.png), depois clique em **Ativar**.
   1. Clique em **Excluir** para excluir a automação. Uma automação excluída não pode ser recuperada.

      Os registros que foram criados usando uma automação excluída permanecem conectados ao registro selecionado originalmente.

## Usar uma automação do Workfront Planning para criar um objeto ou um registro

1. No Workfront Planning, abra a página tipo de registro que contém a automação que deseja usar para criar e conectar automaticamente registros ou objetos.
1. Abra a exibição de tabela.
1. Selecione um ou mais registros.

   Uma barra azul é exibida na parte inferior da tabela com botões adicionais, incluindo botões de automação.
1. Clique no botão de automação próximo ao canto inferior direito da tela.

   ![Botão de automação](assets/automation-custom-button.png)

   As seguintes situações ocorrem:

   * Uma mensagem de confirmação é exibida na parte inferior da tela, caso a automação tenha criado um objeto ou um registro com êxito.

   * O novo objeto é exibido no campo conectado indicado na configuração do botão de automação. Talvez seja necessário atualizar a página antes de visualizar o novo objeto. O novo objeto tem o mesmo nome do registro original.

   * Se vários projetos foram criados com base nas opções de campos de seleção múltipla ou única, os projetos são nomeados automaticamente de acordo com o seguinte padrão:

     `[ Name of the record ] Name of the field choice`

     Por exemplo, se uma campanha chamada `Summer breeze` gerou um projeto a partir de uma escolha de campo de `EMEA`, o projeto é nomeado como `[ Summer breeze ] EMEA`.

   * O registro do qual você está acionando a automação é adicionado ao campo conectado dos novos registros.

   >[!NOTE]
   >
   >Recomendamos verificar se os objetos ou registros foram criados e conectados conforme esperado.

1. (Opcional) Clique no novo objeto no campo conectado. A página do objeto é aberta e você pode fazer alterações adicionais no novo objeto.

<!--ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements. 

You must have the following access to perform the steps in this article:  

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
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

