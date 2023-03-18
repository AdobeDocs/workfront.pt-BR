---
content-type: overview
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Visão geral da seção Atualizações
description: A seção Atualizações mostra até 200 das atualizações mais recentes feitas nos últimos 90 dias.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: f8bf374f-703d-416a-9f36-28a6708620bc
source-git-commit: 39647f235c2e131e0ddd5d3b72d2f073387e531e
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 6%

---

# Visão geral da seção Atualizações

<!--take "Beta" references out when we remove the beta-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the Updates section of an object. You can access the new design by enabling the commenting Beta. 
Currently, the Beta is available for <span class="preview">issues</span>. 
For more information about the new commenting  experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 

-->

A seção Atualizações de um objeto exibe os comentários que os usuários fazem sobre as atualizações de objeto ou sistema que rastreiam as alterações no objeto.

## Visão geral da seção Atualizações

<!--drafted for the commenting beta for issues: 
The information is organized differently in the Updates section, depending on which environment you access it from. 

###  Overview of the current Updates section 
-->

A seção Atualizações de um objeto exibe até 200 das atualizações mais recentes feitas nos últimos 90 dias.

<!--drafted for the commenting beta for issues: 
The current Updates section shows the following information:

************** AND REMOVE THE SENTENCE BELOW WHEN MAKING THIS LIVE:
-->

A seção Atualizações mostra as seguintes informações:

* Comentários feitos pelos usuários e respostas a esses comentários.
* Atualizações do sistema que são mensagens informativas criadas pelo Workfront para registrar determinados eventos em um objeto. Por exemplo, você pode capturar alterações em campos de status, nome ou personalizados com atualizações do sistema. Seu Workfront ou administrador de grupo pode ativar atualizações do sistema para seus objetos. Para obter mais informações, consulte [Configurar atualizações do sistema](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

A seção Atualizações é exibida para os seguintes objetos:

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

<!--drafted for the commenting beta for issues: 
###  Overview of the Updates section in the Beta commenting experience

The Updates section displays information in the following tabs in the Beta commenting experience: 

* **Updates**: Displays comments made by users and replies to those comments. 
* **System Activity**: Displays system updates which are informational messages that Workfront creates to record certain events on an objects. For example, you can capture changes in status, name, or custom fields with system updates. Your Workfront or group administrator can enable system updates for your ojects. For more information, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

Currenlty, you can make comments and reply to updates using the Beta commenting experience on the following objects:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Goals</li> 
     </ul> </td> 
   <td> 
    <ul> 
     <li><span class="preview">Issues</span></li> 
     </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>The commenting experience Beta is the default current experience for goals. You must have an additional license to access Workfront Goals. For information, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

## Atualizações que também aparecem em objetos de classificação superior

Como mostrado na tabela a seguir, as respostas feitas às atualizações em determinados objetos também aparecem na seção Atualizações de objetos classificados mais alto.

Por exemplo, quando você adiciona uma atualização a uma tarefa, a atualização aparece na seção Atualizações da tarefa e na seção Atualizações do projeto que contém a tarefa.

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

## Limitações da seção de atualizações

### Limitações para usuários e equipes

Não é possível fazer atualizações em equipes. A seção Atualizações para equipes é preenchida por atualizações inseridas nos seguintes objetos:

* Usuários
* Folhas de horas
* Histórias
* Iterações

Na seção Atualizações de usuários e equipes, é possível visualizar as atualizações inseridas nos últimos 90 dias.

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
