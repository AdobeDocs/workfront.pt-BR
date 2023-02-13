---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar status do problema
description: Você pode atualizar o status de um problema para informar outras pessoas sobre onde ele está e como ele está progredindo.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# Atualizar status do problema

Você pode atualizar o status de um problema para informar outras pessoas sobre onde ele está e como ele está progredindo.

## Requisitos de acesso

<!--drafted for P&P;

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
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para o problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Status da emissão

A seguir estão os status padrão para problemas no Workfront:

* Novo(a)
* Em andamento
* Aguardando Retorno
* Em Espera
* Não Será Resolvido
* Reaberta
* Fechado
* Solucionado

O administrador do Adobe Workfront pode adicionar status personalizados para problemas da organização. Eles também podem disponibilizar status dependendo do tipo de problema.

Para obter mais informações sobre status personalizados e tipos de edição, consulte os seguintes artigos:

* [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Criar problemas](../../../manage-work/issues/manage-issues/create-issues.md)

Você pode atualizar manualmente os status de problemas ou permitir que o Workfront os atualize automaticamente quando determinadas ações ocorrerem.

## Atualizar manualmente o status do problema

Ao atualizar um status de problema, você também pode adicionar uma explicação sobre o novo status e alterar outras informações de problema, como a data de confirmação.

1. Vá para um problema atribuído para o qual deseja atualizar o status.
1. Clique no botão **Status** no cabeçalho da ocorrência e selecione um novo status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. Para fornecer uma indicação visual da conclusão da ocorrência, arraste ou clique duas vezes na bolha em **Porcentagem concluída** no cabeçalho do problema.

   Ou

   Clique dentro da bolha no cabeçalho da edição para inserir uma porcentagem.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Opcional) Siga qualquer um dos procedimentos a seguir para fornecer informações adicionais sobre a atualização, em seguida, clique em **Atualizar** ou, se o problema tiver um status que seja igual a Concluído, clique em **Feito em:**

   * Para adicionar uma observação sobre a atualização, acesse o **Atualizações** e clique em **Iniciar uma nova atualização** e digite a nota.

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Para notificar determinados usuários sobre a atualização, digite os nomes deles na **Notificar** que é exibida quando você digita uma nota sobre a atualização. Para obter mais informações, consulte [Marcar outras pessoas em atualizações](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Para atualizar a condição do problema, clique em **Condição**, em seguida, selecione a condição que reflete melhor a condição atual do problema. Selecione dentre as seguintes opções:

      * Indo Bem
      * Algumas Dificuldades
      * Com Problemas
   * Para atualizar a Data de confirmação do problema, expanda a **Data de confirmação** calendário suspenso e selecione uma nova data.


## Atualizar automaticamente o status do problema

O Workfront atualiza automaticamente o status existente de um problema para um status diferente quando as ações listadas na tabela abaixo ocorrem.

>[!NOTE]
>
>Os status na tabela a seguir são status padrão do sistema. O administrador do Workfront ou um administrador de grupo pode renomear os status na instância do Workfront. Para obter informações sobre como criar e gerenciar status no Workfront, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Ação</td> 
   <td>Status original</td> 
   <td>Novo status</td> 
  </tr> 
  <tr> 
   <td>Atualizar o percentual de conclusão do problema para 100%</td> 
   <td>Novo ou Em Andamento</td> 
   <td>Fechado</td> 
  </tr> 
  <tr> 
   <td>Atualize a porcentagem de problema concluída de 100% para um número menor</td> 
   <td>Fechado </td> 
   <td>Em andamento</td> 
  </tr> 
  <tr> 
   <td>Atualizar o status de um objeto de resolução anexado ao problema</td> 
   <td>Vários status</td> 
   <td> <p>Vários status</p> <p>Para obter informações sobre como resolver objetos e como eles afetam o status de problemas, consulte a seção "Sincronizar o status do objeto resolvível com o do objeto solucionável" no artigo <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Clique no botão Iniciar problema para aceitar trabalhar em um problema atribuído a você</span> </td> 
   <td><span>Novo(a)</span> </td> 
   <td> <p>Qualquer status associado ao botão Iniciar Problema nas configurações da Equipe Inicial. </p> <p>Para obter informações sobre a substituição do botão Trabalho nele por um botão Iniciar problema, consulte <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substitua o botão Trabalho nele por um botão Iniciar</a></span><span>.</span> </p> <p>Dica: Clicar <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">o botão Desfazer</span> depois de clicar em Iniciar problema, o status é revertido para Novo. </p> </td> 
  </tr> 
 </tbody> 
</table>
