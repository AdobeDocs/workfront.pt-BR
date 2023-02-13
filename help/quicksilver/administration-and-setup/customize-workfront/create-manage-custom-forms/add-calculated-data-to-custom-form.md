---
title: Adicionar dados calculados a um formulário personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Em um formulário personalizado, é possível criar um campo personalizado calculado que gera cálculos. Para fazer isso, crie uma declaração que use expressões de dados e nomes de campos existentes, que podem ser campos personalizados, campos de dados personalizados calculados e campos Workfront incorporados. Essa instrução calcula os dados inseridos e exibe o resultado no novo campo personalizado calculado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: e24a0408049e7eb2e7cb97833e7f41ea66e8131b
workflow-type: tm+mt
source-wordcount: '2563'
ht-degree: 0%

---

# Adicionar dados calculados a um formulário personalizado

Em um formulário personalizado, é possível adicionar um campo personalizado calculado que use dados existentes para gerar novos dados quando o formulário personalizado estiver anexado a um objeto.

Um campo personalizado calculado pode conter:

* Uma referência simples a um único campo integrado.

   >[!INFO]
   >
   > **Exemplo:** Para calcular a receita gerada pelos projetos e tarefas, é possível criar um campo personalizado calculado que contenha o campo incorporado Receita real . Quando alguém anexa o formulário personalizado a um projeto ou tarefa, a receita do projeto ou tarefa é exibida no campo .

* Uma expressão que faz referência a um ou mais campos. Esses podem ser campos personalizados, outros campos personalizados calculados e campos incorporados.

   >[!INFO]
   >
   >**Exemplo:** Para calcular o lucro gerado pelos projetos e tarefas, você pode criar um campo personalizado calculado chamado Lucro contendo uma expressão matemática que subtrai o custo da receita.
   >
   >Para fazer isso, você pode usar a expressão matemática SUB (subtrair) com os campos incorporados do Workfront Custo real e Receita real.
   >
   >Nas etapas abaixo, você pode ver como esse exemplo pode ser executado.

Para obter informações sobre como criar formulários personalizados para sua organização e entender o tipo de campos que você pode associar a eles, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plano Adobe Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com o administrador da Workfront.

## Adicionar um campo calculado a um formulário personalizado {#add-a-calculated-field-to-a-custom-form}

Você pode usar campos integrados do Workfront e campos personalizados já criados.

>[!IMPORTANT]
>
>Antes de criar um novo campo personalizado calculado, identifique os campos existentes que deseja incluir para ter certeza de que os dados necessários para o cálculo estão presentes no Workfront.

1. Comece a criar ou editar um formulário personalizado, conforme descrito em [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. No **Adicionar um campo** clique em **Calculado**.

   Na área de exibição à direita, o campo é exibido *12345*. Este é apenas um indicador para lembrá-lo de que o campo é um campo personalizado calculado enquanto você cria ou edita o formulário personalizado. Quando o formulário é anexado a um objeto e os usuários o preenchem, eles veem o resultado do cálculo no campo, nunca a variável *12345* indicador.

1. Especifique as seguintes informações para o campo calculado:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td>Digite um rótulo para o campo. É o que os usuários verão ao usar o formulário personalizado. O campo <b>Nome</b>, que preenche automaticamente, é referenciado pelo Workfront nos relatórios.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instruções</td> 
      <td> Por padrão, a fórmula criada para o campo é armazenada aqui. É possível adicionar texto para fornecer informações adicionais sobre o campo e a fórmula nele. Isso pode ser útil de duas maneiras: 
       <ul> 
        <li> <p>Lembrando o que é a fórmula e como ela funciona. Isso será especialmente útil se você planeja usar esse campo personalizado calculado em vários formulários.</p> </li> 
        <li> <p>Como uma dica de ferramenta, os usuários podem ver quando passam o mouse sobre o campo. Adicione qualquer texto aqui que você deseja que eles vejam na dica de ferramenta.</p> <p>Se você não quiser que eles vejam a fórmula na dica de ferramenta, o que pode ser confuso para eles, você pode ocultá-la. Para obter instruções, consulte a linha da tabela "Exibir fórmula em instruções" na seção <a href="#build-the-calculation-for-your-calculated-custom-field" class="MCXref xref">Criar o cálculo para o seu campo personalizado calculado</a> neste artigo.</p> </li> 
       </ul> <p>Para obter informações sobre como usar o mesmo campo personalizado calculado em um novo formulário, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">Reutilizar um campo personalizado calculado existente em um formulário personalizado</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formatar</td> 
      <td> <p>O formato no qual você deseja que os resultados do campo sejam armazenados e exibidos.</p> <p>Se o campo for usado em cálculos matemáticos, sempre use um <strong>Número</strong> ou <strong>Moeda</strong> formato. Quando você seleciona Número ou Moeda, o sistema trunca automaticamente os números que começam com 0.</p> 
      <p><b>IMPORTANTE</b>: Antes de escolher um formato, considere o formato correto para o novo campo. O campo de formato não pode ser editado depois que o formulário personalizado é salvo. E a seleção do formato incorreto pode afetar cálculos futuros e valores agregados em agrupamentos de relatório e lista.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Continue para [Criar o cálculo para o seu campo personalizado calculado](#build-the-calculation-for-your-calculated-custom-field) neste artigo.

## Criar o cálculo para o seu campo personalizado calculado {#build-the-calculation-for-your-calculated-custom-field}

1. Comece a criar o campo personalizado calculado, conforme explicado na seção [Adicionar um campo calculado a um formulário personalizado](#add-a-calculated-field-to-a-custom-form) neste artigo.

1. Clique em **Maximizar** para abrir o **Editor de cálculos** e crie o cálculo.

   >[!INFO]
   >
   >**Exemplo:** Usando o exemplo na introdução a este artigo, você pode criar um campo personalizado calculado chamado Lucro em um formulário personalizado para projetos e tarefas. Este campo pode conter um cálculo que exibe a diferença entre Receita Real e Custo Real:
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >Neste exemplo, `SUB` é a expressão e os campos referenciados são `actualRevenue` e `actualCost`.

   Um cálculo geralmente começa com uma expressão, seguida de parênteses contendo os campos que você deseja referenciar quando o formulário personalizado é anexado a um objeto. Para obter informações sobre as expressões disponíveis, consulte [Expressões de dados calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   Cada campo deve estar rodeado de chaves, conforme explicado na seção [Sintaxe necessária nos campos personalizados calculados](#syntax-required-in-calculated-custom-fields) neste artigo. Ao começar a digitar o nome de um campo, o sistema faz sugestões e você pode selecionar uma para inseri-lo no cálculo.

   É possível fazer referência a qualquer tipo de campo personalizado em um cálculo, exceto por dois: Campo de texto com tipo de formatação e Texto descritivo. Para obter informações sobre os tipos de campos personalizados, consulte [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)

1. Clique em na caixa de texto grande e, em seguida, clique em **Expressões** e **Campos** que estão disponíveis para adicioná-las ao cálculo.

   Você também pode começar a digitar uma expressão ou um campo na caixa de texto grande e, em seguida, selecioná-lo quando for exibido. Cada item é exibido com um &quot;F&quot; para campo ou um &quot;E&quot; para expressão.

   Se você digitar um parêntese de abertura, o parênteses de fechamento será adicionado automaticamente.

   >[!TIP]
   >
   >Você pode fazer qualquer um dos seguintes procedimentos para obter ajuda com o cálculo:
   > 
   >* Passe o mouse sobre uma expressão no cálculo para ver uma descrição, um exemplo mostrando como ela pode ser usada e um link &quot;Saiba mais&quot; para obter mais informações no artigo [Expressões de dados calculadas](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
   >* Use a codificação de cores para identificar os componentes adicionados. As expressões são exibidas em azul e os campos são exibidos em verde.
      >  ![](assets/colors-fields-expressions.jpg)
   >* Encontre erros de cálculo, destacados em rosa, em seguida. Você pode passar o mouse sobre um erro destacado para exibir uma breve descrição da causa.
      >  ![](assets/error-help.png)
   >* Na área abaixo do cálculo, visualize os resultados em um objeto Workfront existente.

   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* Faça referência a expressões em um cálculo longo usando os números de linha exibidos à esquerda.


1. Clique em **Minimizar** quando você terminar de criar o cálculo para o campo personalizado calculado.

   >[!NOTE]
   >
   >Na área de exibição à direita, o campo é exibido *12345.* Este é apenas um indicador para lembrá-lo de que o campo é um campo personalizado calculado enquanto você cria ou edita o formulário personalizado. Quando o formulário é anexado a um objeto e os usuários o preenchem, eles veem o resultado do cálculo no campo, nunca a variável *12345* indicador.

1. (Opcional) Use qualquer uma das seguintes opções para configurar ainda mais o campo personalizado calculado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Adicionar Lógica</td> 
      <td>Você pode adicionar Lógica de exibição para determinar se o campo calculado é exibido, com base em pelo menos uma opção que um usuário faz em um campo de escolha múltipla anterior (Suspensão, Caixas de seleção ou Botões de opção) ao preencher o formulário. Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Adicionar lógica de exibição e ignorar lógica a um formulário personalizado</a>. <p>Isso só estará disponível quando pelo menos uma caixa de seleção, um botão de opção ou um campo suspenso preceder o campo personalizado calculado no formulário. </p> <p>A opção Ignorar lógica não está disponível para campos personalizados calculados.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atualizar cálculos anteriores</td> 
      <td>Ao editar um campo personalizado calculado existente, é possível selecionar essa opção para acionar uma atualização no cálculo ao salvar o formulário personalizado. Isso acontece somente uma vez quando o formulário personalizado é salvo. A opção retornará ao estado desativado depois de fazer isso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir a fórmula nas instruções</td> 
      <td>Deixe essa opção habilitada se desejar que os usuários que preencherem o formulário personalizado vejam a fórmula do campo quando passarem o mouse sobre ele. Para obter mais informações, consulte as informações sobre <a href="#instructions" class="MCXref xref">Instruções</a> anteriormente nesta tabela.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Concluído** quando todas as alterações forem concluídas no campo personalizado calculado.

   Ou, clique em **Aplicar** para aplicar as alterações no formulário, se desejar continuar adicionando campos personalizados ao formulário.

   Ou, clique em **Salvar + Fechar** quando todas as alterações forem concluídas no formulário personalizado.
1. Para verificar se o campo personalizado calculado funciona corretamente, anexe o formulário personalizado a um objeto e, em seguida, revise o resultado no campo personalizado calculado.

   Para obter instruções sobre como anexar um formulário personalizado, consulte [Adicionar um formulário personalizado a um objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Se quiser continuar criando seu formulário personalizado de outras maneiras, continue para um dos seguintes artigos:

   * [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Posicionar campos e widgets personalizados em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Reutilizar um campo personalizado calculado existente em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Adicionar lógica de exibição e ignorar lógica a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Visualizar e preencher um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Sintaxe necessária nos campos personalizados calculados

Cada campo deve usar a sintaxe explicada abaixo, com colchetes ao redor de cada nome de campo. Ao começar a digitar o nome de um campo, o sistema faz sugestões e você pode selecionar uma para inseri-lo no cálculo. Se você inserir dados em um cálculo incorretamente, uma mensagem de aviso o alertará. Não é possível salvar o formulário a menos que você edite o cálculo para conter campos válidos e uma expressão calculada válida.

>[!NOTE]
>
>Atualmente, o sistema faz sugestões apenas quando você começa a digitar o nome de um campo que deseja referenciar em um objeto ao qual o formulário personalizado será anexado, não no pai do objeto.

### Marque nomes de campos com chaves

* Se você quiser que o cálculo faça referência a um campo incorporado, o nome do campo deverá estar rodeado por colchetes.

Por exemplo: `{actualRevenue}`

Os nomes de campos fazem distinção entre maiúsculas e minúsculas e devem aparecer no cálculo exatamente como aparecem no sistema Workfront.

* Se desejar que o cálculo faça referência a um campo personalizado, o nome do campo deve estar rodeado por colchetes e precedido por `DE:` entre parênteses.

Por exemplo: `{DE:Profit}`

O sistema lista todos os campos personalizados que você pode escolher ao digitar `DE:`.

* Se desejar que o cálculo faça referência a um campo que extrairá dados do *parent* quando o formulário personalizado estiver anexado a um objeto, será necessário preceder o nome do campo ao tipo de objeto do objeto pai, também entre colchetes.

   Por exemplo, se o formulário personalizado estiver configurado para funcionar com tarefas e você quiser que o campo calcule a receita real do objeto pai quando o formulário estiver anexado a uma tarefa, será necessário indicar `Project` como o tipo de objeto do campo:

   `{project}.{actualRevenue}`

   Ou, se for um campo personalizado:

   `{project}.{DE:profit}`

   Se você não tiver certeza de qual será o tipo de objeto do objeto pai, pois o objeto personalizado para está configurado para vários tipos de objeto, poderá usar a variável de filtro curinga `$$OBJCODE` para permitir que o cálculo funcione para cada um dos tipos possíveis. Para obter mais informações, consulte [Campos personalizados calculados em formulários personalizados com vários objetos](#calculated-custom-fields-in-multi-object-custom-forms) neste artigo.

### Separar itens com pontos

Quando você faz referência a um objeto relacionado em um campo personalizado calculado, é necessário separar os nomes e os atributos do objeto por períodos.

Por exemplo, em um formulário personalizado do tipo tarefa, para exibir o nome do Proprietário do Portfolio em um campo personalizado calculado, digite o seguinte:

`{project}.{porfolio}.{owner}`

Isso determinaria o seguinte: No objeto do formulário personalizado (uma tarefa), é possível acessar o próximo objeto relacionado à tarefa (um projeto). A partir daí, você pode acessar o próximo objeto relacionado do projeto (um portfólio) e, em seguida, o próximo objeto relacionado do portfólio (o proprietário).

### Sintaxe de nome para referência a um campo personalizado

Ao fazer referência a outro campo personalizado em um campo personalizado calculado, é necessário inserir o nome do campo como ele é exibido na interface do usuário do Workfront.

Por exemplo, para fazer referência à opção selecionada em um campo personalizado chamado Patrocinador executivo, digite o seguinte:

`{DE:Executive sponsor}`

>[!NOTE]
>
>A sintaxe de um campo typeforward é um pouco diferente de outros tipos de campos, pois é necessário adicionar `:name` no final.
>
>Por exemplo, para fazer referência à opção selecionada em um campo de tipo personalizado com o nome &quot;Patrocinador executivo&quot;, você digitaria:
>
>`{DE:Executive sponsor:name}`


## Campos personalizados calculados em formulários personalizados com vários objetos {#calculated-custom-fields-in-multi-object-custom-forms}

Em um formulário personalizado com vários objetos, os tipos de objetos selecionados devem ser compatíveis com todos os campos referenciados nos campos personalizados calculados do formulário. Se houver uma incompatibilidade, uma mensagem alertará você para fazer ajustes.

>[!INFO]
>
>**Exemplo:**
>
>Em um formulário personalizado configurado para funcionar com o tipo de objeto Tarefa, você cria um campo personalizado calculado chamado Em encargo. Você o configura para fazer referência ao campo incorporado, de modo que ele possa mostrar o nome do destinatário principal em questão sempre que o formulário for anexado a uma tarefa:
>
>`{assignedTo}.{name}`
>
>Posteriormente, é possível adicionar o tipo de objeto Project ao formulário personalizado. Uma mensagem de aviso informa que o tipo de objeto Projeto é incompatível com o campo personalizado calculado.

Quando isso ocorrer, você poderá executar um dos seguintes procedimentos:

* Remova um dos dois itens incompatíveis do formulário personalizado, seja o tipo de objeto ou o campo personalizado calculado referenciado.
* Manter ambos os itens e usar a variável de filtro curinga `$$OBJCODE` como uma condição em uma expressão IF para criar duas versões diferentes do campo In Charge . Isso permite que o campo funcione com êxito, independentemente do tipo de objeto ao qual o formulário está anexado.

>[!INFO]
>
>**Exemplo:** Embora não haja Atribuído a: Nome nos projetos, há um campo Proprietário incorporado (que preenche automaticamente com o nome da pessoa que criou o projeto, a menos que alguém altere isso manualmente).
>
>Portanto, em seu campo Personalizado Em Encargo , você pode usar `$$OBJCODE` conforme mostrado abaixo para fazer referência ao campo Proprietário quando o formulário personalizado está anexado a um projeto e o campo Atribuído a: Campo Nome quando o formulário é anexado a uma tarefa:
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

Para obter mais informações sobre variáveis como `$$OBJCODE,` see [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Atualizações automáticas de campos personalizados calculados

Os campos personalizados calculados em um objeto são recalculados automaticamente quando as seguintes coisas acontecem:

* Algo no objeto muda, como um cálculo diário da linha do tempo.
* Alguém edita outro campo referenciado por um campo personalizado calculado no objeto.
* A expressão calculada está vazia e o campo contém um valor. Isso define o valor como nulo.

   >[!NOTE]
   >
   ><div>Em um formulário personalizado anexado a um objeto, as declarações de data e hora em campos personalizados calculados são calculadas e salvas pelo Tempo Universal Coordenado (UTC), não pelas configurações de fuso horário definidas para a instância da sua organização e o perfil do usuário. Os cálculos em um formulário personalizado são gerados com base nos fusos horários individuais de cada usuário.</div>

