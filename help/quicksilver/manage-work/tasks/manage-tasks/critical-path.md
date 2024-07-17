---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Visão geral do Caminho crítico do projeto
description: Determinar o Caminho crítico de um projeto é uma maneira automática de o Adobe Workfront sinalizar uma sequência de tarefas em um projeto que têm o potencial de afetar a linha do tempo do projeto. As tarefas que podem afetar a linha do tempo do projeto são sinalizadas como sendo tarefas de Caminho Crítico.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# Visão geral do Caminho crítico do projeto

Determinar o Caminho crítico de um projeto é uma maneira automática de o Adobe Workfront sinalizar uma sequência de tarefas em um projeto que têm o potencial de afetar a linha do tempo do projeto. As tarefas que podem afetar a linha do tempo do projeto são sinalizadas como sendo tarefas de Caminho Crítico.

Os seguintes recursos podem afetar o Caminho Crítico de um projeto:

* A Estrutura de detalhamento de trabalho do projeto.

  Para obter mais informações sobre a Estrutura Analítica de Projeto, consulte [Determinar Estrutura Analítica de Projeto em um projeto](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* O tempo (duração) que cada tarefa levará para ser concluída.
* As dependências entre as tarefas.

  Considere o seguinte:

   * Quando uma tarefa no Caminho Crítico tem uma relação predecessora, suas predecessoras e sucessoras também estarão no Caminho Crítico se as alterações nas datas das predecessoras ou sucessoras afetarem diretamente suas dependentes.

     >[!TIP]
     >
     >Quando a data da sucessora de uma tarefa não afeta diretamente a data de suas tarefas dependentes e não afeta as datas do projeto, a tarefa sucessora não está no Caminho Crítico.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Quando uma subtarefa é identificada como uma tarefa de Caminho Crítico, a tarefa pai também é identificada como uma tarefa de Caminho Crítico, se a Data e a Hora de Início Projetadas da tarefa pai forem iguais às da subtarefa.

Levando esses recursos em consideração, o sistema calcula o Caminho Crítico usando o caminho mais longo entre a tarefa mais antiga e a tarefa que determina o fim do projeto. O Cálculo do Caminho Crítico leva em conta qual é a primeira e a última vez que cada tarefa pode ser iniciada e concluída sem tornar o projeto mais longo. Esse processo determina quais tarefas são &quot;críticas&quot; (e pertencem ao caminho mais longo) e quais têm &quot;flutuação total&quot; (pode ser adiada sem tornar o projeto mais longo).

Qualquer atraso na atividade de uma tarefa no Caminho Crítico afeta diretamente a Data de conclusão projetada do projeto (não há flutuação no caminho crítico).

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
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso maior ou igual a tarefas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir ou aumentar permissões em uma tarefa </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Visualizar o caminho crítico

Você pode exibir as tarefas que pertencem ao Caminho Crítico nas seguintes áreas do aplicativo do Workfront:

* [Exibir o Caminho Crítico no gráfico de Gantt](#view-the-critical-path-in-the-gantt-chart)
* [Exibir o Caminho Crítico em uma lista de tarefas ou relatório](#view-the-critical-path-in-a-task-list-or-report)

### Exibir o Caminho Crítico no Gráfico de Gantt {#view-the-critical-path-in-the-gantt-chart}

Para exibir tarefas no Caminho Crítico no gráfico de Gantt:

1. Vá para um projeto cujo Caminho Crítico você deseja exibir.
1. Clique em **Tarefas** no painel esquerdo.
1. Clique no ícone **Gráfico de Gantt** no canto superior direito da lista de tarefas.

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. Expanda o menu **Opções** e habilite a opção **Caminho Crítico**.

   As tarefas no Caminho Crítico têm uma linha vermelha acima da linha do tempo no gráfico de Gantt.

   ![caminho_crítico_no_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Exibir o Caminho Crítico em uma lista de tarefas ou relatório {#view-the-critical-path-in-a-task-list-or-report}

Para exibir quais tarefas estão no caminho crítico em uma lista de tarefas:

1. Vá para um projeto cujo Caminho Crítico você deseja exibir.
1. Clique em **Tarefas** no painel esquerdo.
1. No menu suspenso **Exibir**, selecione **Status**.

   As tarefas que estão no Caminho Crítico têm um sinalizador **Caminho Crítico** na coluna **Sinalizadores** da lista.

   É possível aplicar a mesma visualização a um relatório de tarefa.

   Para obter mais informações sobre como criar relatórios, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   Ou

   No menu suspenso **Filtro**, selecione **Novo Filtro**.

1. Clique em **Adicionar regra de filtro** e comece a digitar **É crítico** em **Mostrar apenas tarefas em que o campo ...**.

1. Selecione-o quando ele aparecer na lista.
1. Clique em **Salvar filtro**.

   A lista só deve exibir tarefas que estejam no Caminho Crítico.
