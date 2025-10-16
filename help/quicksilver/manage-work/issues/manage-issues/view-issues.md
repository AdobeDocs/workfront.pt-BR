---
product-area: projects
navigation-topic: manage-issues
title: Exibir problemas
description: Você pode visualizar os problemas associados a um projeto, tarefa ou iteração.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: dc4b6dc284c59281206a457395765e634067ba91
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Exibir problemas

<!--Audited: 10/2025-->

Você pode visualizar os problemas associados a um projeto, tarefa ou iteração.

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
   <ul><li><p>Colaborador ou superior</p></li> <li><p>Licença leve ou superior para visualizar os problemas na seção Problemas de um projeto.</p></li>

Ou

<ul><li><p>Solicitação ou superior</p></li> <li><p>Licença de revisão ou superior para exibir problemas na seção Problemas de um projeto.</p></li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir acesso a ocorrências</p> <p>Acesso de visualização ou superior a projetos e tarefas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o problema</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> <p>Review or higher license to view issues in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## Exibir problemas com base no Status

Para exibir problemas em um projeto, tarefa ou iteração:

1. Abra um projeto, tarefa ou iteração que contenha problemas, em seguida, clique em **Problemas** no painel esquerdo.

1. Para exibir todos os problemas, abertos ou fechados, clique em qualquer um dos filtros listados abaixo no menu suspenso **Filtro**.

>[!TIP]
>
>A lista de filtros varia dependendo do que o administrador de sistema ou de grupo selecionou para exibição nela.

* **Abrir:** Exibe os problemas que estão abertos.

  Isso inclui aqueles associados a um Objeto de resolução e aqueles em um status Fechado - Pendente de aprovação.

  Para obter informações sobre Objetos de Resolução, consulte [Visão Geral de Objetos de Resolução e Resolução](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Concluído:** Exibe todos os problemas que têm uma Data de Término Efetivo.
* **Todos** Exibe todos os problemas.

## Compreender informações sobre problemas

É possível exibir informações sobre um problema ao acessá-lo.

Para acessar uma ocorrência e exibir informações sobre ela:

1. Abra um projeto, tarefa ou iteração que contenha problemas, em seguida, clique em **Problemas** no painel esquerdo.
1. No menu suspenso **Filtro**, selecione o filtro para exibir os problemas que você está tentando exibir.

   Selecione entre as seguintes opções:

   * Abrir
   * Concluídos
   * Todas

1. Clique no nome de um problema.

   Quando você tem permissões de gerenciamento para o problema, pode editar qualquer campo editável no problema e adicionar aprovações, horas ou documentos ao problema.

1. No painel esquerdo, clique em qualquer uma das opções a seguir para obter mais informações sobre o problema:

* **Atualizações**: você pode executar as seguintes ações:

   * Comente sobre o problema ou responda a um comentário existente.
   * Registrar tempo.
   * Alterar o status da ocorrência.

     Para obter mais informações sobre como atualizar o trabalho no Workfront, consulte [Atualizar trabalho](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Documentos**: anexe documentos ao problema. Para obter mais informações sobre como adicionar documentos ao Workfront, consulte [Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Detalhes do Problema**: expanda este link para exibir as áreas **Visão Geral** e **Forms Personalizado**.

  Se você tiver permissões de gerenciamento para o problema e direitos de edição no formulário personalizado, poderá editar algumas das informações aqui.

  Exiba ou edite os seguintes campos na área **Visão geral**:

   * **Nome**
   * **Caminho**: o caminho pelo qual o problema foi registrado no projeto.

     Se um problema foi enviado como uma solicitação em uma fila de solicitações, os nomes do projeto, do Grupo de tópicos e do Tópico da fila são listados aqui. Este campo não pode ser editado.

     Para obter mais informações sobre o envio de solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Descrição**
   * **URL**: qualquer endereço Web relacionado ao problema.
   * **Prioridade**: um sinalizador visual que permite priorizar problemas.
   * **Gravidade**: um sinalizador visual que indica a gravidade do problema descrito no problema.
   * **Contato Primário**: o contato Primário padrão é o usuário que criou o problema. Este campo pode ser editado.
   * **Horas planejadas**: exibe o tempo que leva para alguém concluir o problema. O padrão é 8 horas. Este campo pode ser editado.
   * **Horas efetivas**: exibe o tempo que levou para concluir a ocorrência. Esta é a hora real em que alguém registra o problema.
   * **Data de Início Planejada**: a data em que o problema está planejado para começar. O padrão é a data e a hora em que a ocorrência foi criada.
   * **Data de Início Real**: a data e a hora em que o status do problema foi alterado para Em Andamento.
   * **Data de conclusão planejada**: a data em que o problema está planejado para ser concluído.
   * **Data de conclusão real**: a data quando o problema é realmente concluído. Este campo é preenchido automaticamente quando o status do problema é alterado para Closed ou Resolved, ou pode ser editado manualmente.
   * **Custo Real**: o custo baseado nas Horas Reais registradas na questão. Este campo não é editável. O Custo Efetivo de uma ocorrência é calculado com base na seguinte fórmula, em que a Taxa de Custo do Usuário é a taxa de custo associada ao usuário que registra o tempo da ocorrência:

     Custo Real do Problema = Horas Registradas * Taxa de Custo do Usuário

   * **Informado por**: este é o usuário que criou o problema. Este campo não é editável.
   * **Última Atualização por**: este é o usuário que atualizou qualquer campo sobre o problema por último. Este campo não é editável.

     Na área **Forms personalizado**, exiba um ou vários formulários personalizados para associar ao problema.

* **Horas**: mostra uma lista de entradas de horas na ocorrência.
* **Aprovações:** mostra os caminhos de aprovação associados à questão.

  Para obter mais informações sobre como associar aprovações a um problema, consulte a seção [Associando um processo de aprovação a um item de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) em [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Exibir quais projetos e tarefas têm problemas

Você pode adicionar ícones no modo de exibição de um relatório ou lista de projetos ou tarefas para mostrar se eles têm problemas anexados.

Adicionar ícones à exibição de um relatório ou lista é semelhante para projetos e tarefas.

Para adicionar ícones que mostram se um projeto tem problemas em um relatório de projeto:

{{step1-click-main-menu}}

1. Clique em **Relatórios** > **Novo Relatório** > **Relatório de Projeto**.
1. No campo **Mostrar nesta coluna**, comece digitando **Ícones de Status** e selecione-os quando ele aparecer na lista.

1. Clique em **Salvar + Fechar**.

   Os ícones de problema são exibidos nos projetos que têm problemas na coluna **Ícones de Status**.

   ![Lista de projetos com ícone de problema](assets/project-list-with-issue-icon-350x132.png)
