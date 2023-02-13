---
product-area: projects
navigation-topic: manage-issues
title: Criar problemas
description: Ao trabalhar em um projeto, você pode descobrir que surgem eventos inesperados. Você pode registrar esses eventos inesperados como problemas para um projeto específico ou de uma tarefa. Os usuários com o acesso apropriado podem visualizar e monitorar o status dos problemas à medida que o projeto ou a tarefa avança para a conclusão, eliminando a necessidade de longas cadeias de email ou reuniões de status. Ao contrário de tarefas, que são eventos planejados, os problemas representam itens de trabalho não planejados no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# Criar problemas

Ao trabalhar em um projeto, você pode descobrir que surgem eventos inesperados. Você pode registrar esses eventos inesperados como problemas para um projeto específico ou de uma tarefa. Os usuários com o acesso apropriado podem visualizar e monitorar o status dos problemas à medida que o projeto ou a tarefa avança para a conclusão, eliminando a necessidade de longas cadeias de email ou reuniões de status. Ao contrário de tarefas, que são eventos planejados, os problemas representam itens de trabalho não planejados no Adobe Workfront.

Você também pode adicionar problemas a projetos como solicitações. Para obter mais informações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Problemas e solicitações são usados alternadamente no Workfront. Você pode registrar problemas em projetos e tarefas para indicar trabalhos imprevistos que precisam ser abordados. Também é possível enviar solicitações registradas como problemas em um projeto designado como Fila de solicitações.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior para adicionar problemas a um projeto ou tarefa</p> <p>Solicite ou superior para adicionar problemas como solicitações, usando uma Fila de solicitações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p>Visualizar ou aumentar o acesso a Projetos e Tarefas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a problemas no Nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acesso a problemas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribua com permissões mais altas ou com a capacidade de adicionar problemas à tarefa ou projeto em que você cria o problema</p> <p> Para obter informações sobre a concessão de permissões para problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartilhar um problema </a></p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitações na criação de problemas

Quando tiver o acesso e as permissões corretas, você poderá criar problemas em um projeto ou tarefa. No entanto, os seguintes são casos em que talvez você não consiga criar problemas:

* O administrador do Workfront ou um administrador de grupo deve habilitar a adição de problemas a um projeto que esteja em um status Concluído ou Inativo na área Preferências do projeto . Para obter informações sobre como definir preferências de projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Não é possível adicionar problemas a um projeto que esteja em Aprovação pendente.

## Preparar o formulário de nova ocorrência

Sua organização deve ter um processo bem definido em vigor para quando e como registrar um problema. Ao configurar esse processo, a primeira etapa é criar o formulário necessário para o envio de um problema. Permita a adição direta de problemas a tarefas e projetos, ou se tiver filas de solicitações em que os problemas são enviados, é possível definir quais campos do Workfront, bem como quais campos personalizados estarão disponíveis para os usuários quando enviarem novos problemas e precisarem ser concluídos. O formulário Novo problema pode conter informações importantes que serão úteis para resolver o problema rapidamente.

Os campos para os novos problemas em um projeto são definidos na seção Detalhes da fila do projeto, onde os problemas serão registrados. Para obter informações sobre como configurar a seção Detalhes da fila do projeto, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Para obter informações sobre como criar problemas enviando-os para uma fila de solicitações, consulte o [Criar problemas inserindo uma nova solicitação](#create-issues-by-entering-a-new-request) neste artigo.

## Criar problemas em uma tarefa ou projeto usando o botão Nova ocorrência

Após definir os campos de um novo formulário de edição em seu projeto, você pode começar a criar problemas.

Para criar um problema em uma tarefa ou projeto:

1. Vá para um projeto em que deseja criar o problema.
1. (Opcional) Se quiser registrar o problema para uma tarefa, acesse o **Tarefas** e clique no nome de uma tarefa.
1. Clique no botão **Problemas** seção.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Clique em **Novo problema**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (Condicional) Se o criador do projeto criou Tópicos da fila ou Grupos de tópicos no projeto, eles serão adicionados ao novo formulário de edição. Especifique a **Grupo de tópicos** ou **Tópico da fila** do seu novo problema. Eles devem ter nomes personalizados para o seu ambiente.\
   Para obter mais informações sobre como criar Grupos de tópicos, consulte [Criar grupos de tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obter mais informações sobre como criar tópicos da fila, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * Se houver apenas um Tópico da fila definido no projeto, ele será exibido automaticamente.
   * Se o Grupo de tópicos não tiver tópicos da fila ou grupos de tópicos sob ele, nada estará disponível na lista suspensa Grupo de tópicos .

1. (Condicional) Se o criador do projeto tiver permitido **Tipo de problema** para exibir no formulário Nova ocorrência, selecione o tipo de seu problema nas seguintes opções:

   * Registro de Defeito
   * Pedido de alteração
   * Problema
   * Solicitar\
      Dependendo de como o administrador do Workfront configurou as Preferências do projeto, os nomes dos tipos de problema podem ser diferentes para você.

1. Especifique qualquer um dos campos disponíveis no **Novo problema** formulário. Para obter mais informações sobre como definir campos à medida que você informa uma nova edição, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).
1. (Condicional) Se os Tópicos da fila estiverem associados a um formulário personalizado, esse formulário personalizado será exibido na **Novo problema** formulário.\
   Ou\
   Se o projeto estiver associado a um formulário personalizado de ocorrência por meio da área Detalhes da fila , o formulário será exibido na **Novo problema** , nos campos padrão do Workfront .

   Para obter mais informações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clique em **Salvar novo problema.**

Os problemas podem ser atribuídos a vários usuários, funções de trabalho ou a uma equipe. Para obter mais informações sobre atribuição e gerenciamento de solicitações, consulte [Gerenciar solicitações de trabalho e de equipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Criar problemas em uma tarefa ou projeto em linha

>[!IMPORTANT]
>
>O proprietário do projeto deve ativar **Permitir que usuários adicionem problemas em linha** ao definir configurações de problemas para o projeto, antes de adicionar problemas em linha ao projeto ou às tarefas. Para obter informações sobre como definir configurações de problemas em um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Quando quiser adicionar vários problemas rapidamente, crie problemas para uma tarefa ou um projeto em linha, adicionando-os a uma lista de problemas.

>[!NOTE]
>
>Quando você adiciona problemas em linha, a Workfront não aplica o formulário Nova ocorrência aos novos problemas. Não é recomendável adicionar problemas em linha se você quiser que os usuários forneçam determinadas informações ao inserir problemas. Isso pode ter um impacto negativo no relatório de problemas e, posteriormente, na capacidade do usuário atribuído ao problema de ter todas as informações necessárias para resolver o problema.

Para criar problemas em linha:

1. Vá para um projeto em que deseja criar o problema.
1. (Opcional) Se quiser registrar o problema para uma tarefa, acesse o **Tarefas** e clique no nome de uma tarefa.
1. Clique no botão **Problemas** seção.
1. Clique em **Adicionar mais problemas**.

   Uma nova linha é criada na lista de problemas na seção Problemas .

   >[!TIP]
   >
   >Essa opção ficará esmaecida se a configuração Permitir que usuários adicionem problemas em linha estiver desmarcada na caixa Editar projeto . Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Comece digitando o nome do problema no campo Nome e continue adicionando mais informações sobre o problema em linha.

   >[!TIP]
   >
   >Os campos disponíveis para edição em linha são disponibilizados pela exibição aplicada à lista de problemas. Talvez não seja possível editar os seguintes tipos de campos em linha:
   >   
   >* Campos pertencentes a outro objeto
   >* Campos que você não tem acesso para editar
   >* Campos que são cálculos e são atualizados automaticamente pelo Workfront


1. Clique em Enter para concluir a edição em linha e adicione o problema ao projeto ou tarefa.

## Criar problemas inserindo uma nova solicitação {#create-issues-by-entering-a-new-request}

Você pode designar projetos para receptáculos para receber problemas. Esses tipos de projetos são chamados de Filas de solicitações no Workfront. Você pode acessar Filas de solicitações por meio da área Solicitações no Menu principal.

>[!TIP]
>
>Os termos &quot;emissão&quot; e &quot;solicitação&quot; são permutáveis no Workfront.

Para obter mais informações sobre como configurar projetos como Filas de solicitação para receber problemas, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Para obter informações sobre como enviar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
