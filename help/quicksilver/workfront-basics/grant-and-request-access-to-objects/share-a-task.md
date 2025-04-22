---
title: Compartilhar uma tarefa
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront pode conceder acesso para exibir ou editar tarefas ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a tarefas, consulte Conceder acesso a tarefas.
author: Courtney
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: eb4bf18407562b88bf0c946c905b202e5b62a5fe
workflow-type: tm+mt
source-wordcount: '1201'
ht-degree: 1%

---

# Compartilhar uma tarefa

O administrador do Adobe Workfront pode conceder acesso para exibir ou editar tarefas ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a tarefas, consulte [Conceder acesso a tarefas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir, Contribute ou Gerenciar tarefas específicas que você tenha acesso para compartilhar.

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para compartilhar objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Padrão</p> 
   Ou
   <p>Atual: trabalho ou superior</p>
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

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações ao compartilhar uma tarefa

Além das considerações abaixo, consulte também [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Por padrão, o criador de uma tarefa tem Permissões de gerenciamento para ela.
* É possível compartilhar tarefas individualmente ou várias delas de uma vez, em massa.\
  O compartilhamento de tarefas é idêntico ao compartilhamento de outros objetos. Para obter mais informações sobre como compartilhar itens no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Você pode conceder as seguintes permissões a uma tarefa: 

   * Exibir
   * Gerenciar
   * Contribuir
* Quando você compartilha uma tarefa, os usuários herdam as mesmas permissões em todos os objetos filhos associados à tarefa por padrão. Por exemplo, elas herdam as mesmas permissões nas tarefas filhas, problemas e documentos anexados à tarefa.\
  Para obter mais informações sobre a hierarquia de objetos no Workfront, consulte  [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  O administrador do Workfront pode especificar se os documentos devem herdar permissões de objetos superiores no nível de acesso do usuário. Para obter mais informações sobre como restringir permissões herdadas em documentos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Você pode remover permissões herdadas de uma tarefa.\
  Para obter mais informações sobre como remover permissões herdadas de objetos, consulte  [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Maneiras de compartilhar uma tarefa

Você pode compartilhar uma tarefa das seguintes maneiras:

* Manualmente, individualmente ou em massa.

* Automaticamente, fazendo o seguinte:

   * Especifique as permissões em qualquer um dos objetos principais da tarefa: projeto, programa ou portfólio. As tarefas herdam as permissões de seus objetos principais. Para obter informações sobre a exibição de permissões herdadas em objetos, consulte [Exibir permissões herdadas em objetos](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Adicione entidades ao Compartilhamento de projeto em um modelo usado para criar o projeto no qual a tarefa está. Para obter informações sobre como compartilhar projetos a partir de modelos, consulte [Compartilhar um modelo](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Especifique as permissões em todas as tarefas em um projeto ao editá-lo. Para obter informações sobre como gerenciar o acesso a tarefas no projeto com base nas permissões de um usuário para o projeto, consulte a seção [](../../manage-work/projects/manage-projects/edit-projects.md#access) no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

  >[!TIP]
  >
  >Se você não especificar as permissões de tarefa que deseja que os usuários tenham quando são atribuídos às tarefas no projeto, eles receberão as mesmas permissões que têm no projeto por padrão.

## Compartilhar uma tarefa

1. Navegue até a tarefa que deseja compartilhar.

1. À direita do nome da tarefa, clique em **Compartilhar**. A caixa de diálogo **Compartilhar [Nome da Tarefa]** é aberta.

   ![Botão Compartilhar tarefa](assets/share-task-button.png)

1. No campo **Conceder acesso à tarefa**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar a tarefa e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar uma tarefa com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso da tarefa:

   * **Somente pessoas convidadas podem acessar:** Somente usuários convidados para a tarefa podem acessá-la (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir a tarefa sem um convite.

1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para essa tarefa:

   * **Exibir**: o usuário pode revisar e compartilhar a tarefa.
   * **Contribute**: o usuário pode fazer atualizações, registrar informações, fazer pequenas edições e compartilhar a tarefa (também inclui todas as permissões de exibição).
   * **Gerenciar**: o usuário tem acesso total à tarefa sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição e Contribute).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas na tarefa.

   ![Opções avançadas de permissão configuradas](assets/advanced-permission-options.png)

1. (Opcional) Para desativar as permissões herdadas para os objetos filhos da tarefa, clique em **Desativar** embutido com **Permissões herdadas**.

1. (Opcional) Para compartilhar a tarefa rapidamente usando um link, clique em **Copiar link** e encaminhe-o para o destinatário.

1. Clique em **Salvar**.


## Compartilhar tarefas em massa

1. Navegue até o projeto que contém as tarefas que você deseja compartilhar.

1. Na guia **Tarefas** da página do projeto, marque a caixa à esquerda de cada tarefa que você deseja compartilhar e clique no ícone **Compartilhar** ![Ícone Compartilhar](assets/share-icon.png) na parte superior da página. O modal de compartilhamento é aberto.

   ![Tarefas de compartilhamento em massa](assets/bulk-share-tasks.png)

1. No campo **Conceder acesso à tarefa para**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar as tarefas e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar tarefas com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso das tarefas:

   * **Somente pessoas convidadas podem acessá-las:** Somente usuários convidados para as tarefas podem acessá-las (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir as tarefas sem um convite.


1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para as tarefas:

   * **Exibir**: o usuário pode revisar e compartilhar as tarefas.
   * **Contribute**: o usuário pode fazer atualizações, registrar informações, fazer pequenas edições e compartilhar as tarefas (também inclui todas as permissões de exibição).
   * **Gerenciar**: o usuário tem acesso total às tarefas sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição e Contribute).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas nas tarefas.

   ![Opções avançadas de permissão configuradas](assets/advanced-permission-options.png)

1. Clique em **Salvar**.

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
