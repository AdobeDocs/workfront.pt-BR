---
product-area: reporting
navigation-topic: reporting-elements
title: Usar a exibição de Marco
description: É possível aplicar a visualização de Marco a uma lista de projetos ou relatório.
author: Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: dcdcf21903d0fceb3c05039689bb87ae4c834d07
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 1%

---

# Usar a exibição de Marco

É possível aplicar a visualização de Marco a uma lista de projetos ou relatório.

Antes de usar a visualização de marcos, os marcos precisam ser configurados, os Caminhos de marcos precisam ser adicionados aos projetos e os Marcos precisam ser associados às tarefas, conforme descrito nos artigos [Criar um caminho de marco](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) e [Associar marcos a tarefas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

A exibição Marco está disponível ao visualizar uma lista de projetos ou um relatório de projeto. As seções a seguir descrevem como visualizar e usar a visualização do marco.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Trabalho ou superior </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Visualizar ou obter acesso superior a Relatórios, Painéis, Calendários</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Visualizar permissões de um relatório de projeto para aplicar a visualização de Marco a um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Alternar para a exibição de Marco {#switch-to-the-milestone-view}

1. Vá para a lista de projetos ou para o relatório do projeto que contém os marcos que deseja visualizar.
1. Clique no botão **Exibir** menu suspenso e, em seguida, clique em **Marco**.

   A lista ou o relatório é exibido em uma exibição de Marco.

   Para obter informações sobre a exibição de marco, consulte a seção [Visão geral da exibição de marco](#milestone-view-overview) neste artigo.

## Visão geral da exibição de marco {#milestone-view-overview}

A exibição Marco está disponível em listas de projetos e relatórios de projetos. Essa visualização permite que você visualize rapidamente todos os marcos associados às tarefas nos projetos que você está visualizando.


>[!NOTE]
>
>A exibição de Marco não está disponível nas seguintes áreas:
>* Folhas de horas, na lista de projetos ao adicionar um projeto.



Para obter informações sobre como alternar para a exibição de Marco, consulte a seção [Alternar para a exibição de Marco](#switch-to-the-milestone-view) neste artigo.

![Projeto com exibição de marco](assets/project-with-milestone-view-with-complete.png)

### Seções da exibição de marco

Ao aplicar a visualização de Marco a uma lista de projetos, os projetos são exibidos nas seguintes seções:

* Os projetos associados a um Caminho de marco são exibidos primeiro, listados sob o nome de seus respectivos Caminhos de marco.

   A Workfront classifica os projetos na primeira seção de acordo com os seguintes critérios, nesta ordem:

   1. ID do Caminho de Etapas. Você pode exibir a ID do caminho do marco em um relatório de Caminho do marco.

   2. O campo selecionado como o primeiro campo de classificação para a lista de projetos na exibição aplicada anteriormente à lista de projetos, antes de selecionar a exibição Marco.

* Os projetos não associados a um Caminho de marco serão exibidos em seguida, na seção Não atribuído . O Workfront classifica os projetos na seção Não atribuído pelo campo selecionado como o primeiro campo de classificação para a lista de projetos na exibição aplicada anteriormente à lista de projetos, antes de você selecionar a exibição Marco.

### Informações do projeto na exibição Marco

Ao visualizar uma lista de projetos ou um relatório de projeto na exibição de Marco, as seguintes informações estarão disponíveis:

* **Datas planejadas ou datas previstas:** Especifique se deseja exibir Datas Planejadas ou Datas Projetadas na exibição de Marco.\
   As datas são exibidas para o Início e Conclusão, bem como para cada Marco dentro do Caminho do Marco.\
   Se você estiver visualizando Datas planejadas e também tiver acesso de Gerenciar ao projeto, poderá editar as seguintes datas diretamente da visualização de Marco: (Se você estiver visualizando Datas projetadas, as datas não poderão ser editadas porque as Datas projetadas são calculadas e não podem ser alteradas manualmente).

   * **Datas de início do projeto:** Se um projeto for programado a partir da Data inicial, é possível alterar manualmente a Data inicial do projeto e a Data de conclusão é calculada.
   * **Datas de conclusão do projeto:** Se um projeto for programado a partir da Data de conclusão, é possível alterar manualmente a Data de conclusão do projeto e a Data de início é calculada.
   * **Datas de conclusão da tarefa:** Você pode atualizar manualmente a Conclusão de tarefas diretamente da exibição de Marco.

* **Porcentagem concluída:** Exibe a porcentagem de conclusão de cada tarefa e projeto.\
   Você pode desativar a exibição da porcentagem de conclusão, conforme descrito na seção [Configurar quais informações são exibidas na exibição de Marco](#configure-what-information-displays-in-the-milestone-view) neste artigo.\
   Você pode ajustar a porcentagem de conclusão diretamente na exibição de Marco, conforme descrito na seção [Ajustar porcentagem concluída para tarefas na exibição de Marco](#adjust-percent-complete-for-tasks-in-the-milestone-view) neste artigo.

* **Ícones de status da tarefa:** Um ícone de status é exibido ao lado de cada projeto e tarefa na exibição de Marco.

   * No Prazo\
      ![](assets/gantt-ontime.png)

   * Fora do Cronograma\
      ![](assets/gantt-behind.png)

   * Em Risco\
      ![](assets/gantt-atrisk.png)

   * Atrasado\
      ![](assets/gantt-late.png)
   Você pode desativar a exibição desses ícones de status, conforme descrito na seção [Configurar quais informações são exibidas na exibição de Marco](#configure-what-information-displays-in-the-milestone-view) neste artigo.\
   Para obter informações mais detalhadas sobre cada tipo de status, consulte o artigo [Visão geral do status de progresso da tarefa](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Sombreamento do status da tarefa para tarefas concluídas**: Depois que uma tarefa é marcada como Concluída, o plano de fundo da tarefa é sombreado na exibição de Marco para indicar se a tarefa foi concluída a tempo ou atrasada:

   * **Sombreamento vermelho para coluna de tarefa**: O plano de fundo de uma tarefa é vermelho quando o Status de Andamento é **Atraso**.

   * **Sombreamento verde para coluna de tarefa**: O plano de fundo de uma tarefa fica verde quando o Status de Andamento é **Hora de ligar**.

* **Sombreamento do status do projeto para as colunas Início e Conclusão do projeto**:

   * **Coluna de Início do Projeto**: O plano de fundo da coluna Início do projeto fica vermelho ou verde somente quando a Data de início real é preenchida:

      * **Sombreamento vermelho para a coluna Início do projeto**: O plano de fundo da coluna Início do projeto fica vermelho quando o Status de Andamento do projeto é **Atraso**.

      * **Sombreamento verde para a coluna Início do projeto**: O plano de fundo da coluna Início do projeto fica verde quando o Status de Andamento do projeto é **Hora de ligar**.
   * **Coluna Conclusão do projeto**: O plano de fundo da coluna Conclusão do projeto é vermelho ou verde somente quando a Data de conclusão real é preenchida:

      * **Sombreamento vermelho para coluna de conclusão de projeto**: O plano de fundo da coluna Conclusão do projeto fica vermelho quando o Status de Andamento do projeto é **Atraso**.

      * **Sombreamento verde para a coluna Conclusão do projeto**: O plano de fundo da coluna Conclusão do projeto fica verde quando o Status de Andamento do projeto é **Hora de ligar**.
   * Nenhum sombreamento de cores é atribuído às colunas Início e Conclusão quando as tarefas têm um Status de progresso de Em risco ou Atrás.

   ![Exibição de marco com sombreamento](assets/milestone-view-with-shading.png)

* **Nome do projeto**: O nome do projeto é exibido com um link para o projeto.
* **Ícone Condição do projeto**: Um ícone é exibido ao lado do nome do projeto, indicando a condição do projeto.

## Configurar quais informações são exibidas na exibição de Marco {#configure-what-information-displays-in-the-milestone-view}

Você pode configurar se os seguintes elementos são exibidos na visualização de Marco:

* Ícones de status de progresso
* Porcentagem de conclusão de projetos e tarefas

Por padrão, os ícones de status do projeto e a porcentagem de conclusão de projetos são exibidos.

As alterações feitas nessas opções se aplicam somente a você; outros usuários não são afetados. As alterações feitas serão retidas na próxima vez que você fizer logon no Adobe Workfront.

Para configurar se os ícones de status do projeto e a porcentagem de conclusão dos projetos são exibidos:

1. Vá para a lista de projetos ou para o relatório do projeto que contém os marcos que deseja visualizar.
1. Clique no botão **Exibir** menu suspenso e, em seguida, clique em **Marco**.\
   Se você estiver visualizando uma lista de projetos dentro de um Portfolio ou Programa, selecione a **Marco** subguia .

1. Clique em **Opções** no canto superior direito da exibição Marco.\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. Selecione dentre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Progresso - Status de Progresso</td> 
      <td> <p>Selecione essa opção para exibir ícones de status de progresso ao lado de cada projeto e tarefa.</p> <p>Essa opção é ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentual concluído</td> 
      <td> <p>Selecione essa opção para exibir a porcentagem de conclusão ao lado de cada projeto e tarefa.</p> <p>Essa opção é ativada por padrão.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Ajustar porcentagem concluída para tarefas na exibição de Marco {#adjust-percent-complete-for-tasks-in-the-milestone-view}

É possível ajustar a porcentagem de conclusão para tarefas na exibição de Marco. Não é possível ajustar a porcentagem concluída para uma tarefa pai (uma tarefa que contém subtarefas).

Para ajustar a porcentagem de conclusão de uma tarefa na exibição de Marco:

1. Vá para a lista de projetos ou para o relatório do projeto que contém os marcos que deseja visualizar.
1. Clique no botão **Exibir** menu suspenso e, em seguida, clique em **Marco**.

1. (Condicional) Se as porcentagens de conclusão não estiverem sendo exibidas no momento na exibição do Marco, clique em **Opções** no canto superior direito da exibição de Marco, verifique se **Porcentagem concluída** estiver ativado.

1. Clique na porcentagem de conclusão abaixo de uma tarefa, especifique uma nova porcentagem e pressione Enter.
