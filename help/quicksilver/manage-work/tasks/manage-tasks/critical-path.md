---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Visão geral do Caminho Crítico do Projeto
description: Determinar o Caminho crítico de um projeto é uma maneira automática de o Adobe Workfront sinalizar uma sequência de tarefas em um projeto que têm o potencial de afetar a linha do tempo do projeto. As tarefas que podem afetar a linha do tempo do projeto são sinalizadas como sendo tarefas de Caminho Crítico.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Visão geral do Caminho crítico do projeto

<!-- Audited: 5/2025 -->

Determinar o caminho crítico de um projeto é uma maneira automática de o Adobe Workfront sinalizar uma sequência de tarefas em um projeto que têm o potencial de afetar a linha do tempo do projeto. As tarefas que podem afetar a linha do tempo do projeto são sinalizadas como tarefas de Caminho Crítico.

Os seguintes recursos podem afetar o Caminho Crítico de um projeto:

* A Estrutura de detalhamento de trabalho do projeto.

  Para obter mais informações, consulte [Determinar a estrutura do detalhamento do trabalho em um projeto](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md).

* O tempo (duração) que cada tarefa levará para ser concluída.
* As dependências entre as tarefas.

  Considere o seguinte:

   * Quando uma tarefa no Caminho Crítico tem uma relação predecessora, seus predecessores e sucessores também estarão no Caminho Crítico se as alterações nas datas dos predecessores ou sucessores afetarem diretamente seus dependentes.

     >[!TIP]
     >
     >Quando a data sucessora de uma tarefa não afeta diretamente a data de suas tarefas dependentes ou as datas do projeto, a tarefa sucessora não está no Caminho Crítico.
     >
     >
     >![](assets/successor-not-on-critical-path-350x150.png)     >
     >

   * Quando uma subtarefa é identificada como uma tarefa de Caminho Crítico, a tarefa pai também é identificada como uma tarefa de Caminho Crítico se a Data Inicial Projetada e a hora da tarefa pai forem iguais às da subtarefa.

Levando esses recursos em consideração, o sistema calcula o Caminho Crítico usando o caminho mais longo entre a tarefa mais antiga e a tarefa que determina o fim do projeto. O Cálculo do Caminho Crítico leva em conta qual é a primeira e a última vez que cada tarefa pode ser iniciada e concluída sem tornar o projeto mais longo. Esse processo determina quais tarefas são &quot;críticas&quot; (e pertencem ao caminho mais longo) e quais têm &quot;flutuação total&quot; (pode ser adiada sem tornar o projeto mais longo).

Qualquer atraso na atividade de uma tarefa no Caminho Crítico afeta diretamente a Data de conclusão projetada do projeto (não há flutuação no caminho crítico).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Standard<p>
   <p>Trabalhar ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso maior ou igual a tarefas</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir ou aumentar permissões em uma tarefa </p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on a task </p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Visualizar o caminho crítico

Você pode exibir as tarefas que pertencem ao Caminho Crítico nas seguintes áreas do aplicativo do Workfront:

* [Exibir o Caminho Crítico no gráfico de Gantt](#view-the-critical-path-in-the-gantt-chart)
* [Exibir o Caminho Crítico em uma lista de tarefas ou relatório](#view-the-critical-path-in-a-task-list-or-report)

### Exibir o Caminho Crítico no Gráfico de Gantt {#view-the-critical-path-in-the-gantt-chart}

Para exibir tarefas no Caminho Crítico no gráfico de Gantt:

{{step1-to-projects}}

1. Na lista de projetos, selecione um projeto.

1. No painel esquerdo, clique em **Tarefas**. A guia **Tarefas** é aberta.

1. No canto superior direito da lista de tarefas, clique no ícone **Gráfico de Gantt**.

   ![gantt_chart_icon__1_.png](assets/gantt-icon.png)

1. No canto superior direito da seção do Gráfico de Gantt, clique no ícone **Opções** ícone ![Opções ícone](assets/options-icon.png) e selecione a opção **Caminho Crítico** na lista suspensa exibida. As tarefas no Caminho Crítico agora têm uma linha vermelha acima da linha do tempo.

   ![caminho_crítico_no_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Exibir o Caminho Crítico em uma lista de tarefas ou relatório {#view-the-critical-path-in-a-task-list-or-report}

Para exibir quais tarefas estão no caminho crítico em uma lista de tarefas:

{{step1-to-projects}}

1. Na lista de projetos, selecione um projeto.

1. No painel esquerdo, clique em **Tarefas**. A guia **Tarefas** é aberta.

1. Clique no ícone **Exibir** ![Ícone Exibir](assets/view-icon.png) e selecione **Status**. As tarefas que estão no Caminho Crítico exibem um sinalizador **Caminho Crítico** na coluna **Sinalizadores** da lista.

   Ou

   Clique no ícone **Filtro** ![Ícone Filtros](assets/filters-icon.png) e selecione **+ Novo Filtro**.
1. No primeiro campo, digite *É Crítico* e selecione-o quando ele aparecer na seção **Tarefas** da lista.

   ![A tarefa é um filtro crítico](assets/task-is-critical.png)

1. Verifique se **É verdadeiro** está selecionado no segundo menu suspenso.

   ![É o menu suspenso verdadeiro](assets/critical-path-filter.png)

1. Feche o painel Filtros. A lista de tarefas agora exibe somente tarefas que estão no Caminho Crítico.
