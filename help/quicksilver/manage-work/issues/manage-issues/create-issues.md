---
product-area: projects
navigation-topic: manage-issues
title: Criar Problemas
description: Ao trabalhar em um projeto, você pode descobrir que eventos inesperados surgem. Você pode registrar esses eventos inesperados como problemas para um projeto específico ou de uma tarefa. Os usuários com acesso apropriado podem visualizar e monitorar o status dos problemas à medida que o projeto ou a tarefa avança até a conclusão, eliminando a necessidade de longas cadeias de email ou reuniões de status. Ao contrário das tarefas, que são eventos planejados, os problemas representam itens de trabalho não planejados no Adobe Workfront.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 0%

---

# Criar problemas

<!--Audited: 08/2025-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

Ao trabalhar em um projeto, você pode descobrir que eventos inesperados surgem. Você pode registrar esses eventos inesperados como problemas para um projeto específico ou de uma tarefa. Os usuários com acesso apropriado podem visualizar e monitorar o status dos problemas à medida que o projeto ou a tarefa avança até a conclusão, eliminando a necessidade de longas cadeias de email ou reuniões de status. Ao contrário das tarefas, que são eventos planejados, os problemas representam itens de trabalho não planejados no Adobe Workfront.

Você também pode adicionar problemas a projetos como solicitações. Para obter informações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Problemas e solicitações são usados alternadamente no Workfront. Você pode registrar problemas em projetos e tarefas para indicar trabalho imprevisto que precisa ser resolvido. Você também pode enviar solicitações que são registradas como ocorrências em um projeto designado como uma Fila de solicitações.

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
   <td>
   <ul><li>Colaborador ou superior</li>
   <li>Leve ou superior para editar problemas na seção Problemas de uma tarefa ou projeto</li></ul>
   Ou
   <ul><li>Solicitação ou superior</li> <li>Revisar ou editar problemas na seção Problemas de uma tarefa ou projeto</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior a projetos e tarefas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões do Contribute ou superior com capacidade para adicionar problemas à tarefa ou projeto em que você cria o problema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license:</p>
   <ul><li>Contributor or higher</li>
   <li>Light or higher to edit issues in the Issues section of a task or project</li></ul>
   <p>Current license:</p>
  <ul><li>Request or higher</li> <li>Review or higher to edit issues in the Issues section of a task or a project</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions with ability to Add Issues to the task or project where you create the issue</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitações na criação de problemas

Quando você tem o acesso e as permissões corretas, é possível criar problemas em um projeto ou tarefa. No entanto, os seguintes casos ocorrem quando talvez você não consiga criar problemas:

* O administrador do Workfront ou um administrador de grupo deve ativar a adição de problemas a um projeto com status Concluído ou Inativo na área Preferências do projeto. Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Não é possível adicionar problemas a um projeto que está em Aprovação pendente.

## Preparar o formulário Novo problema

Sua organização deve ter um processo bem definido para quando e como registrar um problema. Ao configurar esse processo, a primeira etapa é criar o formulário necessário para enviar um problema.

Os usuários podem adicionar problemas a um projeto das seguintes maneiras:

* Adicioná-los diretamente a tarefas e projetos.
* Submetê-las a uma fila de solicitações.

O formulário Novo problema pode conter informações importantes que serão úteis para resolver o problema rapidamente.

Você pode configurar o formulário Novo problema para incluir as seguintes informações quando os usuários adicionarem problemas ao projeto ou às suas tarefas:

* Campos personalizados
* Aprovações
* Atribuições (Regras de Encaminhamento)

Os campos para novos problemas ou solicitações são definidos na seção Detalhes da fila do projeto onde os problemas serão registrados.

Para obter informações sobre como configurar a seção Detalhes da Fila do projeto, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Para obter informações sobre como criar problemas enviando-os para uma fila de solicitações, consulte a seção [Criar problemas inserindo uma nova solicitação](#create-issues-by-entering-a-new-request) neste artigo.

## Criar problemas em uma tarefa ou projeto usando o botão Novo Problema

Depois de definir os campos de um novo formulário de problema em seu projeto, você pode começar a criar problemas.

Para criar um problema em uma tarefa ou um projeto:

1. Vá para um projeto em que deseja criar o problema.
1. (Opcional) Se quiser registrar o problema de uma tarefa, vá para a área **Tarefas** e clique no nome de uma tarefa.
1. Clique na seção **Problemas**.

   A lista de problemas do projeto é exibida

1. Clique em **Novo problema** na parte superior da lista de problemas.
A caixa Nova ocorrência é exibida.

   ![Caixa Novo problema](assets/new-issue-box-matches-new-request-ui.png)

1. (Condicional) Se o criador do projeto criou Tópicos de fila ou Grupos de tópicos no projeto, eles serão adicionados ao novo formulário de problema. Especifique o **Grupo de Tópicos** ou o **Tópico da Fila** do novo problema. Grupos de tópicos e Tópicos de fila têm nomes personalizados para o seu ambiente.\
   Para obter mais informações sobre como criar Grupos de Tópicos, consulte [Criar Grupos de Tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obter mais informações sobre como criar Tópicos da Fila, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Se houver apenas um Tópico da fila definido no projeto, ele será exibido automaticamente.
   * Se o Grupo de tópicos não tiver nenhum Tópico ou Grupo de tópicos na fila, nada estará disponível no menu suspenso Grupo de tópicos.

1. Adicione o nome do problema no campo **Assunto** e adicione uma **Descrição**.

1. (Condicional) Se o criador do projeto permitiu que o campo **Tipo de solicitação** fosse exibido no formulário Novo problema, selecione o tipo do seu problema dentre as seguintes opções:

   * Relatório de erro
   * Pedido de alteração
   * Problema
   * Solicitação\
     Dependendo de como o administrador do Workfront configurou as Preferências do projeto, os nomes dos tipos de problemas podem ser diferentes para você.

   >[!TIP]
   >
   >Os Tipos de solicitação devem ser ativados em Detalhes da fila e ao criar o Tópico da fila para ser exibido como uma seleção no formulário Novo problema. Para obter informações, consulte os seguintes artigos:
   >* [Criar uma Fila de Solicitações](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Criar Tópicos de Fila](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Continue especificando os campos disponíveis no formulário **Novo problema**. Para obter mais informações sobre os campos disponíveis quando você insere um novo problema, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Nem todos os campos relacionados a problemas estão disponíveis no formulário Novo problema. O criador do projeto ativa os campos disponíveis ao criar um problema ao definir a área Detalhes da fila do projeto. Para obter mais informações, consulte [Criar uma fila de solicitações](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Condicional) Se os Tópicos da fila estiverem associados a um formulário personalizado, ele será exibido no formulário **Novo problema**.\
   Ou\
   Se o projeto estiver associado a um formulário personalizado de problema por meio da área Detalhes da fila, o formulário será exibido no formulário **Novo problema**, após os campos padrão do Workfront.

   Para obter informações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clique em **Enviar**.

   Problemas podem ser atribuídos a vários usuários, funções de trabalho ou a uma equipe. Para obter mais informações sobre como atribuir e gerenciar solicitações, consulte [Gerenciar solicitações de trabalho e de equipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).


## Criar problemas em uma tarefa ou projeto em linha

>[!IMPORTANT]
>
>O proprietário do projeto deve habilitar **Permitir que os usuários adicionem problemas embutidos** ao definir configurações de problemas para o projeto antes que você possa adicionar problemas embutidos no projeto ou nas tarefas. Para obter informações sobre como definir configurações de problemas em um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Quando quiser adicionar vários problemas rapidamente, você pode criar problemas para uma tarefa ou um projeto em linha, adicionando-os a uma lista de problemas.

>[!NOTE]
>
>Ao adicionar problemas em linha, a Workfront não aplica o formulário Novo problema aos novos problemas. Não recomendamos adicionar problemas em linha se você quiser que os usuários forneçam determinadas informações ao inserir problemas. Isso pode ter um impacto negativo no relatório de problemas e, posteriormente, na capacidade do usuário atribuído ao problema de ter todas as informações necessárias para resolvê-lo.

Para criar problemas em linha:

1. Vá para um projeto em que deseja criar o problema.
1. (Opcional) Se quiser registrar o problema de uma tarefa, vá para a seção **Tarefas** e clique no nome de uma tarefa.
1. Clique na seção **Problemas** no painel esquerdo.
1. Clique em **Adicionar mais problemas** na parte inferior da lista de problemas.

   Uma nova linha é criada na lista de problemas na seção Problemas.

   >[!TIP]
   >
   >Essa opção estará esmaecida se a configuração Permitir que os usuários adicionem problemas em linha estiver desmarcada na caixa Editar projeto. Para obter informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![Botão Adicionar mais problemas](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Comece digitando o nome do problema no campo Nome e continue adicionando mais informações sobre o problema em linha.

   >[!TIP]
   >
   >Os campos disponíveis para edição em linha são disponibilizados pela visualização aplicada à lista de problemas. Talvez não seja possível editar em linha os seguintes tipos de campos:
   >   
   >* Campos que pertencem a outro objeto
   >* Campos que você não tem acesso para editar
   >* Campos que são cálculos e que são atualizados automaticamente pelo Workfront

1. Clique em Inserir para concluir a edição em linha e adicionar o problema ao projeto ou tarefa.

## Criar problemas inserindo uma nova solicitação {#create-issues-by-entering-a-new-request}

Você pode designar projetos para serem recipientes de problemas de recebimento. Esses tipos de projetos são chamados de Filas de solicitações no Workfront. Você pode acessar Filas de solicitações na área Solicitações do Menu principal.

>[!TIP]
>
>Os termos &quot;problema&quot; e &quot;solicitação&quot; são intercambiáveis no Workfront.

Para obter mais informações sobre como configurar projetos como Filas de solicitações para receber problemas, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Para obter informações sobre o envio de solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
