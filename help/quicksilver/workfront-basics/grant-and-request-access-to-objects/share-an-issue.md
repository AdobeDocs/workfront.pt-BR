---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Compartilhar um problema
description: O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar problemas ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a problemas, consulte Conceder acesso a problemas.
author: Courtney
feature: Get Started with Workfront
exl-id: 91ee72e0-20a9-4b06-9f80-a343dd4fbe06
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 4%

---

# Compartilhar um problema

O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar problemas ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a problemas, consulte [Conceder acesso a problemas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md).

Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir, Contribute ou Gerenciar problemas específicos que você tenha acesso para compartilhar. Para obter mais informações sobre níveis de acesso e permissões, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.


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
   <p>Trabalhar ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir o acesso ou superior aos objetos que você deseja compartilhar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores aos objetos que você deseja compartilhar</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre problemas de compartilhamento

Além das considerações abaixo, consulte também [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

* Por padrão, o criador de um problema tem permissões de gerenciamento.
* Você pode compartilhar problemas individualmente ou compartilhar vários deles de cada vez. O compartilhamento de problemas é idêntico ao compartilhamento de outros itens no Workfront. Para obter mais informações sobre como compartilhar itens no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Você pode conceder as seguintes permissões a um problema: 

   * Exibir
   * Contribuir
   * Gerenciar

* Quando você compartilha um problema, todos os documentos anexados ao problema herdam as mesmas permissões.

  O administrador do Workfront pode especificar se os documentos devem herdar permissões de objetos superiores no nível de acesso do usuário. Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Você pode remover permissões herdadas de um problema. Para obter mais informações, consulte [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Maneiras de compartilhar um problema

* Manualmente, que é semelhante ao compartilhamento de qualquer outro objeto no Workfront.
* Automaticamente, seguindo um destes procedimentos:

   * Especifique as permissões em qualquer um dos objetos principais do problema: projeto, programa ou portfólio. Os problemas herdam as permissões de seus objetos principais. Para obter informações sobre a exibição de permissões herdadas em objetos, consulte [Exibir permissões herdadas em objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Adicione entidades ao Compartilhamento de projeto em um modelo usado para criar o projeto no qual o problema está. Para obter informações sobre como compartilhar projetos a partir de modelos, consulte [Compartilhar um modelo](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Especifique as permissões em todos os problemas em um projeto ao editá-lo. Para obter informações sobre como gerenciar o acesso a problemas ou solicitações no projeto com base nas permissões de um usuário para o projeto, consulte a seção [&#128279;](../../manage-work/projects/manage-projects/edit-projects.md#access) no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Se você não especificar as permissões de problema que deseja que os usuários tenham quando são atribuídos aos problemas no projeto, eles receberão as mesmas permissões que têm no projeto por padrão.

   * Especifique as permissões que os usuários recebem sobre problemas enviados em uma fila de solicitações ao criar uma fila de solicitações. Para obter informações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

     >[!IMPORTANT]
     >
     >As permissões são concedidas de forma diferente se o projeto for publicado ou não como uma fila de solicitações:
     >
     >   
     >   
     >   * Quando um usuário envia uma solicitação a um projeto publicado como uma fila de solicitações, o contato principal e os usuários Cadastrados por recebem a permissão especificada.
     >   * Quando um usuário envia uma solicitação a um projeto não publicado como uma fila de solicitações, o contato principal (se for diferente do usuário Informado por) recebe a permissão especificada e o usuário Informado por recebe as permissões Gerenciar para a ocorrência.
     >   
     >

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue at the project level</h2>
<p>(NOTE: this info duplicates in Edit projects - linked there instead (above).)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are added to a project.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2"> Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. </li>
<li value="3">In the <strong>Edit Project</strong> box that displays, click <strong>Access</strong>.</li>
<li value="4">In the <strong>When someone is assigned to an ISSUE</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><strong>Manage</strong><br>Now, when someone is assigned to an issue on the selected project, they are granted the specified permissions to the issue.&nbsp;</li>
</ul></li>
<li value="5">(Optional) Select the <strong>Also grant ... access to the project</strong> field to also grant View, Contribute, or Manage permissions to the projects to the user assigned to the issue</li>
<li value="6">In the <strong>When someone submits a REQUEST ...</strong> field, select from the following permissions levels:
<ul>
<li><strong>View</strong></li>
<li><strong>Contribute</strong></li>
<li><p><strong>Manage</strong></p><note type="important">
<p>Permissions are granted differently depending on whether or not the project is published as a request queue:</p>
<ul>
<li>When a user submits a request to a project published as a request queue, the Primary Contact and Entered By users are granted the permission specified.</li>
<li>When a user submits a request to a project not published as a request queue, the Primary Contact (if different from Entered By user) is granted the permission specified, and the Entered By user is granted Manage permissions to the issue.</li>
</ul>
</note></li>
</ul></li>
<li value="7"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong> field.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="8">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Automatically share an issue in request queues</h2>
<p>(NOTE: drafted because it's duplicated from Create a Request Queue which is linked above)&nbsp;</p>
<p>As the Project Owner, you can grant permissions automatically to users as the issues are submitted to a request queue.</p>
<ol>
<li value="1">Go to the project whose issues you want to share automatically.</li>
<li value="2">Click <strong>Edit Project</strong>.</li>
<li value="3">Click <strong>More</strong> then click <strong>Queue Setup</strong>. </li>
<li value="4"> <p>On the <strong>Queue Details</strong> sub-tab, in the drop-down menu under <strong>When someone makes a request, automatically grant</strong>, select from the following permissions levels:</p>
<ul>
<li><strong>View Access</strong> </li>
<li><strong>Contribute Access</strong> </li>
<li> <p><strong>Manage Access</strong> </p> </li>
</ul> <p>Now, when someone submits a request to the selected project, they are granted the specified permissions to the request.</p> </li>
<li value="5"> <p>(Optional) Select the <strong>People from the same company will inherit the same permissions for all requests</strong>.</p> <p>People from the same company as the user submitting the request are granted the same permissions on the requests as the user.&nbsp;</p> </li>
<li value="6">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Compartilhar um problema

1. Navegue até o problema que deseja compartilhar.

1. À direita do nome do problema, clique em **Compartilhar**. A caixa de diálogo **Compartilhar [Nome do Problema]** é aberta.

   ![Botão Compartilhar problema](assets/share-issue-button.png)

1. No campo **Conceder acesso ao problema**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar o problema e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar um problema com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso do problema:

   * **Somente pessoas convidadas podem acessar:** Somente usuários convidados para o problema podem acessá-lo (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir o problema sem um convite.

1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para esse problema:

   * **Exibir**: o usuário pode revisar e compartilhar o problema.
   * **Contribute**: o usuário pode fazer atualizações, registrar informações, fazer pequenas edições e compartilhar o problema (também inclui todas as permissões de exibição).
   * **Gerenciar**: o usuário tem acesso total ao problema sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição e Contribute).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas sobre o problema.

   ![Opções avançadas de permissão configuradas](assets/advanced-permission-options.png)

1. (Opcional) Para compartilhar o problema rapidamente usando um link, clique em **Copiar link** e encaminhe-o para o destinatário.

1. Clique em **Salvar**.

## Compartilhar problemas em massa

1. Navegue até o projeto que contém os problemas que você deseja compartilhar.

1. Na guia **Problemas** da página do projeto, selecione a caixa à esquerda de cada problema que você deseja compartilhar e clique no ícone **Compartilhar** ícone ![Compartilhar](assets/share-icon.png) na parte superior da página. O modal de compartilhamento é aberto.

   ![Problemas de compartilhamento em massa](assets/bulk-share-issues.png)

1. No campo **Conceder acesso ao problema para**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar os problemas e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar problemas com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso dos problemas:

   * **Somente pessoas convidadas podem acessar:** Somente usuários convidados para os problemas podem acessá-los (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir os problemas sem um convite.


1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para os problemas:

   * **Exibir**: o usuário pode revisar e compartilhar os problemas.
   * **Contribute**: o usuário pode fazer atualizações, registrar informações, fazer pequenas edições e compartilhar os problemas (também inclui todas as permissões de exibição).
   * **Gerenciar**: o usuário tem acesso total aos problemas sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição e Contribute).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas nos problemas.

   ![Opções avançadas de permissão configuradas](assets/advanced-permission-options.png)

1. Clique em **Salvar**.

## Permissões de problema

A tabela a seguir mostra quais permissões você pode conceder aos usuários ao permitir que eles vejam, contribuam ou gerenciem um problema:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Ações</strong> </td> 
   <td><strong>Gerenciar</strong> </td> 
   <td><strong>Contribute</strong> </td> 
   <td><strong>Exibir</strong> </td> 
  </tr> 
  <tr> 
   <td> <p>Adicionar problemas</p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Anexar Formulário Personalizado</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar campos personalizados</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aprovar problema</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Adicionar Um Processo De Aprovação</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Adicionar documentos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Copiar Problema*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Mover Problema</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Registre as horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Converter em Projeto*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aceitar atribuição</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Atualizações/comentários</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Modificar Datas Planejadas</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Faça Atribuições</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartilhar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Compartilhe com todo o sistema</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Controlado pelos níveis de acesso e permissões no projeto.
