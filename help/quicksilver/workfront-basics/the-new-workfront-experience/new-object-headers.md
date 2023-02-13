---
content-type: overview
navigation-topic: the-new-workfront-experience
title: Visão geral dos cabeçalhos de objeto
description: Você pode exibir informações de relance sobre objetos em [!DNL Adobe Workfront] ao revisar o cabeçalho. As informações em um cabeçalho podem incluir o proprietário do objeto, o status ou a porcentagem concluída.
feature: Get Started with Workfront
exl-id: 76e21df0-9272-4bfb-8a97-c16ae5f4b5dc
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '3646'
ht-degree: 0%

---

# Visão geral dos cabeçalhos de objeto

Você pode exibir informações de relance sobre objetos em [!DNL Adobe Workfront] ao revisar o cabeçalho.

Além do nome do objeto, o cabeçalho pode incluir o proprietário do objeto, o status ou a porcentagem concluída.

[!DNL Workfront] dá prioridade ao nome do objeto, alocando o maior espaço possível nele no cabeçalho. Quando um nome de objeto é muito longo, ele é truncado. Para exibir o nome completo de um objeto, é possível passar o mouse sobre ele.

## Acessar o cabeçalho de um objeto

Acessar o cabeçalho de um objeto em [!DNL Workfront] é idêntica para todos os objetos que a possuem.

Por exemplo, para acessar o cabeçalho de um projeto:

1. Vá para um projeto.\
   O cabeçalho é exibido na parte superior da página e contém o nome do projeto.

   ![](assets/project-header-350x18.png)

## [!UICONTROL Início] visão geral do cabeçalho

Os seguintes cabeçalhos estão disponíveis em Início:

* Tarefa: Para obter mais informações sobre como usar esse cabeçalho, consulte a [Visão geral do cabeçalho da tarefa](#task-header-overview) neste artigo.
* Problema: Para obter mais informações sobre como usar esse cabeçalho, consulte a [Visão geral do cabeçalho da ocorrência](#issue-header-overview) neste artigo.

## Cabeçalhos personalizáveis

Seu [!DNL Workfront]  O ou o administrador de grupo pode personalizar o cabeçalho de projetos, tarefas e problemas usando um modelo de layout.

Este artigo descreve os cabeçalhos padrão para todos os objetos, incluindo projetos e tarefas e problemas.

Para obter informações sobre personalização no cabeçalho de um objeto, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).


## Visão geral do cabeçalho do projeto

![](assets/project-header-350x18.png)

O cabeçalho do projeto exibe as seguintes informações, por padrão:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Navegação estrutural com objetos pai</td> 
   <td>Se o projeto estiver associado a um programa ou a um portfólio, ele será exibido na navegação estrutural no canto superior esquerdo do cabeçalho. Clicar no nome do pai abre esse objeto pai.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone roxo do [!UICONTROL Project] <img src="assets/nwe-projects-icon.png"> é exibido à esquerda do nome do projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do projeto</td> 
   <td>Você pode editar o nome do projeto no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL PROJECT]" é exibido acima do nome do projeto no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações da tarefa</td> 
   <td> <p>Ao lado do nome do projeto, a área de ações é exibida.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Porcentagem concluída]</td> 
   <td>Não é possível editar a porcentagem de projeto concluída no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietário do projeto]</td> 
   <td> <p>Você pode editar o [!UICONTROL Project Owner] no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de conclusão planejada] </td> 
   <td> <p>Você pode editar o projeto [!UICONTROL Data de conclusão planejada] e a hora no cabeçalho, se o projeto estiver programado a partir da [!UICONTROL Data de conclusão]. Se o projeto estiver agendado a partir da [!UICONTROL Data de início], essas informações serão atualizadas das tarefas no projeto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Condição] </td> 
   <td> <p>Ao definir o [!UICONTROL Tipo de condição] do projeto como Manual, você pode atualizar o projeto [!UICONTROL condição] no cabeçalho.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>Você pode editar o projeto [!UICONTROL Status] no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área [!UICONTROL Aprovações]</td> 
   <td> <p>Quando você for um dos aprovadores, use os seguintes ícones para gerenciar as aprovações do projeto:</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> </img> [!UICONTROL Aprovar]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> </img> [!UICONTROL Rejeitar]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> </img> [!UICONTROL Lembrar]</p> <p>Se você não for um aprovador, clique no ícone [!UICONTROL Mais] <img src="assets/more-icon-for-approvals-area.png"> para exibir informações sobre a etapa de aprovação atual.</p> <p>Para saber mais sobre aprovações, consulte <a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho da tarefa

![](assets/task-header-350x18.png)

O cabeçalho da tarefa inclui as seguintes informações, por padrão:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Navegação estrutural com objetos pai</td> 
   <td> <p>Os objetos pai da tarefa são exibidos na navegação estrutural. Clicar no nome do pai abre esse objeto pai.</p> <p>Para obter mais informações, consulte <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral das navegações estruturais</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone verde [!UICONTROL Tarefa] <img src="assets/nwe-tasks-icon.png"> é exibida à esquerda do nome da tarefa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome da tarefa</td> 
   <td>Você pode editar o nome da tarefa no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL TASK]" é exibido acima do nome da tarefa no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações da tarefa</td> 
   <td> <p>Ao lado do nome da tarefa, a área [!UICONTROL ações] é exibida.</p> <p> <img src="assets/nwe-dependency-action-area.png"> </p> <p>Se o ícone Dependência for exibido, você poderá clicar no ícone para ver qualquer antecessor ou sucessor da tarefa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Porcentagem concluída]</td> 
   <td>É possível editar o percentual de conclusão da tarefa no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuições]</td> 
   <td>É possível editar os destinatários de uma tarefa a partir do cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Trabalho nela], [!UICONTROL concluído] ou o botão [!UICONTROL Iniciar tarefa]</p> </td> 
   <td> <p>Se a tarefa for atribuída a você, clique no [!UICONTROL Trabalho nela] <span>ou [!UICONTROL Iniciar tarefa]</span> para indicar que agora está trabalhando na tarefa, ou no botão [!UICONTROL Concluído] para indicar que você concluiu a tarefa.</p> <p><span>Para obter informações sobre a substituição do botão [!UICONTROL Trabalhar nele] por um botão [!UICONTROL Iniciar tarefa], consulte <a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substitua o botão [!UICONTROL Trabalhar nele] por um botão [!UICONTROL Iniciar]</a></span>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de conclusão planejada]</td> 
   <td> <p>É possível editar a tarefa [!UICONTROL Data de conclusão planejada] <span>e hora</span> no cabeçalho.</p> <p>Dica: Observe que a [!UICONTROL Commit Date] não está visível no cabeçalho. Você pode visualizá-lo na página [!UICONTROL Detalhes].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>Você pode editar a tarefa [!UICONTROL Status] no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área [!UICONTROL Aprovações]</td> 
   <td> <p>Quando você for um dos aprovadores, use os seguintes ícones para gerenciar as aprovações da tarefa:</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> </img> [!UICONTROL Aprovar]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> </img> [!UICONTROL Rejeitar]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> </img> [!UICONTROL Lembrar]</p> <p>Se você não for um aprovador, clique no ícone [!UICONTROL Mais] <img src="assets/more-icon-for-approvals-area.png"> para exibir informações sobre a etapa de aprovação atual.</p> <p>Para saber mais sobre aprovações, consulte <a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho da ocorrência

![](assets/issue-header-350x19.png)

O cabeçalho do problema inclui as seguintes informações, por padrão:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Navegação estrutural com objetos pai</td> 
   <td> <p>Os objetos pai do problema são exibidos na navegação estrutural. Clicar no nome do pai abre esse objeto pai.</p> <p>Para obter mais informações, consulte <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral das navegações estruturais</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone rosa [!UICONTROL Problema] <img src="assets/nwe-issues-icon.png"> é exibido à esquerda do nome da ocorrência.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do problema</td> 
   <td>Você pode editar o nome do problema no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL PROBLEMA]" é exibido acima do nome do problema no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações do problema</td> 
   <td> <p>Ao lado do nome do problema, a área [!UICONTROL ações] é exibida.</p> <p> <img src="assets/nwe-dependency-action-area.png"> </p> <p>Se o ícone [!UICONTROL Dependência] for exibido, você poderá clicar no ícone para ver qualquer antecessor ou sucessor do problema.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Porcentagem concluída]</td> 
   <td> <p>Você pode editar a porcentagem completa do problema no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuições]</td> 
   <td>É possível editar os destinatários de um problema no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Trabalhar nisso], [!UICONTROL Concluído], <span>ou o botão [!UICONTROL Start Issue]</span></td> 
   <td>Se o problema for atribuído a você, você pode clicar no [!UICONTROL Trabalho com ele] <span>ou [!UICONTROL Start Issue]</span> para indicar que você está trabalhando no problema ou no botão [!UICONTROL Concluído] para indicar que você concluiu o problema.<span>Para obter informações sobre a substituição do botão [!UICONTROL Trabalhar nele] por um botão [!UICONTROL Iniciar tarefa], consulte</span> <span href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substitua o botão [!UICONTROL Trabalhar nele] por um botão [!UICONTROL Iniciar]</a></span><span>.</span></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de conclusão planejada]</td> 
   <td> <p>Você pode editar o problema [!UICONTROL Data de conclusão planejada] <span>e hora</span> no cabeçalho.</p> <p>Dica: Observe que a [!UICONTROL Commit Date] não está visível no cabeçalho. Você pode visualizá-lo na página [!UICONTROL Detalhes].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>Você pode editar o problema [!UICONTROL Status] no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área [!UICONTROL Aprovações]</td> 
   <td> <p>Quando você for um dos aprovadores, use os seguintes ícones para gerenciar as aprovações da emissão:</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> [!UICONTROL Aprovar]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> [!UICONTROL Rejeitar]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> [!UICONTROL Lembrar]</p> <p>Se você não for um aprovador, clique no ícone [!UICONTROL Mais] <img src="assets/more-icon-for-approvals-area.png"> para exibir informações sobre a etapa de aprovação atual.</p> <p>Para saber mais sobre aprovações, consulte <a href="../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho do programa

![](assets/program-header-350x18.png)

O cabeçalho do programa exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Caminho com o nome do Portfolio</td> 
   <td> <p>Você pode acessar o [!UICONTROL Portfolio] a partir do cabeçalho do [!UICONTROL Program]. Clicar no nome do pai abre esse objeto pai.</p> <p>Para obter mais informações, consulte <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral das navegações estruturais</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone laranja [!UICONTROL Program] <img src="assets/nwe-programs-icon.png"> é exibido à esquerda do nome do programa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do programa</td> 
   <td>Você pode editar o nome do programa no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>Se o programa estiver marcado como [!UICONTROL Ativo], o texto "[!UICONTROL PROGRAM]" será exibido acima do nome do programa no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status da ativação</td> 
   <td> <p>Se o programa estiver desativado, o texto "[!UICONTROL PROGRAM DEACTIVATED]" será exibido acima do nome do programa no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Domínio de ação do programa</td> 
   <td> <p>Ao lado do nome do programa, a área [!UICONTROL ações] é exibida.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Porcentagem concluída]</td> 
   <td> <p>Não é possível editar a [!UICONTROL Porcentagem concluída] do programa no cabeçalho. Estas informações são atualizadas a partir dos projetos do programa.</p> <p>Dica: Por padrão, a porcentagem completa do programa é uma média dos valores de porcentagem concluídos dos projetos em um [!UICONTROL Atual] ou [!UICONTROL Status Aprovado] que pertence ao programa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gerenciador do programa]</td> 
   <td> <p>Você pode editar o [!UICONTROL Program Manager] no cabeçalho. É o mesmo que o [!UICONTROL Program Owner].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de conclusão planejada]</td> 
   <td>Não é possível editar o programa [!UICONTROL Data de conclusão planejada] no cabeçalho. Essas informações são atualizadas na [!UICONTROL Data de conclusão planejada] dos projetos do programa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Condição de projetos ativos]</td> 
   <td>Este é um cálculo do percentual de projetos ativos no programa que têm a [!UICONTROL Condição] definida como [!UICONTROL No Target], [!UICONTROL Em Risco] ou [!UICONTROL Em Problema].</td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho do Portfolio {#portfolio-header-overview}

![](assets/portfolio-header-350x19.png)

O cabeçalho do portfólio inclui as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone azul [!UICONTROL Portfolio] <img src="assets/nwe-portfolios-icon.png">é exibido à esquerda do nome do portfólio.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do portfólio</td> 
   <td>Você pode editar o nome do portfólio no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>Se o portfólio estiver marcado como ativo, o texto "[!UICONTROL PORTFOLIO]" será exibido acima do nome do portfólio no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status da ativação</td> 
   <td> <p>Se o portfólio estiver desativado, o texto "[!UICONTROL PORTFOLIO DEACTIVATED]" será exibido acima do nome do portfólio no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área [!UICONTROL ações] do portfólio</td> 
   <td> <p>Ao lado do nome do portfólio, a área [!UICONTROL ações] é exibida.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
   <td>Você pode editar o [!UICONTROL Portfolio Manager] no cabeçalho. É o mesmo que o [!UICONTROL Portfolio Owner].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL No Horário]</td> 
   <td>Este é um cálculo da porcentagem de projetos no portfólio que estão no momento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL No Orçamento]</td> 
   <td>Este é um cálculo da porcentagem de projetos na carteira que estão atualmente no orçamento.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Alinhado]</td> 
   <td>Este é um cálculo do percentual de projetos no portfólio alinhados ao portfólio.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ROI]</td> 
   <td>Este é o cálculo do [!UICONTROL Retorno do investimento] para todos os projetos da carteira.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor líquido]</td> 
   <td>Este é o cálculo do [!UICONTROL Net Value] para todos os projetos no portfólio.</td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho do modelo {#template-header-overview}

![](assets/template-header-350x18.png)

O cabeçalho do modelo exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone verde [!UICONTROL Modelo] <img src="assets/nwe-templates-icon.png">é exibido à esquerda do nome do modelo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do template</td> 
   <td>Você pode editar o nome do modelo no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>Se o modelo estiver marcado como ativo, o texto "[!UICONTROL TEMPLATE]" será exibido acima do nome do modelo no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Status da ativação</td> 
   <td> <p>Se o modelo estiver desativado, o texto "[!UICONTROL TEMPLATE DEACTIVATED]" será exibido acima do nome do modelo no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações do modelo</td> 
   <td> <p>Ao lado do nome do modelo, a área de ações é exibida.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietário do modelo]</td> 
   <td>Você pode editar o campo [!UICONTROL Proprietário do modelo] no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Duração]</td> 
   <td>A duração do template. Não é possível editar esse campo no cabeçalho.</td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho da Tarefa de Modelo

![](assets/template-task-header-350x18.png)

O cabeçalho da tarefa do modelo exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Caminho para objetos pai</td> 
   <td> <p>Os objetos pai da tarefa modelo são exibidos na navegação estrutural. Clicar no nome de um objeto pai abre esse objeto pai.</p> <p>Para obter mais informações, consulte <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral das navegações estruturais</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone verde [!UICONTROL Tarefa] <img src="assets/nwe-tasks-icon.png">é exibido à esquerda do nome da tarefa do modelo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome da tarefa do template</td> 
   <td>Você pode editar o nome da tarefa do modelo no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL TEMPLATE TASK]" é exibido acima do nome da tarefa do modelo no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações da tarefa de modelo</td> 
   <td> <p>Ao lado do nome da tarefa do modelo, a área de ações é exibida.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Atribuições]</td> 
   <td>Você pode editar as [!UICONTROL Atribuições] da tarefa do modelo no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dia de conclusão]</td> 
   <td>Este é o dia na duração do template em que a tarefa do template deve ser concluída.</td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho Registro de Faturamento

![](assets/billing-record-header-nwe-350x19.png)

O cabeçalho do registro de faturamento exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Caminho para objetos pai</td> 
   <td> <p>Os objetos pai do registro de faturamento são exibidos na navegação estrutural. Clicar no nome de um objeto pai abre esse objeto pai.</p> <p>Para obter mais informações, consulte <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral das navegações estruturais</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone azul [!UICONTROL Registro de Faturamento] <img src="assets/nwe-billing-record-icon-57x55.png" style="width: 57;height: 55;"> é exibido à esquerda do nome do registro de cobrança.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do registro de faturação</td> 
   <td>Você pode editar o nome do registro de faturamento no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL FATURANDO REGISTRO]" é exibido acima do nome do registro de faturamento no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações do registro de faturamento</td> 
   <td> <p>Ao lado do nome do registro de faturamento, o menu [!UICONTROL Mais] <img src="assets/more-menu.png"> , que permite selecionar as seguintes opções:</p> 
    <ul> 
     <li> <p>[!UICONTROL Editar]</p> </li> 
     <li> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Registro de Faturamento Total]</td> 
   <td>Esta é a quantia total do registro de faturamento. Não é possível editar esse campo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data de faturamento]</td> 
   <td>Esta é a data em que o registro de faturamento foi criado, a menos que tenha sido alterado manualmente quando o registro de faturamento foi criado. Você pode editar a [!UICONTROL Data de faturamento] no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td> <p>Quando o registro de cobrança tem um status de [!UICONTROL Faturado], você não pode mais editá-lo.</p> <p>Você pode editar o Status do registro de faturamento no cabeçalho.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho do usuário

![](assets/user-header-350x20.png)

O cabeçalho do usuário exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Imagem do perfil do usuário</td> 
   <td>Não é possível atualizar a imagem do perfil no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do usuário e título</td> 
   <td> <p> O título do usuário é exibido em todas as letras maiúsculas acima do nome. Não é possível editar o nome do usuário no cabeçalho.</p> </td> 
  </tr> <!--
   <tr> 
    <td role="rowheader">Name of the object type</td> 
    <td> <p>The name of the object type does not display.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Status da ativação</td> 
   <td> <p>Se o usuário tiver sido desativado, todo o texto e a imagem do perfil no cabeçalho estarão esmaecidos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações do usuário</td> 
   <td> <p>Ao lado do nome do usuário, a área de ações é exibida.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Endereço de email</td> 
   <td>Não é possível editar o endereço de email no cabeçalho. Geralmente, esse também é o nome de usuário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Telefone</td> 
   <td>Não é possível editar o número de telefone no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Equipes</td> 
   <td> <p>Você pode exibir as equipes às quais o usuário pertence. Passe o mouse sobre um avatar da equipe para exibir o nome da equipe. Não é possível editar as equipes no cabeçalho.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho da equipe

![](assets/team-header-350x23.png)

O cabeçalho da equipe exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone roxo da [!UICONTROL Team] <img src="assets/nwe-teams-icon.png"> é exibido à esquerda do nome da equipe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome da equipe</td> 
   <td>Você pode editar o nome da equipe no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL TEAM]" é exibido acima do nome da equipe no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações da equipe</td> 
   <td> <p>Ao lado do nome da equipe, a área [!UICONTROL ações] é exibida.</p> <p> <img src="assets/nwe-switch-team-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Imagens do perfil do membro da equipe</td> 
   <td>As imagens do perfil dos membros da equipe. Passe o mouse sobre uma imagem para exibir o nome do usuário.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Descrição</td> 
   <td>Esta é uma breve descrição sobre os membros da equipe. Não é possível editar a descrição da equipe no cabeçalho.</td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho de iteração

![](assets/iteration-header-350x19.png)

O cabeçalho de iteração exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone laranja [!UICONTROL Iteration] <img src="assets/nwe-iteration-icon-58x58.png" style="width: 58;height: 58;"> é exibido à esquerda do nome da iteração.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome da iteração</td> 
   <td>Você pode editar o nome da iteração no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL ITERATION]" é exibido acima do nome da iteração no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações da iteração</td> 
   <td> <p>No canto superior direito do cabeçalho, a área de ações é exibida.</p> <p> <img src="assets/nwe-iteration-action-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proprietário</td> 
   <td>Este é o [!UICONTROL Proprietário] da iteração. Não é possível editar o [!UICONTROL Proprietário] no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linha do tempo]</td> 
   <td>A [!UICONTROL Linha do tempo] mostra as datas de início e término da iteração. Não é possível editar a [!UICONTROL Linha do tempo] no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Equipe]</td> 
   <td>Não é possível editar a equipe da iteração no cabeçalho. Clicar no nome da equipe o direcionará para a página da equipe.</td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho do grupo

![](assets/nwe-group-header-350x20.png)

O cabeçalho do grupo exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone laranja [!UICONTROL Group] <img src="assets/nwe-group-icon.png"> é exibido à esquerda do nome do grupo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do grupo</td> 
   <td>Você pode editar o nome do grupo no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL GROUP]" é exibido acima do nome do grupo no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área [!UICONTROL ações] do grupo</td> 
   <td> <p>Ao lado do nome do grupo, o menu [!UICONTROL Mais] <img src="assets/more-menu.png"> , que permite selecionar as seguintes opções:</p> 
    <ul> 
     <li> <p>[!UICONTROL Editar]</p> </li> 
     <li> <p>[!UICONTROL Copiar]</p> </li> 
     <li> <p>[!UICONTROL Excluir]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Business Leader]</td> 
   <td>Você pode editar o [!UICONTROL Business Leader] no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Licenças em uso] </td> 
   <td> <p>A caixa [!UICONTROL Licenças em uso] exibe o número de usuários de licença do [!UICONTROL Plan] e do [!UICONTROL Work] no grupo e em seus subgrupos. Você pode clicar nos números para ver essas informações para todos os 5 tipos de licença.</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md" class="MCXref xref">Exibir o número de licenças alocadas e usadas em um grupo no novo [!DNL Adobe Workfront] experiência</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Administradores de grupo]</td> 
   <td>Você pode editar os Administradores de grupo no cabeçalho.</td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho do documento

![](assets/document-header-350x19.png)

O cabeçalho do documento exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Navegação estrutural com objetos pai</td> 
   <td> <p>Os objetos pai do documento são exibidos na navegação estrutural. Clicar no nome de um objeto pai abre esse objeto pai.</p> <p>Para obter mais informações, consulte <a href="../../workfront-basics/the-new-workfront-experience/breadcrumb-overview.md" class="MCXref xref">Visão geral das navegações estruturais</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone azul [!UICONTROL Documento] <img src="assets/nwe-documents-icon-53x50.png" style="width: 53;height: 50;"> é exibido à esquerda do nome do documento.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do documento</td> 
   <td>Você pode editar o nome do documento no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL DOCUMENT]" é exibido acima do nome do documento no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações do documento</td> 
   <td> <p>Ao lado do nome do documento, a área de ações é exibida.</p> <p> <img src="assets/nwe-doc-version-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Área de aprovação [!UICONTROL Decisão]</td> 
   <td> <p>Quando o documento está em uma etapa de aprovação, a área [!UICONTROL Decisões] é exibida no canto superior direito do cabeçalho do Documento.</p> <p>Use os seguintes ícones para gerenciar as aprovações do documento:</p> <p> <img src="assets/nwe-approvals-approve-16x18.png" style="width: 16;height: 18;"> [!UICONTROL Aprovar]</p> <p> <img src="assets/nwe-approvals-recall-16x16.png" style="width: 16;height: 16;"> [!UICONTROL Lembrar]</p> <p> <img src="assets/nwe-approvals-reject-16x19.png" style="width: 16;height: 19;"> [!UICONTROL Rejeitar]</p> <p>Para obter mais informações sobre decisões de aprovação, consulte <a href="../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Aprovar trabalho </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho da empresa {#company-header-overview}

![](assets/company-header-350x20.png)

O cabeçalho da empresa exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone azul da [!UICONTROL Company] <img src="assets/nwe-company-icon.png"> é exibido à esquerda do nome da empresa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome da empresa</td> 
   <td>Você pode editar o nome da empresa no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL COMPANY]" é exibido acima do nome da empresa no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações da empresa</td> 
   <td> <p>Ao lado do nome da empresa, o menu [!UICONTROL Mais] <img src="assets/more-menu.png"> , que permite selecionar as seguintes opções:</p> 
    <ul> 
     <li> <p>[!UICONTROL Editar]</p> </li> 
     <li> <p>[!UICONTROL Excluir empresa]</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do cabeçalho do plano

![](assets/nwe-plan-header-350x34.png)

Os planos são os objetos do [!DNL Workfront Scenario Planner]. Para obter informações sobre o [!DNL Scenario Planner], consulte [O [!DNL Scenario Planner] visão geral](../../scenario-planner/scenario-planner-overview.md).

O cabeçalho do plano exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Retornar aos planos</td> 
   <td>Clicar neste link o direciona para a lista [!UICONTROL Planos].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone azul [!UICONTROL Plan] <img src="assets/nwe-plan-icon-65x62.png" style="width: 65;height: 62;">é exibido à esquerda do nome do plano.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do plano</td> 
   <td>Você pode editar o nome do plano no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL PLAN]" é exibido acima do nome do plano no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Área de ações do plano</td> 
   <td> <p>Ao lado do nome do plano, a área de ações é exibida.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ações adicionais do plano</td> 
   <td> <p>Abaixo do nome do plano e da área de ações, você pode concluir as seguintes ações:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mostrar conflitos]</strong>: Clicar nesse botão mostra ou oculta conflitos nas iniciativas.</p> </li> 
     <li> <p><strong>[!UICONTROL Comparar cenários]</strong>: Clicar neste link exibe uma comparação lado a lado dos cenários criados.</p> </li> 
     <li> <p><strong>[!UICONTROL Seleção de cenário]</strong>: Nesse menu suspenso, é possível copiar um cenário ou selecionar para exibir um cenário diferente.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Informações sobre a função de trabalho</td> 
   <td>Na caixa [!UICONTROL Função do trabalho], você pode ver quantas funções de trabalho estão disponíveis para o plano em comparação a quantas são necessárias. Clicar na caixa permite ajustar as funções de trabalho disponíveis.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Informações [!UICONTROL Financial]</td> 
   <td>Na caixa [!UICONTROL Financeiro], você pode ver o orçamento, o custo e a porcentagem de utilização do plano. Clicar na caixa permite ajustar a quantia do orçamento e determinar se os custos de pessoas estão incluídos no plano.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Valor líquido]</td> 
   <td>Na caixa [!UICONTROL Valor líquido], você pode ver o valor líquido do plano com base no orçamento e nos custos inseridos para o plano.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Informações do [!UICONTROL compartilhado com]</td> 
   <td>Os usuários que têm acesso para visualizar ou gerenciar o plano são exibidos no canto superior direito do cabeçalho. Passar o mouse sobre as imagens do perfil exibe seus nomes.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ir para publicação]</td> 
   <td>Ao clicar em [!UICONTROL Ir para publicação], você pode criar ou atualizar um projeto vinculado a uma iniciativa no cenário que está visualizando.</td> 
  </tr> 
 </tbody> 
</table>


## Visão geral do cabeçalho da meta

![](assets/goal-header.png)

Você pode criar metas estratégicas quando sua empresa tem acesso às Metas da Workfront. Para obter mais informações sobre [!DNL Workfront Goals], consulte [Introdução a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

O cabeçalho da meta exibe as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Informações do cabeçalho</th> 
   <th>Notas</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ícone Objeto </td> 
   <td> <p>O ícone roxo [!UICONTROL Meta] <img src="assets/goal-icon.png" > é exibida à esquerda do nome da meta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome da meta</td> 
   <td>Você pode editar o nome da meta no cabeçalho.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do tipo de objeto</td> 
   <td> <p>O texto "[!UICONTROL GOAL]" é exibido acima do nome da meta no cabeçalho.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">A área de ações da meta</td> 
   <td> <p>Ao lado do nome da meta, a área de ações é exibida.</p> <p> <img src="assets/nwe-general-actions-area.png"> </p>
   Você pode executar as seguintes ações a partir da área de ações da meta:
   <ul><li>[!UICONTROL Editar]</li>
   <li>[!UICONTROL Copiar meta]</li>
   <li>[!UICONTROL Excluir meta]</li>
   <li>[!UICONTROL Compartilhar]</li>
   <li>[!UICONTROL Ativar] ou [!UICONTROL Desativar]</li>
   <li>[!UICONTROL Fechar] ou [!UICONTROL Reabrir]</li>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Progress]</td> 
   <td>A porcentagem da meta de progresso, indicando quanto da meta foi concluída. Não é possível atualizar o progresso da meta. O Workfront calcula com base no progresso de cada indicador de progresso na meta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Proprietário]</td> 
   <td>Este é o proprietário da meta. Você pode atualizar manualmente o proprietário da meta. Usuários, equipes, grupos ou sua organização podem ser proprietários de metas.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Período]</td> 
   <td>O período durante o qual a meta deve ser concluída. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Condição]</td> 
   <td>A condição de meta indica se a meta está no target para ser concluída a tempo ou se está ficando para trás </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>Indica se a meta está ativa, nova ou fechada. Não é possível atualizar manualmente o Status da meta. Para obter mais informações, consulte <a href="../../workfront-goals/goal-management/goal-status-overview.md" class="MCXref xref">Visão geral do status da meta em [!DNL Adobe Workfront Goals]</a></td> 
  </tr> 
 </tbody> 
</table>