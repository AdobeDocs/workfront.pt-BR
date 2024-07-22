---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Visão geral dos Tipos de Defasagem
description: Atraso é o tempo que deve decorrer após a conclusão de um predecessor imposto até que a tarefa dependente possa começar (Atraso Positivo) ou o tempo que uma tarefa dependente poderia iniciar antes que o predecessor fosse iniciado (Atraso Negativo).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: ed179058cfec1332384ef76cb04598278109291b
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 0%

---

# Visão geral dos Tipos de Defasagem

<!-- Audited: 01/2024 -->

Atraso é a quantidade de tempo que deve transcorrer após a Conclusão Planejada de um predecessor até que a tarefa dependente possa começar (Atraso Positivo) ou a quantidade de tempo que uma tarefa dependente poderia iniciar antes que o predecessor iniciasse (Atraso Negativo).

As datas Planejada, Projetada e Estimada das tarefas sucessoras são calculadas levando em conta o atraso e as datas Planejada, Projetada e Início Estimado (Conclusão) das tarefas predecessoras.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: Plano </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação da Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de Defasagem {#lag-types}

Um exemplo de uma tarefa que exigiria um tempo de atraso pode ser serrar árvores em madeira. Se a madeira recém-cortada tiver de secar durante um certo tempo antes de poder ser cortada, haverá um atraso entre o corte das árvores e a sua serragem em madeira.

A tabela a seguir ilustra os Tipos de Defasagem e como indicar a quantidade de tempo para cada um:

<table border="1" cellspacing="15"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Valor</strong> </p> </td> 
   <td> <p><strong>Descrição</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Dias (d ou de)</p> </td> 
   <td> <p>O atraso entre duas tarefas vinculadas por dependência é medido em dias úteis. Este é o Tipo de Defasagem padrão. </p> <p>Por exemplo, se houver uma dependência término-início com um atraso de 2 dias úteis e a tarefa predecessora terminar na sexta-feira, a tarefa dependente começará na quarta-feira. Os dias do fim de semana não contam como parte do atraso. </p> <p>Observação: o limite máximo de atraso para dias é 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dias do Calendário (c ou ce)</p> </td> 
   <td> <p>O atraso entre duas tarefas é medido em dias corridos, incluindo feriados e finais de semana. </p> <p>Nota: Embora esse tipo de defasagem conte dias não úteis como parte do defasagem, uma tarefa dependente nunca pode iniciar em um dia não útil. Se esse tipo de defasagem fizer com que a tarefa dependente inicie em um dia não útil, a Data Inicial Planejada da tarefa dependente será programada para o dia útil seguinte. </p> <p>Por exemplo, se houver uma dependência de término-início com um atraso de 2 dias de calendário e a tarefa predecessora terminar na quinta-feira, a tarefa dependente começará na segunda-feira em vez de no domingo. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Percentual (p ou pe)</p> </td> 
   <td> <p>O atraso é expresso como uma porcentagem do tempo estimado para concluir a tarefa predecessora. </p> <p>Por exemplo, se houver uma dependência de término-início com um atraso de 20% em uma tarefa predecessora de 10 dias, o sistema calculará quantos dias representam 20% da duração da tarefa predecessora e a usará como atraso. Nesse caso, seriam 2 dias após a conclusão da tarefa. </p>

<p><b>Nota</b></p> O limite máximo de atraso para a porcentagem é 2000%.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dia da Semana (w ou we) </p> </td> 
   <td> <p>O atraso entre duas tarefas é medido indicando os dias da semana da semana que contém a Data de conclusão planejada do antecessor.</p> <p>Para esse Tipo de Defasagem, cada dia da semana está associado a um número:</p> 
    <ul> 
     <li>Domingo=1</li> 
     <li>Segunda-feira=2</li> 
     <li>Terça-feira=3</li> 
     <li>Quarta=4</li> 
     <li>Quinta-feira=5</li> 
     <li>Sexta=6</li> 
     <li>Sábado=7</li> 
    </ul> <p>Se você quiser indicar que a Data Inicial Planejada do sucessor deve cair em uma terça-feira da semana atual, e a terça-feira for anterior à Data de Conclusão Planejada do antecessor, você codificaria seu sucessor com a seguinte fórmula: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>Nota</b></p>

Se a Data Inicial da sucessora for calculada para ser uma determinada terça-feira e esse dia tiver passado para a semana atual, a Data Inicial Planejada da tarefa sucessora será o mesmo dia (terça-feira) da semana seguinte, se disponível. </p> <p>Se você quiser indicar que o atraso deve cair em um sábado da semana atual, e o sábado for posterior à Data de Término Planejada do antecessor, você codificará seu sucessor com a seguinte fórmula:</p> <p><code>4fs+7w</code> </p> <p>Se sábado for um dia não útil, o próximo dia disponível após sábado (para indicar atraso positivo) será selecionado como a Data Inicial Planejada da sucessora. </p>

<p>Isso não se aplica às exceções de programação. Se uma data também for uma exceção de programação e a Data inicial da sucessora for calculada para esse dia, o sistema tentará encontrar a data disponível mais próxima, que é o dia da semana especificado na expressão predecessora.</p>

<p>Por exemplo, se a Data Inicial for calculada para ser uma determinada terça-feira e esse dia for uma exceção de programação e o atraso do antecessor for positivo, ele escolherá a terça-feira seguinte (se também for um dia útil) como a Data Inicial do sucessor. Se o atraso for negativo, o sistema escolherá a terça-feira anterior como a Data inicial.</p>

<p>Para indicar semanas passadas ou futuras, você pode adicionar um número na frente do número do dia para o tipo de atraso. </p> <p>Por exemplo, para indicar a segunda-feira de 10 semanas atrás, você pode usar esse código para indicar o antecessor do seu sucessor:</p> <p><code>4fs-102w</code> </p> <p>10 indica 10 semanas atrás e 2 é o número atribuído à segunda-feira. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dia da semana diferente de zero (k ou ke)</p> </td> 
   <td> <p>O atraso entre duas tarefas é medido de forma idêntica ao tipo de atraso Dia da semana, exceto se o tempo do antecessor terminar no mesmo dia da semana especificada. O tempo de atraso é calculado para a semana adjacente (+/-). </p> <p>Nesse caso, o tempo de atraso nunca pode ser 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Atraso Negativo

Você pode usar um Atraso negativo para indicar a necessidade ou a capacidade de a tarefa começar antes de a tarefa predecessora terminar.

Considere as seguintes regras ao usar intervalos negativos:

* O Atraso Negativo não pode forçar que as datas de Início/Término de uma tarefa sejam anteriores ou posteriores às datas de Início/Término Planejadas do projeto. Essas datas são especificadas no campo Agendar de do projeto.

  Nesse caso, considere o seguinte:

   * Agendar o projeto a partir da data de conclusão.
   * A última tarefa do projeto deve usar a restrição Deve ser concluída na tarefa. É recomendável conceder à tarefa uma duração suficiente para cuidar de todas as tarefas do projeto. As tarefas restantes funcionam bem com a restrição Assim que possível.

* Usar uma relação de predecessora de Término-Início com tarefas pode produzir uma mensagem de erro.

  Nesse caso, considere o seguinte:

   * Defina uma relação predecessora Término-Término entre tarefas.
   * A Duração da tarefa sucessora deve ser igual ou superior ao número pretendido de dias de atraso entre as tarefas.

## Indicar Tipos de Defasagem e Defasagem em tarefas

É possível indicar tipos de defasagem em tarefas ao definir suas relações de predecessoras.

### Indicar Tipos de Defasagem na seção Predecessores de uma tarefa {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Vá para uma tarefa para a qual deseja definir o predecessor e o Tipo de Defasagem.
1. Clique em **Predecessores** no painel esquerdo. Talvez seja necessário clicar em **Mostrar Mais** e depois em **Predecessores**.
1. Clique em **Adicionar predecessor**.
1. (Opcional) Se você deseja adicionar um predecessor entre projetos, substitua o nome do **Projeto pai** por outro projeto.
1. Comece digitando o nome da tarefa predecessora e selecione-a quando ela aparecer na lista.
1. Selecione o **Tipo de dependência**.

   Para obter mais informações sobre os Tipos de Dependência predecessores, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Especifique um valor numérico para **Lag**. Você pode especificar números negativos para indicar um atraso negativo.
1. Selecione entre as seguintes opções para identificar o tipo de atraso que você deseja indicar para seu predecessor:

   * **Dias**
   * **Dias do Calendário**
   * **Percentual**
   * **Dia da semana**
   * **Dia da Semana (Sem Zero)**

     Para obter mais informações sobre esses Tipos de Defasagem e como eles são calculados, consulte a seção [Tipos de Defasagem](#lag-types) neste artigo.

1. Clique em **Salvar**.

### Indicar Tipos de Defasagem em uma lista de tarefas  {#indicate-lag-types-in-a-task-list}

1. Vá para uma lista de tarefas e selecione a exibição **Padrão**.

1. Clique dentro da coluna **Predecessores** correspondente à tarefa para a qual você deseja especificar um predecessor e uma quantidade de atraso.
1. Digite o seguinte sem espaços:

   * o número da tarefa que você deseja indicar como predecessora da tarefa selecionada
   * a abreviação do tipo de dependência que você deseja indicar entre as tarefas

     Para obter mais informações sobre as abreviações de Tipos de Dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * um **+** para um atraso positivo ou um **-** para um atraso negativo

   * a quantidade do atraso
   * a abreviação do Tipo de Defasagem que você deseja usar

     Para obter mais informações sobre as abreviações para Tipos de Defasagem, consulte a seção [Tipos de Defasagem](#lag-types) neste artigo.

   Por exemplo, para indicar que uma tarefa tem uma predecessora e um atraso positivo de 2 dias, digite `1fs+2d` na coluna Predecessoras.

1. Pressione Enter no teclado para salvar as alterações na tarefa.