---
product-area: templates
navigation-topic: templates-navigation-topic
title: Compartilhar modelos de projeto
description: Você pode compartilhar um modelo com usuários ou definir como os projetos criados a partir de um modelo serão compartilhados com usuários usando as seguintes opções de compartilhamento no nível do modelo.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: 87bf2a4485d3b0c29fcfe8e00dcca57874cdec04
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 3%

---

# Compartilhar modelos de projeto

Você pode compartilhar um modelo com usuários ou definir como os projetos criados a partir de um modelo serão compartilhados com usuários usando as seguintes opções de compartilhamento no nível do modelo.

Ao compartilhar um objeto no Adobe Workfront, você permite que outros usuários visualizem, contribuam ou editem esse objeto.

Para obter informações sobre permissões do Workfront, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obter informações sobre as permissões que você pode conceder aos usuários ao compartilhar um modelo, consulte [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a modelos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um modelo</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Compartilhar um modelo {#share-a-template}

Você pode compartilhar seus modelos com outros usuários usando o Compartilhamento de modelos. Essa ação define quem tem permissões para o modelo.

>[!NOTE]
>
>Quando você designa um usuário ativo como o Proprietário do modelo, esse usuário recebe automaticamente permissões Gerenciar no modelo. Para obter informações sobre como designar alguém como o Proprietário do Modelo, consulte [Editar modelos de projeto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Para compartilhar um modelo:

{{step1-to-templates}}

1. Siga um destes procedimentos:\
   Clique no nome de um modelo para abri-lo e no menu **Mais**, ícone ![Mais](assets/more-icon.png) e **Compartilhamento de Modelos**.

   Ou

   Selecione um modelo na lista, clique no ícone Compartilhar ![](assets/share-icon.png) e clique em **Modelo.**

   >[!TIP]
   >
   >Você pode compartilhar um objeto somente com usuários, equipes, funções ou empresas ativos.

1. Na caixa **Acesso ao modelo**, selecione as pessoas, equipes, funções, grupos ou empresas com as quais deseja compartilhar o modelo.

   Você também pode clicar no ícone **Opções** para disponibilizar o modelo para todo o sistema:

1. No menu suspenso de cada entidade com a qual você está compartilhando, selecione uma das seguintes opções:

   * **Exibir**: os usuários com essas permissões podem exibir o modelo e criar um projeto usando-o ou anexá-lo a um projeto existente.

     >[!TIP]
     >
     >O administrador do Workfront deve fornecer acesso de Edição aos projetos para poder criar projetos.

   * **Gerenciar**: os usuários com essas permissões podem editar ou excluir o modelo.

     Para obter informações sobre as Configurações Avançadas ![](assets/gear-icon-in-access-levels.png) disponíveis aqui, consulte a seção [Configurações Avançadas para compartilhamento de modelos](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) no artigo [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Clique em **Salvar**.

## Compartilhar um projeto a partir de um modelo {#share-a-project-from-a-template}

Com o Compartilhamento de projeto de modelo, você pode definir quem tem permissões nos projetos criados a partir do modelo no nível do modelo.

Para compartilhar projetos futuros criados a partir de um modelo com os usuários:

1. Siga um destes procedimentos:\
   Clique no nome de um modelo para abri-lo e no menu **Mais**, ícone ![Mais](assets/more-icon.png) e **Compartilhamento de Modelos**.

   ![Compartilhar projeto a partir do modelo](assets/project-sharing-on-template-nwe-2022-350x172.png)

   Ou

   Selecione um modelo na lista, clique em **Compartilhar** e em **Projeto.**

1. Na caixa **Acesso ao Projeto**, selecione as pessoas, equipes, funções, grupos ou empresas com as quais o modelo é compartilhado.

   >[!TIP]
   >
   >Você pode compartilhar um objeto somente com usuários, equipes, funções ou empresas ativos.

1. No menu suspenso de cada entidade, selecione uma das seguintes opções:

   * **Sem acesso**: você pode especificar quais usuários não terão acesso ao modelo.\
     Essa opção está disponível somente ao compartilhar projetos em massa a partir de modelos. 
   * **Exibir**: os usuários com essas permissões podem exibir projetos criados a partir do modelo.
   * **Contribute**: os usuários com essas permissões podem contribuir para projetos criados a partir do modelo 
   * **Gerenciar**: os usuários com essas permissões podem gerenciar ou excluir projetos criados a partir desse modelo.

1. (Opcional) Clique no ícone **Opções** para disponibilizar os projetos para todo o sistema.
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

## Compartilhar modelos e projetos a partir de modelos em massa

É possível compartilhar vários modelos, bem como projetos de vários modelos ao mesmo tempo.

>[!NOTE]
>
>Ao selecionar vários modelos, não é possível visualizar quem já tem permissões para os modelos individuais.

1. Ir para uma lista de modelos.
1. Selecione vários modelos e clique em ![Compartilhar](assets/share-icon.png).

   ![Compartilhar modelos ou projetos em massa](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >Você pode compartilhar um objeto somente com usuários, equipes, funções ou empresas ativos.

1. Clique em **Modelo** para compartilhar os modelos selecionados.

   Ou

   Clique em **Projeto** para compartilhar os projetos que serão criados a partir dos modelos selecionados.

1. Continue compartilhando os modelos ou projetos, conforme descrito nas seguintes seções neste artigo:

   * [Compartilhar um modelo](#share-a-template)
   * [Compartilhar um projeto a partir de um modelo](#share-a-project-from-a-template)
