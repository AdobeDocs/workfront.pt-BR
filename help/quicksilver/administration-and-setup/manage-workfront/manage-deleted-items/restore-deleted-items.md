---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Restaurar itens excluídos
description: Se você for um administrador do Workfront, poderá restaurar projetos, tarefas, problemas, documentos e modelos no Adobe Workfront se eles tiverem sido excluídos nos últimos 30 dias. Após 30 dias, esses itens são excluídos permanentemente e não podem ser restaurados. Quando um objeto é restaurado, todos os objetos e campos filhos também são restaurados. Por exemplo, se você restaurar um projeto, todas as tarefas, problemas, documentos, horas, notas, atribuições e dados personalizados no projeto também serão restaurados.items
feature: System Setup and Administration
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 1fb283df7090173d8f4dd36b9474ced10c8d30d1
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 1%

---

# Restaurar itens excluídos

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Se você for um administrador do Workfront, poderá restaurar projetos, tarefas, problemas, documentos e modelos no Adobe Workfront se eles tiverem sido excluídos nos últimos 30 dias. Após 30 dias, esses itens são excluídos permanentemente e não podem ser restaurados.

Quando um objeto é restaurado, todos os objetos e campos filhos também são restaurados. Por exemplo, se você restaurar um projeto, todas as tarefas, problemas, documentos, horas, notas, atribuições e dados personalizados no projeto também serão restaurados.

Um administrador de grupo também pode restaurar esses objetos para um grupo que ele gerencia.

>[!IMPORTANT]
>
>* Se você excluir um relatório, painel, usuário, grupo, equipe ou iteração, ele não poderá ser restaurado.
>* Em um grupo, quando alguém diferente do administrador de grupo faz o upload de um documento diretamente na área Documentos de um objeto, somente um administrador do Workfront pode restaurar o documento.
>
>* Se você mover uma tarefa ou um problema e optar por não mover também os documentos anexados à tarefa ou ao problema, os documentos serão excluídos e colocados na Lixeira por 30 dias. Um administrador pode restaurá-los e eles serão reconectados à tarefa ou problema movido. Se a tarefa ou o problema tiver sido excluído desde que foi movido, os documentos serão restaurados na área Documents da página do usuário do administrador que os restaura.


## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano ou tipo de licença você possui, entre em contato com o administrador da Workfront.

## Informações que são recuperadas quando você restaura um projeto, uma tarefa ou um problema

Quando você restaura um projeto, tarefa ou problema, as seguintes informações associadas são recuperadas junto com ele:

* Comentários e respostas na área Atualizações
* Aprovações
* Atribuições
* Formulários personalizados
* Configuração da fila
* Casos de negócios, incluindo scorecards, metas e riscos
* Equipes de projeto
* Datas
* Problemas
* Tarefas
* Subtarefas
* Status
* Informações financeiras:

   * Registros de cobrança
   * Taxas de faturação
   * Despesas

* Informações da linha do tempo:

   * Predecessoras
   * Restrições de tarefa
   * Tipo de duração

* Linhas de base

   As linhas de base de tarefas são recuperadas quando você restaura o projeto ou a tarefa pai, mas não quando você restaura tarefas excluídas individualmente.

* Horas (e IDs de hora)

   Se as horas são restauradas para o item excluído depende das configurações que você escolheu ao definir preferências para folhas de horas e horas. Para obter mais informações, consulte [Configurar o efeito em horas quando um objeto é excluído e restaurado](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* O URL do item

   Quando restaurado, o URL do item permanece o mesmo. Se as pessoas criaram marcadores de navegador para o item, eles permanecem válidos.

* Acesso e permissões

   Os usuários que tiveram acesso ao item antes de ele ser excluído recuperam o acesso depois que ele é restaurado.

* Documentos (incluindo documentos comprovados)

   Considere o seguinte ao restaurar documentos e versões do documento:

   * Os documentos que foram excluídos individualmente podem ser restaurados individualmente.

      Os documentos que foram excluídos junto com o projeto, a tarefa ou o problema pai são recuperados quando você restaurar o pai, mas não pode restaurá-los individualmente.

   * Todas as versões de um documento ou uma prova de documento são restauradas quando o documento é restaurado.\
      As versões individuais de um documento ou prova de documento que foram excluídos individualmente não podem ser recuperadas.

## Informações que não são recuperadas quando você restaura um projeto, uma tarefa ou um problema

Quando você restaura um projeto, tarefa ou problema, as seguintes informações associadas não são recuperadas junto com ele:

* Curtidas
* Endossos
* Inserir endereço de email em uma fila de solicitações
* Favoritos

   Um projeto, tarefa ou problema que você adicionou ao menu Favoritos antes de excluí-lo não reaparece no menu Favoritos após restaurá-lo.

* Solução de objetos

   Um objeto de resolução é um problema convertido configurado com a opção **Mantenha o problema original e vincule sua resolução a esse** &lt;**projeto** ou **task)**>. Se você excluir o projeto ou a tarefa pai, o problema não será mais identificado como um objeto de resolução porque não há mais um link conectando-o ao projeto ou à tarefa. Se você restaurar o pai, o link não será restaurado.

   Para obter mais informações sobre como um administrador do Workfront ou um administrador de grupo configura os problemas para corresponder ao objeto de resolução quando convertido, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) e [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   Para obter mais informações sobre conversão de problemas, consulte, [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Restaurar itens

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Lixeira** > **Recentemente Excluído**.
1. Clique no botão **Projetos**, **Tarefas**, **Problemas** ou **Documentos** , dependendo do tipo de item que deseja restaurar.

   Os itens são classificados pela variável **Data de exclusão** por padrão.

1. Selecione até 10 itens que você deseja restaurar.

   Se você excluir uma tarefa filho, ela será exibida na lista.

   Se você excluir uma tarefa pai, somente a tarefa pai será exibida na lista. Mas todas as tarefas filho são restauradas quando você restaura uma tarefa pai.

1. Clique em **Restaurar** para restaurar os itens selecionados para o local original.
1. (Opcional) Para visualizar rapidamente o item restaurado, siga as etapas em [Exibir item restaurado](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Para obter mais informações sobre o que acontece depois que você restaura um item, consulte [O que acontece depois que você restaurar os itens](#what-happens-after-you-restore-items) neste artigo.

## O que acontece depois que você restaurar os itens {#what-happens-after-you-restore-items}

* Quando você restaurar tarefas e subtarefas, elas aparecerão na ordem em que tinham antes de serem excluídas.

   No entanto, se a ordem de outras tarefas for alterada enquanto a tarefa for excluída, a tarefa poderá ser restaurada para a parte inferior da lista de tarefas ou subtarefas.

* Depois de restaurar um item:

   * Uma mensagem é exibida para informar se você foi bem-sucedido.

      Você também recebe uma notificação por email. Se você restaurou vários itens, o email os lista.

   * Um comentário é exibido na área Atualizações do projeto, tarefa ou problema e na do objeto pai.

      Isso não acontece quando você restaura um documento.

## Provas restauradas

No momento, quando alguém restaura um documento que tem uma prova, a página Atividades de Verificação Linguística da prova pode exibir o nome do primeiro administrador ativo do Workfront listado para a instância da organização (na ordem da ID do perfil) em vez da pessoa real que restaurou a prova.
