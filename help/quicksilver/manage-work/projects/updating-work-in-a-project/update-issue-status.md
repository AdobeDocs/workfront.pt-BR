---
product-area: projects
navigation-topic: update-work-in-a-project
title: Atualizar status do problema
description: Você pode atualizar o status de um problema para informar a outras pessoas onde o problema está e como ele está progredindo.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 2%

---

# Atualizar status do problema

<!--Audited: 01/2024-->

Você pode atualizar o status de um problema para informar a outras pessoas onde o problema está e como ele está progredindo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Nova licença: Contributor ou superior</p>
   Ou
   <p>Licença atual: Solicitação ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Status de problemas

A seguir estão os status padrão para problemas no Workfront:

* Novo(a)
* Em andamento
* Aguardando Retorno
* Em Espera
* Não Será Resolvido
* Reaberta
* Fechado
* Solucionado

O administrador do Adobe Workfront pode adicionar status personalizados para ocorrências em sua organização. Eles também podem disponibilizar os status dependendo do tipo de ocorrência.

Para obter mais informações sobre status personalizados e tipos de problemas, consulte os seguintes artigos:

* [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
* [Criar problemas](../../../manage-work/issues/manage-issues/create-issues.md)

Você pode atualizar manualmente os status dos problemas ou permitir que o Workfront os atualize automaticamente quando determinadas ações ocorrerem.

## Atualizar manualmente o status do problema

Você pode atualizar o status do problema nas seguintes áreas do Workfront:

* O cabeçalho do problema na página de tarefas.
* A caixa Editar problema, ao editar um problema.
* A seção Detalhes na página do problema.
* Em uma lista de problemas ou relatório, quando o campo Status está visível na visualização.
* No painel Resumo da ocorrência.

Para atualizar manualmente o status do problema no cabeçalho do problema:

1. Vá para um problema para o qual deseja atualizar o status.
1. Clique no campo **Status** no cabeçalho do problema e selecione um novo status.
1. Para fornecer uma indicação visual da conclusão do problema, arraste ou clique duas vezes na bolha em **Percentual concluído** no cabeçalho do problema

   Ou

   Clique dentro da bolha no cabeçalho do problema para inserir uma porcentagem.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Opcional) Siga qualquer um destes procedimentos para fornecer informações adicionais sobre a atualização:

   * Para adicionar uma observação sobre a atualização, vá para a seção **Atualizações**, clique em **Novo comentário** e digite uma observação.

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Para notificar determinados usuários sobre a atualização, digite seus nomes no campo **Marcar pessoas ou equipes**, que aparece quando você digita um comentário. Para obter mais informações, consulte [Marcar outros em atualizações](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Para atualizar a Data de confirmação do problema, clique em **Detalhes do problema** e edite o campo **Data de confirmação**. Para obter informações, consulte [Editar problemas](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  Somente os atribuídos da ocorrência podem atualizar a Data de confirmação.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## Atualizar automaticamente o status do problema

O Workfront atualiza automaticamente o status existente de um problema para um status diferente quando ocorrem as ações listadas na tabela abaixo.

>[!NOTE]
>
>Os status na tabela a seguir são os status padrão do sistema. O administrador do Workfront ou um administrador de grupo pode renomear os status na sua instância do Workfront. Para obter informações sobre como criar e gerenciar status no Workfront, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Ação</b></td> 
   <td><b>Status Original</b></td> 
   <td><b>Novo Status</b></td> 
  </tr> 
  <tr> 
   <td>Atualizar a porcentagem concluída do problema para 100%</td> 
   <td>Novo ou em andamento</td> 
   <td>Fechado</td> 
  </tr> 
  <tr> 
   <td>Atualizar o percentual de conclusão do problema de 100% para um número mais baixo</td> 
   <td>Fechado </td> 
   <td>Em andamento</td> 
  </tr> 
  <tr> 
   <td>Atualizar o status de um objeto de resolução anexado ao problema</td> 
   <td>Vários status</td> 
   <td> <p>Vários status</p> <p>Para obter informações sobre a resolução de objetos e como eles afetam o status de problemas, consulte a seção "Sincronizar o Status do Objeto Resolvível com o do Objeto de Resolução" no artigo <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral de Objetos Resolvíveis e Resolvíveis </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Clique no botão Iniciar Problema para aceitar trabalhar em um problema atribuído a você</span> </td> 
   <td><span>Novo</span> </td> 
   <td> <p>Qualquer status associado ao botão Iniciar problema nas configurações da Equipe da página inicial. </p> <p>Para obter informações sobre a substituição do botão Trabalhar na tarefa pelo botão Iniciar problema, consulte <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substituir o botão Trabalhar na tarefa por um botão Iniciar</a></span><span>.</span> </p> <p>Dica: Clicar em <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">o botão Desfazer</span> depois de clicar em Iniciar problema reverte o status para Novo. </p> </td> 
  </tr> 
 </tbody> 
</table>
