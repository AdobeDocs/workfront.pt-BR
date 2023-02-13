---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral da data de início real do projeto
description: Projetos, tarefas e problemas têm uma Data de início real na Adobe Workfront. Para tarefas e problemas, essa é a data em que foram marcados como Em andamento. Para projetos, essa é a data em que a primeira tarefa no projeto é marcada como Em andamento ou foi concluída.
author: Alina
feature: Work Management
exl-id: 4357b072-24f6-4f89-b624-f066f8af0722
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Visão geral da data de início real do projeto

Projetos, tarefas e problemas têm uma Data de início real na Adobe Workfront. Para tarefas e problemas, essa é a data em que foram marcados como Em andamento. Para projetos, essa é a data em que a primeira tarefa no projeto é marcada como Em andamento ou foi concluída.

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
   <td> <p>Exibir ou ter acesso superior a Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões superiores a um projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre as datas de início reais no Workfront

* A Data de início real está localizada na seção Detalhes de projetos, tarefas e problemas. 
* A Data de Início Real de um projeto, tarefa ou problema não é preenchida quando esses itens são criados.
* A Data de Início Real é preenchida quando o trabalho realmente inicia no projeto, tarefa ou problema.
* A Data de início real não é exibida na guia Detalhes do projeto se o trabalho no projeto ainda não tiver sido iniciado.

   A Data de início real é exibida em branco nas guias Tarefa e Detalhes da ocorrência se o trabalho ainda não tiver sido iniciado nelas.

* Você pode modificar manualmente a Data inicial real de uma tarefa ou de um problema, mas não pode modificar a Data inicial real de um projeto.

## Considerações sobre as datas de início reais dos projetos

* O Workfront define automaticamente a Data real de um projeto quando qualquer um dos seguintes casos ocorrer:

   * Um destinatário da tarefa altera o status de uma tarefa de *Novo* para qualquer outro status que não seja igual *Novo*.

   * Um destinatário da tarefa altera a porcentagem de conclusão de uma tarefa.

      >[!IMPORTANT]
      >
      >A Data de início real do projeto não é preenchida quando o projeto é marcado como Atual. O trabalho real deve começar nas tarefas do projeto antes da Data de início real do projeto ser preenchida.

      Nesses casos, a Data de início real do projeto é definida como a data e a hora em que essas ações ocorreram para a tarefa mais antiga no projeto. Isso indica que o projeto realmente começou nessa data e hora.

## Localizar a Data de Início Real de um projeto

Você pode localizar a Data inicial real de um projeto nas seguintes áreas:

* Na seção Detalhes de um projeto.
* Em um relatório ou exibição de projeto, ao adicionar a Data de início real do projeto objeto no relatório.

   Para obter informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para localizar a Data de início real na seção Detalhes do projeto:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Projetos**.
1. Clique no projeto para o qual deseja visualizar a Data de início real.
1. Clique em **Detalhes do projeto** no painel esquerdo, em seguida, vá para o **Visão geral** seção.

   A Data de início real é exibida ao longo de outras datas do projeto .

   ![](assets/nwe-project-actual-start-date--highlighted-350x367.png)

 
