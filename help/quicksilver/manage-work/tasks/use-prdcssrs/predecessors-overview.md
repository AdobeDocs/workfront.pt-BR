---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Visão geral dos antecessores de tarefas
description: Um antecessor é a tarefa da qual outra tarefa (chamada de tarefa sucessora ou dependente) depende. O Adobe Workfront suporta cinco tipos de dependências de antecessores.
author: Alina
feature: Work Management
exl-id: b2020a50-0921-4ed2-8a34-1a0411992b99
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---

# Visão geral dos antecessores de tarefas

<!-- 

CONTEXT SENSITIVE HELP article. DO NOT CHANGE THE NAME OF THE ARTICLE/ DO NOT MOVE OR DELETE! -->

Um antecessor é a tarefa da qual outra tarefa (chamada de tarefa sucessora ou dependente) depende. O Adobe Workfront suporta cinco tipos de dependências de antecessores. Para entender as dependências do antecessor, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Visão geral dos antecessores

Entender a funcionalidade do antecessor é importante para entender as linhas do tempo em seus projetos.

As relações antecessoras entre tarefas existem em um único projeto e em vários projetos.

No caso de dependência de vários projetos, você pode estabelecer antecessores de vários projetos.

Independentemente de as tarefas predecessoras e sucessoras pertencerem ao mesmo projeto ou a dois projetos diferentes, as dependências e as linhas do tempo são calculadas da mesma forma.

Quando se trata de antecessores, a linha do tempo do projeto é afetada pelo seguinte:

* Dependência de antecessor
* Atrasar valor e tipo\
   Para obter mais informações sobre dependência e atraso, consulte [Exemplos de valores do antecessor em uma lista de tarefas](#examples-of-predecessor-values-in-a-task-list).

Por exemplo, se a tarefa A for um antecessor da tarefa B em um relacionamento de finalização de início e a tarefa B tiver uma restrição de tarefa o Mais rápido possível, o Workfront atribuirá à tarefa B uma data de início planejada imediatamente após a data de conclusão planejada da tarefa A, independentemente de o antecessor ser ou não empregado.

Para entender as relações entre antecessores, você deve entender:

* **Tipos de dependência:** Os antecessores são vinculados por vários tipos de dependência. Para obter mais informações sobre tipos de dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* **Impor um antecessor:** Ao aplicar um antecessor, a tarefa sucessora não poderá ser iniciada até que o antecessor seja concluído. A tarefa sucessora é exibida como começando imediatamente após a conclusão do antecessor.

   O Workfront não permite que ele seja marcado como Em andamento ou Concluído até que o antecessor seja concluído. No entanto, o Workfront permite que horas sejam relatadas na tarefa.\
   Para obter mais informações sobre como impor predecessores, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

* **Perdas:** Você pode criar atrasos em suas dependências que criam um atraso que deve ocorrer após a conclusão de uma tarefa antecessora e antes que a tarefa sucessora possa começar. Os atrasos afetam a linha do tempo do projeto.

   Para entender os tipos de atraso, consulte [Visão geral dos tipos de atraso](../../../manage-work/tasks/use-prdcssrs/lag-types.md).

## Criar relacionamentos de antecessor

Para criar antecessores, consulte qualquer um dos seguintes artigos:

* Para estabelecer predecessores usando a guia Predecessores da tarefa, consulte [Criar uma relação de antecessor usando a área Predecessores](../../../manage-work/tasks/use-prdcssrs/create-predecessors-in-predecessors-area.md).
* Para estabelecer predecessores em uma lista de tarefas, consulte [Criar uma relação de antecessor na lista de tarefas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).
* Para estabelecer relações de antecessor por tarefas encadeadas, consulte [Criar relações de antecessor por tarefas encadeadas](../../../manage-work/tasks/use-prdcssrs/create-predecessors-by-chaining-tasks.md).
* Para estabelecer antecessores entre projetos, consulte [Criar antecessores entre projetos](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).

## Localizar os antecessores de uma tarefa {#locate-the-predecessors-of-a-task}

Para localizar os antecessores de uma tarefa, execute um dos seguintes procedimentos:

* Vá para o projeto em que você está trabalhando e faça o seguinte:

   1. Encontre a tarefa para a qual deseja encontrar os antecessores e clique na tarefa.
   1. Clique em **Predecessores** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, em seguida **Predecessores**.
   1. O nome do projeto no qual o antecessor está mostra na **Projeto** coluna.

      O número na variável **#** mostra o número da tarefa predecessora. Por exemplo, &quot;6&quot; significa a sexta tarefa do projeto.

      ![Seção de tarefas antecessores](assets/predecessors-area-with-task-header.png)

* Vá para o projeto em que você está trabalhando e faça o seguinte:

   1. Clique no botão **Tarefas** guia .
   1. Escolha a **Exibição padrão** na parte superior da lista de tarefas.
   1. O **Predecessores** mostra os números de tarefa do antecessor.

      Para um antecessor de projeto cruzado, a coluna Predecessores mostra o número de referência do projeto ao qual o antecessor pertence e o número da tarefa, separado por dois pontos.

      O ícone antecessor fica verde quando a tarefa antecessora é marcada como concluída. Isso indica que a tarefa dependente está pronta para o trabalho.

      Passe o mouse sobre esse valor para obter mais informações sobre o antecessor, o projeto e as datas.

      ![Detalhes do antecessor](assets/predecessor-details-in-task-list.png)

## Exemplos de valores do antecessor em uma lista de tarefas {#examples-of-predecessor-values-in-a-task-list}

Ao exibir antecessores em uma lista de tarefas, você poderá ver qualquer um dos seguintes tipos de antecessores com seus respectivos Tipos de dependência e Quantias de atraso:

* **1fs -** O número da tarefa antecessora é 1. O tipo de dependência é Finish-Start. Na linha do tempo do projeto, essa tarefa é agendada para iniciar imediatamente após a conclusão da tarefa 1. Apesar disso, ainda pode ser marcado como Em andamento ou Concluído.
* **1 -** O número da tarefa antecessora é 1. É o mesmo que **1fs**, porque **fs** é a relação predecessora padrão no Workfront.

* **1fse -** O número da tarefa antecessora é 1. O tipo de dependência é Finish-Start-Enforced. Na linha do tempo do projeto, essa tarefa é exibida como começando imediatamente após a conclusão da tarefa 1. O Workfront não permite que ele seja marcado como Em andamento ou Concluído até que a tarefa 1 seja concluída. No entanto, o Workfront permite que horas sejam relatadas na tarefa.
* **1fs+3d -** O número da tarefa antecessora é 1. O tipo de dependência é Finish-Start com um tempo de atraso de 3 dias. Na linha do tempo do projeto, essa tarefa é exibida como iniciando 3 dias úteis após a conclusão da tarefa 1.
* **1fs-3d -** O número da tarefa antecessora é 1. O tipo de dependência é Finish-Start com um tempo de atraso de 3 dias. Na linha do tempo do projeto, essa tarefa é exibida como iniciando 3 dias úteis antes da conclusão da tarefa antecessora.
* **1fs+3de** -O número da tarefa antecessora é 1. O tipo de dependência é Finish-Start-Enforced com um tempo de atraso de 3 dias. Na linha do tempo do projeto, essa tarefa é exibida como iniciando 3 dias úteis após a conclusão da tarefa 1. O Workfront não permite que ele seja marcado como Em andamento ou Concluído até que a Tarefa 1 seja concluída. No entanto, o Workfront permite que horas sejam relatadas na tarefa.

   >[!NOTE]
   >
   >O valor imposto (**e**) deve ser adicionado ao Atraso, não ao antecessor.

* **4515:2** O número da tarefa antecessora é 2. - Trata-se de uma dependência Finish to Start, não imposta com o antecessor no projeto com número de referência **4515**; o número da tarefa predecessora é **2**.

## Exibir informações do antecessor

Você pode exibir as informações do antecessor nas seguintes áreas do Workfront. Isso inclui informações sobre antecessores de vários projetos:

* No nível da tarefa, na seção Predecessors .

   Para obter informações sobre a exibição de informações do antecessor na seção Predecessores , consulte a seção [Localizar os antecessores de uma tarefa](#locate-the-predecessors-of-a-task) neste artigo.

* No gráfico de Gantt.

   Para obter informações sobre como exibir predecessores no gráfico de Gantt, consulte [Configurar como as informações são exibidas no Gráfico de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

* Em uma lista de tarefas.

   Para exibir informações sobre os antecessores de suas tarefas em uma lista de tarefas, é possível fazer um dos seguintes procedimentos:

   * Aplique a visualização padrão integrada em uma lista de tarefas.

      Para obter informações sobre a exibição de informações do antecessor na exibição Padrão, consulte a seção [Localizar os antecessores de uma tarefa](#locate-the-predecessors-of-a-task) neste artigo.

   * Crie uma visualização de tarefa ou relatório e adicione a coluna Predecessores a essa visualização.

      Para obter mais informações sobre como criar uma exibição personalizada para tarefas com informações do antecessor, consulte [Exibir: detalhes do antecessor](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-predecessor-details.md).

* No cabeçalho da tarefa ao acessar a tarefa.

   ![](assets/qs-predecessor-info-in-task-header-350x141.png)
