---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Visão geral do compartilhamento de permissões em objetos
description: É possível compartilhar ou remover permissões de um objeto criado ou compartilhado com você.
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: e3211ac5801c1318978427bc0a48d9b3a3028984
workflow-type: tm+mt
source-wordcount: '1156'
ht-degree: 1%

---

# Visão geral do compartilhamento de permissões em objetos

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->

Não é necessário ser um administrador do Adobe Workfront para compartilhar permissões em objetos aos quais você tem acesso, mas as permissões em objetos funcionam dentro dos níveis de acesso definidos pelo administrador do Workfront.

É possível compartilhar ou remover permissões de um objeto criado ou compartilhado com você. Quando você não é o criador do objeto, deve ter acesso de Compartilhamento no objeto que deseja compartilhar no nível de acesso, além de Compartilhar permissões no objeto. Para obter informações sobre níveis de acesso, consulte [Visão geral dos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) ou [Visão geral dos níveis de acesso herdados](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões de qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

## Objetos que você pode compartilhar no Workfront

É possível compartilhar os seguintes objetos no Workfront com outros usuários:

* **Projetos**: Para obter mais informações, consulte [Compartilhar um projeto no Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Modelos**: Para obter mais informações, consulte [Compartilhar modelos de projeto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolio**: Para obter mais informações, consulte [Compartilhar um portfólio](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio..md).

* **Programas**: Para obter mais informações, consulte [Compartilhar um programa](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Tarefas**: Para obter mais informações, consulte [Compartilhar uma tarefa](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Problemas**: Para obter mais informações, consulte [Compartilhar um problema](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Documentos**: Para obter mais informações, consulte [Compartilhar um documento](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Pastas de documentos**: Para obter mais informações, consulte [Compartilhar uma pasta de documentos](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Provas**: Para obter mais informações, consulte [Compartilhar uma prova na Workfront Proof](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

* **Relatórios, painéis e calendários**: Para obter mais informações, consulte [Compartilhar relatórios, painéis e calendários](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). Além disso, consulte os seguintes artigos:

   * [Compartilhar um relatório no Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Compartilhar um painel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Compartilhar um relatório de calendário](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filtros, visualizações e agrupamentos**: Para obter mais informações, consulte [Compartilhar um filtro, visualização ou agrupamento](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Planos**: Para obter mais informações, consulte [Compartilhar um plano no Planejador de Cenários](../../scenario-planner/share-a-plan.md).

   Isso requer uma licença adicional.

* **Metas**: Para obter mais informações, consulte [Compartilhar uma meta na Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

   Isso requer uma licença adicional.

## Considerações sobre o compartilhamento de objetos

* Você pode compartilhar somente o mesmo nível ou um nível inferior de permissões que tem no objeto.

   Por exemplo, se você tiver permissões do Contribute no objeto, não poderá conceder a outro usuário as permissões Gerenciar nesse objeto.

* Não é possível compartilhar um objeto com um nível de permissão superior ao nível de acesso de um usuário. Por exemplo, se um usuário tiver acesso à Exibição de projetos em seu nível de acesso, você não poderá conceder a ele permissões de Gerenciamento em um projeto.
* Um usuário com permissões para, pelo menos, Exibir um objeto pode compartilhá-lo com outra pessoa.
* É possível compartilhar objetos com usuários ativos, funções de trabalho, equipes, grupos ou empresas.

   >[!NOTE]
   >
   >Você pode compartilhar um plano ou uma meta somente com outros usuários ativos. Isso requer licenças adicionais.
   >
   >
   >Para obter mais informações, consulte:
   >
   >* [Compartilhar um plano no Planejador de Cenários](../../scenario-planner/share-a-plan.md)
   >* [Compartilhar uma meta na Workfront](../../workfront-goals/workfront-goals-settings/share-a-goal.md)


## Compartilhar limitações

É possível compartilhar um objeto com até 100 entidades (usuários, equipes, grupos, funções, empresas). Recomendamos que você compartilhe objetos com grupos, equipes ou empresas, em vez de usuários individuais, para evitar essa limitação.

## Compartilhar permissões para objetos

A tabela a seguir ilustra o nível de permissões que você pode selecionar ao compartilhar um objeto. Nem todos os objetos têm todas essas configurações disponíveis. É possível conceder a outra entidade permissões para Exibir ou gerenciar um objeto. Se você estiver compartilhando um projeto, tarefa ou problema, também poderá conceder permissões para o Contribute para ele.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Exibir</td> 
   <td> <p>É possível executar as seguintes ações no objeto :</p> 
    <ul> 
     <li>Exibir o objeto</li> 
     <li>Adicionar documentos ao objeto</li> 
     <li>Exibir informações financeiras sobre o objeto</li> 
     <li> <p>Compartilhar o objeto<br></p> <p>Quando você compartilha o objeto, pode conceder a outros usuários o mesmo nível de permissão que você tem somente no objeto, não um nível superior.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Contribuir</td> 
   <td> <p>É possível executar as seguintes ações no objeto :</p> 
    <ul> 
     <li>Visualizar o projeto</li> 
     <li>Todas as ações foram incluídas com a permissão Exibir.</li> 
     <li>Adicionar despesas a ele</li> 
     <li>Adicionar problemas a ele (se for uma tarefa ou um projeto)</li> 
     <li>Adicionar tarefas a ele (se for um projeto)</li> 
     <li>Editar Forms personalizada nele</li> 
     <li>Registrar horas no objeto</li> 
     <li>Fazer atribuições nele</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gerenciar</td> 
   <td> <p>É possível executar as seguintes ações no objeto :</p> 
    <ul> 
     <li>Visualizar o projeto</li> 
     <li>Todas as ações incluídas com as permissões Exibir e Contribuir</li> 
     <li>Exclua</li> 
     <li>Gerenciar informações financeiras nele</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tornar isto público para usuários externos</td> 
   <td> <p>Qualquer pessoa que não tenha uma conta Workfront pode exibir o objeto clicando em um link para ele. Isso não está disponível para todos os objetos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Torne isto visível para todo o sistema.</td> 
   <td> <p>O objeto pode ser encontrado em pesquisas e visualizado por qualquer pessoa com uma conta do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Entender as permissões herdadas e a hierarquia de objetos

* [Permissões herdadas de objetos pai](#permissions-inherited-from-parent-objects)
* [Permissões adquiridas através de associações organizacionais](#permissions-acquired-through-organizational-memberships) 

### Permissões herdadas de objetos pai {#permissions-inherited-from-parent-objects}

As permissões no Workfront são herdadas hierarquicamente. Isso significa que, se você estiver concedendo permissões a um usuário em um objeto pai, ele obterá as mesmas permissões nos objetos filhos associados a ele por padrão.

Por exemplo, se você conceder permissões do Contribute a um usuário a um projeto, ele terá permissões do Contribute para todas as tarefas e problemas (objetos filhos) associados ao projeto.

Continuando com o exemplo acima, não é possível restringir permissões a objetos filhos. Se você não quiser que o usuário tenha permissões do Contribute para objetos filhos associados ao projeto, remova manualmente as Permissões herdadas dos objetos e ajuste as permissões para o usuário individual, incluindo quaisquer Configurações avançadas. 

Para obter mais informações sobre a hierarquia e interdependência de objetos no Workfront, consulte a seção [Interdependência e hierarquia de objetos](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) no artigo [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>O administrador do Workfront pode desativar permissões herdadas para documentos no nível de acesso. Para obter mais informações sobre como desativar permissões herdadas para documentos no nível de acesso, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Permissões adquiridas através de associações organizacionais  {#permissions-acquired-through-organizational-memberships}

Se você conceder permissões de Gerenciamento a um Grupo de usuários em um objeto e conceder permissões de Exibição a um usuário individual nesse Grupo no mesmo objeto, o usuário terá o nível mais alto de permissões (Gerenciar) concedidas por meio da associação de Grupo no objeto. 

Se você quiser conceder permissões mais baixas a um usuário que já faz parte de uma unidade organizacional (Grupo, Equipe, Função de Trabalho ou Empresa) com um nível de permissão mais alto, remova as permissões da unidade organizacional e adicione usuários individualmente com um nível mais baixo de permissões.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Compartilhar um objeto

Para obter informações sobre como compartilhar objetos, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Remover permissões de objetos

Para obter informações sobre como remover permissões de objetos, consulte [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Solicitar permissões para objetos

Quando alguém enviar um link para um objeto que você não tem permissões para Exibir ou quando você tem permissões mais baixas em um objeto e deseja solicitar um nível mais alto de permissões, é possível solicitar permissões no objeto. 

Você pode solicitar acesso a um objeto de qualquer pessoa que tenha permissão de compartilhamento para esse objeto. 

Para obter mais informações sobre a solicitação de permissões para objetos, consulte [Solicitar acesso a objetos](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
