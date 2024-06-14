---
product-area: reporting
navigation-topic: text-mode-reporting
title: Editar um filtro usando o modo de texto
description: É possível editar um filtro em uma lista ou relatório usando o modo de texto para acessar campos que não estão disponíveis na interface padrão e criar filtros mais complexos.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# Editar um filtro usando o modo de texto

<!-- Audited: 01/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

É possível editar um filtro em uma lista ou relatório usando o modo de texto para acessar campos que não estão disponíveis na interface padrão e criar filtros mais complexos.

Para obter mais exemplos de modo de texto ao criar um filtro, consulte também a seção [Exemplos de filtros personalizados](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) no artigo [Exibição personalizada, filtro e amostras de agrupamento: índice do artigo](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td><p>Novo: Padrão</p>
    <p>ou</p>
    <p>Atual: Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações e Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis e Calendários para editar elementos de relatórios em um relatório</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar filtros em um relatório</p> <p>Gerenciar permissões de um filtro para editá-lo</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar a usar o modo de texto em um relatório ou lista, sempre verifique se você está familiarizado com a sintaxe do modo de texto do Workfront.

Para obter mais informações, consulte:

* [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exibição personalizada, filtro e amostras de agrupamento: índice do artigo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modo de edição de texto em um filtro

A edição de um filtro usando o modo de texto é idêntica para relatórios e listas. O acesso ao filtro a partir de um relatório ou de uma lista é diferente.

>[!TIP]
>
>Recomendamos que você crie o máximo possível do filtro no modo padrão e, em seguida, converta o filtro no modo de texto para editá-lo.

Para obter mais informações sobre a criação de filtros, consulte [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Siga um destes procedimentos:

   1. Para acessar o filtro a partir de um relatório, vá para o relatório e clique em **Ações de Relatório** > **Editar** > **Filtros** guia.
   1. Para acessar o filtro em uma lista, vá para a lista e no **Filtro** menu, passe o mouse sobre o filtro que deseja modificar e clique em **Editar** ícone ![](assets/edit-icon.png).

      O construtor de filtros é aberto.

1. Clique em **Adicionar uma regra de filtro** para começar a adicionar as condições do filtro, clique em **Modo de texto** ou **Alternar para modo de texto** no lado direito do construtor.
1. Adicione instruções de filtro usando o modo de texto. Cada declaração de filtro pode conter as seguintes linhas e informações adicionais:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Filtrar linha/informações</b></td> 
      <td><b>Exemplo</b></td> 
     </tr> 
     <tr> 
      <td> <p>Nome do campo e o valor igual ao que aparecem no banco de dados do Workfront.</p> <p>Esta linha é obrigatória.</p> <p> Para obter mais informações sobre como os objetos e campos aparecem no banco de dados, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Para filtrar tarefas com status Em andamento, use a seguinte linha:</p> <p><code>status=INP</code> </p> <p><b>DICA</b>

   Ao filtrar por status, é necessário usar o código de três letras do status, não o nome.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Modificador do nome do campo e o modificador é igual a. Isso indica quais condições o campo que você está filtrando deve atender.</p> <p>Esta linha é obrigatória.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Para indicar que o status das tarefas filtradas deve ser igual a Em andamento, use a seguinte linha, além da linha acima:</p> <p><code>status_Mod=in</code> </p> <p>Se o modificador for uma faixa, há duas linhas para indicar o modificador.</p> 
       <div> <span class="autonumber"><span><b>EXEMPLO </b></span></span> 
        <p>Este é um filtro de modo de texto que procura tarefas em andamento, que tenham uma Data de conclusão planejada para o mês atual e estejam atribuídas a um usuário com uma GUID específica:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Para obter uma lista completa de modificadores de filtro no modo de texto, consulte o artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filtro e modificadores de condição</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Operador de instrução. Por padrão, cada instrução de filtro é conectada pelo operador "AND". Isso não é exibido na interface do modo de texto. Você também pode adicionar um operador "OR" entre duas instruções para indicar que deseja filtrar por objetos que podem atender a uma ou outra de duas condições.</p> <p>Os operadores de filtro são necessários somente para filtros que tenham mais de uma instrução.</p> <p>Dica:   
        <ul> 
         <li> <p>"OR" diferencia maiúsculas de minúsculas e sempre deve ser capitalizado.</p> </li> 
         <li> <p>Quando você altera o operador de AND para OR, o número de itens da lista pode aumentar.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>EXEMPLO </b></span></span> 
        <p>Para filtrar tarefas com status Em Andamento ou com Data de Conclusão Planejada de Hoje, use o seguinte: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Um curinga, que permite generalizar as informações em um filtro e fazer referência à hora atual do usuário que está conectado.</p> <p>Os curingas são opcionais.</p> <p>Dica:   <p>Recomendamos usar curingas sempre que possível para tornar seus filtros mais dinâmicos e não duplicar os mesmos filtros para cada usuário ou períodos semelhantes.</p> <p>Para obter informações sobre curingas de filtro, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Visão geral das variáveis de filtro curinga</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>EXEMPLO</b></span></span> 
        <p>Para filtrar tarefas atribuídas ao usuário que está conectado no momento, use o seguinte:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Para adicionar uma instrução de filtro conectada pelo operador &quot;OR&quot;, faça o seguinte:

   1. Adicione uma nova linha de código e digite OR:1: seguido pelo objeto ou atributo pelo qual você deseja filtrar e pelo valor com o qual você deseja compará-lo. Para referenciar tarefas que estão em qualquer status, exceto Nova, use a seguinte linha:

      `OR:1:status=NEW`

   1. Adicione uma segunda linha e digite OR:1: seguido pelo objeto, pelo modificador e pelo código do modificador. Para definir o modificador para a linha de código que faz referência a todos os status de tarefa, exceto para Novo, use a seguinte linha do modificador:

      `OR:1:status_Mod=notin`

      Cada linha da nova instrução deve ser precedida por &quot;OR:`<number>`:&quot;.

      Para obter informações sobre como criar instruções &quot;OR&quot; em um filtro, consulte [Criar instruções &quot;OR&quot; em filtros do modo de texto](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >Você pode ter várias instruções &quot;OR&quot; no mesmo filtro. Toda vez que você tem uma nova instrução &quot;OR&quot;, o número após &quot;OR:&quot; aumenta.
      >
      >Para filtrar tarefas com status Em Andamento, atribuídas ao usuário conectado ou com Data de conclusão planejada para hoje, use o seguinte:
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. Clique em **Sair do modo texto** ou **Concluído** para salvar as alterações no modo de texto e continuar editando o relatório ou o filtro.
1. Clique em **Salvar + Fechar** para salvar seu relatório ou **Salvar Filtro** para salvar o filtro na lista.


