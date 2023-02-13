---
title: Compartilhar uma tarefa
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront pode conceder acesso para exibir ou editar tarefas ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a tarefas, consulte Conceder acesso a tarefas.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 4%

---

# Compartilhar uma tarefa

O administrador do Adobe Workfront pode conceder acesso para exibir ou editar tarefas ao atribuir níveis de acesso. Para obter mais informações sobre a concessão de acesso a tarefas, consulte [Conceder acesso a tarefas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Além do nível de acesso que os usuários recebem, você também pode conceder permissões para Exibir, Contribuir ou Gerenciar tarefas específicas que você tem acesso para compartilhar.

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.

## Considerações ao compartilhar uma tarefa

Além das considerações abaixo, consulte também [Visão geral do compartilhamento de permissões em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Por padrão, o criador de uma tarefa tem permissões de gerenciamento.
* Você pode compartilhar tarefas individualmente ou pode compartilhá-las várias de cada vez, em massa.\
   O compartilhamento de tarefas é idêntico ao compartilhamento de outros objetos. Para obter mais informações sobre como compartilhar itens no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Você pode conceder as seguintes permissões a uma tarefa: 

   * Exibir
   * Gerenciar
   * Contribuir\
      ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* Quando você compartilha uma tarefa, os usuários herdam as mesmas permissões em todos os objetos filhos associados à tarefa, por padrão. Por exemplo, eles herdam as mesmas permissões nas tarefas secundárias, problemas e documentos anexados à tarefa.\
   Para obter mais informações sobre a hierarquia de objetos no Workfront, consulte  [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   O administrador do Workfront pode especificar se os documentos devem herdar permissões de objetos mais altos no nível de acesso do usuário. Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Você pode remover permissões herdadas de uma tarefa.\
   Para obter mais informações sobre como remover permissões herdadas de objetos, consulte  [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Maneiras de compartilhar uma tarefa

Você pode compartilhar uma tarefa das seguintes maneiras:

* Manualmente, individualmente ou em massa. O compartilhamento manual de tarefas é semelhante ao compartilhamento de qualquer outro objeto no Workfront.

   Para obter mais informações sobre o compartilhamento de objetos no Workfront, consulte  [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automaticamente, fazendo o seguinte:

   * Especifique as permissões em qualquer um dos objetos pai da tarefa: projeto, programa ou portfólio. As tarefas herdam as permissões de seus objetos pai. Para obter informações sobre como visualizar permissões herdadas em objetos, consulte [Exibir permissões herdadas em objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Adicione entidades ao Compartilhamento de projeto em um modelo usado para criar o projeto no qual a tarefa está. Para obter informações sobre o compartilhamento de projetos a partir de modelos, consulte [Compartilhar um modelo](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Especifique as permissões em todas as tarefas em um projeto ao editar o projeto. Para obter informações sobre como gerenciar o acesso a tarefas no projeto com base nas permissões de um usuário para o projeto, consulte o [](../../manage-work/projects/manage-projects/edit-projects.md#access) no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).
   >[!TIP]
   >
   >Se você não especificar quais permissões de tarefa você deseja que os usuários tenham quando estiverem atribuídos às tarefas no projeto, eles receberão as mesmas permissões que têm no projeto, por padrão.

## Permissões de tarefa

A tabela a seguir exibe quais permissões você pode conceder aos usuários ao permitir que eles visualizem, colaborem ou gerenciem uma tarefa:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Ação</strong> </th> 
   <th><strong>Gerenciar</strong> </th> 
   <th><strong>Contribuir</strong> </th> 
   <th><strong>Exibir</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Adicionar tarefa(s)</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Adicionar predecessores</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Adicionar problemas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Excluir Tarefa</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>Edição de Tarefa Geral<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Alterar Status da Tarefa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar Restrição de Tarefa</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Exibir Tarefa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Adicionar documento(s)</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Copiar Tarefa*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Mover Tarefa*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Registre as horas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Modificar Datas Planejadas</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aceitar Atribuição</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Fazer uma atribuição</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Anexar Formulário Personalizado</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Editar campos personalizados</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Criar um processo de aprovação</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aprovar Uma Tarefa</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Editar finanças*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Adicionar/Editar Despesas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Exibir finanças</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Atualizações/comentários</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Compartilhe com todo o sistema</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Controlada pelo nível de acesso e pelas permissões no projeto.
