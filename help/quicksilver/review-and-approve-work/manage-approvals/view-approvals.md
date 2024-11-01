---
product-area: projects
navigation-topic: approvals
title: Exibir aprovações
description: Os processos de aprovação oferecem flexibilidade para criar aprovações em várias etapas para projetos, tarefas e problemas. Os administradores do Adobe Workfront definem processos de aprovação para oferecer consistência em todo o sistema.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: b0b83e8a8a2a076ec20691183605e3d25d10129d
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Exibir aprovações

Os processos de aprovação oferecem flexibilidade para criar aprovações em várias etapas para projetos, tarefas e problemas. Os administradores do Adobe Workfront definem processos de aprovação para oferecer consistência em todo o sistema.

Para obter informações sobre como criar processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Para obter informações sobre como associar aprovações ao trabalho no Workfront, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou ter maior acesso aos objetos associados às aprovações</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou mais altas para os objetos associados às aprovações</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

+++

## Localizar aprovações no Adobe Workfront

Você pode visualizar ou gerenciar aprovações de várias áreas do Workfront. Para obter informações sobre como gerenciar aprovações em várias áreas, consulte [Aprovando trabalho](../../review-and-approve-work/manage-approvals/approving-work.md).

Você pode exibir ou gerenciar aprovações das seguintes áreas:

* Na área Início

   * Todos os projetos, tarefas, problemas, folhas de horas, documentos e acessos que aguardam sua aprovação são exibidos no widget Minhas aprovações na área Página inicial.
   * As aprovações enviadas por você mesmo também são exibidas no widget Minhas aprovações na área Página inicial, ao escolher a opção de filtro Aprovações enviadas. Para obter mais informações, consulte a seção [Revisar trabalho enviado para aprovação na área Página inicial](#review-work-you-submit-for-approval-in-the-home-area) neste artigo.
   * As aprovações são removidas do widget Minhas aprovações na área Página inicial quando o projeto, tarefa ou problema associado é marcado como Resolvido, Em espera, Fechado ou Cancelado.

  Para obter informações sobre como usar a Página inicial, consulte [Introdução à Página inicial](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* No cabeçalho de um projeto, tarefa, problema, documento ou prova
* Na seção Aprovações de um projeto, tarefa ou problema
* Em um relatório

  >[!NOTE]
  >
  >Você não pode tomar uma decisão sobre uma aprovação de um relatório.

  Você pode criar um relatório de aprovação de projeto, tarefa, problema ou documento que contenha informações de aprovação.

  Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Revise o trabalho que você envia para aprovação na área Página inicial {#review-work-you-submit-for-approval-in-the-home-area}

1. Clique no **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito e em **[!UICONTROL Página inicial]**.
1. (Condicional) Clique em **Personalizar** para adicionar o widget **Minhas aprovações**.
1. (Condicional) Clique no menu suspenso **Filtro** e selecione **Aprovações que enviei** para ver as aprovações que você enviou.


## Exibir o status de aprovação de um objeto

Você pode exibir o status de aprovação de um objeto nas seguintes seções do objeto:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Atualizações </td> 
   <td> <p>Exibe todos os status de aprovação quando eles ocorrem. Os status de aprovação são exibidos em linha com outros status exibidos na seção <strong>Atualizações</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aprovações</td> 
   <td> <p>Exibe informações mais detalhadas sobre o processo de aprovação, como cada estágio do processo de aprovação e se os aprovadores concederam a aprovação.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Use a área Atualizações para exibir um status de aprovação {#use-the-updates-area-to-view-an-approval-status}

Quando uma aprovação é iniciada em um projeto, tarefa ou problema, um status é exibido na guia **Atualizações** do objeto, indicando o status de aprovação. Um novo status é exibido sempre que o objeto passa pelo processo de aprovação. Isso inclui os seguintes eventos:

* Um processo de aprovação é iniciado em um objeto. O processo de aprovação é iniciado quando o status é alterado.
* O objeto foi rejeitado
* O objeto foi aprovado

>[!TIP]
>
>Se uma aprovação for aplicada a uma tarefa, as atualizações de aprovação serão mostradas na guia Updates da tarefa, não na guia Updates do projeto em que a tarefa reside.

### Usar a área Aprovações para exibir um status de aprovação {#use-the-approvals-area-to-view-an-approval-status}

Você pode obter visibilidade sobre onde uma tarefa ou problema em que está trabalhando no momento está no processo de aprovação. Você pode ver as seguintes informações:

* A fase do processo de aprovação
* Quais aprovadores já aprovaram
* Quais aprovadores ainda não aprovaram

Para ver o estado atual de onde uma tarefa ou problema está no processo de aprovação:

1. Vá para o projeto, tarefa ou problema ao qual a aprovação está associada.
1. No painel esquerdo, clique em **Aprovações**. Talvez seja necessário clicar primeiro em **Mostrar mais**.

   A guia Approvals exibe as informações completas sobre todos os caminhos e estágios de aprovação anteriores. Você pode ver exatamente quem tomou uma decisão sobre a aprovação ou se a aprovação está definida para uma equipe, função de trabalho ou usuário.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Para obter informações sobre como criar um Processo de Aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
