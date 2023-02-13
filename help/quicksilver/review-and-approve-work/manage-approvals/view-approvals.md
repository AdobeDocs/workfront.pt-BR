---
product-area: projects
navigation-topic: approvals
title: Exibir aprovações
description: Os processos de aprovação fornecem a flexibilidade para criar aprovações em várias etapas para projetos, tarefas e problemas. Os administradores da Adobe Workfront definem processos de aprovação para fornecer consistência ao sistema.
author: Courtney
feature: Work Management
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Exibir aprovações

Os processos de aprovação fornecem a flexibilidade para criar aprovações em várias etapas para projetos, tarefas e problemas. Os administradores da Adobe Workfront definem processos de aprovação para fornecer consistência ao sistema.

Para obter informações sobre a criação de processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Para obter informações sobre como associar aprovações ao trabalho no Workfront, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisitos de acesso

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
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Exibir ou obter acesso mais alto aos objetos associados às aprovações</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar permissões ou permissões superiores para os objetos associados às aprovações</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Localizar aprovações no Adobe Workfront

Você pode visualizar ou gerenciar aprovações de várias áreas do Workfront. Para obter informações sobre como gerenciar aprovações em várias áreas, consulte [Aprovar trabalho](../../review-and-approve-work/manage-approvals/approving-work.md).

Você pode exibir ou gerenciar aprovações nas seguintes áreas:

* Na área de residência

   * Todos os projetos, tarefas, problemas, folhas de ponto, documentos e acesso que aguardam sua aprovação são exibidos na área Início quando você seleciona exibir Todos ou Aprovações.
   * As aprovações que você enviou também são exibidas na área inicial, na seção Aprovações que enviei da lista de trabalho. Para obter mais informações, consulte o [Analise o trabalho enviado para aprovação na área inicial](#review-work-you-submit-for-approval-in-the-home-area) neste artigo.
   * As aprovações são removidas da área Inicial quando o projeto, tarefa ou problema associado é marcado como Resolvido, Em Retenção, Fechado ou Cancelado.

   Para obter informações sobre como usar o Início, consulte [Introdução ao Início](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* No cabeçalho de um projeto, tarefa, emissão, documento ou prova
* Na seção Aprovações de um projeto, tarefa ou problema
* Em um relatório

   >[!NOTE]
   >
   >Não é possível tomar uma decisão sobre uma aprovação a partir de um relatório.

   Você pode criar um projeto, tarefa, problema ou relatório de aprovação de documento que contenha informações de aprovação.

   Para obter informações sobre como criar relatórios, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Analise o trabalho enviado para aprovação na área inicial {#review-work-you-submit-for-approval-in-the-home-area}

1. Clique no botão **Início** ícone ![](assets/home-icon-30x29.png) no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início no seu ambiente:
   >
   >* Substitua por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone terá uma aparência diferente da mostrada neste artigo.
   >* Substitua a página vinculada a ela por uma página diferente. Nesse caso, clique no botão **Menu principal** ![](assets/main-menu-icon.png) no canto superior direito da página, em seguida, clique em **Início**.


1. Selecionar **Lista de Trabalho**, em seguida, clique no botão **Filtro** e selecione **Aprovações**.
1. Expanda o **Aprovações que enviei** e encontre as aprovações enviadas.

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## Exibir o status de aprovação de um objeto

É possível exibir o status de aprovação de um objeto nas seguintes seções do objeto:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Atualizações </td> 
   <td> <p>Exibe todos os status de aprovação quando eles ocorrem. Os status de aprovação são exibidos em linha com outros status exibidos na <strong>Atualizações</strong> seção.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aprovações</td> 
   <td> <p>Exibe informações mais detalhadas sobre o processo de aprovação, como cada estágio do processo de aprovação e se os aprovadores concederam a aprovação.</p> </td> 
  </tr> 
 </tbody> 
</table>

* [Usar a área Atualizações para exibir um status de aprovação](#use-the-updates-area-to-view-an-approval-status)
* [Usar a área Aprovações para exibir um status de aprovação](#use-the-approvals-area-to-view-an-approval-status)

### Usar a área Atualizações para exibir um status de aprovação {#use-the-updates-area-to-view-an-approval-status}

Quando uma aprovação é iniciada em um projeto, tarefa ou ocorrência, um status é exibido na variável **Atualizações** do objeto, indicando o status de aprovação. Um novo status é exibido sempre que o objeto é transferido por meio do processo de aprovação. Isso inclui os seguintes eventos:

* Um processo de aprovação é iniciado em um objeto. O processo de aprovação é iniciado quando o status é alterado.
* O objeto é rejeitado
* O objeto foi aprovado 

>[!TIP]
>
>Se uma aprovação for aplicada a uma tarefa, as atualizações de aprovação serão mostradas na guia Updates da tarefa, não na guia Updates do projeto em que a tarefa reside.

### Usar a área Aprovações para exibir um status de aprovação {#use-the-approvals-area-to-view-an-approval-status}

Você pode obter visibilidade sobre onde uma tarefa ou problema que você está trabalhando atualmente está no processo de aprovação. Você pode ver as seguintes informações:

* A fase do processo de aprovação
* Que aprovadores já o aprovaram
* Que aprovadores ainda não o aprovaram

Para ver o estado atual de onde uma tarefa ou problema está no processo de aprovação:

1. Vá para o projeto, tarefa ou problema ao qual a aprovação está associada.
1. No painel esquerdo, clique em **Aprovações**. Talvez seja necessário clicar primeiro **Mostrar mais**.

   A guia Approvals exibe as informações completas sobre todos os caminhos e estágios de aprovação anteriores. Você pode ver exatamente quem tomou uma decisão sobre a aprovação ou se a aprovação foi definida para uma equipe, função de trabalho ou usuário.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Para obter informações sobre como criar um Processo de Aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
