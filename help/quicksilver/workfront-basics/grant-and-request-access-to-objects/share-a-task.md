---
title: Compartilhar uma tarefa
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront pode conceder acesso para exibir ou editar tarefas ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a tarefas, consulte Conceder acesso a tarefas.
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: b8a2fea8c1eac376f49201dc840f7a4fcc67d759
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 2%

---

# Compartilhar uma tarefa

O administrador do Adobe Workfront pode conceder acesso para exibir ou editar tarefas ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a tarefas, consulte [Conceder acesso a tarefas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir, Contribute ou Gerenciar tarefas específicas que você tenha acesso para compartilhar.

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.

## Considerações ao compartilhar uma tarefa

Além das considerações abaixo, consulte também [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Por padrão, o criador de uma tarefa tem Permissões de gerenciamento.
* É possível compartilhar tarefas individualmente ou várias delas de uma vez, em massa.\
  O compartilhamento de tarefas é idêntico ao compartilhamento de outros objetos. Para obter mais informações sobre como compartilhar itens no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Você pode conceder as seguintes permissões a uma tarefa: 

   * Exibir
   * Gerenciar
   * Contribuir
* Quando você compartilha uma tarefa, os usuários herdam as mesmas permissões em todos os objetos filhos associados à tarefa, por padrão. Por exemplo, elas herdam as mesmas permissões nas tarefas filhas, problemas e documentos anexados à tarefa.\
  Para obter mais informações sobre a hierarquia de objetos no Workfront, consulte  [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  O administrador do Workfront pode especificar se os documentos devem herdar permissões de objetos superiores no nível de acesso do usuário. Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Você pode remover permissões herdadas de uma tarefa.\
  Para obter mais informações sobre como remover permissões herdadas de objetos, consulte  [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Maneiras de compartilhar uma tarefa

Você pode compartilhar uma tarefa das seguintes maneiras:

* Manualmente, individualmente ou em massa. O compartilhamento manual de tarefas é semelhante ao compartilhamento de qualquer outro objeto no Workfront.

  Para obter mais informações sobre o compartilhamento de objetos no Workfront, consulte  [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Automaticamente, fazendo o seguinte:

   * Especifique as permissões em qualquer um dos objetos principais da tarefa: projeto, programa ou portfólio. As tarefas herdam as permissões de seus objetos principais. Para obter informações sobre a exibição de permissões herdadas em objetos, consulte [Exibir permissões herdadas em objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Adicione entidades ao Compartilhamento de projeto em um modelo usado para criar o projeto no qual a tarefa está. Para obter informações sobre como compartilhar projetos a partir de modelos, consulte [Compartilhar um modelo](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Especifique as permissões em todas as tarefas em um projeto ao editá-lo. Para obter informações sobre como gerenciar o acesso a tarefas no projeto com base nas permissões de um usuário para o projeto, consulte a seção [](../../manage-work/projects/manage-projects/edit-projects.md#access) no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >Se você não especificar as permissões de tarefa que deseja que os usuários tenham quando são atribuídos às tarefas no projeto, eles receberão as mesmas permissões que têm no projeto, por padrão.

## Permissões de tarefa

A tabela a seguir mostra quais permissões você pode conceder aos usuários ao permitir que eles exibam, contribuam ou gerenciem uma tarefa:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Ação</strong> </th> 
   <th><strong>Gerenciar</strong> </th> 
   <th><strong>Contribute</strong> </th> 
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
   <td scope="row">Adicionar problema(s)</td> 
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
   <td scope="row"> <p>Edição de tarefa geral<br></p> </td> 
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
   <td scope="row">Copiar tarefa*</td> 
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
   <td scope="row">Aceitar atribuição</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Faça uma atribuição</td> 
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
   <td scope="row">Atualizações/Comentários</td> 
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

&#42;Controlado pelo nível de acesso e pelas permissões no projeto.
