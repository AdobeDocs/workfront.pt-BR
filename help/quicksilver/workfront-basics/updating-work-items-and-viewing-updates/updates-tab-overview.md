---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visão geral da guia Atualizações
description: A guia Atualizações mostra até 200 das atualizações mais recentes feitas nos últimos 90 dias.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 19872953e847921c0fee6d383026641c05012ead
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 7%

---

# Visão geral da guia Atualizações

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only for a limited number of objects when you opt in to the new commenting experience Beta.</span> -->

<!-- for preview commenting beta: at the release of commenting beta: change the title to: Updates section overview - also update ALL articles from which this is linked-->

A guia Atualizações mostra até 200 das atualizações mais recentes feitas nos últimos 90 dias.

Você pode fazer comentários e responder a atualizações nos seguintes objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Documentos</li> 
     <li>Metas</li> 
     <li>Problemas</li> 
     <li>Iterações</li> 
     <li>Projetos</li> 
     <li>Programas</li> 
     <li>Portfólios</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Histórias</li> 
     <li>Tarefas</li> 
     <li>Modelos</li> 
     <li>Modelo de Tarefa</li> 
     <li>Folhas de horas</li> 
     <li>Usuários</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizações que também aparecem em objetos de classificação superior

Como mostrado na tabela a seguir, as respostas às atualizações em determinados objetos também aparecem na guia Atualizações de objetos classificados mais alto.

Por exemplo, quando você adiciona uma atualização a uma tarefa, a atualização aparece na guia Updates da tarefa e na guia Updates do projeto que contém a tarefa.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objeto no qual a atualização original foi adicionada</strong> </th> 
   <th> <p><strong>Objeto com classificação mais alta, onde a atualização original também é exibida</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Problema</td> 
   <td>Projeto</td> 
  </tr> 
  <tr> 
   <td>Tarefa</td> 
   <td>Projeto</td> 
  </tr> 
  <tr> 
   <td>Projeto</td> 
   <td>Programa, Portfolio</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Documento </td> 
   <td>Objeto onde o documento está anexado, Projeto </td> 
  </tr> 
  <tr> 
   <td>Programa</td> 
   <td>Portfólio</td> 
  </tr> 
  <tr> 
   <td>Usuário</td> 
   <td>Equipe</td> 
  </tr> 
  <tr> 
   <td>Planilha de horas</td> 
   <td>Usuário, Equipe</td> 
  </tr> 
  <tr> 
   <td>Modelo de Tarefa</td> 
   <td>Modelo</td> 
  </tr> 
  <tr> 
   <td>História</td> 
   <td>Iteração, Equipe</td> 
  </tr> 
  <tr> 
   <td>Iteração</td> 
   <td>Equipe</td> 
  </tr>

<tr> 
   <td>Metas</td> 
   <td>Resultado, Atividade</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>As respostas adicionadas às atualizações do sistema não são acumuladas no objeto pai. Somente respostas diretas em um objeto filho e respostas adicionadas a atualizações existentes são acumuladas em objetos pai.
>
>Para obter informações sobre a hierarquia de objetos no Adobe Workfront, consulte [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

<!-- drafted for the new commenting experience for issues in beta: Add this paragraph to the note above: 
><span class="preview"> It is not possible to reply to system updates in the new commenting experience Beta. For more information, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).</span> -->

## Limitações da guia Atualizações

### Limitações para usuários e equipes

Não é possível fazer atualizações em equipes. A guia Atualizações para equipes é preenchida por atualizações inseridas nos seguintes objetos:

* Usuários
* Folhas de horas
* Histórias
* Iterações

Na guia Atualizações de usuários e equipes, é possível visualizar as atualizações inseridas nos últimos 90 dias.

Se quiser ver todas as atualizações feitas em um usuário ou equipe, além do limite de 90 dias, crie um relatório para observações. O relatório não deve ter um filtro de tempo que exiba todas as atualizações feitas para usuários ou equipes. Para obter mais informações, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Limitações ao inserir comentários em nome de outro usuário

Os administradores do Adobe Workfront e administradores de grupo podem fazer logon como outros usuários e executar ações no Workfront, como inserir comentários. (Para obter mais informações, consulte [Fazer logon como outro usuário](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).) Quaisquer comentários feitos em nome de outro usuário são indicados no comentário.

Um administrador de grupo pode comentar em nome de outra pessoa, mas não pode excluir esse comentário. Somente um administrador do Adobe Workfront pode excluir um comentário feito em nome de outro usuário.

## Exibir atualizações do sistema em itens de trabalho com o relatório Entrada de Lançamento

O relatório de Lançamento exibe atualizações do sistema da área Atualizações de projetos, tarefas e problemas.

O relatório permite visualizar:

* Quantas alterações de status ocorreram
* Quando uma tarefa ou problema foi excluído
* Como os valores em campos personalizados importantes foram alterados durante um projeto
* As datas importantes mudaram ao longo de um projeto
* Se a prioridade tiver mudado no decurso de um projeto
* Se o proprietário de um projeto tiver sido alterado

Para obter mais informações, consulte [Relatório sobre a área Atualizações](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).
