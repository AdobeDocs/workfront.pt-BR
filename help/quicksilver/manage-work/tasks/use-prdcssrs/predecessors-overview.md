---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Visão geral das predecessoras da tarefa
description: Um predecessor é a tarefa da qual outra tarefa (chamada de tarefa sucessora ou dependente) depende. O Adobe Workfront oferece suporte a cinco tipos de dependências de predecessoras.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Visão geral das predecessoras da tarefa

<!--Audited: 12/2023-->

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Um predecessor é a tarefa da qual outra tarefa (chamada de tarefa sucessora ou dependente) depende. O Adobe Workfront oferece suporte a cinco tipos de dependências de predecessoras. Para entender as dependências de predecessoras, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Visão geral dos predecessores

Entender a funcionalidade do antecessor é importante para entender as linhas do tempo em seus projetos.

Existem relações de predecessoras de tarefas entre tarefas em um único projeto e entre tarefas de projetos diferentes.

No caso de dependência entre projetos, é possível estabelecer predecessores entre projetos entre tarefas de dois projetos diferentes.

Se as tarefas predecessoras e sucessoras pertencerem ao mesmo projeto ou a dois projetos diferentes, as dependências e as linhas do tempo de cada projeto serão calculadas da mesma forma.

Quando se trata de predecessores, a linha do tempo do projeto é afetada pelo seguinte:

* Dependência predecessora
* Valor e tipo de defasagem\
  Para obter mais informações sobre dependências e atrasos, consulte [Exemplos de valores predecessores em uma lista de tarefas](#examples-of-predecessor-values-in-a-task-list).

  Por exemplo, se a tarefa A for uma predecessora da tarefa B em um relacionamento de término-início e a tarefa B tiver uma restrição de tarefa O Mais Breve Possível, o Workfront atribuirá à tarefa B uma data de início planejada imediatamente após a data de conclusão planejada da tarefa A, independentemente de a predecessora ser imposta ou não.

Para entender os relacionamentos de predecessores, você deve entender:

* **Tipos de Dependência:** Predecessores são vinculados por vários tipos de dependência. Para obter mais informações sobre tipos de dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Impondo um predecessor:** Ao impor um predecessor, a tarefa sucessora não pode absolutamente iniciar até que o predecessor seja concluído. A tarefa sucessora é exibida como iniciando imediatamente após a conclusão da predecessora.

  Quando a predecessora não está concluída (ou iniciada) e não é imposta, a tarefa sucessora pode ser iniciada, mas a linha do tempo do projeto ainda é afetada pelas datas das tarefas predecessoras e sucessoras.

  Com uma predecessora imposta, o Workfront não permite que a tarefa sucessora seja marcada como Em andamento ou Concluída até que a predecessora seja concluída.

  No entanto, o Workfront permite que horas sejam relatadas na tarefa.\
  Para obter mais informações sobre como impor predecessores, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Defasagens:** você pode criar defasagens em suas dependências, o que cria uma defasagem que deve ocorrer após a conclusão de uma tarefa predecessora e antes do início da tarefa sucessora. Os atrasos afetam a linha do tempo do projeto.

  Para entender os tipos de retardo, consulte [visão geral dos Tipos de retardo](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Criar relacionamentos predecessores

Para criar predecessores, consulte qualquer um dos seguintes artigos:

* Para estabelecer predecessores usando a guia Predecessores da tarefa, consulte [Criar uma relação de predecessoras usando a área Predecessores](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Para estabelecer predecessores em uma lista de tarefas, consulte [Criar uma relação de predecessora na lista de tarefas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Para estabelecer relações de predecessoras por encadeamento de tarefas, consulte [Criar relações de predecessoras por encadeamento de tarefas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Para estabelecer predecessores entre projetos, consulte [Criar predecessores entre projetos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Localizar os predecessores de uma tarefa {#locate-the-predecessors-of-a-task}

Para localizar os predecessores de uma tarefa, siga um destes procedimentos:

* Vá para o projeto em que você está trabalhando e faça o seguinte:

   1. Localize a tarefa para a qual deseja encontrar as predecessoras e clique na tarefa.
   1. Clique em **Predecessores** no painel esquerdo.
   1. O nome do projeto do qual o antecessor é exibido na coluna **Projeto**.

      O número na coluna **#** mostra o número da tarefa predecessora. Por exemplo, &quot;6&quot; significa a sexta tarefa no projeto.

      ![Seção de predecessores da tarefa](assets/predecessors-area-with-task-header.png)

* Vá para o projeto em que você está trabalhando e faça o seguinte:

   1. Clique na guia **Tarefas**.
   1. Escolha a **Exibição Padrão** na parte superior da lista de tarefas.
   1. A coluna **Predecessores** mostra os números de tarefas predecessoras.

      Para uma predecessora entre projetos, a coluna Predecessores mostra o número de referência do projeto ao qual a predecessora pertence e o número da tarefa, separados por dois pontos.

      O ícone predecessor fica verde quando a tarefa predecessora é marcada como concluída. Isso indica que a tarefa dependente está pronta para o trabalho.

      Passe o mouse sobre esse valor para obter mais informações sobre o predecessor, o projeto e as datas.

      ![Detalhes do predecessor](assets/predecessor-details-in-task-list.png)

## Exemplos de valores predecessores em uma lista de tarefas {#examples-of-predecessor-values-in-a-task-list}

Ao exibir predecessores em uma lista de tarefas, você pode ver qualquer um dos seguintes tipos de predecessores com seus respectivos Tipos de dependência e Valores de atraso:

* **1fs -** O número da tarefa predecessora é 1. O tipo de dependência é Término-Início. Na linha do tempo do projeto, essa tarefa é agendada para iniciar imediatamente após a conclusão da tarefa 1. Apesar disso, ainda pode ser marcado como Em andamento ou Concluído.
* **1 -** O número da tarefa predecessora é 1. Isto é o mesmo que **1fs**, porque **fs** é a relação de predecessor padrão no Workfront.

* **1fse -** O número da tarefa predecessora é 1. O tipo de dependência é Finish-Start-Enforced. Na linha do tempo do projeto, essa tarefa é mostrada como iniciando imediatamente após a conclusão da tarefa 1. O Workfront não permite que ela seja marcada como In Progress (Em andamento) ou Complete (Concluído) até que a tarefa 1 seja concluída. No entanto, o Workfront permite que horas sejam relatadas na tarefa.
* **1fs+3d -** O número da tarefa predecessora é 1. O tipo de dependência é Término-Início com um tempo de atraso de 3 dias. Na linha do tempo do projeto, essa tarefa é exibida como iniciando 3 dias úteis após a conclusão da tarefa 1.
* **1fs-3d -** O número da tarefa predecessora é 1. O tipo de dependência é Término-Início com um tempo de atraso de 3 dias. Na linha do tempo do projeto, essa tarefa é exibida como tendo início 3 dias úteis antes da conclusão da tarefa predecessora.
* **1fs+3de** -O número da tarefa predecessora é 1. O tipo de dependência é Finish-Start-Enforced com um tempo de atraso de 3 dias. Na linha do tempo do projeto, essa tarefa é exibida como iniciando 3 dias úteis após a conclusão da tarefa 1. A Workfront não permite que ele seja marcado como Em andamento ou Concluído até que a Tarefa 1 seja concluída. No entanto, o Workfront permite que horas sejam relatadas na tarefa.

  >[!NOTE]
  >
  >Você deve adicionar o valor imposto (**e**) ao Lag, e não ao antecessor.

* **4515:2** O número da tarefa predecessora é 2. - Esta é uma dependência não imposta do Término para o Início com o predecessor no projeto com o número de referência **4515**.

## Exibir informações da predecessora

Você pode exibir as informações da predecessora nas seguintes áreas do Workfront. Isso inclui informações sobre predecessores entre projetos:

* No nível da tarefa, na seção Predecessoras.

  Para obter informações sobre como exibir informações predecessoras na seção Predecessores , consulte a seção [Localizar os predecessores de uma tarefa](#locate-the-predecessors-of-a-task) neste artigo.

* No gráfico de Gantt.

  Para obter informações sobre a exibição de predecessores no gráfico de Gantt, consulte [Configurar como as informações são exibidas no Gráfico de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* Em uma lista de tarefas.

  Para exibir informações sobre os predecessores de suas tarefas em uma lista de tarefas, você pode executar um dos seguintes procedimentos:

   * Aplique o modo de exibição Padrão interno em uma lista de tarefas.

     Para obter informações sobre como exibir informações predecessoras no modo Padrão, consulte a seção [Localizar predecessores de uma tarefa](#locate-the-predecessors-of-a-task) neste artigo.

   * Crie uma exibição de tarefa ou um relatório e adicione a coluna Predecessores a essa exibição.

     Para obter mais informações sobre como criar um modo de exibição personalizado para tarefas com informações predecessoras, consulte [Exibir: detalhes predecessores](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* No cabeçalho da tarefa ao acessar a tarefa.

  ![](assets/qs-predecessor-info-in-task-header-350x141.png)
