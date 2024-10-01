---
title: Criar um formulário com o Form Designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode criar um formulário personalizado com o designer do formulário. Você pode anexar formulários personalizados a diferentes objetos do Workfront para capturar dados sobre esses objetos.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: eee683edc36b33b74d67a9ffbcab9697826e3a86
workflow-type: tm+mt
source-wordcount: '5575'
ht-degree: 5%

---

# Criar um formulário com o designer de formulário

{{highlighted-preview}}

Você pode criar um formulário personalizado com o designer do formulário. Você pode anexar formulários personalizados a diferentes objetos do Workfront para capturar dados sobre esses objetos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Comece a criar um formulário personalizado

{{step-1-to-setup}}

1. Clique em **Forms Personalizado** no painel esquerdo.

1. Clique em **Novo formulário personalizado.**
1. Selecione a quais tipos de objeto você deseja anexar o formulário personalizado e clique em **Continuar**.

   ![](assets/choose-object-type.jpg)

1. Na área **Título obrigatório**, digite o título do formulário personalizado.
1. (Opcional) Se quiser adicionar mais tipos de objeto ao formulário para que ele possa ser anexado a mais objetos, clique no ícone **Adicionar** ![](assets/add-objects-icon.png) depois de **Tipos de Objeto** e selecione o tipo desejado no menu exibido. Você pode repetir isso para adicionar quantos tipos de objetos desejar.

   Você também pode clicar no X em um tipo de objeto para excluí-lo do formulário.

   >[!CAUTION]
   >
   >A exclusão de um formulário personalizado também exclui todos os dados personalizados nos objetos associados ao formulário. Os dados excluídos não podem ser recuperados. Considere desativar um formulário personalizado. Ao desativar um formulário personalizado que não é mais usado, todos os dados históricos associados serão retidos.
   >
   >Para obter mais informações, consulte [Adicionar ou excluir tipos de objetos de um formulário personalizado existente](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md) e [Desativar ou reativar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md).


1. Em seguida, você pode começar a adicionar campos ao formulário personalizado. Consulte as seguintes seções:
   * [Reutilizar um campo ou widget existente já usado em outro formulário personalizado](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Observações sobre nomes e rótulos de campos](#notes-on-field-names-and-labels)
   * [Adicionar campos de texto](#add-text-fields)
   * [Adicionar campos calculados](#add-calculated-fields)
   * [Adicionar botões de opção, grupos de caixas de seleção e menus suspensos](#add-radio-buttons-checkboxes-and-dropdowns)
   * [Adicionar campos de digitação antecipada e data](#add-typeahead-and-date-fields)
   * [Adicionar campos de pesquisa externos](#add-external-lookup-fields)
   * [Adicionar imagens, PDF e vídeos](#add-images-pdfs-and-videos)
   * [Adicionar campos nativos do Workfront](#add-workfront-native-fields)
   * [Adicionar arquivos do Adobe XD](#add-adobe-xd-files)

## Adicionar campos novos ou existentes ao formulário personalizado

Você pode usar campos novos ou existentes ao criar o formulário personalizado.

<span class="preview">Os formulários personalizados estão limitados a 500 campos. Um contador na parte inferior esquerda exibe quantos campos são usados no formulário e ele fica sempre visível à medida que você rola a tela dentro do designer do formulário.</span>

### Reutilizar um campo ou widget existente já usado em outro formulário personalizado

1. Na parte superior esquerda da tela, clique em **Biblioteca de campos**.

1. Arraste o campo ou widget aqui que você deseja no formulário personalizado.
1. (Opcional) Repita a etapa anterior para adicionar outros campos ou widgets.

   >[!NOTE]
   >
   >Você pode adicionar até 500 campos e widgets em um único formulário personalizado. No entanto, a degradação do desempenho pode ocorrer quando existem mais de 100 em um formulário, dependendo de sua complexidade.
   >
   >
   >Exemplos de formulários complexos incluem formulários com parâmetros em cascata, campos de dados personalizados calculados e várias opções de valor em um único campo.

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

### Observações sobre nomes e rótulos de campos {#notes-on-field-names-and-labels}

O **rótulo** está disponível para a maioria dos campos. É um rótulo descritivo que aparece acima do campo ou widget no formulário personalizado. Você pode alterar o rótulo a qualquer momento.

>[!NOTE]
>
>Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios.

Um **nome** é necessário para cada campo. Esse nome é como o sistema identifica o campo personalizado ao adicioná-lo a várias áreas no Workfront, como relatórios, Página inicial e interações de API. Quando você está configurando o campo ou widget pela primeira vez e digita o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.

Cada nome de campo personalizado deve ser exclusivo na instância do Workfront da organização. Dessa forma, é possível reutilizar um que já foi criado para outro formulário personalizado.

>[!NOTE]
>
>Embora seja possível fazer isso, recomendamos que você não altere esse nome depois que você ou outros usuários começarem a usar o formulário personalizado no Workfront. Se você fizer isso, o sistema não reconhecerá mais o campo personalizado onde ele pode agora ser referenciado em outras áreas do Workfront.
>Por exemplo, se você adicionar o campo personalizado a um relatório e depois alterar seu nome, o Workfront não o reconhecerá no relatório e ele deixará de funcionar corretamente lá, a menos que você o adicione novamente ao relatório usando o novo nome.
>
>Recomendamos que você não digite um nome que já esteja sendo usado para campos integrados do Workfront.
>
>Recomendamos que você não use o caractere ponto no nome do campo personalizado para evitar erros ao usar o campo em diferentes áreas do Workfront.

Os caracteres especiais a seguir não são aceitos em rótulos e nomes de campos personalizados.

* \ t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* :
* `{`
* `}`

### Adicionar campos de texto

É possível adicionar vários campos de texto diferentes a um formulário personalizado.

+++ **Expanda para ver descrições de campos de texto disponíveis**

* **Campo de texto de linha única**: permite que os usuários digitem uma única linha de texto no campo.
* **Campo de parágrafo**: permite que os usuários digitem várias linhas de texto no campo.
* **Campo de texto com formatação**: permite aos usuários digitar várias linhas de texto no campo e formatar o texto com negrito, itálico, sublinhado, marcadores, numeração, hiperlinks e aspas de bloco. Um limite de 15.000 caracteres permite bastante texto e formatação.

  Esse tipo de campo personalizado não é compatível com filtros em listas e relatórios.

  Para obter informações sobre como acessar este campo por meio da API, consulte [Armazenamento de campo Rich Text na API](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md).

  >[!NOTE]
  >
  >Os campos de texto com formatação não estão disponíveis para aplicativos móveis Workfront (disponíveis nas próximas versões).

* **Texto descritivo**: permite incluir instruções e vincular a páginas fora do Workfront.

+++

Para adicionar um campo de texto:

1. No lado esquerdo da tela, localize um dos seguintes campos de texto e arraste-o para uma seção da tela:

   * Texto de linha única
   * Parágrafo
   * Texto com formatação
   * Texto descritivo

   ![](assets/drag-field-to-section.png)

1. No lado direito da tela, configure as opções disponíveis para o tipo de campo personalizado que você está adicionando:

   <table>
    <tr>
    <td>Entrada em</td>
    <td>Descrição</td>
    <td>Disponível para </td>
    </tr>
    <tr>
    <td>Tamanho</td>
    <td><p>Altere o tamanho dos campos de texto no formulário.<p>
   </td>
    <td><ul>
    <li>Texto de linha única</li>
    <li>Parágrafo</li>
    <li>Texto com formatação</li>
    <li>Texto descritivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Rótulo</td>
    <td><p>(Obrigatório) Digite um rótulo descritivo para exibir acima do campo. Você pode alterar o rótulo a qualquer momento.<p>
    <p>IMPORTANTE: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios. Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p></td>
    <td><ul>
    <li>Texto de linha única</li>
    <li>Parágrafo</li>
    <li>Texto com formatação</li>
    </ul></td>
    </tr>
    <tr>
     <td>Nome</td>
    <td><p>(Obrigatório) Esse nome é a forma como o sistema identifica o campo. Quando você está configurando o widget pela primeira vez e digita o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p>
    <p>Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p>
    </td>
    <td><ul>
    <li>Texto de linha única</li>
    <li>Parágrafo</li>
    <li>Texto com formatação</li>
    <li>Texto descritivo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Instruções</td>
    <td>Digite quaisquer informações adicionais sobre o campo. Quando os usuários preencherem o formulário personalizado, poderão passar o mouse sobre o ícone de ponto de interrogação para exibir uma dica de ferramenta contendo as informações digitadas aqui.
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>Texto de linha única</li>
    <li>Parágrafo</li>
    <li>Texto com formatação</li>
    </ul></td>
    </tr>
    <tr>
    <td>Formatar</td>
    <td><p>Selecione o tipo de dados que será capturado no campo personalizado.</p> <p><b>NOTA</b>:   
    <ul> 
    <li>Este campo não pode ser editado depois que o formulário é salvo. Se você pretende usar seu campo em cálculos matemáticos, certifique-se de selecionar um formato de Número ou Moeda.</li> 
    <li>Ao selecionar Número ou Moeda, o sistema trunca automaticamente os números que começam com 0.</li>
    <li>O limite de caracteres para campos de Número é de 16. Você também pode usar um campo Texto para inserir números e evitar o limite.</li>
     </ul></p></td> </td>
    <td><ul>
    <li>Texto de linha única</li>
    <li>Parágrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Tipo de Exibição</td>
    <td>Alternar entre campos de texto de linha única e de parágrafo.</td>
    <td><ul>
    <li>Texto de linha única</li>
    <li>Parágrafo</li>
    </ul></td>
    </tr>
    <tr>
    <td>Hiperlink</td>
    <td> Se quiser aplicar um hiperlink ao Texto descritivo digitado, adicione-o aqui. O texto descritivo é exibido como um link em objetos aos quais o formulário está anexado.</td>
    <td><ul><li>Texto descritivo</li></ul></td>
    </tr>
   </table>

1. (Opcional) Repita a etapa anterior para adicionar outros campos ou widgets.

   ou

   Para copiar um campo, passe o mouse sobre um campo e clique no ícone de cópia.

   ![ícone de cópia](assets/copy-field.png)

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

### Adicionar campos calculados

Em um formulário personalizado, você pode adicionar um campo personalizado calculado que usa dados existentes para gerar novos dados quando o formulário personalizado é anexado a um objeto.

Para adicionar um campo calculado, consulte [Adicionar campos calculados com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### Adicionar botões de opção, grupos de caixas de seleção e menus suspensos

Você pode adicionar botões de opção, grupos de caixas de seleção, menus suspensos e menus suspensos de seleção múltipla em um formulário personalizado.

+++ **Expanda para ver descrições dos campos disponíveis**

* **Botões de opção**: requer que os usuários selecionem apenas uma opção.
* **Grupo de caixas de seleção**: permite que os usuários selecionem várias opções.
* **Lista suspensa de seleção única**: fornece uma lista de opções suspensas.
* **Lista suspensa de várias seleções**: permite que os usuários selecionem várias opções em uma lista suspensa.

+++

>[!NOTE]
>
>Os campos que permitem várias seleções, como Grupo de caixas de seleção e Lista suspensa de seleção múltipla, são difíceis de representar em gráfico e agrupar nos relatórios. Para facilitar a criação de gráficos e o agrupamento em relatórios, é possível criar campos separados para cada escolha (por exemplo, um campo de texto de linha única).

Para adicionar botões de opção, grupos de caixas de seleção e menus suspensos:

1. No lado esquerdo da tela, encontre um dos campos a seguir e arraste-o para uma seção da tela.

   * Botões de seleção
   * Grupo de caixas de seleção
   * Lista suspensa de seleção única
   * Lista suspensa com seleção múltipla

   ![Arraste um campo até a tela](assets/drag-field-to-section.png)

1. No lado direito da tela, configure as opções disponíveis para o tipo de campo personalizado que você está adicionando:

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>Entrada em</td>
    <td>Descrição</td>
    <td>Disponível para </td>
    </tr>
    <tr> 
     <td role="rowheader">Rótulo</td> 
     <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do campo personalizado. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios. Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td> 
     <td><ul>
    <li>Botões de seleção</li>
    <li>Grupo de caixas de seleção</li>
    <li>Lista suspensa de seleção única</li>
    <li>Lista suspensa com seleção múltipla</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">Nome</td> 
     <td> <p>(Obrigatório) Esse nome é a forma como o sistema identifica o campo. Quando você está configurando o widget pela primeira vez e digita o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p> 
    <p>Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td>
     <td><ul>
    <li>Botões de seleção</li>
    <li>Grupo de caixas de seleção</li>
    <li>Lista suspensa de seleção única</li>
    <li>Lista suspensa com seleção múltipla</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Instruções</td> 
    <td> <p>Digite quaisquer informações adicionais sobre o campo personalizado. Quando os usuários preencherem o formulário personalizado, poderão passar o mouse sobre o ícone de ponto de interrogação para exibir uma dica de ferramenta contendo as informações digitadas aqui.</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>Botões de seleção</li>
    <li>Grupo de caixas de seleção</li>
    <li>Lista suspensa de seleção única</li>
    <li>Lista suspensa com seleção múltipla</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">Formatar</td> 
    <td> <p>Selecione o tipo de dados que será capturado no campo personalizado.</p> <p><b>NOTA</b>:   
     <ul> 
    <li>Este campo não pode ser editado depois que o formulário é salvo. Se você pretende usar seu campo em cálculos matemáticos, certifique-se de selecionar um formato de Número ou Moeda.<br></li> 
    <li>Ao selecionar Número ou Moeda, o sistema trunca automaticamente os números que começam com 0.</li>
    <li>O limite de caracteres para campos de Número é de 16. Você também pode usar um campo Texto para inserir números e evitar o limite.</li>
     </ul></p></td> 
     <td><ul>
    <li>Botões de seleção</li>
    <li>Grupo de caixas de seleção</li>
    <li>Lista suspensa de seleção única</li>
    <li>Lista suspensa com seleção múltipla</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">Tipo de Exibição</td> 
    <td>Alterne entre botões de opção, grupo de caixas de seleção, lista suspensa de seleção única ou lista suspensa de seleção múltipla para o campo.</td> 
    <td><ul>
    <li>Botões de seleção</li>
    <li>Grupo de caixas de seleção</li>
    <li>Lista suspensa de seleção única</li>
    <li>Lista suspensa com seleção múltipla</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">Tornar um campo obrigatório</td> 
    <td>Selecione essa opção se desejar que o campo seja obrigatório para que o usuário preencha o formulário personalizado. </td> 
    <td><ul>
    <li>Botões de seleção</li>
    <li>Grupo de caixas de seleção</li>
    <li>Lista suspensa de seleção única</li>
    <li>Lista suspensa com seleção múltipla</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">Seleções </td> 
    <td> 
    <ol> 
    <li> <p>Clique em <b>Opções</b> e habilite qualquer um dos itens a seguir:</p> 
    <ul> 
    <li><strong>Mostrar Valores</strong>: mostra os valores de cada escolha no campo. O rótulo de cada opção é exibido por padrão.</li> 
     <li><strong>Classificar seleções de A a Z</strong>: classifica as seleções adicionadas em ordem alfabética no campo.</li> 
    </ul> 
    </li> 
    <li> <p>Para cada opção adicionada para o usuário, clique no ícone de engrenagem <img src="assets/gear-icon-settings.png"> e selecione uma das seguintes opções:</p> 
    <ul> 
    <li><strong>Selecionar por padrão</strong>: selecione a opção por padrão no campo.</li> 
    <li> <p><strong>Ocultar opção</strong>: oculta a opção no campo. As opções ocultas permanecem acessíveis nos relatórios.</p> </li> 
    <li> <p><strong>Remover Opção</strong>: remova a opção do campo.</p> <p><b>AVISO</b>: se você tiver objetos atuais usando essa opção, não remova-a do campo. Sua remoção fará com que os dados do histórico sejam perdidos. Em vez disso, selecione a opção para ocultá-la, o que impede que os usuários a selecionem no futuro.</p> </li> 
    </ul> 
     </li> 
    </ol> </td> 
    <td><ul>
    <li>Botões de seleção</li>
    <li>Grupo de caixas de seleção</li>
    <li>Lista suspensa de seleção única</li>
    <li>Lista suspensa com seleção múltipla</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. (Opcional) Repita a etapa anterior para adicionar outros campos ou widgets.

   ou

   Para copiar um campo, passe o mouse sobre um campo e clique no ícone de cópia.

   ![ícone de cópia](assets/copy-field.png)

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

### Adicionar campos de digitação antecipada e data

Você pode adicionar campos de digitação antecipada e data a um formulário personalizado.

+++ **Expanda para ver descrições dos campos disponíveis**

* **Typeahead**: permite que os usuários digitem o nome de um objeto que existe no Workfront. Uma lista de sugestões é exibida quando o usuário começa a digitar. Esse tipo de campo oferece suporte aos seguintes objetos:
   * Usuário
   * Grupo
   * Função no trabalho
   * Portfólio
   * Programa
   * Projeto
   * Equipe
   * Modelo
   * Empresa
* **Data**: exibe um calendário em que os usuários podem selecionar uma data e hora.

+++

Para adicionar campos de digitação antecipada e data:

1. No lado esquerdo da tela, encontre um dos campos a seguir e arraste-o para uma seção da tela.

   * Typeahead
   * Data

   ![](assets/drag-field-to-section.png)

1. No lado direito da tela, configure as opções disponíveis para o tipo de campo personalizado que você está adicionando:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>Configuração de campo</td>
    <td>Descrição</td>
    <td>Disponível para </td>
    </tr>
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do campo personalizado. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios. Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obrigatório) Esse nome é a forma como o sistema identifica o campo. Quando você está configurando o widget pela primeira vez e digita o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p> 
      <p>Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td>
    <td><ul>
    <li>Typeahead</li>
    <li>Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>Digite quaisquer informações adicionais sobre o campo personalizado. Quando os usuários preencherem o formulário personalizado, poderão passar o mouse sobre o ícone de ponto de interrogação para exibir uma dica de ferramenta contendo as informações digitadas aqui.</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>Typeahead</li>
    <li>Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Exibir horário</td> 
      <td>Selecione essa opção se desejar mostrar a hora do dia junto com a data no campo.</td> 
         <td><ul>
    <li>Data</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto referenciado</td> 
      <td> <p>Selecione o tipo de objeto que deseja associar ao campo.</p> <p>Depois de clicar em Aplicar ou Salvar+Fechar, não é possível alterar o tipo de objeto do campo.</p> <p><b>NOTA</b>:   
        <ul> 
         <li>Se o administrador do Workfront personalizou o nome de Portfolio, Programas ou Projetos na interface do usuário do Workfront, o nome padrão do Workfront para o objeto será exibido nessa lista suspensa, não no nome personalizado. Consulte o administrador do Workfront se precisar de ajuda com isso.<br></li> 
         <li>Os seguintes tipos de objetos são suportados nos aplicativos móveis iOS e Android Workfront: usuário, empresa, grupo, função de trabalho, Portfolio, programa, projeto e modelo.</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>Typeahead</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">Adicionar Filtro</td>
      <td><p>Adicione um filtro para um tipo de objeto para limitar os objetos que os usuários podem escolher quando estiverem usando o campo. </p> <p>Por exemplo, é possível limitar um campo para que os nomes de usuários possam ser selecionados somente se atenderem aos seguintes critérios:</p> 
       <ul> 
        <li>Eles pertencem a um ou mais grupos especificados por você</li> 
        <li>Eles estão associados a uma função ou a um cargo especificado por você</li> 
        <li>Eles pertencem ao mesmo grupo que a pessoa que está usando o campo</li> 
       </ul> <p>Você deve definir o filtro para o tipo de objeto selecionado usando a sintaxe do Modo de texto. Para obter informações sobre como criar um filtro usando o Modo Texto, consulte <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">Editar um filtro usando o modo texto</a>.</p>
       <p><b>NOTA</b>:
       <ul> 
        <li>Se você estiver editando um formulário personalizado existente, adicionar um filtro a um campo Digitação antecipada não removerá nenhum objeto (fora do escopo do filtro) que os usuários já tenham adicionado usando o campo.</li> 
        <li>Este filtro não está disponível em dispositivos móveis. Se você usar o filtro para um campo Digitação antecipada, o campo aparecerá nos dispositivos móveis dos usuários não afetados pelo filtro.</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>Typeahead</li>
       </ul>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Tornar um campo obrigatório</td> 
      <td>Selecione essa opção se desejar que o campo seja obrigatório para que o usuário preencha o formulário personalizado. </td> 
       <td><ul>
    <li>Typeahead</li>
    <li>Data</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita a etapa anterior para adicionar outros campos ou widgets.

   ou

   Para copiar um campo, passe o mouse sobre um campo e clique no ícone de cópia.

   ![ícone de cópia](assets/copy-field.png)

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

### Adicionar campos de pesquisa externos

Um campo de pesquisa externo chama uma API externa e retorna valores como opções em um campo suspenso. Os usuários que trabalham com o objeto ao qual o formulário personalizado está anexado podem selecionar uma ou mais dessas opções na lista suspensa. O campo de pesquisa externo também está disponível em listas e relatórios.

Para obter exemplos de como usar o campo de pesquisa externa para chamar a mesma instância do Workfront ou uma API pública, consulte [Exemplos do campo de pesquisa externa em um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md).

>[!NOTE]
>
>* No momento, os campos de pesquisa externa de formulários personalizados não são compatíveis com painéis. Não é possível editar o valor do campo em linha e ele pode não ser exibido corretamente em um painel. (Campos de pesquisa externa são aceitos nos Painéis do Canvas.)
>* Não há suporte para campos de pesquisa externos no plug-in do Outlook.
>* Os campos de pesquisa externos estão disponíveis em listas, a menos que o campo tenha uma dependência em outro campo.

Para adicionar uma pesquisa externa:

1. No lado esquerdo da tela, encontre **Pesquisa externa** e arraste-a para uma seção da tela.
1. No lado direito da tela, configure as opções do campo personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do campo personalizado. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios. Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obrigatório) Esse nome é a forma como o sistema identifica o campo. Quando você está configurando o widget pela primeira vez e digita o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p>
      <p>Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td>
     </tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>Digite quaisquer informações adicionais sobre o campo personalizado. Quando os usuários preencherem o formulário personalizado, poderão passar o mouse sobre o ícone de ponto de interrogação para exibir uma dica de ferramenta contendo as informações digitadas aqui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formatar</td>
      <td><p>Selecione o tipo de dados que será capturado no campo personalizado.</p>
      <p><strong>NOTA:</strong></p>
      <ul><li>É possível alterar o tipo de formato depois que o formulário é salvo, com uma limitação: todos os valores existentes em objetos devem poder ser convertidos para o novo tipo. (Por exemplo, se o tipo de formato for Texto e um objeto estiver armazenando o valor "abc", você não poderá converter o campo e receberá um erro de que o sistema não poderá converter "abc" em número/moeda.) Se você pretende usar seu campo em cálculos matemáticos, certifique-se de selecionar um formato de Número ou Moeda.</li>
      <li>Ao selecionar Número ou Moeda, o sistema trunca automaticamente os números que começam com 0.</li>
      <li>O limite de caracteres para campos de Número é de 16. Você também pode usar um campo Texto para inserir números e evitar o limite.</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">URL da API base</td> 
      <td><p>Digite ou cole o URL da API.</p><p>O URL da API deve retornar um conteúdo JSON das opções que você deseja mostrar na lista suspensa. Você pode usar o campo Caminho JSON para selecionar os valores específicos das opções suspensas do JSON retornado.</p><p>Ao inserir o URL da API, você pode passar os seguintes valores no URL:</p>
      <ul>
      <li>$$HOST - representa o host atual do Workfront e pode ser usado para fazer chamadas de API /search para a API do Workfront. Quando esse curinga é usado, a autenticação é tratada e os usuários não precisam enviar cabeçalhos de autenticação. (Por exemplo, os usuários podem pesquisar tarefas usando a URL base <code>$$HOST/attask/api/task/search</code> e isso permitirá pesquisar tarefas e selecionar valores de uma lista de tarefas retornada.)</li>
      <li><p>$$QUERY - Representa o texto de pesquisa que o usuário final digita no campo e permite implementar a filtragem de consultas para seus usuários finais. (O usuário pesquisará pelo valor na lista suspensa.)</p>
      <p>Se a API à qual você está fazendo referência permitir, também será possível incluir modificadores na consulta de pesquisa para identificar como a pesquisa deve funcionar. Por exemplo, você pode usar o seguinte como a URL da API Base para permitir que as pessoas pesquisem por qualquer projeto do Workfront que contenha texto específico: <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>.</p><p>Saiba mais sobre os modificadores de pesquisa do Workfront em <a href="/help/quicksilver/wf-api/general/api-basics.md">Noções básicas sobre API</a>.</p>
      <p><strong>OBSERVAÇÃO:</strong> se você não estiver usando o $$QUERY e o usuário digitar o texto na caixa de pesquisa, ele restringirá as opções que você já tem. No entanto, se você usar $$QUERY e o usuário digitar algo, uma nova chamada de rede para sua API será executada. Portanto, se você tiver mais de 2000 valores em sua API e a API for compatível com consultas, será possível utilizar o $$QUERY não apenas para pesquisar a partir dos valores de 2000 existentes, mas a partir da API original com as opções limitadas.</p></li>
      <li><p>{fieldName} - Onde fieldName é qualquer campo personalizado ou nativo no Workfront. Dessa forma, você pode implementar filtros de opção de lista suspensa em cascata ao passar o valor de um campo já selecionado para o campo de pesquisa Externo para filtrar opções. (Por exemplo, o campo Região já existe no formulário e você está restringindo uma lista de países da API para aqueles que estão em uma região específica.)</p>
      <p>Para um campo de pesquisa externo que tem uma dependência em outros campos (usando a sintaxe {fieldName}), as opções retornadas da API são limitadas àquelas que correspondem a qualquer cadeia de caracteres ou valor inserido em outros campos. (Essa funcionalidade não é compatível com listas e relatórios.)</p></li>
      <li>{referenceObject}.{fieldName} - Onde o campo faz parte de um objeto. Essa sintaxe é semelhante às expressões personalizadas. (Por exemplo, portfolioID={project}.{portfolioID})</li></ul>
      <p><strong>OBSERVAÇÃO:</strong> revise a documentação da API com a qual você está trabalhando para as consultas específicas que você pode definir.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Método HTTP</td> 
      <td>Selecione <strong>Obter</strong>, <strong>Postar</strong> ou <strong>Colocar</strong> para o método.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Caminho JSON</td>
      <td><p>Digite ou cole o caminho JSON para a API.</p> <p>Essa opção permite extrair dados do JSON retornado pelo URL da API. Ela serve como uma maneira de selecionar quais valores dentro do JSON aparecerão nas opções suspensas.</p><p>Por exemplo, se a URL da API retornar JSON neste formato:</br>
      <pre>
      {
       dados: {
         { name: "USA"},
         { name: "Canada"}
       }
      }
      </pre>
      </p>
      <p>em seguida, use "$.data[*].name" para selecionar EUA e Canadá como opções suspensas.</p> <p>Para obter mais informações sobre o Caminho JSON e verificar se você grava o Caminho JSON correto, consulte <a href="https://jsonpath.com/">https://jsonpath.com/</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Cabeçalhos</td>
      <td><p>Clique em <strong>Adicionar Cabeçalho</strong> e digite ou cole o par de valores chave necessário para autenticação com a API.</p><p><strong>OBSERVAÇÃO:</strong> os campos de Cabeçalho não são um local seguro para armazenar credenciais, e você deve ter cuidado com o que inseriu e salvou.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Menu suspenso com múltipla escolha</td>
      <td><p>Selecione essa opção para permitir que o usuário selecione mais de um valor na lista suspensa.</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">Tornar um campo obrigatório</td>
      <td><p>Selecione essa opção se desejar que o campo seja obrigatório para que o usuário preencha o formulário personalizado.</p></td>
     </tr>       
    </tbody>
   </table>

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

>[!NOTE]
>
>Os itens a seguir são limitações técnicas da chamada para a API externa:
>
>* Número máximo de opções: 2000 (somente as primeiras 2000 opções exclusivas do JSON retornado são exibidas)
>* Tempo limite: 3 segundos
>* Número de tentativas: 3
>* Duração da espera entre tentativas: 500 ms
>* Status de resposta esperados: 2xx

### Adicionar imagens, PDF e vídeos

Você pode adicionar imagens, PDF e vídeos a um formulário personalizado. Os usuários que trabalham com o objeto ao qual o formulário personalizado está anexado podem ver a imagem, o PDF ou o vídeo somente nas seguintes áreas:

* A área Detalhes do objeto (por exemplo, para um projeto, a área Detalhes do projeto)
* A caixa Editar do objeto, se ele tiver a nova aparência da experiência do Adobe Workfront (por exemplo, as caixas Editar projeto e Editar tarefa )

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **Expanda para ver descrições dos campos disponíveis**

* **Imagem**: permite que usuários adicionem arquivos de imagem.
* **PDF**: permite que usuários adicionem PDF
* **Vídeos**: permite que os usuários adicionem arquivos de vídeo.

+++

Para adicionar imagens, PDF ou vídeos:

1. No lado esquerdo da tela, encontre um dos campos a seguir e arraste-o para uma seção da tela.

   * Imagem
   * PDF
   * Vídeo

   ![](assets/drag-field-to-section.png)

1. Digite ou edite qualquer uma das seguintes propriedades do widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do widget. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios. Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obrigatório) Esse nome é como o sistema identifica o widget. Quando você está configurando o widget pela primeira vez e digita o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p> <p>Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obrigatório) Digite ou cole o URL do widget onde ele está armazenado na Internet.</p> 
      <p>Se você estiver adicionando um widget de vídeo, é possível fazer isso adicionando o seguinte na caixa de URL:</p> 
      <ul> 
      <li> <p>Link para o YouTube ou Vimeo</p> </li> 
      <li> <p>Link de vídeo da Google Drive</p> </li> 
      <li> <p>Link para vídeo com extensão MP4 e MOV</p> </li> 
      <li> <p>Link para vídeo já carregado na área Documentos na sua instância do Workfront. Para obter instruções, consulte <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Adicionar um widget de vídeo a um formulário personalizado na área Documentos</a> neste artigo.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>Digite quaisquer informações adicionais sobre o widget. Quando os usuários preencherem o formulário personalizado, poderão passar o mouse sobre o ícone de ponto de interrogação para exibir uma dica de ferramenta contendo as informações digitadas aqui.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamanho</td> 
      <td>Altere o tamanho de exibição do widget, conforme necessário.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita a etapa anterior para adicionar outros campos ou widgets.

   ou

   Para copiar um campo, passe o mouse sobre um campo e clique no ícone de cópia.

   ![ícone de cópia](assets/copy-field.png)

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

#### Adicionar um widget de vídeo a um formulário personalizado na área Documentos{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Ao adicionar um vídeo a um formulário personalizado dessa maneira, somente as permissões definidas para o formulário personalizado se aplicam ao vídeo quando os usuários acessam o formulário em um objeto, não as permissões definidas para o vídeo na área Documentos.

1. Vá para o vídeo na área Documentos e gere uma prova para ele, conforme descrito em [Criar uma prova interativa para um site ou outro conteúdo da Web](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Abra a prova.
1. Clique com o botão direito do mouse em qualquer lugar do vídeo e selecione **Copiar Endereço de Vídeo**.
1. No formulário personalizado ao qual você está adicionando o widget de vídeo, cole o endereço copiado na caixa **URL**.
1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

### Adicionar campos nativos do Workfront

Você pode adicionar campos nativos Workfront aos seus formulários personalizados. Quando o formulário personalizado é anexado a um objeto, o campo é preenchido a partir dos dados do objeto. Por exemplo, o campo Descrição em um formulário personalizado anexado a um projeto extrairá a descrição do projeto. (O campo pode mostrar &quot;N/D&quot; se nenhum dado estiver disponível.)

+++ **Expanda para ver a lista de campos nativos com suporte**

Esta tabela lista os campos nativos disponíveis para objetos Workfront específicos em um formulário personalizado.

| Nome do campo | Projeto | Tarefa | Problema | Modelo | Modelo de Tarefa | Portfólio | Programa | Grupo |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| Data de Término Efetivo | ✓ µ | ✓ µ | ✓ µ |   |   |   |   |   |
| Duração Efetiva | ✓ µ |   |   |   |   |   |   |   |
| Horas efetivas | ✓ µ |   | ✓ µ |   |   |   |   |   |
| Data do Início Efetivo | ✓ µ | ✓ µ | ✓ µ |   |   |   |   |   |
| Empresa | ✓ µ |   |   | ✓ µ |   |   |   |   |
| Condição | ✓ µ | ✓ µ | ✓ µ |   |   |   |   |   |
| Tipo de condição | ✓ µ |   |   | ✓ µ |   |   |   |   |
| Descrição | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |
| Duração |   | ✓ µ |   |   | ✓ µ |   |   |   |
| Tipo de Duração |   | ✓ µ |   |   | ✓ µ |   |   |   |
| Unidade de Duração |   | ✓ µ |   |   | ✓ µ |   |   |   |
| Cadastrado por | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |   | ✓ µ |
| Data de Entrada | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |   | ✓ µ |
| Grupo | ✓ µ |   |   | ✓ µ |   | ✓ µ | ✓ µ |   |
| Última Atualização realizada por | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |   |   |
| Última data de atualização | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |   |   |
| Nome | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |
| Proprietário | ✓ µ |   |   | ✓ µ |   | ✓ µ | ✓ µ |   |
| Data de conclusão planejada | ✓ µ | ✓ µ | ✓ µ |   |   |   |   |   |
| Duração Planejada | ✓ µ |   |   | ✓ µ |   |   |   |   |
| Horas planejadas | ✓ µ | ✓ µ | ✓ µ |   | ✓ µ |   |   |   |
| Data de início planejado | ✓ µ |   |   |   |   |   |   |   |
| Portfólio | ✓ µ |   |   | ✓ µ |   |   | ✓ µ |   |
| Prioridade | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |   |   |
| Programa | ✓ µ |   |   | ✓ µ |   |   |   |   |
| Data de Término Projetada | ✓ µ | ✓ µ |   |   |   |   |   |   |
| Minutos de Duração do Projeto |   | ✓ µ |   |   |   |   |   |   |
| Data de Início Projetada | ✓ µ | ✓ µ |   |   |   |   |   |   |
| Número de Referência | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |   |   |
| Modo de cronograma | ✓ µ |   |   | ✓ µ |   |   |   |   |
| Severidade |   |   | ✓ µ |   |   |   |   |   |
| Patrocinador | ✓ µ |   |   | ✓ µ |   |   |   |   |
| Status | ✓ µ | ✓ µ |   |   |   |   |   |   |
| Pontos da história |   | ✓ µ |   |   |   |   |   |   |
| Modelo | ✓ µ |   |   |   |   |   |   |   |
| URL | ✓ µ | ✓ µ |   | ✓ µ | ✓ µ |   |   |   |

{style="table-layout:auto"}

+++

1. No lado esquerdo da tela, localize a **Referência de campo nativo** e arraste-a para uma seção da tela.
1. No lado direito da tela, configure as opções do campo personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do campo. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios. Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td>
      <td> <p>(Obrigatório) Esse nome é a forma como o sistema identifica o campo. Ao configurar o campo pela primeira vez e digitar o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p>
      <p>Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>Digite quaisquer informações adicionais sobre o campo. Quando os usuários preencherem o formulário personalizado, poderão passar o mouse sobre o ícone de ponto de interrogação para exibir uma dica de ferramenta contendo as informações digitadas aqui.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo de referência</td> 
      <td><p>(Obrigatório) Selecione um campo nativo do Workfront.<p><p>Somente campos nativos para os objetos do formulário estão disponíveis. Por exemplo, se a lista Tipos de objeto na parte superior do designer do formulário mostrar Projeto, você poderá selecionar campos nativos para projetos, mas não campos específicos para tarefas.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Tamanho</td> 
      <td>(Opcional) Altere o tamanho de exibição do campo, conforme necessário.</td> 
     </tr> 
    </tbody> 
   </table>

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

### Adicionar arquivos do Adobe XD

Você pode adicionar um protótipo do Adobe XD diretamente a um formulário personalizado. Os usuários que trabalham com o objeto ao qual o formulário personalizado está anexado podem ver o arquivo do Adobe XD somente nas seguintes áreas:

* A área Detalhes do objeto (por exemplo, para um projeto, a área Detalhes do projeto)
* A caixa Editar do objeto, se ele tiver a nova aparência da experiência do Adobe Workfront (por exemplo, as caixas Editar projeto e Editar tarefa )

Para adicionar um arquivo Adobe XD:

1. No lado esquerdo da tela, localize o **Adobe XD** e arraste-o para uma seção da tela.
1. Digite ou edite qualquer uma das seguintes propriedades do widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do widget. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios. Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obrigatório) Esse nome é como o sistema identifica o widget. Quando você está configurando o widget pela primeira vez e digita o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p>
    <p>Para obter mais informações, consulte <a href="design-a-form.md#notes-on-field-names-and-labels">Notas sobre nomes e rótulos de campos</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obrigatório) Digite ou cole um link de protótipo XD válido.</p> 
      <p>Observação: a configuração Acesso ao link na guia Compartilhar no Adobe XD deve ser definida como Qualquer pessoa com o link. Caso contrário, os usuários não poderão visualizar o protótipo. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>Digite quaisquer informações adicionais sobre o widget. Quando os usuários preencherem o formulário personalizado, poderão passar o mouse sobre o ícone de ponto de interrogação para exibir uma dica de ferramenta contendo as informações digitadas aqui.
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamanho</td> 
      <td>(Opcional) Altere o tamanho de exibição do widget conforme necessário.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita a etapa anterior para adicionar outros campos ou widgets.

   ou

   Para copiar um campo, passe o mouse sobre um campo e clique no ícone de cópia.

   ![ícone de cópia](assets/copy-field.png)

1. Para salvar as alterações, clique em **Aplicar** e vá para outra seção para continuar criando o formulário.

   ou

   Clique em **Salvar e fechar**.

## Organizar e visualizar um formulário com o designer de formulário

Para obter informações sobre como organizar um formulário personalizado com quebras de seção e pré-visualizar o formulário, consulte [Organizar e pré-visualizar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
