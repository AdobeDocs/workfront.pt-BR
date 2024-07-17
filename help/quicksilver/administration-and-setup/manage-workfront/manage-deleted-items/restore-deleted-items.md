---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurar itens excluídos
description: Se você for um administrador do Workfront, poderá restaurar projetos, tarefas, problemas, documentos e modelos no Adobe Workfront se eles tiverem sido excluídos nos últimos 30 dias. Após 30 dias, esses itens são excluídos permanentemente e não podem ser restaurados. Quando você restaura um objeto, todos os seus objetos e campos filhos também são restaurados. Por exemplo, se você restaurar um projeto, todas as tarefas, problemas, documentos, horas, notas, atribuições e dados personalizados no projeto também serão restaurados.itens
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '1082'
ht-degree: 1%

---

# Restaurar itens excluídos

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Se você for um administrador do Workfront, poderá restaurar projetos, tarefas, problemas, documentos e modelos no Adobe Workfront se eles tiverem sido excluídos nos últimos 30 dias. Após 30 dias, esses itens são excluídos permanentemente e não podem ser restaurados.

Quando você restaura um objeto, todos os seus objetos e campos filhos também são restaurados. Por exemplo, se você restaurar um projeto, todas as tarefas, problemas, documentos, horas, notas, atribuições e dados personalizados no projeto também serão restaurados.

Um administrador de grupo também pode restaurar esses objetos para um grupo que gerencia.

>[!IMPORTANT]
>
>* Se você excluir um relatório, painel, usuário, grupo, equipe ou iteração, ele não poderá ser restaurado.
>* Em um grupo, quando alguém que não seja o administrador de grupo faz upload de um documento diretamente na área Documentos de um objeto, somente um administrador do Workfront pode restaurar o documento.
>
>* Se você mover uma tarefa ou um problema e optar por não mover também os documentos anexados à tarefa ou ao problema, os documentos serão excluídos e colocados na Lixeira por 30 dias. Um administrador pode restaurá-los e eles serão reanexados à tarefa ou problema movido. Se a tarefa ou o problema tiver sido excluído desde que foi movido, os documentos serão restaurados na área Documentos da página do usuário do administrador que os restaurará.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
   ou
   <p>Atual: Plano</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber que tipo de plano ou licença você tem, contate o administrador do Workfront.

+++

## Informações recuperadas quando você restaura um projeto, tarefa ou problema

Quando você restaura um projeto, tarefa ou problema, as seguintes informações associadas são recuperadas junto com ele:

* Comentários e respostas na área Atualizações
* Aprovações
* Atribuições
* Formulários personalizados
* Configuração da fila
* Casos de negócios, incluindo cartões de pontuação, metas e riscos
* Equipes do projeto
* Datas
* Problemas
* Tarefas
* Subtarefas
* Status
* Informações Financeiras:

   * Registros de faturamento
   * Preços
   * Despesas

* Informações da linha do tempo:

   * Predecessoras
   * Restrições de tarefa
   * Tipo de duração

* Linhas de base

  As linhas de base de tarefas são recuperadas quando você restaura o projeto ou tarefa pai, mas não quando você restaura tarefas excluídas individualmente.

* Horas (e IDs de horas)

  Se as horas são restauradas para o item excluído depende das configurações que você escolheu ao configurar as preferências para folhas de horas e horas. Para obter mais informações, consulte [Configurar efeito em horas quando um objeto for excluído e restaurado](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* O URL do item

  Quando restaurado, o URL do item permanece o mesmo. Se as pessoas tiverem criado marcadores de navegador para o item, eles permanecerão válidos.

* Acesso e permissões

  Os usuários que tinham acesso ao item antes de ele ser excluído obtêm acesso novamente após sua restauração.

* Documentos (incluindo documentos comprovados)

  Considere o seguinte ao restaurar documentos e versões de documentos:

   * Os documentos que foram excluídos individualmente podem ser restaurados individualmente.

     Os documentos que foram excluídos junto com o projeto, tarefa ou problema pai são recuperados quando você restaura o pai, mas não é possível restaurá-los individualmente.

   * Todas as versões de um documento ou de uma prova de documento são restauradas quando o documento é restaurado.\
     As versões individuais de um documento ou de uma prova de documento que foram excluídas individualmente não podem ser recuperadas.

## Informações que não são recuperadas quando você restaura um projeto, tarefa ou problema

Quando você restaura um projeto, tarefa ou problema, as seguintes informações associadas não são recuperadas junto com elas:

* Curtidas
* Endossos
* Endereço de e-mail de entrada em uma fila de solicitações
* Favoritos

  Um projeto, tarefa ou problema que você adicionou ao menu Favoritos antes de excluí-lo não reaparecerá no menu Favoritos depois que você restaurá-lo.

* Resolvendo objetos

  Um objeto de resolução é um problema convertido configurado com a opção **Manter o problema original e vincular sua resolução a este** &lt;**projeto** ou **tarefa)**>. Se você excluir o projeto ou a tarefa pai, o problema não será mais identificado como um objeto de resolução porque não há mais um link que o conecta ao projeto ou à tarefa. Se você restaurar o pai, o link não será restaurado.

  Para obter mais informações sobre como um administrador ou administrador de grupo do Workfront configura problemas para corresponder ao objeto de resolução quando convertidos, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) e [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  Para obter mais informações sobre a conversão de problemas, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Restaurar itens

{{step-1-to-setup}}

1. Clique em **Lixeira** > **Excluída Recentemente**.
1. Clique na guia **Projetos**, **Tarefas**, **Problemas**, **Modelos** ou **Documentos**, dependendo do tipo de item que você deseja restaurar.

   Por padrão, os itens são classificados pela coluna **Data de Exclusão**.

1. Selecione até 10 itens que deseja restaurar.

   Se você excluir uma tarefa filho, ela será exibida na lista.

   Se você excluir uma tarefa pai, somente ela será exibida na lista. Mas todas as tarefas filho são restauradas quando você restaura uma tarefa pai.

1. Clique em **Restaurar** para restaurar os itens selecionados para seu local original.
1. (Opcional) Para visualizar rapidamente o item restaurado, siga as etapas em [Exibir item restaurado](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Para obter mais informações sobre o que acontece após a restauração de um item, consulte a seção [O que acontece após a restauração de itens](#what-happens-after-you-restore-items) neste artigo.

## O que acontece depois que você restaura itens {#what-happens-after-you-restore-items}

* Quando você restaura tarefas e subtarefas, elas são exibidas na ordem em que estavam antes de serem excluídas.

  No entanto, se a ordem de outras tarefas for alterada enquanto a tarefa for excluída, a tarefa poderá ser restaurada na parte inferior da lista de tarefas ou subtarefas.

* Após restaurar um item:

   * Uma mensagem é exibida para informar se você foi bem-sucedido.

     Você também receberá uma notificação por email. Se você restaurou vários itens, o email os lista.

   * Um comentário é exibido na área Atualizações do projeto, tarefa ou problema e na área do objeto principal.

     Isso não acontece quando você restaura um documento ou um modelo.

## Provas restauradas

Quando alguém restaura um documento que tem uma prova, a página Atividades de prova da prova pode exibir o nome do primeiro administrador ativo do Workfront listado para a instância da sua organização (em ordem de ID do perfil) em vez da pessoa real que restaurou a prova.
