---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão Geral da Data de Início Efetivo do projeto
description: Projetos, tarefas e problemas têm uma Data de início efetiva no Adobe Workfront. Para tarefas e problemas, esta é a data em que eles foram marcados como Em andamento. Para projetos, esta é a data em que a primeira tarefa no projeto é marcada como Em andamento ou foi concluída.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# Visão Geral da Data de Início Efetivo do projeto

Projetos, tarefas e problemas têm uma Data de início efetiva no Adobe Workfront. Para tarefas e problemas, esta é a data em que eles foram marcados como Em andamento. Para projetos, esta é a data em que a primeira tarefa no projeto é marcada como Em andamento ou foi concluída.

## Requisitos de acesso

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
   <td> <p>Acesso de visualização ou superior aos Projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar ou aumentar as permissões de um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Considerações sobre as datas de início reais no Workfront

* A Data de início efetiva está localizada na seção Detalhes de projetos, tarefas e problemas. 
* A Data de Início Efetivo de um projeto, tarefa ou problema não é preenchida quando esses itens são criados.
* A Data de Início Efetivo é preenchida quando o trabalho começa no projeto, tarefa ou problema.
* A Data de início efetiva não será exibida na guia Detalhes do projeto se o trabalho no projeto ainda não tiver sido iniciado.

  A Data de Início Real é exibida em branco nas guias de Detalhes da Tarefa e da Ocorrência se o trabalho ainda não tiver sido iniciado nelas.

* Você pode modificar manualmente a Data Inicial Real de uma tarefa ou um problema, mas não pode modificar a Data Inicial Real de um projeto.

## Considerações sobre as datas de início efetivas dos projetos

* O Workfront define automaticamente a Data real de um projeto quando qualquer uma das situações a seguir ocorrer:

   * Um destinatário da tarefa altera o status de uma tarefa de *Nova* para qualquer outro status que não seja igual a *Nova*.

   * Um destinatário da tarefa altera o Percentual concluído de uma tarefa.

     >[!IMPORTANT]
     >
     >A Data de início efetiva do projeto não é preenchida quando o projeto é marcado como Atual. O trabalho real deve começar nas tarefas do projeto antes que a Data de início real do projeto seja preenchida.

     Nesses casos, a Data de início efetiva do projeto é definida como a data e a hora em que essas ações ocorreram para a tarefa mais antiga no projeto. Isso indica que o projeto começou realmente nesta data e hora.

## Localizar a Data de Início Efetivo de um projeto

Você pode localizar a Data de Início Efetivo de um projeto nas seguintes áreas:

* Na seção Detalhes de um projeto.
* Em um relatório ou exibição de projeto, ao adicionar a Data de Início Efetivo do projeto de objeto no relatório.

  Para obter informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para localizar a Data de Início Efetivo na seção Detalhes do projeto:

1. Clique no ícone **Menu principal** ![Ícone do Menu principal](assets/main-menu-icon.png), no canto superior direito do Workfront, e clique em **Projetos**.
1. Clique no projeto para o qual você deseja exibir a Data de Início Efetivo.
1. Clique em **Detalhes do projeto** no painel esquerdo e vá para a seção **Visão geral**.

   A Data de Início Efetivo é exibida ao longo de outras datas do projeto.

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
