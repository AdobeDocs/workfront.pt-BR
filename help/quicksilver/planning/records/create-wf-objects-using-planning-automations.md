---
title: Criar Objetos Workfront Usando Automações de Registro do Adobe Workfront Planning
description: Você pode configurar automações no Workfront Planning que, quando ativadas, criam objetos no Workfront.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 3%

---

# Criar objetos usando automações de registro do Adobe Workfront Planning

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Você pode configurar automações no Adobe Workfront Planning que, quando ativadas, criam objetos no Workfront ou no Workfront Planning.

Você pode configurar e ativar a automação na página do registro. O objeto criado é conectado ao registro do Planning e colocado no campo especificado na automação.

Por exemplo, você pode criar uma automação que use uma campanha do Workfront Planning e crie um projeto no Workfront para rastrear o progresso dessa campanha. O projeto seria conectado à campanha de Planejamento do Workfront.

Para obter mais informações sobre registros conectados, consulte [Visão geral dos registros conectados](/help/quicksilver/planning/records/connected-records-overview.md).

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
   <td> Padrão
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p> 
   <p>Edite o acesso no Workfront para os tipos de objeto que deseja criar (projetos, portfólios, programas). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Gerencie permissões no espaço de trabalho ao qual deseja adicionar registros. </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   <p>Gerencie permissões para objetos do Workfront (portfólios) para adicionar objetos secundários (projetos).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerações sobre a criação de objetos e registros usando uma automação

* O novo objeto ou nome de registro é igual ao nome do registro a partir do qual você o cria.
* Se o registro usado para a automação já tiver objetos do mesmo tipo conectados no campo selecionado para adicionar novos objetos, os novos objetos serão adicionados ao campo de conexão e os objetos existentes também permanecerão conectados.

## Configurar uma automação no Workfront Planning

Você deve configurar uma automação no Workfront Planning antes de usá-la para criar objetos.

{{step1-to-planning}}

1. Clique em um cartão de tipo de registro e no nome de um registro.

   A página de tipo de registro é aberta.
1. Clique no menu **Mais** ![](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Gerenciar automações**.

   A lista de automações disponíveis é aberta.

1. Clique em **Nova automação** no canto superior direito da tela. A caixa **Nova automação** é aberta.
1. Atualize os seguintes campos:

   * Substitua **Automação sem título** pelo texto que você deseja que apareça no botão de automação. Os usuários clicarão nesse botão ao usar a automação para criar um objeto do Workfront.
   * **Descrição**: adicione uma descrição para identificar a finalidade da automação.

1. Na página de detalhes da automação, atualize os seguintes campos na seção **Triggers**:

   * **Acionador**: selecione a ação que acionará a automação. Por exemplo, selecione **Botão, clique**. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Atualize os seguintes campos na seção **Ações**:
   * **Tipo de objeto**: selecione o objeto que você deseja que a automação crie. Este campo é obrigatório.

     Você pode criar os seguintes objetos a partir dos registros do Workfront Planning:

      * Projeto
      * Portfólio
      * Programa
      * Grupo
      * Registro
1. (Condicional) Dependendo do tipo de objeto que você deseja criar, atualize os seguintes campos:

   * **Projeto**:
      * **Campo conectado onde o objeto é criado**: este é o campo conectado onde o novo projeto será exibido. Este campo é obrigatório
      * **Modelo a partir do qual criar o projeto**: selecione um modelo de projeto que a Workfront usará para criar o projeto.
   * **Portfolio**:
      * **Campo conectado onde o objeto é criado**: este é o campo conectado onde o novo portfólio será exibido. Este campo é obrigatório.
      * **Formulário personalizado para anexar ao novo portfólio**: selecione um formulário personalizado para anexar ao novo portfólio. Você deve criar um formulário personalizado do portfólio antes de selecioná-lo.
   * **Programa**:
      * **Campo conectado onde o objeto é criado**: este é o campo conectado onde o novo programa será exibido. Este campo é obrigatório.
      * **Portfólio de programas**: selecione um portfólio onde o novo programa será adicionado. Este campo é obrigatório.
      * 
         * **Formulário personalizado para anexar ao novo programa**: selecione um formulário personalizado para anexar ao novo programa. Você deve criar um formulário personalizado de programa antes de selecioná-lo.
   * **Grupo**:
      * **Campo conectado onde o objeto é criado**: este é o campo conectado onde o novo grupo será exibido. Este campo é obrigatório.
      * **Formulário personalizado para anexar ao novo grupo**: selecione um formulário personalizado para anexar ao novo programa. Você deve criar um formulário personalizado de programa antes de selecioná-lo.
   * **Registro**:
      * **Tipo de registro conectado**: selecione o tipo de registro que deseja criar.
      * **Campo conectado onde o registro é criado**: é o campo conectado onde o novo registro será exibido. Este campo é obrigatório.
      * **Mapear campo**: selecione campos do tipo de registro para o qual a automação é criada para mapeá-los aos campos do tipo de registro conectado.
      * **Para o campo de registro conectado**: selecione campos do registro conectado que corresponderão aos campos do tipo de registro para o qual você criou a automação.
1. (Opcional e condicional) Se você não tiver um campo de conexão para um tipo de objeto do Workfront, clique no ícone ![](assets/create-a-connection-field-icon.png) **Criar um campo de conexão** para adicionar um campo.
1. (Opcional e condicional) Se você optou por adicionar um registro, clique em **Adicionar** na área **Mapear campos** para adicionar e mapear campos adicionais, em seguida, selecione um campo para **Transferir de** e um campo para **Transferir para** para indicar qual campo do registro selecionado originalmente deve ser exibido em qual campo do registro conectado.
1. Clique em **Salvar**.

   A automação aparece na lista de automações e está disponível para uso em registros.
1. (Opcional) Para editar, desativar ou excluir uma automação, faça o seguinte:

   Na lista de automações, passe o mouse sobre o nome de uma automação salva, em seguida, clique no menu **Mais** ![](assets/more-menu.png) e escolha uma das seguintes opções:

   * **Editar**: atualize as informações sobre os campos e configure-os na automação.
   * **Desabilitar**: a automação não será exibida como uma opção na barra de ferramentas da exibição de tabela dos registros, e os usuários não poderão mais usá-la para criar registros ou objetos. Para torná-lo disponível novamente, clique novamente no menu **Mais** ![](assets/more-menu.png) e clique em **Ativar**.
   * **Excluir**: a automação foi excluída e não pode ser recuperada. Os registros criados por meio da automação permanecem conectados ao registro selecionado originalmente.

## Usar uma automação do Workfront Planning para criar um objeto

1. No Workfront Planning, abra a página tipo de registro que contém os registros que você deseja usar para criar objetos do Workfront.
1. Abra a exibição de tabela.
1. Selecione um ou mais registros.

   Uma barra azul é exibida na parte inferior da tabela com botões adicionais, incluindo botões de automação.
1. Clique no botão de automação próximo ao canto inferior direito da tela.

   ![Botão de automação](assets/automation-custom-button.png)

   O novo objeto é exibido no campo conectado indicado na configuração do botão de automação.

   >[!NOTE]
   >
   >Recomendamos verificar se o objeto foi criado e conectado conforme esperado.

1. (Opcional) Clique no novo objeto no campo conectado. A página do objeto é aberta e você pode fazer alterações adicionais no novo objeto.

<!--you might need to add something about notifications and emails?!-->
