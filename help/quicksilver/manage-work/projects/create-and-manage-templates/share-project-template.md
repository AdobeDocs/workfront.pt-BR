---
product-area: templates
navigation-topic: templates-navigation-topic
title: Compartilhar modelos de projeto
description: Você pode compartilhar um modelo com os usuários ou definir como os projetos criados a partir de um modelo serão compartilhados com os usuários usando as seguintes opções de compartilhamento no nível do modelo.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# Compartilhar modelos de projeto

Você pode compartilhar um modelo com os usuários ou definir como os projetos criados a partir de um modelo serão compartilhados com os usuários usando as seguintes opções de compartilhamento no nível do modelo.

Ao compartilhar um objeto no Adobe Workfront, você permite que outros usuários visualizem, contribuam ou editem esse objeto.

Para obter informações sobre permissões do Workfront, consulte [Visão geral do compartilhamento de permissões em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obter informações sobre as permissões que você pode conceder aos usuários ao compartilhar um modelo, consulte [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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
   <td> <p>Editar acesso a modelos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um modelo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Compartilhar um modelo {#share-a-template}

Você pode compartilhar seus modelos com outros usuários usando o Compartilhamento de modelo. Essa ação define quem tem permissões para o modelo.

>[!NOTE]
>
>Quando você designa um usuário ativo como o Proprietário do modelo, esse usuário recebe automaticamente permissões de Gerenciamento no modelo. Para obter informações sobre como designar alguém como Proprietário do Modelo, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Para compartilhar um modelo:

1. No **Menu principal** ícone ![](assets/main-menu-icon.png), clique em **Modelos**.

1. Siga um destes procedimentos:\
   Clique no nome de um modelo para abri-lo, depois clique no botão **Mais** menu ![](assets/qs-more-icon-on-an-object.png), em seguida **Compartilhamento de modelo**.

   Ou

   Selecione um modelo na lista, clique no ícone Compartilhar ![](assets/share-icon.png), depois clique em **Modelo.**

   >[!TIP]
   >
   >É possível compartilhar um objeto somente com usuários, equipes, funções ou empresas ativas.

1. No **Acesso ao modelo** selecione as pessoas, equipes, funções, grupos ou empresas com as quais deseja compartilhar o modelo.

   Você também pode clicar no botão **Opções** ícone para disponibilizar o modelo em todo o sistema:

1. No menu suspenso de cada entidade com a qual você está compartilhando, selecione:

   * **Exibir**: Os usuários com essas permissões podem exibir o modelo e criar um projeto usando-o, ou anexá-lo a um projeto existente.

      >[!TIP]
      >
      >O administrador do Workfront deve conceder acesso ao Edit aos projetos para poder criar os projetos.

   * **Gerenciar**: Os usuários com essas permissões podem editar ou excluir o modelo.

      Para obter informações sobre as Configurações avançadas ![](assets/gear-icon-in-access-levels.png) disponível aqui, consulte a seção [Configurações avançadas para compartilhamento de modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) no artigo [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Clique em **Salvar**.

## Compartilhar um projeto a partir de um modelo {#share-a-project-from-a-template}

Com o modelo Compartilhamento de projeto, você pode definir quem tem permissões nos projetos criados a partir do modelo no nível do modelo.

Para compartilhar projetos futuros criados a partir de um modelo com os usuários:

1. Siga um destes procedimentos:\
   Clique no nome de um modelo para abri-lo, depois clique no botão **Mais** menu ![](assets/qs-more-icon-on-an-object.png), em seguida **Compartilhamento de modelo**.

   ![Compartilhar projeto do modelo](assets/project-sharing-on-template-nwe-2022-350x172.png)

   Ou

   Selecione um modelo na lista e clique em **Compartilhar**, depois clique em **Projeto.**

1. No **Acesso ao projeto** selecione as pessoas, equipes, funções, grupos ou empresas com as quais o modelo é compartilhado.

   >[!TIP]
   >
   >É possível compartilhar um objeto somente com usuários, equipes, funções ou empresas ativas.

1. No menu suspenso de cada entidade, selecione uma das seguintes opções:

   * **Sem acesso**: Você pode especificar quais usuários não terão acesso ao modelo.\
      Essa opção está disponível somente quando projetos de compartilhamento em massa são compartilhados a partir de modelos. 
   * **Exibir**: Os usuários com essas permissões podem visualizar projetos criados no modelo.
   * **Contribute**: Os usuários com essas permissões podem contribuir com projetos criados a partir do modelo 
   * **Gerenciar**: Os usuários com essas permissões podem gerenciar ou excluir projetos criados a partir desse modelo.

1. (Opcional) Clique no botão **Opções** ícone para disponibilizar os projetos em todo o sistema.
1. Clique em **Salvar**.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## Compartilhar modelos e projetos de modelos em massa

É possível compartilhar vários modelos, bem como projetos de vários modelos ao mesmo tempo.

>[!NOTE]
>
>Ao selecionar vários modelos, não é possível visualizar quem já tem permissões para os modelos individuais.

1. Vá para uma lista de templates.
1. Selecione vários modelos e clique em ![Compartilhar](assets/share-icon.png).

   ![Compartilhar modelos ou projetos em massa](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >É possível compartilhar um objeto somente com usuários, equipes, funções ou empresas ativas.

1. Clique em **Modelo** para compartilhar os modelos selecionados.

   Ou

   Clique em **Projeto** para compartilhar os projetos que serão criados a partir dos modelos selecionados.

1. Continue compartilhando os modelos ou os projetos, conforme descrito nas seguintes seções deste artigo:

   * [Compartilhar um modelo](#share-a-template)
   * [Compartilhar um projeto a partir de um modelo](#share-a-project-from-a-template)
