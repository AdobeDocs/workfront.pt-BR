---
title: Acesse a lista de status de problemas do sistema
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Você pode usar o status de um problema para mostrar aos usuários no sistema em que estágio de desenvolvimento um problema está em um determinado momento.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Acesse a lista de status de problemas do sistema

Você pode usar o status de um problema para mostrar aos usuários no sistema em que estágio de desenvolvimento um problema está em um determinado momento.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Acessar status de problema

Você pode acessar e modificar status de problemas no nível do sistema. Você pode editar algumas informações sobre os status padrão do sistema ou criar novos status personalizados. Para obter mais informações sobre como criar status personalizados ou editar status do sistema, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Para acessar os status de problemas no nível do sistema:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Preferências do projeto** > **Status**.

1. Clique no botão **Problemas** para ver os status do problema disponíveis no Workfront.

   ![](assets/issue-status.png)

## Status de problemas do sistema

O Workfront vem com 10 status de edição original. Os primeiros 4 da tabela abaixo são obrigatórios, o que significa que você pode desbloquear, renomear e reorganizá-los, mas não pode ocultá-los ou excluí-los.

Você pode adicionar status de problema personalizado para atender às necessidades em sua organização. Para obter mais informações, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Para usuários, a alteração do status de um problema geralmente é um processo manual. No entanto, há situações, descritas na lista a seguir, em que o status de um problema muda automaticamente, dependendo de outros fatores que estão acontecendo no sistema.

Os seguintes status de problema são fornecidos com sua instância do Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status de problema do sistema</th> 
   <th>Como você pode usar o status</th> 
   <th>O que acontece no status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Novo (status obrigatório)</td> 
   <td>Esse é o status padrão para cada problema recém-criado.</td> 
   <td>Se o problema estiver em um projeto com status Atual, o problema será exibido na guia Solicitações de trabalho dos usuários atribuídos ao problema. Agora os usuários podem começar a trabalhar no problema.</td> 
  </tr> 
  <tr> 
   <td>Em Andamento (status obrigatório)</td> 
   <td> <p>Você pode colocar um problema nesse status para indicar que o trabalho sobre esse problema foi iniciado.</p> <p>Se a resolução do problema estiver conectada a outro objeto (uma tarefa, projeto ou outro problema), o status do problema será alterado para Em andamento automaticamente, quando você alterar o status do objeto de resolução para Em andamento. </p> <p>Para obter mais informações sobre como resolver objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</p> </td> 
   <td> <p>Se o problema estiver em um projeto com o status Atual, o problema será exibido na guia Trabalhar em dos usuários atribuídos ao problema.</p> <p>Quando um problema está em andamento, o problema mostra um valor para a Data de início real.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Fechado (status obrigatório)</td> 
   <td> <p>Você pode marcar um problema manualmente como Fechado quando o trabalho nele for concluído. </p> <p>Se a resolução do problema estiver conectada a outro objeto (uma tarefa, projeto ou outro problema), o status do problema será alterado para Fechado automaticamente, quando você alterar o status do objeto que resolve para Fechado.</p> <p>Para obter mais informações sobre como resolver objetos, consulte <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Visão Geral da Solução e Objetos Resolvíveis </a>.</p> </td> 
   <td> <p>Quando um problema é Fechado, o problema é removido da lista Trabalhar no destinatário. Nesse caso, o problema mostra um valor para a Data de conclusão real. </p> <p>Quando todas as tarefas são concluídas e os problemas são fechados em um projeto, o projeto pode ser concluído.</p> </td> 
  </tr> 
  <tr> 
   <td>Em Retenção (status obrigatório)</td> 
   <td> <p>Você pode marcar um problema manualmente como Em Retenção, para indicar que houve um atraso na conclusão do problema. </p> </td> 
   <td> <p>Se o problema estiver em um projeto com o status Atual, o problema será exibido na guia Trabalhar em dos usuários atribuídos ao problema. </p> <p>Quando todas as tarefas são concluídas em um projeto, mas há pelo menos um problema em espera no projeto, o projeto não pode ser concluído. </p> </td> 
  </tr> 
  <tr> 
   <td>Reaberto (Equações com Em Andamento)</td> 
   <td> <p>Você pode colocar um problema nesse status para indicar que o trabalho sobre esse problema não estava totalmente concluído quando o problema foi fechado anteriormente e que era necessário reabri-lo para concluir o trabalho.</p> </td> 
   <td> <p>Se o problema estiver em um projeto com status Atual, o problema será exibido na guia Solicitações de trabalho dos usuários atribuídos ao problema. Agora os usuários podem começar a trabalhar no problema.</p> <p>Esse status é importante nos relatórios, para diferenciar entre problemas que estão abertos pela primeira vez (geralmente no status Novo) e problemas que são abertos depois de terem sido fechados antes (normalmente no status Reaberto). </p> </td> 
  </tr> 
  <tr> 
   <td>Aguardando Feedback (Igua com Em Espera)</td> 
   <td>Você pode colocar um problema nesse status para indicar que está aguardando feedback (normalmente do Contato principal) antes de continuar trabalhando sobre o problema. </td> 
   <td> <p>Se o problema estiver em um projeto com o status Atual, o problema será exibido na guia Trabalhar em dos usuários atribuídos ao problema.</p> <p>Se um problema estiver Aguardando feedback, um projeto não poderá ser concluído.</p> <p>Esse status é importante nos relatórios, para diferenciar entre problemas que estão abertos no momento, mas que estão sendo trabalhados (geralmente no status Em andamento) e problemas que estão abertos no momento, mas não estão sendo trabalhados, pois é necessário mais feedback para concluí-los (geralmente no status Aguardando feedback).</p> </td> 
  </tr> 
  <tr> 
   <td>Não é Possível Duplicar (Equates com Fechado)</td> 
   <td>Você pode colocar um problema nesse status para indicar que está fechando o problema, mas não pode ver o problema que acionou a abertura do problema. O problema pode ainda existir, mas não pode ser replicado em um determinado momento. </td> 
   <td> <p>Esse status é importante nos relatórios, para diferenciar entre problemas que são concluídos e cujo problema foi resolvido (geralmente no status Closed ) e problemas cujo problema não é visível em um determinado momento (geralmente no status Cannot Duplicate ).</p> <p>Quando um problema é marcado como Não é possível duplicar, o problema é removido da lista Trabalhar no destinatário. Nesse caso, o problema mostra um valor para a Data de conclusão real.</p> <p>Se todas as tarefas em um projeto forem concluídas e alguns problemas estiverem em um status Não é possível duplicar, o projeto poderá ser concluído.</p> </td> 
  </tr> 
  <tr> 
   <td>Resolvido (Equates com Fechado)</td> 
   <td>Você pode colocar um problema nesse status para indicar que está fechando o problema e que o problema que o criou foi realmente resolvido.</td> 
   <td> <p>Esse status é importante nos relatórios, para diferenciar entre problemas que são fechados com ou sem uma resolução (geralmente no status Fechado) e problemas que são fechados com uma resolução real (geralmente no status de Resolvido).</p> <p>Quando um problema é marcado como Resolvido, o problema é removido da lista Trabalhar no destinatário. Nesse caso, o problema mostra um valor para a Data de conclusão real.</p> <p>Se todas as tarefas em um projeto forem concluídas e pelo menos um problema estiver em um status Resolvido, o projeto poderá ser concluído. </p> </td> 
  </tr> 
  <tr> 
   <td>Verified Complete (Equações com Fechado)</td> 
   <td>Você pode colocar um problema nesse status para indicar que está fechando o problema e que verificou que o problema que gerou o problema foi resolvido.</td> 
   <td> <p>Quando um problema é marcado como Verified Complete (Verificação concluída), o problema é removido da lista Working On do destinatário. Nesse caso, o problema mostra um valor para a Data de conclusão real.</p> <p>Se todas as tarefas em um projeto forem concluídas e alguns problemas estiverem em um status Verificado concluído, o projeto poderá ser concluído.</p> </td> 
  </tr> 
  <tr> 
   <td>Não Resolverá (Equata com Fechado)</td> 
   <td>Você pode colocar um problema nesse status para indicar que está fechando o problema, mas o problema que o gerou não pode ser resolvido.</td> 
   <td> <p>Esse status é importante nos relatórios, para diferenciar entre problemas que são fechados com ou sem uma resolução (geralmente no status Fechado) e problemas que são fechados sem uma resolução real (geralmente no status de Não Resolver).</p> <p>Quando um problema é marcado como Não Resolver, o problema é removido da lista Trabalhar no destinatário. Nesse caso, o problema mostra um valor para a Data de conclusão real.</p> <p>Se todas as tarefas em um projeto forem concluídas e pelo menos um problema estiver em um status Não Resolver , o projeto poderá ser concluído.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalização de status de problemas

Um administrador do Workfront pode adicionar status de problemas de nível de sistema e de grupo ao Workfront e alterar a ordem em que os usuários os veem. Para obter mais informações, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Um administrador de grupo pode adicionar um status personalizado específico a um grupo. Para obter mais informações, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
