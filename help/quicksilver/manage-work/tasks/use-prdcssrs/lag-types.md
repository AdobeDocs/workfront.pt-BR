---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Visão geral dos tipos de atraso
description: Atraso é a quantidade de tempo que deve decorrer após a conclusão de um antecessor empregado até que a tarefa dependente possa começar (Atraso Positivo), ou a quantidade de tempo que uma tarefa dependente poderia iniciar antes que o antecessor iniciasse (Atraso Negativo).
author: Alina
feature: Work Management
exl-id: 9b3cac9a-1b8d-4697-b5d4-a2d669c790a9
source-git-commit: ad6ade3ff700f1e73c05dfc59aa0108a5d113f2e
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 0%

---

# Visão geral dos tipos de atraso

Atraso é a quantidade de tempo que deve decorrer após a conclusão de um antecessor empregado até que a tarefa dependente possa começar (Atraso Positivo), ou a quantidade de tempo que uma tarefa dependente poderia iniciar antes que o antecessor iniciasse (Atraso Negativo).

As datas Planejadas, Projetadas e Estimadas das tarefas sucessoras são calculadas levando em conta o atraso e as datas Planejadas, Projetadas e Estimadas de Início (Conclusão) das tarefas antecessoras.

## Requisitos de acesso

<!--drafted - replace table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Indicar os tipos de atraso e atraso nas tarefas

Você pode indicar tipos de atraso em tarefas ao definir suas relações de antecessor.

* [Indicar os tipos de atraso na seção Predecessores de uma tarefa](#indicate-lag-types-in-the-predecessors-section-of-a-task)
* [Indicar os tipos de atraso em uma lista de tarefas](#indicate-lag-types-in-a-task-list)

### Indicar os tipos de atraso na seção Predecessores de uma tarefa {#indicate-lag-types-in-the-predecessors-section-of-a-task}

1. Vá para uma tarefa para a qual deseja definir o antecessor e o Tipo de atraso.
1. Clique em **Predecessores** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais** e depois **Predecessores**.
1. Clique em **Adicionar antecessor**.
1. (Opcional) Se quiser adicionar um antecessor entre projetos, substitua o **Projeto pai** com outro projeto.
1. Comece digitando o nome da tarefa predecessora e selecione-a quando ela for exibida na lista.
1. Selecione o **Tipo de dependência**.

   Para obter mais informações sobre os Tipos de Dependência de Antecessores, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. Especifique um **Atraso** usando um valor numérico. Você pode especificar números negativos para indicar um atraso negativo.
1. Selecione entre as seguintes opções para identificar o tipo de atraso que deseja indicar para o antecessor:

   * **Dias**
   * **Dias do Calendário**
   * **Percentual**
   * **Dia da semana**
   * **Dia da semana (não zero)**

      Para obter mais informações sobre esses Tipos de atraso e como eles são calculados, consulte a seção [Visão geral dos tipos de tag](#lag-types-overview) neste artigo.

1. Clique em **Salvar**.

### Indicar os tipos de atraso em uma lista de tarefas  {#indicate-lag-types-in-a-task-list}

1. Vá para uma lista de tarefas e selecione o **Padrão** Exibir no **Exibir** menu suspenso.

1. Clique dentro do **Predecessores** coluna correspondente à tarefa para a qual você deseja especificar um antecessor e um valor de atraso.
1. Insira o seguinte sem espaços:

   * o número da tarefa que deseja indicar como antecessor da tarefa selecionada
   * a abreviação do tipo de dependência que você deseja indicar entre as tarefas

      Para obter mais informações sobre as abreviações para Tipos de dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

   * ou **+** para um atraso positivo ou um **-** para um atraso negativo

   * o montante do atraso
   * a abreviação do Tipo de atraso que deseja usar.

      Para obter mais informações sobre as abreviações dos Tipos de Atraso, consulte a seção [Visão geral dos tipos de tag](#lag-types-overview) neste artigo.
   Por exemplo, para indicar que uma tarefa tem um antecessor e um atraso positivo de 2 dias, você deve inserir

   ```
   1fs+2d
   ```

   na coluna Predecessors .

1. Clique em Enter no teclado para salvar as alterações na tarefa.

## Visão geral dos tipos de tag {#lag-types-overview}

Um exemplo de tarefa que exigiria um tempo de atraso pode ser serrar árvores em madeira. Se a madeira recentemente cortada precisar de secar durante algum tempo antes de poder ser cortada, haveria um atraso entre o corte das árvores e a sua serra em madeira.

A tabela a seguir ilustra os Tipos de atraso e como indicar a quantidade de tempo para cada um:

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
   <td> <p>Dias (d)</p> </td> 
   <td> <p>O atraso entre duas tarefas vinculadas por dependência é medido em dias úteis. Esse é o Tipo de atraso padrão. </p> <p>Por exemplo, se houver uma dependência de início com atraso de 2 dias úteis e a tarefa antecessora terminar na sexta-feira, a tarefa dependente começará na quarta-feira. Os dias de fim de semana não contam como parte do atraso. </p> <p>Observação: O limite máximo de atraso para dias é 366.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dias de calendário (c)</p> </td> 
   <td> <p>O atraso entre duas tarefas é medido em dias de calendário, incluindo feriados e finais de semana. </p> <p>Observação: Embora esse tipo de atraso conte dias não úteis como parte do atraso, uma tarefa dependente nunca poderá iniciar em um dia não útil. Se esse tipo de atraso fizer com que a tarefa dependente inicie em um dia não útil, a Data Inicial Planejada da tarefa dependente será agendada para o dia útil seguinte. </p> <p>Por exemplo, se houver uma dependência de início completo com um atraso de 2 dias e a tarefa antecessora terminar na quinta-feira, a tarefa dependente iniciará na segunda-feira em vez de um domingo. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Porcentagem (p ou pe)</p> </td> 
   <td> <p>O atraso é expresso como uma porcentagem do tempo estimado para concluir a tarefa antecessora. </p> <p>Por exemplo, se houver uma dependência de início com atraso de 20% em uma tarefa antecessora de 10 dias, o sistema calculará quantos dias representam 20% da duração da tarefa antecessores e usará isso como atraso. Nesse caso, seriam 2 dias após a conclusão da tarefa. </p>

<p><b>Nota</b></p> O limite máximo de atraso para porcentagem é de 2000%.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dia da semana (w) </p> </td> 
   <td> <p>O atraso entre duas tarefas é medido indicando os dias da semana para a semana que contém a Data de conclusão planejada do antecessor.</p> <p>Para esse Tipo de atraso, cada dia da semana é associado a um número:</p> 
    <ul> 
     <li>Domingo=1</li> 
     <li>Segunda-feira=2</li> 
     <li>Terça-feira=3</li> 
     <li>Quarta-feira=4</li> 
     <li>Quinta-feira=5</li> 
     <li>Sexta=6</li> 
     <li>Sábado=7</li> 
    </ul> <p>Se você quiser indicar que a Data Inicial Planejada do sucessor deve cair em uma terça-feira da semana atual e que a terça-feira é anterior à Data de Conclusão Planejada do antecessor, você codificaria seu sucessor com a seguinte fórmula: </p> <p><code style="font-style: normal;">4fs-3w</code> </p>

<p><b>Nota</b></p>

Se a terça-feira tiver passado pela semana da Data de Conclusão Planejada do antecessor, a Data Inicial Planejada da tarefa sucessora será o primeiro dia útil disponível dessa semana. </p> <p>Se você quiser indicar que o atraso deve ocorrer em um sábado da semana atual e que o sábado é posterior à Data de conclusão planejada do antecessor, você codificaria seu sucessor com a seguinte fórmula:</p> <p>4fs+7w</code> </p> <p>Se sábado for um dia inútil, o próximo dia disponível depois de sábado (para indicar atraso positivo) é selecionado como a Data inicial planejada do sucessor. </p>

<p>Isso não se aplica às exceções de programação. No caso de uma data também ser uma exceção de programação e a Data inicial do sucessor ser calculada para ser esse dia, o sistema tenta encontrar a data disponível mais próxima, que é o dia da semana especificado na expressão do antecessor.</p>

<p>Por exemplo, se a Data de início for calculada para ser uma determinada terça-feira e esse dia for uma exceção de programação e o atraso do antecessor for positivo, ele escolherá a terça-feira seguinte (se também for um dia útil) como a Data de início do sucessor. Se o atraso for negativo, o sistema escolhe a terça-feira anterior como a Data inicial.</p>

<p>Para indicar semanas passadas ou futuras, é possível adicionar um número na frente do número do dia para o tipo de atraso. </p> <p>Por exemplo, para indicar a segunda-feira de 10 semanas atrás, você pode usar esse código para indicar o antecessor do seu sucessor:</p> <p><code>4fs-102w</code> </p> <p>10 indica 10 semanas atrás e 2 é o número atribuído a Segunda-feira. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dia da semana Não zero (k)</p> </td> 
   <td> <p>O atraso entre duas tarefas é medido de forma idêntica ao tipo de atraso Day of the Week , exceto se o tempo do antecessor terminar no mesmo dia da semana especificada. O tempo de atraso é então calculado para a semana adjacente (+/-). </p> <p>Nesse caso, o tempo de atraso nunca pode ser 0.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visão geral do atraso negativo

Você pode usar um Atraso negativo para indicar a necessidade ou a capacidade da tarefa de começar antes do fim da tarefa antecessora.

Considere as seguintes regras ao usar intervalos negativos:

* O Atraso Negativo não pode forçar as datas de Início/Término de uma tarefa a serem anteriores ou posteriores às datas de Início/Término Planejadas do projeto. Essas datas são especificadas no campo Agendar de do do projeto.

   Nesse caso, considere o seguinte:

   * Programe o projeto a partir da data de conclusão.
   * A última tarefa no projeto deve usar a Restrição de Tarefa Deve Concluir. É recomendável dar à tarefa uma duração suficiente para considerar todas as tarefas no projeto. As tarefas restantes funcionam bem com a restrição Assim que Possível .

* Usar uma relação de antecessor Finish-Start com tarefas pode gerar uma mensagem de erro.

   Nesse caso, considere o seguinte:

   * Defina uma relação de antecessor Finish-Finish entre tarefas.
   * A Duração da tarefa sucessora deve ser igual ou superior ao número pretendido de dias de atraso entre tarefas.
