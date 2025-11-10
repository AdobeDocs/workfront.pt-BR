---
product-area: reporting
navigation-topic: reporting-elements
title: Usar a visualização de Etapas
description: Você pode aplicar a visualização Marco a uma lista de projeto ou relatório. Você pode usar o modo de exibição Marco para exibir todos os marcos associados às tarefas nos projetos que você está visualizando.
author: Courtney, Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: 1ed84baeacda2717c4f58058fb754e7a79b48baf
workflow-type: tm+mt
source-wordcount: '1370'
ht-degree: 0%

---

# Usar a visualização de Etapas

<!-- Audited: 11/2024 -->

<!--remove Preview and Production mentions from the article when this comes out live-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Você pode aplicar a visualização Marco a uma lista de projeto ou relatório. Você pode usar o modo de exibição Marco para exibir todos os marcos associados às tarefas nos projetos que você está visualizando.

Antes de usar a visualização de etapas, os seguintes elementos devem existir:

* Os caminhos de etapas estão configurados. Para obter informações, consulte [Criar um caminho de etapas](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* Os caminhos de etapas necessários são adicionados aos projetos. Para obter informações, consulte [Editar projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).
* Etapas estão associadas a tarefas. Para obter informações, consulte [Associar marcos a tarefas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

A visualização Marco está disponível ao visualizar uma lista de projetos ou um relatório de projeto. As seções a seguir descrevem como visualizar e usar a visualização de etapas.

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
   <td role="rowheader">Licença do Adobe Workfront</strong></td> 
   <td> 
    <p>Standard</p>
    <p>Trabalhar ou superior</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso maior ou igual a relatórios, painéis, calendários</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
    <td> <p>Exibir permissões para um relatório de projeto para aplicar a exibição de Marco a um relatório</p></td> 
   </td> 
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

A visualização Marco está disponível em listas de projeto e relatórios de projeto. Você pode visualizar rapidamente todos os marcos associados às tarefas nos projetos que está visualizando.

![Projeto com exibição de marco](assets/project-with-milestone-view-with-complete.png)

>[!NOTE]
>
>A visualização Marco não está disponível nas seguintes áreas:
>
>* Folhas de horas, na lista de projetos ao adicionar um projeto.

Para obter informações sobre como alternar para o modo de exibição de Marco, consulte a seção [Alternar para o modo de exibição de Marco](#switch-to-the-milestone-view) neste artigo.


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
  As datas são exibidas para as datas de início e conclusão do projeto, bem como para a conclusão de cada tarefa de etapa no Caminho de Etapas.

  Se você estiver visualizando Datas projetadas, as datas não poderão ser editadas. As datas projetadas são calculadas pela Workfront e não podem ser alteradas manualmente.

  Se você estiver visualizando Datas planejadas e também tiver acesso de Gerenciamento ao projeto, poderá editar as seguintes datas diretamente da visualização de Marco:

   * **Datas de Início do Projeto:** Se um projeto estiver agendado a partir da Data de Início, você poderá alterar manualmente a Data de Início Planejada do projeto, e a Data de Conclusão Planejada será então calculada.
   * **Datas de conclusão do projeto:** se um projeto estiver agendado a partir da Data de conclusão planejada, você poderá alterar manualmente a Data de conclusão planejada do projeto, e a Data de início planejada será calculada.
   * **Datas de conclusão da tarefa:** você pode atualizar manualmente a Data de conclusão planejada para tarefas diretamente do modo de exibição Marco.

* **Percentual concluído:** Exibe o percentual de conclusão de cada tarefa e projeto.

  Você pode desabilitar a exibição da porcentagem de conclusão, conforme descrito na seção [Configurar quais informações serão exibidas na exibição de Marco](#configure-what-information-displays-in-the-milestone-view) deste artigo.

  Você pode ajustar a porcentagem de conclusão diretamente na exibição de Marco, conforme descrito na seção [Ajustar a porcentagem concluída para tarefas na exibição de Marco](#adjust-percent-complete-for-tasks-in-the-milestone-view) deste artigo.

* **Ícones de status de progresso da tarefa:** Estes são ícones que indicam o status de progresso das tarefas:

   * No Prazo - verde
   * Atrás - amarelo
   * Em Risco - azul
   * Atrasado - vermelho

  <!--* In the Production environment, the following status icons display next to each project and task in the Milestone view: 
      * On Time  
      ![On time icon](assets/gantt-ontime.png)
      * Behind  
      ![Behind icon](assets/gantt-behind.png)
      * At Risk  
      ![At risk icon](assets/gantt-atrisk.png)
      * Late  
      ![Late icon](assets/gantt-late.png)
      <!--get new screen shots or hide them for preview or production - could not display all in devtest; idea: use color dots from Task Details tab - New status is blue; Some concerns condition is yellow etc-->

  Você pode desabilitar a exibição desses ícones de status, conforme descrito na seção [Configurar quais informações serão exibidas na exibição de Marco](#configure-what-information-displays-in-the-milestone-view) deste artigo.

  Para obter informações mais detalhadas sobre cada tipo de status, consulte o artigo [Visão geral do status do progresso da tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Sombreamento de status de tarefa para tarefas concluídas**: depois que uma tarefa é marcada como Concluída, o plano de fundo da tarefa é sombreado no modo de exibição Marco para indicar se a tarefa foi concluída no prazo ou atrasada:

   * **Sombreamento vermelho para a coluna de tarefa**: o plano de fundo de uma tarefa é vermelho quando o Status do Progresso é **Atrasado**.

   * **Sombreamento verde para coluna de tarefa**: o plano de fundo de uma tarefa fica verde quando o Status do Progresso é **No Prazo**.

* **Sombreamento de status do projeto para as colunas Início e Conclusão do Projeto**:

   * **Coluna de Início do Projeto**: o plano de fundo da coluna de Início do Projeto é vermelho ou verde somente quando a Data de Início Efetivo é preenchida:

      * **Sombreamento vermelho para a coluna Início do Projeto**: o plano de fundo da coluna Início do Projeto é vermelho quando o Status de Progresso do projeto é **Atrasado**.

      * **Sombreamento verde para a coluna Início do Projeto**: o plano de fundo da coluna Início do Projeto estará verde quando o Status de Progresso do projeto for **No Prazo**.

     >[!TIP]
     >
     >Você deve ir até a página Detalhes do Projeto para visualizar a Data do Início Efetivo do projeto.

   * **Coluna de Término do Projeto**: o plano de fundo da coluna de Término do Projeto é vermelho ou verde somente quando a Data de Término Efetivo é preenchida:

      * **Sombreamento Vermelho para a coluna Conclusão do projeto**: o plano de fundo da coluna Conclusão do projeto fica vermelho quando o Status de Progresso do projeto é **Atrasado**.

      * **Sombreamento verde para a coluna Conclusão do projeto**: o plano de fundo da coluna Conclusão do projeto estará verde quando o Status de Progresso do projeto for **No Prazo**.

     >[!TIP]
     >
     >Você deve ir até a página Detalhes do Projeto para visualizar a Data de Término Efetivo do projeto.

   * Nenhuma sombra de cor é atribuída às colunas Início e Conclusão quando as tarefas têm um Status de Progresso de Em Risco ou Atrasado.

  <!--add new screen shot for preview or production release; logged a bug as this is not happening in the new view - if at prod this is still missing, hide this screen shot-->

  ![Modo de exibição de marco com sombreamento](assets/milestone-view-with-shading.png)

* **Nome do projeto**: o nome do projeto é exibido com um link para o projeto.
* **Ícone Condição do projeto**: os seguintes indicadores mostram a Condição do projeto:

   * No Target - verde
   * Em Risco - amarelo
   * Com Problemas - vermelho

  <!--* In the Production environment, an icon displays next to the project name, indicating the condition of the project. The Condition of the project might be one of the following:
      * On Target
      * At Risk
      * In Trouble -->


## Configurar quais informações serão exibidas na visualização de Marco {#configure-what-information-displays-in-the-milestone-view}

Você pode configurar se os seguintes elementos serão exibidos na visualização Marco:

* Ícones de status de progresso
* Porcentagem concluída de projetos e tarefas

Por padrão, os ícones de status do progresso e o percentual concluído de projetos e tarefas são exibidos.

Quaisquer alterações feitas nessas opções se aplicam somente a você; outros usuários não serão afetados. As alterações feitas serão mantidas na próxima vez que você fizer logon no Workfront.

Para configurar se os ícones de status do projeto e a porcentagem de conclusão dos projetos serão exibidos:

{{step1-to-projects}}

1. Clique no menu suspenso **Exibir** e em **Marco**.

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

   ![Opções de exibição de etapas](assets/milestone-view-options-350x141.png)

## Ajustar a Porcentagem Concluída para tarefas na exibição de Marco {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Você pode ajustar a Porcentagem concluída para tarefas na visualização Marco. Não é possível ajustar o Percentual concluído para uma tarefa pai (uma tarefa que contém subtarefas) ou para um projeto.

Para ajustar o percentual concluído de uma tarefa na exibição Marco:

{{step1-to-projects}}

1. Clique no menu suspenso **Exibir** e em **Marco**.

1. (Condicional) Se as porcentagens de conclusão não estiverem sendo exibidas no modo de exibição Marco, habilite a exibição do Percentual Concluído de tarefas e projetos, conforme descrito na seção [Configurar quais informações serão exibidas no modo de exibição Marco](#configure-what-information-displays-in-the-milestone-view) deste artigo.

1. Mova o **slide de Porcentagem Concluída** para a nova porcentagem concluída para atualizá-lo.

   <!--In the Production environment, click the completion percentage below a task, specify a new percentage, then press Enter.-->
