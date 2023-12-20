---
product-area: reporting
navigation-topic: text-mode-reporting
title: Modo de edição de texto em um agrupamento
description: "NOTA: faça com que todos os artigos FVG sejam os mesmos para edição no modo texto)"
author: Nolan
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Modo de edição de texto em um agrupamento

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: make all FVG articles the same for editing in text mode)</p>
-->

É possível editar um agrupamento em uma lista ou relatório usando o modo de texto para acessar campos que não estão disponíveis na interface padrão e criar agrupamentos mais complexos.

>[!TIP]
>
>Recomendamos que você crie o máximo possível do agrupamento no modo padrão e, em seguida, converta-o para o modo de texto para editá-lo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para editar agrupamentos em um relatório</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar agrupamentos em um relatório</p> <p>Gerenciar permissões em um agrupamento para editá-lo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisitos

Antes de começar a usar o modo de texto em um relatório ou lista, sempre verifique se você está familiarizado com a sintaxe do modo de texto do Workfront.

Para obter mais informações, consulte:

* [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exibição personalizada, filtro e amostras de agrupamento: índice do artigo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Modo de edição de texto em um agrupamento

A edição de um agrupamento usando o modo texto é idêntica para relatórios e listas. O acesso ao agrupamento a partir de um relatório ou de uma lista é diferente.

>[!NOTE]
>
>Os agrupamentos são um elemento de relatório obrigatório para a criação de gráficos em relatórios. Os agrupamentos em modo de texto não são suportados em gráficos. Para obter informações sobre como adicionar gráficos aos relatórios, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Para obter mais informações sobre a criação de agrupamentos, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Siga um destes procedimentos:

   1. Para acessar o agrupamento em um relatório, vá para o relatório e clique em **Ações de Relatório** > **Editar** > **Agrupamentos** guia.
   1. Para acessar o agrupamento por uma lista, vá para a lista e no **Agrupamento** menu suspenso, passe o mouse sobre o agrupamento que deseja modificar e clique no **Editar** ícone ![](assets/edit-icon.png).

      O construtor de agrupamento é aberto.

1. Clique em **Adicionar Agrupamento** para adicionar os agrupamentos, clique em **Alternar para modo de texto** no canto superior direito do construtor.

   >[!TIP]
   >
   Você pode adicionar até 3 agrupamentos na interface padrão. Você pode adicionar um quarto agrupamento usando apenas o modo de texto e não pode ter mais de quatro níveis de agrupamento no Workfront.

1. Comece digitando o nome de um campo pelo qual deseja agrupar.

   Selecione o nome do campo ao visualizá-lo na lista.

1. Clique em **Alternar para modo de texto** no canto superior direito do construtor.

   O agrupamento é exibido no modo de texto.

   Ao editar um agrupamento no modo texto, o Workfront adiciona a variável

   ```
   textmode=true
   ```

   linha de código ao agrupamento. Isso indica que o agrupamento é modificado no modo de texto.

   **Exemplo:** Para agrupar uma lista de tarefas pelo Nome do projeto e, em seguida, pelo nome do Destinatário principal, seu agrupamento deve ser semelhante ao seguinte, no modo de texto.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   As linhas em negrito são obrigatórias.

   <!--
   <div class="example" data-mc-autonum="<b>Example: </b>" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <span class="autonumber"><span><b>Example: </b></span></span>
   <p>To group a list of tasks by the Project Name and then by the name of the Primary Assignee, your grouping should look like the following, in text mode:</p>
   <p><code>textmode=true</code> </p>
   <p><code>group.0.linkedname=project</code> </p>
   <p><code>group.0.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.0.valuefield=project:name</code> </p>
   <p><code>group.0.namekeyargkey.0=project</code> </p>
   <p><code>group.0.namekeyargkey.1=name</code> </p>
   <p><code style="font-weight: bold;">group.0.valueformat=string</code> </p>
   <p><code>group.1.linkedname=assignedTo</code> </p>
   <p><code>group.1.namekey=view.relatedcolumn</code> </p>
   <p><code style="font-weight: bold;">group.1.valuefield=assignedTo:name</code> </p>
   <p><code>group.1.namekeyargkey.0=assignedTo</code> </p>
   <p><code>group.1.namekeyargkey.1=nam</code>e</p>
   <p><code style="font-weight: bold;">group.1.valueformat=string</code> </p> <note type="important">
   The lines in bold are mandatory.
   </note>
   </div>
   -->

   Cada campo no agrupamento tem várias linhas de código que se referem a esse campo.

   A tabela abaixo descreve as linhas principais em um agrupamento de modo de texto.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   As linhas-chave em um agrupamento em modo de texto são semelhantes às linhas necessárias para construir visualizações em modo de texto.

   <!--
   <note type="tip">  
   <p>The key lines in a text mode grouping are similar to the lines required to build text-mode views.</p>
   </note>
   -->

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
      <td><strong>grupo.&lt;number&gt;.</strong> </td> 
      <td> <p>Cada linha de código é precedida por este texto. As linhas de código que se referem ao mesmo campo selecionado no agrupamento são numeradas com o mesmo número, da seguinte maneira:</p> 
       <ul> 
        <li>O primeiro agrupamento do relatório tem um número de grupo de 0. Todas as linhas referentes ao primeiro agrupamento começam com <code>group.0</code>.</li> 
        <li>O segundo agrupamento do relatório tem um número de grupo de 1. Todas as linhas que fazem referência ao segundo agrupamento começam com <em><code>group.1</code></em>.</li> 
        <li>O terceiro agrupamento do relatório tem um número de grupo de 2. Todas as linhas que fazem referência ao terceiro agrupamento começam com <em><code>group.2</code></em>.</li> 
        <li>Somente no modo de texto é possível adicionar um número de grupo de 3, para um quarto agrupamento. Todas as linhas que fazem referência ao quarto agrupamento começam com <em><code>group.3</code></em>.</li> 
       </ul> <p>Observação: 4 agrupamentos não são permitidos no construtor. Elas só são compatíveis quando o modo de texto é usado. O Workfront não oferece suporte a mais de quatro níveis de agrupamentos.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>campo de valor</strong>=</p> </td> 
      <td> <p>Esse é o nome do objeto ou do campo como ele aparece no banco de dados. Para obter mais informações sobre como os objetos e campos aparecem no banco de dados, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Existem os seguintes cenários:</p> 
       <ol> 
        <li value="1"> <p> Se o nome do campo exibido for uma frase em vez de um único substantivo, você deverá usar a sintaxe de camel case para <code>valuefield</code>. Por exemplo, para a Data de início planejada de uma tarefa, o código é:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Se quiser exibir um campo personalizado, a variável <code>valuefield</code> value é o nome real do campo, como você o vê na interface. Por exemplo, para um campo personalizado chamado "Mais informações", o código é:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Se você quiser agrupar por objetos que estão relacionados a outros objetos usando o <code>valuefield</code> linha de código os nomes e atributos do objeto são separados por dois pontos.</p> <p>Por exemplo, um agrupamento por Nome de Portfolio para uma lista de tarefas tem o seguinte valor para a linha do campo de valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Isso indica que, a partir do objeto do relatório (tarefa), você pode acessar o próximo objeto relacionado (projeto); a partir daí, você pode acessar o seguinte objeto relacionado a partir do projeto (portfólio); em seguida, o nome do portfólio (nome).</p> </li> 
       </ol> <p>Para obter informações sobre como os objetos se conectam entre si, consulte a seção <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependência e hierarquia de objetos</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Entender objetos no Adobe Workfront</a>.</p> <p>Nota: Se você escolher um campo no modo texto que não seja válido na interface padrão e alternar para a interface padrão, o agrupamento será deletado.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>value format=</strong> </td> 
      <td> <p>Esta linha representa o formato usado para exibir o <code>valuefield</code>. A variável <code>valueformat</code> identifica se um objeto ou campo é exibido como texto, número, porcentagem ou data.</p> <p>Recomendamos usar <code>HTML</code> para seu <code>valueformat</code>, especialmente ao usar <code>valueexpression</code>, para garantir a exibição mais precisa de suas informações.</p> <p>Para obter informações sobre valores adicionais para essa linha, consulte <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Usar formatação condicional no Modo de texto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>expressão de valor=</strong> </p> </td> 
      <td> <p>É possível adicionar esta linha para substituir <code>valuefield</code>, se quiser agrupar sua lista por um cálculo entre vários campos.</p> <p>Você deve incluir o <code>valuefield</code> dos objetos entre chaves sempre que você usá-los em uma <code>valueexpression</code>.</p> <p>Existem os seguintes cenários:</p> 
       <ol> 
        <li value="1"> <p>Se quiser exibir o nome de um agrupamento em maiúsculas, use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>A variável <code>valuefield</code> do objeto é digitado como aparece no API Explorer.</p> </li> 
        <li value="2">Se quiser adicionar vários <code>valuefields</code> unindo-os em uma <code>valueexpression </code>deve separá-los por um ponto.<p>Por exemplo, se você quiser exibir o nome do portfólio em maiúsculas em uma lista de tarefas, use o seguinte código na caixa <code>valueexpression</code> linha:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Se quiser usar um campo personalizado em um <code>valueexpression</code> linha pela qual você deve preceder o nome do campo <code>DE:</code> para indicar que é um campo personalizado. O nome do campo é grafado conforme aparece na interface.</p><p>Importante: <span>Quando você usa um campo personalizado colocado em uma seção de formulário personalizado que tem permissões restritas para alguns usuários, o cálculo do <code>valueexpression </code>fica em branco quando esses usuários exibem esse cálculo em um relatório. Para obter informações sobre como ajustar permissões em seções de formulário personalizadas, consulte</span> <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a></span>.</p><p>Por exemplo, se você tiver um campo personalizado chamado "Nome do desenvolvedor" e quiser agrupar por esse campo e exibi-lo em maiúsculas, poderá usar o seguinte <code>valueexpression</code> para indicar isso:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Ao fazer referência a um campo personalizado do tipo Digitação antecipada, use a seguinte expressão para fazer referência ao nome do objeto selecionado em um campo rotulado como "Nome do desenvolvedor":</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Esta linha define o rótulo de agrupamento. Nesse caso, ele está usando o valor abreviado com base na chave.</p> <p>Se quiser modificar o nome do agrupamento, você poderá alterar esse valor para o seguinte:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> permite inserir qualquer texto para o nome do agrupamento, enquanto <code>namekey</code> requer que você insira uma chave que seja usada para traduzir o nome de um agrupamento.</p> <p>Para alterar o nome do agrupamento, você também pode adicionar a variável <code>displayname </code>linha, se uma não estiver presente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Você pode adicionar a seguinte linha para alterar o nome de uma coluna, o que substitui a <code>namekey/name</code> valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Recomendamos remover todas as linhas que contêm <code>name </code>ao renomear um agrupamento.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Adicione uma das seguintes linhas de código a qualquer agrupamento para indicar se os resultados do agrupamento devem ser exibidos em uma lista expandida ou recolhida. Por padrão, os agrupamentos são exibidos expandidos:


   ```
   group.0.iscollapsed=true
   ```

   se desejar que o agrupamento seja exibido com os resultados recolhidos

   ```
   group.0.iscollapsed=false
   ```

   se desejar que o agrupamento seja exibido com os resultados expandidos

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   * Quando você ajusta agrupamentos manualmente ao visualizar uma lista, o Workfront lembra de sua preferência manual até que você faça logout. Ao fazer logon novamente, a lista é exibida de acordo com essa configuração.
   * Os resultados de um agrupamento sempre são exibidos expandidos depois de acessados de um elemento do gráfico.

1. Clique em **Concluído** se desejar salvar suas alterações e continuar editando o agrupamento ou relatório.
1. Clique em **Salvar Agrupamento** em uma lista ou **Salvar + Fechar** para salvar seu relatório.
