---
product-area: reporting
navigation-topic: text-mode-reporting
title: Coleções de referência em um relatório
description: Coleções de referência em um relatório
author: Nolan
feature: Reports and Dashboards
exl-id: 18ba3f4b-ae03-4694-a2fe-fdbeeb576ea9
source-git-commit: af4a82ad11b57c7a7457d5d7ee74ee18494a1dc0
workflow-type: tm+mt
source-wordcount: '2539'
ht-degree: 0%

---

# Coleções de referência em um relatório

<!-- Audited: 1/2025 -->

Criar um relatório no Adobe Workfront permite exibir um conjunto de objetos, seus respectivos campos ou objetos vinculados em um formato de lista, grade ou gráfico.

Para obter mais informações sobre como criar um relatório no Workfront, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Plano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a relatórios, painéis, calendários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Gerenciar permissões para uma exibição, filtro ou agrupamento </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entender coleções

Uma coleção é uma lista de objetos vinculados a outro objeto.

Você tem os dois relacionamentos a seguir entre objetos no Workfront:

* **Uma relação um para um**: apenas um objeto pode ser vinculado a outro objeto por vez.\
  Por exemplo, um projeto só pode ser vinculado a um portfólio por vez.

* **Uma relação um para muitos**: um objeto pode ser vinculado a vários outros objetos de cada vez.\
  Por exemplo, um projeto pode ter várias tarefas. Nesse caso, a lista de tarefas forma uma coleção para o projeto.

>[!IMPORTANT]
>
>Você pode criar um relatório que mostre a relação um para um entre os objetos usando o Report Builder padrão. No entanto, você só pode criar um relatório que mostre a relação um para muitos entre objetos usando a interface do modo de texto no Report Builder.

Para obter mais informações sobre como criar um relatório no construtor de relatórios padrão, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para obter mais informações sobre como criar um relatório usando a interface do modo de texto, consulte:

* [Visão geral do Modo Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Visão geral dos usos comuns do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
* [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)

## Localizar objetos de coleção e seus campos no API Explorer {#find-collection-objects-and-their-fields-in-the-api-explorer}

Nem todas as coleções podem ser relatadas.

Para entender quais objetos podem ser associados a uma coleção de outros, é necessário usar o API Explorer.\
Para obter mais informações sobre a tabela do API Explorer, consulte o [API Explorer](../../../wf-api/general/api-explorer.md).

Para descobrir quais coleções podem ser relatadas:

1. Vá para o [API Explorer](../../../wf-api/general/api-explorer.md).
1. Encontre o objeto do seu relatório.
1. Selecione a guia **coleções**.

   >[!NOTE]
   >
   >Somente os objetos listados nesta guia podem ser representados como uma coleção em um relatório para o objeto selecionado.

1. Expanda o objeto da coleção clicando nele.
1. Clique no link exibido para ir para o objeto da sua coleção.\
   Isso abre a guia **campos** para o objeto da sua coleção.

   >[!NOTE]
   >
   >Somente os campos listados nesta guia podem ser referenciados no relatório de coleta ou nos campos associados aos objetos listados nesta guia.

## Coleções de referência em relatórios

Você pode fazer referência a objetos de uma coleção nos seguintes elementos de relatório:

* Visualizações
* Filtros
* Prompts

Você não pode fazer referência a objetos de uma coleção nos seguintes elementos de relatório:

* Agrupamento
* Gráfico

Por exemplo, você pode fazer referência às coleções de tarefas ou problemas de um relatório de projeto para mostrar informações de tarefas ou problemas no nível do projeto.

* [Fazer referência a uma coleção na exibição de um relatório](#reference-a-collection-in-the-view-of-a-report)
* [Referenciar uma coleção no Filtro de um relatório](#reference-a-collection-in-the-filter-of-a-report)
* [Referenciar uma coleção no prompt personalizado de um relatório](#reference-a-collection-in-the-custom-prompt-of-a-report)

### Referenciar uma coleção na Exibição de um relatório {#reference-a-collection-in-the-view-of-a-report}

Você pode fazer referência a uma coleção de objetos na exibição de um relatório para mostrar atributos de objetos associados ao objeto do relatório.

Por exemplo, você pode mostrar informações de tarefas ou problemas em um relatório de projeto, criando uma coluna de coleção para tarefas ou problemas na exibição do relatório.

Você pode exibir informações sobre as tarefas ou problemas, como nomes, datas, principais atribuídos, percentual concluído etc. na exibição de coleção.

A exibição mostra informações de tarefas ou problemas em um formato de lista, com cada linha da lista representando informações sobre uma tarefa ou um problema. A lista de tarefas ou problemas e seus campos aparecem na mesma linha do projeto ao qual as tarefas ou problemas pertencem.

![issue_and_tasks_collections_in_reports.png](assets/issue-and-tasks-collections-in-reports-350x171.png){width=400}

* [Adicionar uma coluna de coleção em uma Exibição de relatório](#add-a-collection-column-in-a-report-view)
* [Entender as linhas de uma Exibição de coleção no Modo de Texto](#understand-the-lines-of-a-collection-view-in-text-mode)
* [Limitações de uma Exibição de coleção](#limitations-of-a-collection-view)

### Adicionar uma coluna de coleção em uma Exibição de relatório {#add-a-collection-column-in-a-report-view}

Para adicionar uma coluna de coleção em uma exibição de relatório:

1. Clique no menu **Principal** ![](assets/main-menu-icon.png) e em **Relatórios**.
1. Clique em **Novo Relatório**.
1. Selecione o objeto do relatório.
1. Saia do seu relatório e, usando o [API Explorer](../../../wf-api/general/api-explorer.md), determine quais coleções estão disponíveis para o objeto selecionado para o seu relatório.

   Para obter mais informações sobre como selecionar o objeto de sua coleção, consulte a seção [Localizar objetos de coleção e seus campos no API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) neste artigo.

   Anote qual é o nome do objeto da coleção.

1. Usando o [API Explorer](../../../wf-api/general/api-explorer.md), vá para a lista de campos do objeto que deseja exibir na coleção.

   Para obter mais informações sobre como localizar os campos do objeto de sua coleção, consulte a seção [Localizar objetos de coleção e seus campos no API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) neste artigo.

   Anote qual é o nome do campo que deseja exibir na coleção.

1. Volte para o relatório e, na guia **Colunas (Exibição)**, clique em **Adicionar Coluna**.
1. Clique em **Alternar para Modo de Texto**.
1. Clique em **Editar Modo de Texto**.
1. Selecione todo o texto na caixa de diálogo **Modo de Texto** e remova-o e cole o seguinte código se estiver fazendo referência a um campo do objeto de coleção:

   ```
   valueformat=HTML
   textmode=true
   type=iterate
   listdelimiter=<p>
   displayname=Column Name
   listmethod=nested(collection object name).lists
   valuefield=collection object field
   ```

1. Substitua **Nome da Coluna** pelo nome da sua coluna na linha `displayname`.
1. Substitua o **nome do objeto de coleção** pelo nome do seu objeto de coleção na linha `listmethod`, como aparece no [API Explorer](../../../wf-api/general/api-explorer.md).

1. Substitua o **campo do objeto de coleção** pelo nome do campo do seu objeto de coleção na linha `valuefield`, como ele aparece no [API Explorer](../../../wf-api/general/api-explorer.md).

   Você pode substituir **valuefield** por **valueexpression**, se desejar criar uma expressão personalizada em seu modo de exibição.

   Para obter mais informações sobre expressões personalizadas calculadas, consulte [Visão geral das expressões de dados calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Por exemplo, se você deseja exibir uma lista de tarefas em um relatório de projeto. Esta coleção usa uma linha `valuefield` para fazer referência aos nomes das tarefas.

   Siga um destes procedimentos:

   * Use o código a seguir para criar a coluna:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Project Tasks Names
     listmethod=nested(tasks).lists
     valuefield=name
     ```

   * Use o código a seguir para exibir uma lista de problemas no relatório:

     ```
     displayname=Project Issues Names
     listdelimiter=<p>
     listmethod=nested(issues).lists
     textmode=true
     type=iterate
     valuefield=name
     valueformat=HTML
     ```

     Observe que em uma coleção você deve usar **problemas** para a linha **listmethod**, em vez de **opTasks**, que é o nome do banco de dados para Problemas. Para obter informações sobre quando usar o **problema** e quando usar o **opTask** ao fazer referência a problemas, consulte [Usar &quot;opTask&quot; e &quot;problema&quot; ao fazer referência a problemas](../../../manage-work/issues/issue-information/use-optask-instead-of-issue.md).

   * Para exibir uma lista de tarefas em um relatório de projeto junto com o responsável principal, use uma linha **valueexpression** para fazer referência aos nomes das tarefas adjacentes aos nomes de seus responsáveis principais, em vez de **valuefield**.

     Use o código a seguir para criar a coluna:

     ```
     valueformat=HTML
     textmode=true
     type=iterate
     listdelimiter=<p>
     displayname=Tasks Names - Primary Assignee
     listmethod=nested(tasks).lists
     valueexpression=CONCAT({name},' - ',{assignedTo}.{name})
     ```

1. A coluna a seguir é exibida no relatório de projeto, listando todas as tarefas em cada projeto junto com seus atribuídos principais:

   ![](assets/project-report-with-task-and-assignee-collection-view-nwe-350x222.png){width=400}

1. Clique em **Salvar**.
1. (Opcional) Continue editando o relatório.

   Ou

   Clique em **Salvar + Fechar** para salvar o relatório.

#### Entender as linhas de uma Exibição de coleção no Modo de Texto

As linhas em uma exibição de modo de texto para uma coleção são descritas na tabela a seguir:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Linha de Exemplo</strong> </th> 
   <th><strong>Descrição</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>valueformat=HTML</code> </td> 
   <td> <p>Você pode usar vários valores para esta linha, mas recomendamos que o <code style="font-weight: normal;">valueformat</code> para uma lista de coleção seja <strong>HTML.</strong></p>
   </td> 
  </tr> 
  <tr> 
   <td><code>textmode=true</code> </td> 
   <td> <p>Esta linha indica que a coluna foi configurada usando o modo de texto. Se você remover essa linha, o Workfront a adicionará de volta por padrão.</p> </td> 
  </tr> 
  <tr> 
   <td><code>type=iterate</code> </td> 
   <td> <p>O <code>type</code> de uma lista é sempre <code>iterate</code>, ao criar um modo de exibição.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listdelimiter=&lt;p&gt;</code> </td> 
   <td> <p>Esse é o delimitador usado para separar os valores na lista.<br>Recomendamos usar <code>&lt;p&gt;</code>, que adiciona uma quebra de linha entre os valores.</p> <p>Você também pode usar o seguinte:</p> <p><code>&amp;zwj;</code> (junção de largura zero). Os valores da coleção não têm separação entre eles.<br><strong>,</strong> =separador de vírgula. Os valores da coleção são separados por uma vírgula seguida por nenhum espaço.<br><strong>/</strong> = separador de barras. Os valores da coleção são separados por uma barra.<br><strong>-</strong> = separador de traço. Os valores da coleção são separados por um traço.<br>Deixar esta linha vazia adiciona uma vírgula seguida por um espaço entre os valores da coleção, por padrão.</p> </td> 
  </tr> 
  <tr> 
   <td><code>displayname=</code><em>Nome da coluna</em> </td> 
   <td> <p>Substitua <strong>Nome da coluna</strong> pelo nome real da nova coluna.</p> </td> 
  </tr> 
  <tr> 
   <td><code>listmethod=nested(collection object name).list</code> </td> 
   <td> <p> Essa linha define a coleção que você está referenciando.</p> <p>Substitua o <strong>nome do objeto da coleção</strong> pelo nome do objeto que você está referenciando na sua coleção, como aparece no <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>. Normalmente, esse valor é a forma plural do nome do objeto da coleção.</p> </td> 
  </tr> 
  <tr> 
   <td><code>valuefield=collection object field</code> </td> 
   <td> <p>Essa linha define qual campo você está referenciando a partir do objeto de coleção.</p> <p>Substitua o <strong>campo de objeto da coleção</strong> pelo nome do campo do objeto que você está referenciando na sua coleção, como aparece no <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>É possível substituir essa linha por:</p> <p><strong>valueexpression</strong>=campo/campos de objeto de coleção calculada</p> <p>Usando a <strong>expressão de valor</strong>, você pode  exiba uma expressão personalizada calculada na coluna.</p> <p>Para obter mais informações sobre como formatar linhas <strong>valueexpression</strong>, consulte <a href="../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md" class="MCXref xref">Visão geral da sintaxe do modo de texto</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Limitações de uma Exibição de coleção {#limitations-of-a-collection-view}

Considere as seguintes limitações ao criar uma exibição de coleção:

* Não é possível controlar a ordem na qual os dados da coleção são exibidos.
* Não é possível aplicar formatação condicional a uma exibição de coleção.
* Não é possível transformar um objeto em uma coleção em um link clicável.
* Não é possível criar uma visualização de coleção de outra coleção.\
  Por exemplo, não é possível exibir todos os atribuídos em cada tarefa em um relatório de projeto. Você só pode exibir o responsável principal em cada tarefa em uma visualização de projeto.

### Referência a uma coleção no Filtro de um relatório {#reference-a-collection-in-the-filter-of-a-report}

Você pode fazer referência a uma coleção de objetos no filtro de um relatório para filtrar os atributos de objetos associados ao objeto do relatório.

Por exemplo, você pode filtrar por informações de tarefas ou problemas em um relatório de projeto usando uma referência aos atributos de tarefas ou problemas no projeto na instrução de filtro.

Para adicionar uma referência a uma coleção em um filtro de relatório:

1. Clique no menu **Principal** ![](assets/main-menu-icon.png) e em **Relatórios**.
1. Clique em **Novo Relatório**.
1. Selecione o objeto do relatório.
1. Saia do seu relatório e, usando o [API Explorer](../../../wf-api/general/api-explorer.md), determine quais coleções estão disponíveis para o objeto selecionado para o seu relatório.

   Para obter mais informações sobre como selecionar o objeto de sua coleção, consulte a seção [Localizar objetos de coleção e seus campos no API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) neste artigo.

   Anote qual é o nome do objeto da coleção.

1. Usando o [API Explorer](../../../wf-api/general/api-explorer.md), vá para a lista de campos do objeto que deseja exibir na coleção.

   Para obter mais informações sobre como localizar os campos do objeto de sua coleção, consulte a seção [Localizar objetos de coleção e seus campos no API Explorer](#find-collection-objects-and-their-fields-in-the-api-explorer) neste artigo.

   Anote o campo que deseja exibir na coleção.

1. Volte para o seu relatório e, na guia **Filtros**, clique em **Alternar para Modo de Texto** e depois em **Editar Modo de Texto**.

1. Na área **Definir regras de filtro para seu Relatório**, cole o seguinte código:

   ```
   collection object name:collection object field=collection object value
   collection object name:collection object field_Mod=value of the modifier
   ```

1. Substitua o **nome do objeto de coleção** pelo nome do objeto de coleção como ele aparece no [API Explorer](../../../wf-api/general/api-explorer.md). Normalmente, esse valor é a forma plural do nome do objeto da coleção.

1. Substitua o **campo do objeto de coleção** pelo nome do campo do seu objeto de coleção em, como ele aparece no [API Explorer](../../../wf-api/general/api-explorer.md).

1. Substitua o **valor do objeto de coleção** pelo valor do objeto de coleção como ele aparece no Workfront.
1. Substitua **o valor do modificador** por um modificador válido.

   Para obter uma lista de modificadores, consulte [Modificadores de filtro e condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).\
   Por exemplo, para criar um relatório de projeto que exiba somente projetos com tarefas que tenham &quot;Marketing&quot; em seu nome, use o seguinte código:

   ```
   tasks:name=Marketing
   tasks:name_Mod=cicontains
   ```

   Esse relatório só exibe projetos que tenham pelo menos uma tarefa com a palavra &quot;marketing&quot; no nome.

   ![](assets/marketing-only-tasks-in-project-report-nwe-350x309.png){width=400}

1. Para filtrar o nome de um problema, use o seguinte código:

   ```
   issues:name=Marketing
   issues:name_Mod=cicontains
   ```

   >[!TIP]
   >
   >Observe que você deve usar `issues` como o nome do objeto da coleção, em vez de `optask`, que é a forma como os problemas aparecem no API Explorer.

1. Clique em **Concluído**.
1. (Opcional) Continue editando o relatório.

   Ou

   Clique em **Salvar + Fechar** para salvar o relatório.

### Referenciar uma coleção no prompt personalizado de um relatório {#reference-a-collection-in-the-custom-prompt-of-a-report}

Você pode fazer referência a uma coleção de objetos no prompt personalizado de um relatório para filtrar os resultados do relatório para os atributos de objetos associados ao objeto do relatório.

Por exemplo, você pode solicitar informações sobre tarefas em um relatório de projeto usando uma referência aos atributos de tarefas no projeto no prompt personalizado do relatório.

>[!NOTE]
>
>Você não pode fazer referência a coleções em um prompt padrão.

Um prompt personalizado é um filtro personalizado em que as instruções são unidas por símbolos de E comercial. Recomendamos que você crie sua instrução em um filtro, primeiro, e depois junte as linhas das instruções com &quot;E&quot; comercial.

Para obter mais informações sobre como criar uma instrução de filtro com uma referência de coleção, consulte a seção [Referenciar uma coleção no Filtro de um relatório](#reference-a-collection-in-the-filter-of-a-report) neste artigo.

Para adicionar uma referência a uma coleção no prompt personalizado de um relatório:

1. Clique no menu **Principal** ![](assets/main-menu-icon.png) e em **Relatórios**.
1. Clique em **Novo Relatório**.
1. Selecione o objeto do relatório.
1. Crie um filtro com uma referência de coleção conforme descrito na seção [Referencie uma coleção no Filtro de um relatório](#reference-a-collection-in-the-filter-of-a-report) deste artigo.
1. Clique em **Configurações do relatório**.
1. Clique em **Prompts do Relatório**.
1. Clique em **Adicionar prompt**.
1. Clique em **Personalizar prompt**.
1. Especifique o nome do prompt no campo **Campo***nome**.

1. Especifique um **Rótulo de Item Suspenso**.
1. Especifique o seguinte no campo **Condição**:

   ```
   collection object name:collection object field_Mod=value of the modifier
   ```

1. (Opcional) Especifique se essa opção é exibida por padrão no prompt.
1. Substitua o **nome do objeto de coleção** pelo nome do objeto de coleção como ele aparece no [API Explorer](../../../wf-api/general/api-explorer.md). Normalmente, esse valor é a forma plural do nome do objeto da coleção.
1. Substitua o **campo do objeto de coleção** pelo nome do campo do seu objeto de coleção, como ele aparece no [API Explorer](../../../wf-api/general/api-explorer.md).
1. Substitua o **valor do objeto de coleção** pelo valor do objeto de coleção como ele aparece no Workfront.

   Por exemplo, se estiver filtrando projetos nos quais o nome da tarefa contém &quot;Marketing&quot;, substitua o **valor do objeto de coleção** por **marketing**.

1. Substitua **o valor do modificador** por um modificador válido.

   Para obter uma lista de modificadores, consulte [Modificadores de filtro e condição](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   **Exemplo:** Por exemplo, para criar um relatório de projeto com um prompt personalizado no qual você deseja exibir somente projetos que tenham pelo menos uma tarefa atribuída a um usuário específico, use o código abaixo:

   ```
   tasks:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&tasks:assignedToID_Mod=in
   ```

   Isso gera um relatório em que todos os projetos listados têm pelo menos uma tarefa atribuída ao usuário cuja GUID é 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Você não pode referenciar o nome do destinatário primário (campo &quot;Atribuído a&quot;) de uma tarefa, de acordo com a [API Explorer](../../../wf-api/general/api-explorer.md). Você só pode fazer referência à ID do responsável principal.

   Por exemplo, para filtrar qualquer projeto em que qualquer um dos problemas do projeto seja atribuído a um usuário específico, use o seguinte código para o seu prompt personalizado:

   ```
   issues:assignedToID=57cf1b7a000077c9f02f66cb09c8f86c&issues:assignedToID_Mod=in
   ```

   Isso gera um relatório em que todos os projetos listados têm pelo menos um problema atribuído ao usuário cuja GUID é 57cf1b7a000077c9f02f66cb09c8f86c.

   >[!NOTE]
   >
   >Observe que você deve usar **problemas** para o nome do objeto da coleção. No momento, a API Explorer não oferece um nome de objeto de coleção para problemas.

1. Clique em **Concluído**.
1. (Opcional) Continue editando o relatório.

   Ou

   Clique em **Salvar + Fechar** para salvar o relatório.
