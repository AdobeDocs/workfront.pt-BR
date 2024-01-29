---
product-area: reporting
navigation-topic: reporting-elements
title: Usar a visualização de Etapas
description: Você pode aplicar a visualização Marco a uma lista de projeto ou relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '1291'
ht-degree: 0%

---

# Usar a visualização de Etapas

<!-- Audited: 1/2024 -->

Você pode aplicar a visualização Marco a uma lista de projeto ou relatório.

Antes de usar a visualização de etapas, as Etapas precisam ser configuradas, os Caminhos de etapas precisam ser adicionados aos projetos e as Etapas precisam ser associadas às tarefas, conforme descrito nos artigos [Criar um caminho de etapas](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) e [Associar marcos a tarefas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

A visualização Marco está disponível ao visualizar uma lista de projetos ou um relatório de projeto. As seções a seguir descrevem como visualizar e usar a visualização de etapas.

## Requisitos de acesso

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
   <p>Novo: Padrão</p>
   <p>Atual: trabalho ou superior </p> </td> 
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

## Alternar para a exibição de Marco {#switch-to-the-milestone-view}

{{step1-to-projects}}

1. Clique em **Exibir** e, em seguida, clique em **Etapa**.

   A lista ou o relatório é exibido em uma visualização de Marco.

   Para obter informações sobre a exibição de etapas, consulte a seção [Visão geral da visualização de Etapas](#milestone-view-overview) neste artigo.

## Visão geral da visualização de Etapas {#milestone-view-overview}

A visualização Marco está disponível em listas de projeto e relatórios de projeto. Esta visualização permite que você visualize rapidamente todos os marcos associados às tarefas nos projetos que você está visualizando.


>[!NOTE]
>
>A visualização Marco não está disponível nas seguintes áreas:
>
>* Folhas de horas, na lista de projetos ao adicionar um projeto.


Para obter informações sobre como alternar para a visualização de Marco, consulte a seção [Alternar para a exibição de Marco](#switch-to-the-milestone-view) neste artigo.

![Projeto com visualização de etapas](assets/project-with-milestone-view-with-complete.png)

### Seções de exibição de etapas

Ao aplicar a visualização Marco a uma lista de projetos, os projetos são exibidos nas seguintes seções:

* Os projetos associados a um Caminho de Etapas são exibidos primeiro, listados no nome dos respectivos Caminhos de Etapas.

  O Workfront classifica os projetos na primeira seção pelos seguintes critérios, nesta ordem:

   1. ID do Caminho de Etapas Você pode exibir a ID do Caminho de Etapas em um relatório de Caminho de Etapas.

   2. O campo selecionado como o primeiro campo de classificação da lista de projetos na exibição aplicada anteriormente à lista de projetos, antes da seleção da exibição Marco.

* Os projetos não associados a um Caminho do marco são exibidos em seguida, na seção Não atribuído. O Workfront classifica os projetos na seção Não atribuídos pelo campo selecionado como o primeiro campo de classificação da lista de projetos na exibição aplicada anteriormente à lista de projetos, antes de você selecionar a exibição Marco.

### Informações do projeto na visualização Marco

Ao visualizar uma lista de projetos ou um relatório de projeto na visualização Marco, as seguintes informações estão disponíveis:

* **Datas planejadas ou datas projetadas:** Especifique se deseja exibir Datas Planejadas ou Datas Projetadas na visualização Marco.\
  As datas são exibidas para o início e a conclusão, bem como para cada marco no Caminho de marcos.\
  Se você estiver visualizando Datas planejadas e também tiver acesso de gerenciamento ao projeto, poderá editar as seguintes datas diretamente da visualização de Marco: (Se você estiver visualizando Datas projetadas, as datas não poderão ser editadas porque as Datas projetadas são calculadas e não podem ser alteradas manualmente.)

   * **Datas de início do projeto:** Se um projeto estiver programado a partir da Data inicial, é possível alterar manualmente a Data inicial do projeto e a Data de conclusão será calculada.
   * **Datas de Término do Projeto:** Se um projeto estiver programado a partir da Data de conclusão, você poderá alterar manualmente a Data de conclusão do projeto, e a Data inicial será calculada.
   * **Datas de conclusão da tarefa:** Você pode atualizar manualmente a Conclusão para tarefas diretamente da visualização Marco.

* **Percentual concluído:** Exibe a porcentagem de conclusão de cada tarefa e projeto.\
  Você pode desativar a exibição da porcentagem de conclusão, conforme descrito na seção [Configurar quais informações serão exibidas na visualização de Marco](#configure-what-information-displays-in-the-milestone-view) neste artigo.\
  Você pode ajustar a porcentagem de conclusão diretamente na visualização Marco, conforme descrito na seção [Ajustar a Porcentagem Concluída para tarefas na exibição de Marco](#adjust-percent-complete-for-tasks-in-the-milestone-view) neste artigo.

* **Ícones de status da tarefa:** Um ícone de status é exibido ao lado de cada projeto e tarefa na visualização Marco.

   * No Prazo\
     ![](assets/gantt-ontime.png)

   * Fora do Cronograma\
     ![](assets/gantt-behind.png)

   * Em Risco\
     ![](assets/gantt-atrisk.png)

   * Atrasado\
     ![](assets/gantt-late.png)

  Você pode impedir que esses ícones de status sejam exibidos, conforme descrito na seção [Configurar quais informações serão exibidas na visualização de Marco](#configure-what-information-displays-in-the-milestone-view) neste artigo.\
  Para obter informações mais detalhadas sobre cada tipo de status, consulte o artigo [Visão geral do status de progresso da tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Sombreamento do status de tarefas concluídas**: depois que uma tarefa é marcada como Concluída, o plano de fundo da tarefa é sombreado na exibição Marco para indicar se a tarefa foi concluída no prazo ou atrasada:

   * **Sombreamento vermelho para a coluna de tarefas**: O plano de fundo de uma tarefa é vermelho quando o Status do Progresso é **Atrasado**.

   * **Sombreamento verde para a coluna de tarefas**: O plano de fundo de uma tarefa fica verde quando o Status do progresso é **No Prazo**.

* **Sombreamento de status de projeto para as colunas Início e Término do Projeto**:

   * **Coluna inicial do projeto**: O plano de fundo da coluna Início do projeto é vermelho ou verde somente quando a Data de início real é preenchida:

      * **Sombreamento vermelho para a coluna Início do projeto**: O plano de fundo da coluna Início do projeto é vermelho quando o Status de Progresso do projeto é **Atrasado**.

      * **Sombreamento verde para a coluna Início do projeto**: o plano de fundo da coluna Início do projeto fica verde quando o Status de progresso do projeto é **No Prazo**.

   * **Coluna Conclusão do projeto**: O plano de fundo da coluna Conclusão do projeto é vermelho ou verde somente quando a Data de conclusão real é preenchida:

      * **Sombreamento Vermelho para a coluna Conclusão do projeto**: O plano de fundo da coluna Conclusão do projeto é vermelho quando o Status de progresso do projeto é **Atrasado**.

      * **Sombreamento verde para a coluna Conclusão do projeto**: O plano de fundo da coluna Conclusão do projeto fica verde quando o Status de progresso do projeto é **No Prazo**.

   * Nenhuma sombra de cor é atribuída às colunas Início e Conclusão quando as tarefas têm um Status de Progresso de Em Risco ou Atrasado.

  ![Exibição de marco com sombreamento](assets/milestone-view-with-shading.png)

* **Nome do projeto**: o nome do projeto é exibido com um link para o projeto.
* **Ícone Condição do projeto**: Um ícone é exibido ao lado do nome do projeto, indicando a condição do projeto.

## Configurar quais informações serão exibidas na visualização de Marco {#configure-what-information-displays-in-the-milestone-view}

Você pode configurar se os seguintes elementos serão exibidos na visualização Marco:

* Ícones de status de progresso
* Porcentagem concluída de projetos e tarefas

Por padrão, os ícones de status do projeto e o percentual concluído dos projetos são exibidos.

Quaisquer alterações feitas nessas opções se aplicam somente a você; outros usuários não serão afetados. As alterações feitas serão mantidas na próxima vez que você fizer logon no Adobe Workfront.

Para configurar se os ícones de status do projeto e a porcentagem de conclusão dos projetos serão exibidos:

{{step1-to-projects}}

1. Clique em **Exibir** e, em seguida, clique em **Etapa**.\
   Se você estiver visualizando uma lista de projetos dentro de um Portfolio ou programa, selecione a variável **Etapa** subguia.

1. Clique em **Opções** no canto superior direito da visualização Marco.\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

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

1. Clique em **Exibir** e, em seguida, clique em **Etapa**.

1. (Condicional) Se as porcentagens de conclusão não estiverem sendo exibidas na visualização Marco, clique em **Opções** no canto superior direito da visualização Marco, verifique se **Percentual Completo** está ativado.

1. Clique na porcentagem de conclusão abaixo de uma tarefa, especifique uma nova porcentagem e pressione Enter.
