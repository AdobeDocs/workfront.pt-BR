---
product-area: reporting
navigation-topic: reporting-elements
title: Usar a visualização de Etapas
description: Você pode aplicar a visualização Marco a uma lista de projeto ou relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1312'
ht-degree: 0%

---

# Usar a visualização de Etapas

<!-- Audited: 11/2024 -->

Você pode aplicar a visualização Marco a uma lista de projeto ou relatório.

Antes de usar a exibição de marcos, os Marcos precisam ser configurados, os Caminhos de Etapas precisam ser adicionados aos projetos e os Marcos precisam ser associados às tarefas, conforme descrito nos artigos [Criar um caminho de marcos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) e [Associar marcos a tarefas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

A visualização Marco está disponível ao visualizar uma lista de projetos ou um relatório de projeto. As seções a seguir descrevem como visualizar e usar a visualização de etapas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença do Adobe Workfront</strong></td> 
   <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Trabalhar ou superior</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Acesso maior ou igual a relatórios, painéis, calendários</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Exibir permissões para um relatório de projeto para aplicar a exibição de Marco a um relatório</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Alternar para a exibição de Marco {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Clique no menu suspenso **Exibir** e em **Marco**.

   A lista ou o relatório é exibido em uma visualização de Marco.

   Para obter informações sobre a exibição de etapas, consulte a seção [Visão geral da exibição de etapas](#milestone-view-overview) neste artigo.

## Visão geral da visualização de Etapas {#milestone-view-overview}

A visualização Marco está disponível em listas de projeto e relatórios de projeto. Esta visualização permite que você visualize rapidamente todos os marcos associados às tarefas nos projetos que você está visualizando.


>[!NOTE]
>
>A visualização Marco não está disponível nas seguintes áreas:
>
>* Folhas de horas, na lista de projetos ao adicionar um projeto.


Para obter informações sobre como alternar para o modo de exibição de Marco, consulte a seção [Alternar para o modo de exibição de Marco](#switch-to-the-milestone-view) neste artigo.

![Projeto com exibição de marco](assets/project-with-milestone-view-with-complete.png)

### Seções de exibição de etapas

Ao aplicar a visualização Marco a uma lista de projetos, os projetos são exibidos nas seguintes seções:

* Os projetos associados a um Caminho de Etapas são exibidos primeiro, listados no nome dos respectivos Caminhos de Etapas.

  O Workfront classifica os projetos na primeira seção pelos seguintes critérios, nesta ordem:

   1. ID do Caminho de Etapas Você pode exibir a ID do Caminho de Etapas em um relatório de Caminho de Etapas.

   2. O campo selecionado como o primeiro campo de classificação da lista de projetos na exibição aplicada anteriormente à lista de projetos, antes da seleção da exibição Marco.

* Os projetos não associados a um Caminho do marco são exibidos em seguida, na seção Não atribuído. O Workfront classifica os projetos na seção Não atribuídos pelo campo selecionado como o primeiro campo de classificação da lista de projetos na exibição aplicada anteriormente à lista de projetos, antes de você selecionar a exibição Marco.

### Informações do projeto na visualização Marco

Ao visualizar uma lista de projetos ou um relatório de projeto na visualização Marco, as seguintes informações estão disponíveis:

* **Datas Planejadas ou Datas Projetadas:** especifique se deseja exibir Datas Planejadas ou Datas Projetadas na exibição de Marco.\
  As datas são exibidas para o início e a conclusão, bem como para cada marco no Caminho de marcos.\
  Se você estiver visualizando Datas planejadas e também tiver acesso de gerenciamento ao projeto, poderá editar as seguintes datas diretamente da visualização de Marco: (Se você estiver visualizando Datas projetadas, as datas não poderão ser editadas porque as Datas projetadas são calculadas e não podem ser alteradas manualmente.)

   * **Datas de Início do Projeto:** Se um projeto estiver agendado a partir da Data de Início, você poderá alterar manualmente a Data de Início do projeto, e a Data de Conclusão será calculada.
   * **Datas de Término do Projeto:** Se um projeto estiver agendado a partir da Data de Término, você poderá alterar manualmente a Data de Término do projeto, e a Data de Início será calculada.
   * **Datas de conclusão da tarefa:** você pode atualizar manualmente a conclusão das tarefas diretamente do modo de exibição Marco.

* **Percentual concluído:** Exibe o percentual de conclusão de cada tarefa e projeto.\
  Você pode desabilitar a exibição da porcentagem de conclusão, conforme descrito na seção [Configurar quais informações serão exibidas na exibição de Marco](#configure-what-information-displays-in-the-milestone-view) deste artigo.\
  Você pode ajustar a porcentagem de conclusão diretamente na exibição de Marco, conforme descrito na seção [Ajustar a porcentagem concluída para tarefas na exibição de Marco](#adjust-percent-complete-for-tasks-in-the-milestone-view) deste artigo.

* **Ícones de status de tarefas:** um ícone de status é exibido ao lado de cada projeto e tarefa no modo de exibição Marco.

   * No Prazo\
     ![Ícone On time](assets/gantt-ontime.png)

   * Fora do Cronograma\
     ![Ícone Atrás](assets/gantt-behind.png)

   * Em Risco\
     ![Ícone de risco](assets/gantt-atrisk.png)

   * Atrasado\
     ![Ícone de atraso](assets/gantt-late.png)

  Você pode desabilitar a exibição desses ícones de status, conforme descrito na seção [Configurar quais informações serão exibidas na exibição de Marco](#configure-what-information-displays-in-the-milestone-view) deste artigo.\
  Para obter informações mais detalhadas sobre cada tipo de status, consulte o artigo [Visão geral do status do progresso da tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Sombreamento de status de tarefa para tarefas concluídas**: depois que uma tarefa é marcada como Concluída, o plano de fundo da tarefa é sombreado no modo de exibição Marco para indicar se a tarefa foi concluída no prazo ou atrasada:

   * **Sombreamento vermelho para a coluna de tarefa**: o plano de fundo de uma tarefa é vermelho quando o Status do Progresso é **Atrasado**.

   * **Sombreamento verde para coluna de tarefa**: o plano de fundo de uma tarefa fica verde quando o Status do Progresso é **No Prazo**.

* **Sombreamento de status do projeto para as colunas Início e Conclusão do Projeto**:

   * **Coluna de Início do Projeto**: o plano de fundo da coluna de Início do Projeto é vermelho ou verde somente quando a Data de Início Efetivo é preenchida:

      * **Sombreamento vermelho para a coluna Início do Projeto**: o plano de fundo da coluna Início do Projeto é vermelho quando o Status de Progresso do projeto é **Atrasado**.

      * **Sombreamento verde para a coluna Início do Projeto**: o plano de fundo da coluna Início do Projeto estará verde quando o Status de Progresso do projeto for **No Prazo**.

   * **Coluna de Término do Projeto**: o plano de fundo da coluna de Término do Projeto é vermelho ou verde somente quando a Data de Término Efetivo é preenchida:

      * **Sombreamento Vermelho para a coluna Conclusão do projeto**: o plano de fundo da coluna Conclusão do projeto fica vermelho quando o Status de Progresso do projeto é **Atrasado**.

      * **Sombreamento verde para a coluna Conclusão do projeto**: o plano de fundo da coluna Conclusão do projeto estará verde quando o Status de Progresso do projeto for **No Prazo**.

   * Nenhuma sombra de cor é atribuída às colunas Início e Conclusão quando as tarefas têm um Status de Progresso de Em Risco ou Atrasado.

  ![Modo de exibição de marco com sombreamento](assets/milestone-view-with-shading.png)

* **Nome do projeto**: o nome do projeto é exibido com um link para o projeto.
* **Ícone Condição do projeto**: um ícone é exibido ao lado do nome do projeto, indicando a condição do projeto.

## Configurar quais informações serão exibidas na visualização de Marco {#configure-what-information-displays-in-the-milestone-view}

Você pode configurar se os seguintes elementos serão exibidos na visualização Marco:

* Ícones de status de progresso
* Porcentagem concluída de projetos e tarefas

Por padrão, os ícones de status do projeto e o percentual concluído dos projetos são exibidos.

Quaisquer alterações feitas nessas opções se aplicam somente a você; outros usuários não serão afetados. As alterações feitas serão mantidas na próxima vez que você fizer logon no Adobe Workfront.

Para configurar se os ícones de status do projeto e a porcentagem de conclusão dos projetos serão exibidos:

{{step1-to-projects}}

1. Clique no menu suspenso **Exibir** e em **Marco**.\
   Se você estiver visualizando uma lista de projetos dentro de uma Portfolio ou um Programa, selecione a subguia **Marco**.

1. Clique em **Opções** no canto superior direito da exibição Marco.\
   ![marco_exibição_opções.png](assets/milestone-view-options-350x141.png)

1. Selecione entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status do Progresso</td> 
      <td> <p>Selecione esta opção para exibir ícones de status de progresso ao lado de cada projeto e tarefa.</p> <p>Essa opção está ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentual concluído</td> 
      <td> <p>Selecione esta opção para exibir a porcentagem de conclusão ao lado de cada projeto e tarefa.</p> <p>Essa opção está ativada por padrão.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Ajustar a Porcentagem Concluída para tarefas na exibição de Marco {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Você pode ajustar a Porcentagem concluída para tarefas na visualização Marco. Não é possível ajustar o Percentual de Conclusão para uma tarefa pai (uma tarefa que contém subtarefas).

Para ajustar o percentual concluído de uma tarefa na exibição Marco:

{{step1-to-projects}}

1. Clique no menu suspenso **Exibir** e em **Marco**.

1. (Condicional) Se as porcentagens de conclusão não estiverem sendo exibidas na exibição Marco, clique em **Opções** no canto superior direito da exibição Marco e verifique se **Porcentagem concluída** está habilitada.

1. Clique na porcentagem de conclusão abaixo de uma tarefa, especifique uma nova porcentagem e pressione Enter.
