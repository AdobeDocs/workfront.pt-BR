---
title: Adicionar campos calculados a um formulário
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode adicionar um campo personalizado calculado que use dados existentes para gerar novos dados quando o formulário personalizado for anexado a um objeto.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 407aae49-4bc3-4364-a794-7e170a57a6d3
source-git-commit: 420c26c22cb1e6c0eab0f4cb0e211922d9ed2350
workflow-type: tm+mt
source-wordcount: '2353'
ht-degree: 0%

---

# Adicionar campos calculados a um formulário

Você pode adicionar um campo personalizado calculado que use dados existentes para gerar novos dados quando o formulário personalizado for anexado a um objeto.

Um campo personalizado calculado pode conter:

* Uma referência simples a um único campo incorporado.

  >[!INFO]
  >
  > **Exemplo:** para calcular a receita gerada por projetos e tarefas, você pode criar um campo personalizado calculado que contenha o campo interno Receita real. Quando alguém anexa o formulário personalizado a um projeto ou tarefa, a receita do projeto ou tarefa é exibida no campo.

* Uma expressão que faz referência a um ou mais campos. Podem ser campos personalizados, outros campos personalizados calculados e campos incorporados.

  >[!INFO]
  >
  >**Exemplo:** para calcular o lucro gerado por projetos e tarefas, você pode criar um campo personalizado calculado chamado Lucro contendo uma expressão matemática que subtrai o custo da receita.
  >
  >Para fazer isso, você pode usar a expressão matemática SUB (subtrair) com os campos integrados Custo real e Receita real do Workfront.
  >
  >Nas etapas abaixo, é possível ver como esse exemplo pode ser executado.


## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber quais configurações de plano, tipo de licença ou nível de acesso você tem, contate o administrador do Workfront.

## Reutilizar um campo personalizado calculado existente em um formulário personalizado

Você pode usar o mesmo campo personalizado calculado em formulários personalizados que pertencem a objetos diferentes. Por exemplo, você pode usar o campo calculado Lucro criado para o formulário personalizado de projeto em um formulário personalizado de tarefa.

Ao usar um campo personalizado calculado existente, o cálculo não é transferido para o novo formulário. Você deve adicionar o cálculo novamente, no mesmo campo, no novo formulário personalizado.

Você também pode ter um cálculo diferente para o mesmo campo, no novo formulário. Manter o mesmo nome para o campo personalizado calculado garante a coesão e a consistência em sua convenção de nomenclatura.

>[!IMPORTANT]
>
>As alterações em expressões calculadas podem fazer com que o valor do campo em objetos fique desatualizado. Para garantir que o cálculo sempre esteja atualizado nesses campos, siga um destes procedimentos:
>
>* Depois de salvar um objeto com os dados editados em um formulário personalizado anexado, clique no ícone Mais ![](assets/more-icon.png) na página principal do objeto e em Recalcular Expressões Personalizadas.
>* Selecione a opção Recalcular expressões personalizadas ao editar objetos em massa.
>* Selecione a opção Update previous calculations ao editar um Campo personalizado calculado em um formulário personalizado.

Para reutilizar um campo personalizado calculado existente:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Forms Personalizado** no painel esquerdo.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Clique em **Novo formulário personalizado.**
1. Selecione a quais tipos de objeto você deseja anexar o formulário personalizado e clique em **Continuar**.

1. Na parte superior esquerda da tela, clique em **Biblioteca de campos**.

   ![](assets/field-library.png)

1. Use a caixa de pesquisa ou expanda a seção **Calculado** para localizar o campo calculado necessário e, em seguida, arraste o campo onde deseja que ele apareça no formulário personalizado.

1. (Opcional) Repita a etapa anterior para adicionar outros campos.

   >[!NOTE]
   >
   >Você pode adicionar até 500 campos e widgets em um único formulário personalizado. No entanto, a degradação do desempenho pode ocorrer quando existem mais de 100 em um formulário, dependendo de sua complexidade.
   >
   >
   >Exemplos de formulários complexos incluem formulários com parâmetros em cascata, campos de dados personalizados calculados e várias opções de valor em um único campo.

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

## Adicionar um novo campo calculado

>[!IMPORTANT]
>
>Antes de criar um novo campo personalizado calculado, identifique os campos existentes que deseja incluir para ter certeza de que os dados necessários para o cálculo estão presentes no Workfront.

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Forms Personalizado** no painel esquerdo.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Clique em **Novo formulário personalizado.**
1. Selecione a quais tipos de objeto você deseja anexar o formulário personalizado e clique em **Continuar**.

1. No lado esquerdo da tela, localize **Calculado** e arraste-o para uma seção da tela.

   ![](assets/drag-field-to-section.png)

1. No lado direito da tela, configure as opções disponíveis para o tipo de campo personalizado que você está adicionando:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td>Digite um rótulo para o campo. É o que os usuários verão ao usar o formulário personalizado. O campo <b>Nome</b>, que é preenchido automaticamente, é referenciado pela Workfront nos relatórios.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instruções</td> 
      <td> Por padrão, a fórmula criada para o campo é armazenada aqui. É possível adicionar texto para fornecer informações adicionais sobre o campo e a fórmula nele. Isso pode ser útil de duas maneiras: 
       <ul> 
      <li><p>Como um lembrete do que é a fórmula e como ela funciona. Isso é especialmente útil se você planeja usar esse campo personalizado calculado em vários formulários.</p> </li> 
      <li> <p>Como uma dica de ferramenta, os usuários podem ver quando passam o mouse sobre o campo. Você adiciona qualquer texto aqui que deseja que eles vejam na dica de ferramenta.</p> <p>Se não quiser que eles vejam a fórmula na dica de ferramenta, o que pode ser confuso para eles, você pode ocultá-la.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formatar</td> 
      <td> <p>O formato no qual você deseja que os resultados do campo sejam armazenados e exibidos.</p> <p>Se o campo for usado em cálculos matemáticos, sempre use o formato <strong>Número</strong> ou <strong>Moeda</strong>. Ao selecionar Número ou Moeda, o sistema trunca automaticamente os números que começam com 0.</p> 
      <p><b>IMPORTANTE</b>: antes de escolher um formato, considere o formato correto para o novo campo. O campo de formato não pode ser editado depois que o formulário personalizado é salvo. E selecionar o formato errado poderia afetar cálculos futuros e agregar valores em agrupamentos de relatórios e listas.</p>
      <p><strong>OBSERVAÇÃO:</strong> campos calculados com um formato de Moeda não devem incluir aspas. (Por exemplo, use 800.00 e não "800.00".) O uso de aspas pode causar consequências inesperadas devido a nuances na formatação de idioma para tipos de moeda.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Na caixa **Cálculo**, comece a criar seu cálculo:
   1. Clique em **Maximizar** para abrir o Editor de Cálculo e criar seu cálculo.</p>
Um cálculo geralmente começa com uma expressão, seguida por parênteses contendo os campos que você deseja referenciar quando o formulário personalizado é anexado a um objeto.

      Cada campo deve estar entre chaves. Quando você começa a digitar o nome de um campo, o sistema faz sugestões e você pode selecionar uma para inseri-la no cálculo.

+++ **Expanda para ver a sintaxe necessária em campos personalizados calculados**

      Cada campo deve usar a sintaxe explicada abaixo, com chaves ao redor de cada nome de campo. Quando você começa a digitar o nome de um campo, o sistema faz sugestões e você pode selecionar uma para inseri-la no cálculo. Se você inserir dados em um cálculo incorretamente, uma mensagem de aviso o alertará. Não é possível salvar o formulário, a menos que você edite o cálculo para que ele contenha campos válidos e uma expressão calculada válida.

      >[!NOTE]
      >
      >Atualmente, o sistema faz sugestões somente quando você começa a digitar o nome de um campo que deseja referenciar em um objeto ao qual o formulário personalizado será anexado. Os campos do objeto pai não são sugeridos.

      **Nomes de campo surround com chaves**

      * Se quiser que o cálculo faça referência a um campo incorporado, o nome do campo deverá estar entre chaves.

        Por exemplo: `{actualRevenue}`

        Os nomes de campos fazem distinção entre maiúsculas e minúsculas e devem aparecer no cálculo exatamente como aparecem no sistema Workfront.

        Navegue até o [Workfront API Explorer](https://developer.adobe.com/workfront/api-explorer/) para identificar os nomes de campo que podem ser usados em cálculos.

      * Se você quiser que o cálculo faça referência a um campo personalizado, o nome do campo deverá estar entre chaves e precedido por `DE:` entre colchetes.

        Por exemplo: `{DE:Profit}`

        O sistema lista todos os campos personalizados que você pode escolher ao digitar `DE:`.

         * Para que o cálculo faça referência a um campo que extrairá dados do objeto *pai* quando o formulário personalizado for anexado a um objeto, você deve preceder o nome do campo com o tipo de objeto do objeto pai, também entre chaves.

        Por exemplo, se o formulário personalizado estiver configurado para funcionar com tarefas e você quiser que o campo calcule a receita real do objeto pai quando o formulário for anexado a uma tarefa, será necessário indicar `Project` como o tipo de objeto do campo:

        `{project}.{actualRevenue}`

        Ou, se for um campo personalizado:

        `{project}.{DE:profit}`

        **Separar itens com pontos**

        Ao fazer referência a um objeto relacionado em um campo personalizado calculado, você deve separar nomes de objeto e atributos com pontos.

        Por exemplo, em um formulário personalizado do tipo tarefa, para exibir o nome do Proprietário do Portfolio em um campo personalizado calculado, você digitaria o seguinte:

        `{project}.{porfolio}.{owner}`

        Isso determinaria o seguinte: A partir do objeto do formulário personalizado (uma tarefa), você pode acessar o próximo objeto relacionado à tarefa (um projeto). A partir daí, você pode acessar o próximo objeto relacionado ao projeto (um portfólio) e, em seguida, fazer referência aos campos definidos para o objeto do portfólio (o proprietário)

        **Sintaxe de nome para fazer referência a um campo personalizado**

        Quando você faz referência a outro campo personalizado em um campo personalizado calculado, é necessário inserir o nome do campo como ele é exibido na interface do usuário do Workfront.

        Por exemplo, para fazer referência à opção selecionada em um campo personalizado rotulado como Patrocinador executivo, você digitaria o seguinte:

        `{DE:Executive sponsor}`

        >[!NOTE]
        >
        >A sintaxe de um campo de digitação antecipada é um pouco diferente de outros tipos de campos, pois você precisa adicionar `:name` no final.
        >
        >Por exemplo, para fazer referência à opção selecionada em um campo de digitação antecipada personalizado chamado &quot;Patrocinador executivo&quot;, você digitaria:
        >
        >`{DE:Executive sponsor:name}`


        **Campos personalizados calculados em formulários personalizados de vários objetos**

        Em um formulário personalizado de vários objetos, os tipos de objeto selecionados devem ser compatíveis com pelo menos um campo referenciado nos campos personalizados calculados do formulário. Campos não compatíveis com o objeto exibirão N/D no formulário.

        Para garantir que o campo calculado mostre um resultado correto para todos os tipos de objeto, você deve usar `$$OBJCODE` para definir um cálculo para cada tipo de objeto.

        >[!INFO]
        >
        >**Exemplo:**
        >
        >Em um formulário personalizado configurado para trabalhar com projetos, tarefas e problemas, você pode usar a seguinte fórmula para exibir o tipo de objeto:
        >
        >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
        >
        >Em um projeto, o campo mostrará &quot;Isto é um projeto&quot;, em uma tarefa mostrará &quot;Isto é uma tarefa&quot; e em um problema dirá &quot;Isto é um problema&quot;.


        >[!INFO]
        >
        >**Exemplo:** Embora não haja nenhum campo Atribuído a: Nome nos projetos, há um campo Proprietário interno (que é preenchido automaticamente com o nome da pessoa que criou o projeto, a menos que alguém altere isso manualmente).
        >
        >Portanto, em seu campo personalizado Encargo, você pode usar `$$OBJCODE` como mostrado abaixo para fazer referência ao campo Proprietário quando o formulário personalizado estiver anexado a um projeto, e o campo Atribuído a: Nome quando o formulário estiver anexado a uma tarefa:
        >
        >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

        Para obter mais informações sobre variáveis como `$$OBJCODE,`, consulte [Visão geral das variáveis de filtro curinga](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

        **Atualizações automáticas de campos personalizados calculados**

        Os campos personalizados calculados em um objeto são recalculados automaticamente quando as seguintes situações ocorrem:

         * Algo no objeto muda, como um cálculo diário da linha do tempo.
         * Alguém edita outro campo que é referenciado por um campo personalizado calculado no objeto.
         * A expressão calculada está vazia e o campo contém um valor, isso define o valor como nulo.

           >[!NOTE]
           >
           ><div>Em um formulário personalizado anexado a um objeto, os demonstrativos de data e hora em campos personalizados calculados são calculados e salvos pelo Tempo universal coordenado (UTC), não pelas configurações de fuso horário definidas para a instância da organização e o perfil do usuário. Os cálculos em um formulário personalizado são gerados com base nos fusos horários individuais de cada usuário.</div>

+++

   1. Clique na caixa de texto grande e, em seguida, clique em **Expressões** e **Campos** disponíveis para adicioná-los ao cálculo.

      Você também pode começar a digitar uma expressão ou campo na caixa de texto grande e selecioná-lo quando ele for exibido. Cada item é exibido com um &quot;F&quot; para o campo ou um &quot;E&quot; para a expressão.

      Se você digitar um parêntese de abertura, o parêntese de fechamento será adicionado automaticamente.

+++ **Expanda para ver dicas úteis**

      >[!TIP]
      >
      >Você pode executar qualquer um dos seguintes procedimentos para obter ajuda com o cálculo:
      > 
      >* Passe o mouse sobre uma expressão no cálculo para ver uma descrição, um exemplo mostrando como ela pode ser usada e um link &quot;Saiba mais&quot; para obter mais informações no artigo [Visão geral das expressões de dados calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
      >* Use a codificação de cores para identificar os componentes adicionados. As expressões são exibidas em azul e os campos são exibidos em verde.
      >  ![](assets/colors-fields-expressions.jpg)
      >* Encontre erros de cálculo, destacados em rosa, conforme você avança. Você pode passar o mouse sobre um erro destacado para exibir uma breve descrição da causa.
      >  ![](assets/error-help.png)
      >* Na área abaixo do cálculo, visualize os resultados em um objeto do Workfront existente.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
      >  ![](assets/preview-calc.jpg)
      >* Referencie expressões em um cálculo longo usando os números de linha exibidos à esquerda.

+++
   1. Clique em **Minimizar** quando terminar de criar o cálculo para o campo personalizado calculado.

   1. (Opcional) Use qualquer uma das seguintes opções para configurar ainda mais seu campo personalizado calculado:

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Adicionar Lógica</td> 
      <td>Você pode adicionar Lógica de exibição para determinar se o campo calculado é exibido com base em pelo menos uma escolha que um usuário faz em um campo de múltipla escolha anterior (Suspenso, Caixas de seleção ou Botões de opção) ao preencher o formulário. <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>Isso está disponível somente quando pelo menos uma caixa de seleção, botão de opção ou campo suspenso precede o campo personalizado calculado no formulário. </p> <p>A Lógica de salto não está disponível para campos personalizados calculados.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atualizar cálculos anteriores</td> 
      <td>Ao editar um campo personalizado calculado existente, você pode selecionar essa opção para acionar uma atualização no cálculo ao salvar o formulário personalizado. Isso acontece apenas uma vez quando você salva o formulário personalizado. Depois disso, a opção retornará ao estado desativado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir a fórmula nas instruções</td> 
      <td>Deixe essa opção ativada se quiser que os usuários que preenchem o formulário personalizado vejam a fórmula do campo quando passam o mouse sobre o campo. Para obter mais informações, consulte as informações sobre <a href="#instructions" class="MCXref xref">Instruções</a> anteriormente nesta tabela.</td> 
     </tr> 
    </tbody> 
   </table>

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.
