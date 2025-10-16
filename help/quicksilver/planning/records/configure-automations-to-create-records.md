---
title: Configurar o Adobe Workfront Planning Automations
description: Você pode configurar automações no Adobe Workfront Planning que, quando ativadas, criam objetos no Workfront ou registros no Workfront Planning. Os objetos e registros criados são conectados automaticamente aos registros existentes do Planning. Este artigo descreve como gerenciar automações, incluindo como editá-las, desativá-las ou excluí-las.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: cde20e5a-15a2-413a-8de4-ccf6eeb4395f
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 3%

---

# Configurar automações do Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Você pode configurar automações no Adobe Workfront Planning que, quando ativadas, criam objetos no Workfront ou registros no Workfront Planning quando acionadas a partir de um registro do Planning. Os objetos ou registros criados são conectados automaticamente aos registros dos quais você está acionando a automação.

Você pode configurar e ativar a automação na página do tipo de registro no Workfront Planning.

Por exemplo, você pode criar uma automação que use uma campanha do Workfront Planning e crie um projeto no Workfront para rastrear o progresso dessa campanha.

Este artigo descreve como gerenciar automações, incluindo como editá-las, desativá-las, excluí-las e acioná-las para criar objetos e registros.

Para obter informações sobre como criar registros ou objetos usando uma automação existente, consulte [Criar objetos usando as automações de registro do Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

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
<p>Qualquer Workfront e qualquer pacote do Planning</p> <p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Gerencie permissões para o espaço de trabalho e para o tipo de registro em que deseja criar automações. </p>
   <p>Os administradores do sistema têm permissões de gerenciamento para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
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
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and to the record type where you want to create automations. </p>
   <p>System Administrators have Manage permissions to all workspaces, including the ones they did not create</p>
   </td> 
  </tr> 
</tbody> 
</table> -->

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
      * Criar um projeto único
      * Criar projeto
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
