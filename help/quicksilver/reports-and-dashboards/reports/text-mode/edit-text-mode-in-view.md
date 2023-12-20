---
product-area: reporting
navigation-topic: text-mode-reporting
title: Editar uma visualização usando o modo de texto
description: "OBSERVAÇÃO: adicione uma seção a este artigo: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Além disso, faça um rascunho desta área no artigo de visão geral do Modo de texto)"
author: Nolan
feature: Reports and Dashboards
exl-id: b99a2d14-a226-4075-9b1b-ac9426fd41b8
source-git-commit: dad054fe52bd7c5ca97144567c80e6d340541a50
workflow-type: tm+mt
source-wordcount: '1639'
ht-degree: 0%

---

# Editar uma visualização usando o modo de texto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-views.html *** Also, draft this area in the Text Mode overview article) </p>
-->

É possível editar uma visualização em uma lista ou relatório usando o modo de texto para acessar campos que não estão disponíveis na interface padrão e criar visualizações mais complexas.

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
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a relatórios, painéis e calendários para editar elementos de relatórios em um relatório</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar exibições em um relatório</p> <p>Gerenciar permissões em uma exibição para editá-la</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
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

## Modo de edição de texto em uma visualização

A edição de uma visualização usando o modo de texto é idêntica para relatórios e listas. O acesso à visualização de um relatório ou de uma lista é diferente.

>[!TIP]
>
>Recomendamos que você crie o máximo possível da exibição no modo padrão e, em seguida, converta-a para o modo de texto para editá-la.

Para obter informações sobre a criação de exibições, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Para obter informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Siga um destes procedimentos:

   1. Para acessar a exibição de um relatório, vá para o relatório e clique em **Ações de Relatório** > **Editar** > **Colunas (Exibir)** guia.
   1. Para acessar a visualização em uma lista, vá para a lista e no **Exibir** menu suspenso, passe o mouse sobre a exibição que deseja modificar e clique no **Editar** ícone ![](assets/edit-icon.png).

      O construtor de exibições é aberto.

1. Selecione uma coluna na exibição.

   Ou

   Selecione o **Colunas (Exibir)** do report builder e, em seguida, selecione uma coluna.

   >[!TIP]
   >
   >Para editar uma visualização usando o modo texto, é necessário editar uma coluna de cada vez.

1. Clique em **Alternar para modo de texto** no canto superior direito do construtor.

   >[!NOTE]
   >
   >Ao editar uma coluna no modo texto, o Workfront adiciona a variável `textmode=true` linha de código para a coluna. Isso indica que a coluna é modificada no modo de texto.

   ![](assets/switch-to-text-mode-in-view-nwe-highlighted-350x447.png)

   A tabela a seguir descreve as linhas-chave em uma exibição de modo de texto:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make this a snippet and add it to the grouping article too)</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Linha de Exemplo</th> 
      <th>Descrição</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>campo de valor</strong>=</p> </td> 
      <td> <p>Esse é o nome do objeto ou do campo como ele aparece no banco de dados. Para obter mais informações sobre como os objetos e campos aparecem no banco de dados, consulte <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API Explorer</a>.</p> <p>Existem os seguintes cenários:</p> 
       <ol> 
        <li value="1"> <p> Se o nome do campo exibido for uma frase em vez de um único substantivo, você deverá usar a sintaxe de camel case para <code>valuefield</code>. Por exemplo, para a Data de início planejada de uma tarefa, o código é: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>valuefield=plannedStartDate</code> </p> </li> 
        <li value="2"> <p>Se quiser exibir um campo personalizado, a variável <code>valuefield</code> value é o nome real do campo, como você o vê na interface. Por exemplo, para um campo personalizado chamado "Mais informações", o código é:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>valuefield=More information</code> </p> </li> 
        <li value="3"> <p>Se quiser exibir objetos relacionados a outros objetos em uma view usando o <code>valuefield</code> linha de código os nomes e atributos do objeto são separados por dois pontos. </p> <p>Por exemplo, uma coluna em uma visualização de tarefa que exibiria o nome do Proprietário do Portfolio tem o seguinte valor para a linha do campo de valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>valuefield=project:portfolio:owner:name</code> </p> <p>Isso indica que, do objeto do relatório (tarefa), você pode acessar o próximo objeto relacionado (projeto), a partir daí, você pode acessar o seguinte objeto relacionado do projeto (portfólio), em seguida, o proprietário do portfólio (proprietário) e seu nome (nome). </p> </li> 
       </ol> <p>Para obter informações sobre como os objetos se conectam entre si, consulte a seção <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects" class="MCXref xref">Interdependência e hierarquia de objetos</a> in <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Entender objetos no Adobe Workfront</a>.</p> <p>Observação: Se você escolher um campo no modo de texto que não seja válido na interface padrão, não será possível voltar para a interface padrão na coluna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>value format=</strong> </td> 
      <td> <p>Esta linha representa o formato usado para exibir o <code>valuefield</code>. A variável <code>valueformat</code> identifica se um objeto ou campo é exibido como texto, número, porcentagem ou data.</p> <p>Recomendamos usar <code>HTML</code> para seu <code>valueformat</code>, especialmente ao usar <code>valueexpression</code>, para garantir a exibição mais precisa de suas informações. </p> <p>Para obter informações sobre valores adicionais para essa linha, consulte <a href="../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md" class="MCXref xref">Usar formatação condicional no Modo de texto</a>.</p> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>expressão de valor=</strong> </p> </td> 
      <td> <p>É possível adicionar esta linha para substituir <code>valuefield</code>, se desejar exibir um campo calculado na coluna.</p> <p>Você deve incluir o <code>valuefield</code> dos objetos entre chaves sempre que você usá-los em uma <code>valueexpression</code>.</p> <p>Existem os seguintes cenários: </p> 
       <ol> 
        <li value="1"> <p>Se quiser exibir um campo em uma coluna em maiúsculas, use:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>valueexpression=UPPER({valuefield})</code> </p> <p>A variável <code>valuefield</code> do objeto é digitado como aparece no API Explorer. </p> </li> 
        <li value="2">Se quiser adicionar vários <code>valuefields</code> ao uni-los, você deve separá-los por um ponto.</li> 
        <li value="3"> <p>Por exemplo, se você deseja exibir o nome do Destinatário principal de uma tarefa usando <code>valueexpression</code>, você usaria:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>valueexpreesion={assignedTo}.{name}</code> </p> </li> 
        <li value="4"> <p>Se quiser usar um campo personalizado em um <code>valueexpression</code> linha pela qual você deve preceder o nome do campo <code>DE:</code> para indicar que é um campo personalizado. O nome do campo é grafado conforme aparece na interface. </p> <p>Importante: quando você usa um campo personalizado colocado em uma seção de formulário personalizada que tem permissões restritas para alguns usuários, o cálculo da expressão de valor fica em branco quando esses usuários exibem esse cálculo em um relatório. Para obter informações sobre como ajustar permissões em seções de formulário personalizadas, consulte <span href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md"><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Criar ou editar um formulário personalizado</a></span>.</p> <p>Por exemplo, se você tiver um campo personalizado chamado "Nome do desenvolvedor" e quiser exibir esse campo em maiúsculas em uma coluna, poderá usar o seguinte <code>valueexpression</code> para indicar isso:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>valueexpression=UPPER({DE:Developer Name}</code>) </p> <p>Ao fazer referência a um campo personalizado do tipo Digitação antecipada, use a seguinte expressão para fazer referência ao nome do objeto selecionado em um campo rotulado como "Nome do desenvolvedor":</p> <p><code>valueexpression=UPPER({DE:Developer Name:name})</code> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>descriptionkey= / description=</strong> </p> </td> 
      <td> <p>Essa linha define o texto de uma dica de ferramenta conforme você passa o mouse sobre o nome da coluna. Nesse caso, ele está usando uma chave para traduzir o valor do nome no texto de descrição. Se quiser modificar a descrição, altere esta linha para: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>description=Your Value</code>.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>namekey= / name=</strong> </td> 
      <td> <p>Essa linha define o rótulo da coluna. Nesse caso, ele está usando o valor abreviado com base na chave.</p> <p>Se quiser modificar o nome da coluna, você poderá alterar esse valor para: </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>name=Your Value</code> </p> <p><code>Name</code> permite inserir qualquer texto para o nome da coluna, enquanto<code>namekey</code> requer que você insira uma chave que seja usada para traduzir o nome de uma coluna.</p> <p>Para alterar o nome da coluna, você também pode adicionar a variável <code>displayname </code>linha, se uma não estiver presente.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>displayname =</strong> </td> 
      <td> <p>Você pode adicionar a seguinte linha para alterar o nome de uma coluna, o que suspende a variável <code>namekey/name</code> valor:</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span><code>displayname=Your Value</code> </p> </td> 
     </tr> 
     <tr> 
      <td><strong>querysort=</strong> </td> 
      <td>Essa linha define como os resultados são classificados quando o cabeçalho da coluna é clicado. Se não estiver presente, a coluna não poderá ser classificada após a execução do relatório.</td> 
     </tr> 
     <tr> 
      <td><strong>width=</strong> </td> 
      <td> <p>Essa linha representa o número de pixels usados para a coluna. Se a linha for omitida ou definida como 0 (zero), a coluna não aparecerá na exibição.</p> <p>Ao modificar manualmente esse campo no modo de texto, você também deve adicionar a variável <code>usewidths=true</code> para sua coluna.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>usewidths=true</strong> </td> 
      <td> <p>Você deve usar esta linha além da tag <code>width=</code> linha ao personalizar a largura de uma coluna. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>makeFieldEditable=</strong> </td> 
      <td> <p>Essa linha define se o valor exibido em uma coluna é editável em linha ou não. Se esta linha for igual a <strong>true</strong>, o valor na coluna é editável em linha. Se esta linha for igual a <code>false</code>, o valor na coluna não é editável em linha.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valuefield=</strong> </td> 
      <td> <p>Insira essa linha somente quando quiser que o valor exibido em uma coluna seja vinculado ao objeto associado a ela. O link abre a página de detalhes do objeto. Esse valor deve corresponder ao <code>valuefield=</code> linha. Ao inserir isso, você também deve adicionar a variável <code>link.valueformat=</code> linha. </p> <p> Por exemplo, você pode inserir <code>link.valuefield=priority</code> na visualização de um problema, e a Prioridade do problema é exibida como um link. Clicar nesse link abre a página Problema.</p> </td> 
     </tr> 
     <tr> 
      <td><strong>link.valueformat=</strong> </td> 
      <td> <p>Inserir esta linha somente quando tiver inserido o <code>link.valuefield</code> para adicionar um link ao valor em uma coluna. O link abre a página de detalhes do objeto. Esse valor deve corresponder ao <code>valueformat=</code> e indica o formato usado para exibir a variável <code>valuefield</code>. </p> <p>Importante: ao visualizar o modo de texto em uma coluna interna que também inclui um link, você percebe várias linhas que fazem referência ao link. Algumas dessas linhas podem não ser mais suportadas ou são desnecessárias quando você cria sua própria coluna personalizada no modo de texto e adiciona as instruções de link a ela. As linhas obrigatórias ao adicionar um valor vinculado são<code> link.valuefield</code> e <code>link.valueformat</code>. </p> </td> 
     </tr> 
     <tr> 
      <td><strong>aggregator.function=</strong> </td> 
      <td> <p>Isso se refere à forma como os valores de cada coluna são resumidos. Há várias linhas que começam com <code>aggregator.</code> e todos se referem ao agregador que resume os resultados da coluna. </p> <p>Regra geral, a Comissão <code>aggregator.</code> as linhas correspondem àquelas do objeto de coluna. </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>">
        <span class="autonumber"><span><b>Exemplo: </b></span></span> 
        <p>A coluna Horas planejadas em um relatório de tarefa resumido por Sum pode se parecer com o seguinte: </p> 
        <div>
         <pre>textmode=true</pre>
         <pre>valuefield=workRequired</pre>
         <pre>valueformat=composto</pre>
         <pre>aggregator.function=SUM</pre>
         <pre>aggregator.valuefield=workRequired</pre>
         <pre>aggregator.displayformat=minutesAsHoursString</pre>
         <pre>aggregator.valueformat=compound</pre>
         <pre>namekey=workRequired</pre>
         <pre>shortview=false</pre> 
        </div> 
       </div> 
       <div>
        A variável <code>aggregator. </code>as linhas podem conter um <code>valuefield </code>ou um <code>valueexpression</code>
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Aplicar** se quiser salvar suas alterações e continuar editando a visualização.
1. Clique em **Salvar + Fechar** para salvar seu relatório.

   Ou

   Clique em **Salvar visualização** para salvar a visualização em uma lista.
