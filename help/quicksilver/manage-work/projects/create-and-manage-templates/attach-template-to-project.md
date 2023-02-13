---
product-area: templates
navigation-topic: templates-navigation-topic
title: Anexar um modelo a um projeto
description: Você pode anexar um modelo a um projeto durante a fase de criação inicial do projeto ou após sua criação.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---

# Anexar um modelo a um projeto

Você pode anexar um modelo a um projeto durante a fase de criação inicial do projeto ou após sua criação.

Para obter mais informações sobre como criar um projeto usando um modelo, consulte [Criar um projeto usando um modelo](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas descritas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos </p> <p>Para obter informações sobre o acesso ao projeto, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Conceder acesso aos projetos</a>.</p> <p>Exibir acesso a modelos</p> <p>Para obter informações sobre permissões de modelo, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Compartilhar um modelo</a>. </p> <p>Para obter informações sobre o acesso ao modelo, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Conceder acesso aos modelos</a>.</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto</p> <p>Para obter informações sobre permissões de projeto, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartilhar um projeto no Adobe Workfront</a>. </p> <p>Exibir permissões ou superiores ao modelo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## Anexar um modelo a um projeto existente {#attach-a-template-to-an-existing-project}

Você pode anexar um modelo a um projeto no Workfront a partir da página do projeto ou de uma lista de projetos ou relatório.

1. Vá para o projeto ao qual deseja anexar um modelo e clique no link **Mais** ícone ![](assets/qs-more-icon-on-an-object.png) à direita do nome do projeto

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Ou

   Vá para uma lista de projetos ou relatório, selecione um projeto e clique no botão **Mais** ícone ![](assets/qs-more-icon-on-an-object.png) na parte superior da lista.

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. Clique em **Anexar modelo**.

   A caixa Anexar modelo é exibida.

1. Comece a digitar o nome do modelo que deseja anexar no **Modelos de pesquisa** , em seguida, clique nele quando for exibido.na lista

   Ou

   Clique no nome de um template no **Outros modelos** área.

   Uma visualização do modelo é exibida à direita, contendo as seguintes informações sobre o modelo:

   * Duração
   * Proprietário
   * O número de tarefas de nível superior (inclui uma lista das três primeiras tarefas de nível superior)
   * Número total de tarefas
   * Nomes de formulários personalizados anexados

   ![](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Opcional) Clique no botão **Favoritos** ícone ![](assets/favorites-icon-small.png) à esquerda do nome do modelo para marcá-lo como favorito. Isso move o modelo na lista Favoritos.

   ![](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Opcional) Clique no botão **Favoritos** ícone ![](assets/favorites-icon-selected.png) novamente para removê-lo da lista Favoritos.
1. Clique em **Personalizar e anexar**.

   ![](assets/attach-template-large-box-nwe-350x262.png)

1. Atualize as informações nas seções a seguir antes de anexar o modelo (ou clique em **Anexar modelo** a qualquer momento):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Seção Tarefas</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">As tarefas de modelo selecionadas abaixo são importadas para o projeto. Desmarque as que deseja excluir. </td> 
      <td>Desmarque as tarefas que deseja excluir do modelo antes de anexá-lo ao projeto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Selecione a tarefa do projeto que deseja como predecessor para as tarefas neste template.</td> 
      <td> <p>Clique no campo para exibir uma lista de tarefas do projeto. Selecione a tarefa do projeto que deseja concluir antes que as tarefas do modelo possam ser iniciadas. Como alternativa, ignore esta etapa e configure os relacionamentos no projeto depois que o modelo for anexado. </p> <p> Selecione o <strong>Tipo de dependência</strong>, <strong>Atraso</strong> informações e se deseja que o antecessor <strong>Forçado</strong> ou não. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Selecione a tarefa do projeto que deseja como o pai das tarefas neste template.</td> 
      <td> Selecione qual tarefa do projeto você deseja designar como a tarefa pai para todas as tarefas do modelo. Se não fizer uma seleção, todas as tarefas do modelo serão exibidas no final das tarefas do projeto atual. Ignore esta etapa e mova as tarefas no projeto após o modelo ser anexado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Seção Opções</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Os itens selecionados abaixo são transferidos para o projeto. Desmarque as que deseja excluir.</td> 
      <td> <p>Desmarque as caixas de seleção ao lado de qualquer informação que deseja limpar do modelo antes de anexá-lo ao projeto. Essas informações não são transferidas do modelo para o projeto. Para obter mais informações sobre cada campo, consulte <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Visão geral de anexar um modelo a um projeto</a>. </p> <p>Importante: Se você marcar a <strong>Configuração de Propriedades e Problemas da Fila</strong> , os Detalhes da fila do modelo substituem os do projeto. Nesse caso, as Regras de roteamento, Tópicos da fila e Grupos de tópicos do modelo são adicionados aos do projeto. <br>Se o projeto estiver configurado como uma fila de solicitações e o modelo anexado ao projeto não estiver configurado como uma fila de solicitações, as informações da fila do projeto serão removidas se você deixar a variável <strong>Configuração de Propriedades e Problemas da Fila</strong> caixa marcada. <br>Se você desmarcar a <strong>Propriedades da fila e configuração de ocorrência</strong> , todas as configurações de Configuração da fila do projeto são preservadas e nenhuma configuração de configuração da fila do modelo é anexada. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Seção Forms personalizada</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Forms personalizada</td> 
      <td> <p>Quando formulários personalizados são anexados ao modelo, seus nomes são exibidos no painel esquerdo. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Atualize as informações nos formulários personalizados. Essas informações são transferidas para o projeto.

   >[!TIP]
   >
   >* Essa etapa é obrigatória quando os formulários personalizados no modelo contêm campos obrigatórios que estão vazios.
   >* Se os campos dos formulários personalizados do modelo já existirem no projeto e contiverem informações, eles preservarão as informações já existentes no projeto. Não é possível editá-las durante a anexação do template.


1. Clique em **Anexar modelo.**
1. Clique em **Cancelar anexo** para parar de anexar o template.

   Ou

   Permitir que o anexo termine para adicionar o modelo ao projeto.

   Depois de anexar o modelo, você pode editar o projeto e ajustar quaisquer tarefas, informações ou configurações, conforme necessário.

1. (Opcional) Clique em **Detalhes do projeto**, em seguida **Visão geral** para exibir o nome do modelo anexado no **Relacionamentos do projeto** área.

   >[!TIP]
   >
   >Se mais de um modelo for anexado ao projeto, somente o modelo anexado primeiro será exibido nesse campo. Para obter informações, consulte o [Anexar vários modelos a um projeto existente e exibir informações do modelo](#attach-multiple-templates-to-an-existing-project-and-view-template-information) neste artigo.

1. (Opcional) Remova as informações do modelo do projeto ao qual você anexou o modelo. Para obter mais informações, consulte [Remover informações de modelo de um projeto](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Anexar vários modelos a um projeto existente e exibir informações do modelo {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

Você pode anexar vários modelos (um de cada vez) ao mesmo projeto, seguindo as etapas descritas na seção [Anexar um modelo a um projeto existente](#attach-a-template-to-an-existing-project) neste artigo. Isso adiciona as tarefas e outras informações de cada modelo ao projeto.

>[!TIP]
>
>Ao anexar vários modelos a um projeto, somente o que você anexou primeiro é exibido na área Detalhes do projeto .

Para entender qual modelo é aplicado a um projeto:

1. Navegue até um projeto que tenha um modelo anexado.
1. Clique em **Detalhes do projeto** no painel esquerdo.
1. Encontre o nome do modelo anexado ao projeto no **Modelo** na parte inferior do **Visão geral** seção sob **Relacionamentos do projeto** .

   ![](assets/nwe-template-info-on-project-350x356.png)

 

 
