---
product-area: reporting
navigation-topic: text-mode-reporting
title: Editar um agrupamento usando o modo texto
description: Você pode editar um agrupamento em uma lista ou relatório usando o modo de texto para acessar campos que não estão disponíveis na interface padrão e criar agrupamentos mais complexos.
author: Courtney
feature: Reports and Dashboards
exl-id: 2eeecc16-ea6d-4a56-8ea3-e213706e89bf
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 5%

---

# Editar um agrupamento usando o modo texto

<!-- Audited: 1/2025 -->

Você pode editar um agrupamento em uma lista ou relatório usando o modo de texto para acessar campos que não estão disponíveis na interface padrão e criar agrupamentos mais complexos.

>[!TIP]
>
>Recomendamos que você crie o máximo possível do agrupamento no modo padrão e, em seguida, converta-o no modo de texto para editá-lo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
     <p>Padrão</p>
     <p>Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a filtros, exibições e agrupamentos</p> <p>Acesso de edição a relatórios, painéis e calendários para editar agrupamentos em um relatório</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório editar agrupamentos em um relatório</p> <p>Gerenciar permissões para um agrupamento para editá-lo</p></td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar a usar o modo de texto em um relatório ou lista, sempre verifique se você está familiarizado com a sintaxe do modo de texto do Workfront.

Para obter mais informações, consulte:

* [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Visão geral da sintaxe do modo de texto](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Exemplos de exibição personalizada, filtros e agrupamento: índice do artigo](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Editar um agrupamento usando o modo texto

A edição de um agrupamento usando o modo de texto é idêntica para relatórios e listas. O acesso ao agrupamento a partir de um relatório ou de uma lista é diferente.

>[!NOTE]
>
>Os agrupamentos são um elemento de relatório obrigatório para a criação de gráficos em relatórios. Os agrupamentos do modo de texto não são suportados em gráficos. Para obter informações sobre como adicionar gráficos a relatórios, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

Para obter mais informações sobre como criar agrupamentos, consulte [Criar agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Siga um destes procedimentos:

   1. Para acessar o agrupamento de um relatório, vá para o relatório e clique em **Ações de Relatório** > **Editar** > guia **Agrupamentos**.
   1. Para acessar o agrupamento de uma lista, vá para a lista e, no menu suspenso **Agrupamento**, passe o mouse sobre o agrupamento que você deseja modificar e clique no ícone **Editar** ![Ícone Editar](assets/edit-icon.png).

      O construtor de agrupamento é aberto.

1. Clique em **Adicionar agrupamento** para adicionar os agrupamentos, clique em **Alternar para modo de texto** no canto superior direito do construtor e em **Editar modo de texto**.

   >[!TIP]
   >
   >Você pode adicionar até 3 agrupamentos na interface padrão. Você pode adicionar um quarto agrupamento usando apenas o modo de texto e não pode ter mais de quatro níveis de agrupamento no Workfront.

1. Comece a digitar o nome de um campo pelo qual deseja agrupar.

   Selecione o nome do campo quando ele aparecer na lista.

1. Clique em **Alternar para o modo de texto** no canto superior direito do construtor.

   O agrupamento é exibido no modo de texto.

   Quando você edita um agrupamento no modo de texto, o Workfront adiciona o

   ```
   textmode=true
   ```

   linha de código para o agrupamento. Indica que o agrupamento é modificado no modo de texto.

   **Exemplo:** para agrupar uma lista de tarefas pelo Nome do Projeto e, em seguida, pelo nome do Destinatário Principal, o agrupamento deve ter a seguinte aparência no modo de texto.

   ```
   textmode=true<br>group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br><strong>group.0.valuefield=project:name</strong><br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br><strong>group.0.valueformat=string</strong><br>group.1.linkedname=assignedTo<br>group.1.namekey=view.relatedcolumn<br><strong>group.1.valuefield=assignedTo:name</strong><br>group.1.namekeyargkey.0=assignedTo<br>group.1.namekeyargkey.1=name<br><strong>group.1.valueformat=string</strong>
   ```

   >[!IMPORTANT]
   >
   >As linhas em negrito são obrigatórias.

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

   A tabela abaixo contorna as linhas-chave em um agrupamento de modo de texto.

   <!--
   <div data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <p>(NOTE: Should I add the group.1. information to this table and break the snippet? If yes, delete the snippet)</p>
   <p>(NOTE: this is a snippet, same as view >> same fields >>> see the steps in creating a view and add the same steps here for making a grouping)</p>
   </div>
   -->

   >[!TIP]
   >
   >As linhas-chave em um agrupamento em modo de texto são semelhantes às linhas necessárias para construir visualizações em modo de texto.

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
      <td><strong>grupo.&lt;número&gt;.</strong> </td> 
      <td> <p>Cada linha de código é precedida por este texto. As linhas de código que se referem ao mesmo campo selecionado no agrupamento são numeradas com o mesmo número, da seguinte maneira:</p> 
       <ul> 
        <li>O primeiro agrupamento do relatório tem um número de grupo de 0. Todas as linhas que se referem ao primeiro agrupamento começam com <code>group.0</code>.</li> 
        <li>O segundo agrupamento do relatório tem um número de grupo de 1. Todas as linhas que se referem ao segundo agrupamento começam com <em><code>group.1</code></em>.</li> 
        <li>O terceiro agrupamento do relatório tem um número de grupo de 2. Todas as linhas que se referem ao terceiro agrupamento começam com <em><code>group.2</code></em>.</li> 
        <li>Somente no modo de texto, é possível adicionar um número de grupo de 3 para um quarto agrupamento. Todas as linhas que se referem ao quarto agrupamento começam com <em><code>group.3</code></em>.</li> 
       </ul> <p>Observação: 4 agrupamentos não são suportados no construtor. Eles só são compatíveis ao usar o modo de texto. O Workfront não oferece suporte a mais de 4 níveis de agrupamentos.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>valorcampo</strong>=</p> </td> 
      <td> <p>Este é o nome do objeto ou do campo como aparece no banco de dados. Para obter mais informações sobre como objetos e campos aparecem no banco de dados, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Existem os seguintes cenários:</p> 
       <ol> 
        <li value="1"> <p> Se o nome do campo exibido for uma frase em vez de um único substantivo, você deverá usar a sintaxe de camel case para o <code>valuefield</code>. Por exemplo, para a Data de início planejada de uma tarefa, o código é:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Se você quiser exibir um campo personalizado, o valor <code>valuefield</code> é o nome real do campo, como você o vê na interface. Por exemplo, para um campo personalizado chamado “Mais informações”, o código é:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Se você deseja agrupar por objetos que estão relacionados a outros objetos usando a linha de código <code>valuefield</code>, os nomes e atributos dos objetos são separados por dois-pontos.</p> <p>Por exemplo, um agrupamento por Nome de Portfolio para uma lista de tarefas tem o seguinte valor para a linha do campo de valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valuefield=project:portfolio:name</code> </p> <p>Indica que, a partir do objeto do relatório (tarefa), você pode acessar o próximo objeto relacionado (projeto); a partir daí, você pode acessar o seguinte objeto relacionado a partir do projeto (portfólio); em seguida, o nome do portfólio (nome).</p> </li> 
       </ol> <p>Para obter informações sobre como os objetos se conectam entre si, consulte a seção <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependência e hierarquia de objetos</a> em <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Entender objetos no Adobe Workfront</a>.</p> <p>Nota: Se você escolher um campo no modo de texto que não seja válido na interface padrão e alternar para a interface padrão, o agrupamento será deletado.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>valueformat=</strong> </td> 
      <td> <p>Esta linha representa o formato usado para exibir o <code>valuefield</code>. <code>valueformat</code> identifica se um objeto ou campo é exibido como texto, número, porcentagem ou data.</p> <p>Recomendamos o uso de <code>HTML</code> para <code>valueformat</code>, especialmente ao usar <code>valueexpression</code>, para garantir a exibição mais precisa de suas informações.</p> <p>Para obter informações sobre valores adicionais para esta linha, consulte <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Usar formatação condicional no Modo de Texto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>expressãode valor=</strong> </p> </td> 
      <td> <p>Você pode adicionar esta linha para substituir <code>valuefield</code>, caso queira agrupar sua lista por um cálculo entre vários campos.</p> <p>Você deve colocar <code>valuefield</code> dos objetos entre chaves sempre que usá-los em um <code>valueexpression</code>.</p> <p>Existem os seguintes cenários:</p> 
       <ol> 
        <li value="1"> <p>Para exibir o nome de um agrupamento em maiúsculas, você deve usar:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valueexpression=UPPER({valuefield})</code> </p> <p>O <code>valuefield</code> do objeto está escrito como aparece no API Explorer.</p> </li> 
        <li value="2">Se você quiser adicionar vários <code>valuefields</code> agrupando-os em uma linha <code>valueexpression </code>, separe-os por um ponto.<p>Por exemplo, se você quiser exibir o nome do portfólio em maiúsculas em uma lista de tarefas, você usaria o seguinte código na linha <code>valueexpression</code>:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valueexpression=UPPER({project}.{portfolio}.{name})</code></p><p>Se você quiser usar um campo personalizado em uma linha <code>valueexpression</code>, preceda o nome do campo por <code>DE:</code> para indicar que ele é um campo personalizado. O nome do campo é grafado conforme aparece na interface.</p><p>Importante: <span>Quando você usa um campo personalizado colocado em uma seção de formulário personalizado que tem permissões restritas para alguns usuários, o cálculo de <code>valueexpression </code> fica em branco quando esses usuários exibem esse cálculo em um relatório. Para obter informações sobre como ajustar permissões em seções de formulário personalizadas, consulte</span> <span href="help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md"><a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Criar um formulário personalizado</a></span>.</p><p>Por exemplo, se você tiver um campo personalizado rotulado “Nome do Desenvolvedor” e quiser agrupar por esse campo e exibi-lo em maiúsculas, poderá usar a seguinte <code>valueexpression</code> para indicar isso:</p><p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.valueexpression=UPPER({DE:Developer Name}</code>)</p><p>Ao fazer referência a um campo personalizado do tipo Typeahead, use a seguinte expressão para fazer referência ao nome do objeto selecionado em um campo rotulado como “Nome do desenvolvedor”:</p><p><code>valueexpression=UPPER({DE:Developer Name:name})</code></p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td><strong>chave_nome= / nome=</strong> </td> 
      <td> <p>Esta linha define o rótulo de agrupamento. Nesse caso, ele está usando o valor abreviado com base na chave.</p> <p>Se quiser modificar o nome do agrupamento, você pode alterar esse valor para o seguinte:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.name=Your Value</code> </p> <p><code>Name</code> permite inserir qualquer texto para o nome do agrupamento, enquanto <code>namekey</code> exige a inserção de uma chave usada para traduzir o nome de um agrupamento.</p> <p>Para alterar o nome do agrupamento, você também pode adicionar a linha <code>displayname </code>, se não houver uma.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>nome_de_exibição =</strong> </td> 
      <td> <p>Você pode adicionar a seguinte linha para alterar o nome de uma coluna, o que substitui o valor <code>namekey/name</code>:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>group.0.displayname=Your Value</code> </p> <p>Recomendamos remover todas as linhas que contêm <code>name </code> ao renomear um agrupamento.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Adicione uma das seguintes linhas de código a qualquer agrupamento para indicar se os resultados do agrupamento devem ser exibidos em uma lista expandida ou recolhida. Por padrão, os agrupamentos são exibidos expandidos:


   ```
   group.0.iscollapsed=true
   ```

   se quiser que o agrupamento seja exibido com os resultados recolhidos

   ```
   group.0.iscollapsed=false
   ```

   se quiser que o agrupamento seja exibido com os resultados expandidos

   <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Common uses of text mode, Edit groupings to organize reports, Create a Custom Report) </p>   
     -->

   >[!TIP]
   >   
   >* Quando você ajusta os agrupamentos manualmente ao exibir uma lista, o Workfront se lembra de sua preferência manual até que você faça logoff. Ao efetuar logon novamente, a lista é exibida de acordo com essa configuração.
   >* Os resultados de um agrupamento sempre são exibidos expandidos após acessá-los a partir de um elemento de gráfico.

1. Clique em **Concluído** se você deseja salvar suas alterações e continuar editando o agrupamento ou relatório.
1. Clique em **Salvar Agrupamento** em uma lista ou em **Salvar + Fechar** para salvar seu relatório.
