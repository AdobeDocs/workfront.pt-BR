---
product-area: reporting
navigation-topic: text-mode-reporting
title: Editar um filtro usando o modo de texto
description: '"OBSERVAÇÃO: adicione uma seção neste artigo: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Além disso, crie essa área no artigo de visão geral do Modo de texto)'''
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 1%

---

# Editar um filtro usando o modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

É possível editar um filtro em uma lista ou relatório usando o modo de texto para acessar campos que não estão disponíveis na interface padrão e criar filtros mais complexos.

## Requisitos de acesso

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
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar elementos de relatório em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar filtros em um relatório</p> <p>Gerenciar permissões em um filtro para editá-lo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar a usar o modo de texto em um relatório ou lista, sempre verifique se você está familiarizado com a sintaxe do modo de texto do Workfront.

Para obter mais informações, consulte:

* [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exibição personalizada, filtro e amostras de agrupamento](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Editar modo de texto em um filtro

Editar um filtro usando o modo de texto é idêntico para relatórios e listas. O acesso à exibição de um relatório ou de uma lista é diferente.

>[!TIP]
>
>Recomendamos que você crie o máximo possível de filtros no modo padrão e, em seguida, converta o filtro em modo de texto para editá-lo.

Para obter mais informações sobre criação de filtros, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Siga um destes procedimentos:

   1. Para acessar o filtro de um relatório, vá para o relatório e clique em **Ações de Relatório** > **Editar** > **Filtros** guia .
   1. Para acessar o filtro de uma lista, vá para a lista e do **Filtro** no menu suspenso, passe o mouse sobre o filtro que deseja modificar e clique no botão **Editar** ícone ![](assets/edit-icon.png).

      O construtor de filtros é aberto.

1. Clique em **Adicionar uma regra de filtro** para começar a adicionar as condições do filtro, clique em **Alternar para o modo de texto** no canto superior direito do construtor.
1. Adicione instruções de filtro usando o modo de texto. Cada instrução de filtro pode conter as seguintes linhas e informações adicionais:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Filtrar linha/informação</td> 
      <td>Exemplo</td> 
     </tr> 
     <tr> 
      <td> <p>Nome do campo e o valor ao qual ele é igual ao exibido no banco de dados do Workfront.</p> <p>Esta linha é obrigatória.</p> <p> Para obter mais informações sobre como os objetos e campos são exibidos no banco de dados, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Para filtrar tarefas em um status Em andamento, use a seguinte linha:</p> <p><code>status=INP</code> </p> <p>Dica: Ao filtrar por status, você deve usar o código de três letras do status e não o nome.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Modificador de nome de campo e o que o modificador é igual a. Isso indica quais condições o campo que você está filtrando deve atender.</p> <p>Esta linha é obrigatória.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Para indicar que o status das tarefas filtradas deve ser igual a Em andamento, use a seguinte linha além da acima:</p> <p><code>status_Mod=in</code> </p> <p>Se o modificador for um intervalo, há duas linhas para indicar o modificador.</p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Exemplo: </b></span></span> 
        <p>Este é um filtro de modo de texto que procura tarefas que estão em andamento, que têm uma Data de Conclusão Planejada no mês atual e são atribuídas a um usuário com um GUID específico:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Para obter uma lista completa dos modificadores de filtro no modo de texto, consulte o artigo <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Modificadores de filtro e condição</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Operador de instrução. Por padrão, cada instrução de filtro é conectada pelo operador "AND". Isso não é exibido na interface do modo de texto. Também é possível adicionar um operador "OU" entre duas instruções para indicar que você deseja filtrar por objetos que podem atender uma ou outra de duas condições.</p> <p>Os operadores de filtro são necessários apenas para filtros que têm mais de uma instrução.</p> <p>Dica:   
        <ul> 
         <li> <p>"OR" diferencia maiúsculas de minúsculas e deve sempre estar em maiúsculas.</p> </li> 
         <li> <p>Quando você altera seu operador de AND para OR, o número de itens da lista pode aumentar.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Exemplo: </b></span></span> 
        <p>Para filtrar tarefas em um status Em andamento ou com uma Data de Conclusão Planejada de Hoje, use o seguinte: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Um curinga que permite generalizar as informações em um filtro e fazer referência à hora atual ou ao usuário que está conectado.</p> <p>Os curingas são opcionais.</p> <p>Dica:   <p>Recomendamos usar curingas sempre que possível para tornar seus filtros mais dinâmicos e não duplicar os mesmos filtros para cada usuário ou intervalos de tempo semelhantes.</p> <p>Para obter informações sobre curingas de filtro, consulte <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Variáveis de filtro curinga</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Exemplo: </b></span></span> 
        <p>Para filtrar tarefas atribuídas ao usuário que está conectado no momento, use o seguinte:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Para adicionar uma instrução de filtro conectada pelo operador &quot;OU&quot;, faça o seguinte:

   1. Adicione uma nova linha de código e digite OR:1: seguido pelo objeto ou atributo com o qual você deseja filtrar e pelo valor com o qual deseja compará-lo. Para fazer referência a tarefas que estão em qualquer status, exceto Novo, use a seguinte linha:

      ```
      OR:1:status=NEW
      ```

   1. Adicione uma segunda linha e digite OR:1: seguido pelo objeto, pelo modificador e pelo código do modificador. Para definir o modificador para a linha de código que faz referência a todos os status da tarefa, exceto para Novo, use a seguinte linha do modificador:

      ```
      OR:1:status_Mod=notin
      ```

      Cada linha da nova declaração deve ser precedida por &quot;OR:`<number>`:&quot;.

      Para obter informações sobre como criar instruções &quot;OR&quot; em um filtro, consulte [Criar instruções &quot;OU&quot; em filtros de modo de texto](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>Você pode ter várias instruções &quot;OU&quot; no mesmo filtro. Toda vez que você tem uma nova declaração &quot;OU&quot;, o número depois de &quot;OU:&quot; aumenta.
Para filtrar as tarefas que estão em um status Em andamento ou que estão atribuídas ao usuário conectado ou que têm a Data de conclusão planejada hoje, use o seguinte:
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. Clique em **Concluído** se quiser salvar suas alterações e continuar editando o relatório ou o filtro.
1. Clique em **Salvar + Fechar** para salvar seu relatório ou **Salvar filtro** para salvar o filtro na lista.
