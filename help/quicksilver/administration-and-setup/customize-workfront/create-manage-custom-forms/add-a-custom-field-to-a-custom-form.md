---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Adicionar um campo personalizado a um formulário personalizado com o construtor de formulários herdado
description: Quando estiver trabalhando em um formulário personalizado, você pode criar um novo campo personalizado e adicioná-lo a um formulário personalizado. Você também pode adicionar um campo personalizado que já foi adicionado a outro formulário personalizado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '2208'
ht-degree: 2%

---

# Adicionar um campo personalizado a um formulário personalizado com o construtor de formulários herdado

Quando estiver trabalhando em um formulário personalizado, você pode criar um novo campo personalizado e adicioná-lo a um formulário personalizado.

Você também pode adicionar um campo personalizado que já foi adicionado a outro formulário personalizado. Para obter instruções, consulte [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Para obter informações sobre como adicionar um widget de ativo a um formulário personalizado, que é um processo semelhante à adição de um campo personalizado, consulte [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>Em um formulário personalizado que contém vários campos personalizados ou várias opções de seleção múltipla em campos personalizados, os usuários podem enfrentar um desempenho mais lento ao adicionar ou alterar valores nesses campos. Por exemplo, um formulário que contém 100 campos personalizados ou campos personalizados de seleção múltipla com mais de 200 opções pode ser mais lento quando os usuários interagem com ele.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront*</p> </td> 
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

&#42;Para descobrir quais configurações de plano, tipo de licença ou nível de acesso você tem, entre em contato com o administrador do Workfront.

## Adicionar um campo personalizado a um formulário personalizado

1. Comece a criar ou editar um formulário personalizado, conforme descrito em [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Abra o **Adicionar um campo** guia.

   ![](assets/add-a-field.jpg)

1. Com **Novo campo** ![](assets/new-field.jpg) selecionado, selecione um dos tipos de campo listados abaixo:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Campo de texto de uma linha</td> 
      <td>Permite que os usuários digitem uma única linha de texto no campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo de texto em parágrafo</td> 
      <td>Permite que os usuários digitem várias linhas de texto no campo.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Campo de texto com formatação</td> 
      <td>Permite que os usuários digitem várias linhas de texto no campo e formatem o texto com negrito, itálico, sublinhado, marcadores, numeração, hiperlinks e aspas de bloco. Isso está disponível na Página inicial, na área Atualizações, em listas e na área Detalhes para objetos do Workfront. Um limite de 15.000 caracteres permite bastante texto e formatação.</p> <p>Para obter informações sobre como acessar esse campo por meio da API, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Armazenamento de campo Rich Text na API</a>.</p> <p><b>NOTA</b>: os campos de texto com formatação não estão disponíveis para aplicativos móveis Workfront (disponíveis nas próximas versões). </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suspenso</td> 
      <td>Fornece uma lista de opções suspensas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typeahead </td> 
      <td>Permite que os usuários digitem o nome de um objeto que existe no Workfront. Uma lista de sugestões é exibida quando o usuário começa a digitar.
      Esse tipo de campo oferece suporte aos seguintes objetos:
      <ul><li>Usuário</li>
      <li>Grupo</li>
      <li>Função de trabalho</li>
      <li>Portfólio</li>
      <li>Programa</li>
      <li>Projeto</li>
      <li>Equipe</li>
      <li>Modelo</li>
      <li>Empresa</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calculado</td> 
      <td>Permite definir uma expressão e exibir o resultado no formulário personalizado. Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Adicionar dados calculados a um formulário personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Data</td> 
      <td>Exibe um calendário onde os usuários podem selecionar uma data e hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Caixa de Seleção</td> 
      <td>Permite que os usuários selecionem várias opções.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botões de seleção</td> 
      <td>Exige que os usuários selecionem apenas uma opção.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto descritivo</td> 
      <td>Permite incluir instruções e vincular a páginas fora do Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quebra de seção</td> 
      <td>Na verdade, uma quebra de seção não é um campo. Você pode usar uma quebra de seção para organizar seus campos e widgets personalizados em seções e, se necessário, configurar diferentes permissões de exibição e edição para cada seção. Para obter informações sobre como adicionar e configurar quebras de seção, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Adicionar uma quebra de seção a um formulário personalizado</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. No **Configurações do campo** , configure as opções disponíveis para o tipo de campo personalizado que você está adicionando:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima do campo personalizado. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>(Obrigatório) Esse nome é a forma como o sistema identifica o campo personalizado ao adicioná-lo a várias áreas no Workfront, como relatórios, página inicial e interações de API.</p> <p>Ao configurar o campo personalizado pela primeira vez e digitar o rótulo, o campo Nome é preenchido automaticamente para corresponder a ele. Mas os campos Label e Name não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p> 
      <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Embora seja possível fazer isso, recomendamos que você não altere esse nome depois que você ou outros usuários começarem a usar o formulário personalizado no Workfront. Se você fizer isso, o sistema não reconhecerá mais o campo personalizado onde ele pode agora ser referenciado em outras áreas do Workfront. <p>Por exemplo, se você adicionar o campo personalizado a um relatório e depois alterar seu nome, o Workfront não o reconhecerá no relatório e ele deixará de funcionar corretamente lá, a menos que você o adicione novamente ao relatório usando o novo nome.</p> </li>
      <li> <p>Recomendamos que você não digite um nome que já esteja sendo usado para campos integrados do Workfront.</p> </li>
      <li><p>Recomendamos que você não use o caractere ponto no nome do campo personalizado para evitar erros ao usar o campo em diferentes áreas do Workfront.</p></li>
      </ul> <p>Cada nome de campo personalizado deve ser exclusivo na instância do Workfront da organização. Dessa forma, é possível reutilizar um que já foi criado para outro formulário personalizado. Para obter mais informações, consulte <a href="#Add" class="MCXref xref">Adicionar um campo personalizado a um formulário personalizado</a> neste artigo.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>Digite quaisquer informações adicionais sobre o campo personalizado. Quando os usuários preencherem o formulário personalizado, poderão passar o mouse sobre o ícone de ponto de interrogação para exibir uma dica de ferramenta contendo as informações digitadas aqui.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formatar</td> 
      <td> <p>Selecione o tipo de dados que será capturado no campo personalizado.</p> <p><b>Nota</b>:   
        <ul> 
         <li>Este campo não pode ser editado depois que o formulário é salvo. Se você pretende usar seu campo em cálculos matemáticos, certifique-se de selecionar um formato de Número ou Moeda.<br></li> 
         <li>Ao selecionar Número ou Moeda, o sistema trunca automaticamente os números que começam com 0.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Exibição</td> 
      <td>(Somente lista suspensa, caixas de seleção e botões de opção) Alterne o tipo de seleção de opção desejado para o campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamanho</td> 
      <td>(Somente campos de texto) Selecione uma largura para o campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir horário</td> 
      <td>(Somente campos de data) Selecione essa opção se desejar mostrar a hora do dia junto com a data no campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto referenciado</td> 
      <td> <p>(Somente campos de digitação antecipada) Selecione o tipo de objeto que deseja associar ao campo.</p> <p>Depois de clicar em Aplicar ou Salvar+Fechar, não é possível alterar o tipo de objeto do campo.</p> <p><b>Nota</b>:   
        <ul> 
         <li>Se o administrador do Workfront personalizou o nome de Portfolio, Programas ou Projetos na interface do usuário do Workfront, o nome padrão do Workfront para o objeto será exibido nessa lista suspensa, não no nome personalizado. Consulte o administrador do Workfront se precisar de ajuda com isso.<br></li> 
         <li>Os seguintes tipos de objeto são compatíveis com os aplicativos móveis Workfront para iOS e Android: usuário, empresa, grupo, função de trabalho, Portfolio, programa, projeto e modelo.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Adicionar Filtro</td> 
      <td> <p>(Somente campos de digitação antecipada) Adicione um filtro para um tipo de objeto para limitar os objetos que os usuários podem escolher quando estiverem usando o campo. </p> <p>Por exemplo, é possível limitar um campo para que os nomes de usuários possam ser selecionados somente se atenderem aos seguintes critérios:</p> 
       <ul> 
        <li>Eles pertencem a um ou mais grupos especificados por você</li> 
        <li>Eles estão associados a uma função ou a um cargo especificado por você</li> 
        <li>Eles pertencem ao mesmo grupo que a pessoa que está usando o campo</li> 
       </ul> <p>Você deve definir o filtro para o tipo de objeto selecionado usando a sintaxe do Modo de texto. Para obter informações sobre como criar um filtro usando o Modo de texto, consulte a seção <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">Modo de edição de texto em um filtro</a> no artigo <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Visão geral do modo de texto</a>. </p> <p><b>Nota</b>:   
        <ul> 
         <li>Se você estiver editando um formulário personalizado existente, adicionar um filtro a um campo Digitação antecipada não removerá nenhum objeto (fora do escopo do filtro) que os usuários já tenham adicionado usando o campo.</li> 
         <li>Este filtro não está disponível em dispositivos móveis. Se você usar o filtro para um campo Digitação antecipada, o campo aparecerá nos dispositivos móveis dos usuários não afetados pelo filtro.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto descritivo</td> 
      <td>(Somente campos de Texto descritivo) Digite o texto que deseja exibir para fornecer instruções ou um link no formulário personalizado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hiperlink</td> 
      <td>(Somente campos de Texto descritivo) Se quiser aplicar um hiperlink ao Texto descritivo digitado, adicione-o aqui.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Criar um campo obrigatório</td> 
      <td>Selecione essa opção se desejar que o campo seja obrigatório para que o usuário preencha o formulário personalizado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rastrear alterações de campo nos campos de atualização</td> 
      <td><p>Clique na lista suspensa e selecione os tipos de objeto nos quais deseja rastrear automaticamente as alterações de valor do campo.</p> 
      <p><b>NOTA</b>: Essa opção não está disponível para o seguinte:</p> 
      <ul> 
      <li>Formulários personalizados associados aos seguintes tipos de objeto: Despesa, Empresa, Iteração, Registro de Cobrança e Grupo.</li> 
      <li>Os seguintes tipos de campo: Calculado, Texto descritivo e Quebra de seção</li> 
      </ul>
      <p><b>IMPORTANTE</b>: selecionar ou desmarcar um tipo de objeto aqui afeta todos os formulários personalizados associados ao tipo de objeto selecionado e que contêm esse campo. Por exemplo, se você desmarcar um tipo de objeto aqui e salvar o formulário personalizado, as alterações no valor do campo não serão mais rastreadas para esse tipo de objeto em nenhum formulário personalizado que contenha o campo.</p>
       <p>Depois de selecionar um tipo de objeto aqui para um campo e salvar o formulário personalizado, o campo é exibido na guia Campos personalizados na área Feeds de atualização em Configuração.</p> 
       <p>Por outro lado, se esse campo for excluído na área Feeds de atualização da Configuração, o tipo de objeto dessa configuração será desmarcado em todos os formulários personalizados associados ao tipo de objeto e que contenham esse campo.</p> 
       <p>Para obter mais informações, consulte a seção <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">Adicionar campos que você deseja que o Workfront rastreie</a> no artigo <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">Configurar atualizações do sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adicionar Lógica</td> 
      <td>Especifique quais campos devem aparecer no formulário, com base nas seleções que os usuários fazem nos campos existentes. Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Adicionar lógica de exibição e lógica de salto a um formulário personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seleções </td> 
      <td> <p>(Suspenso, Caixas de seleção ou Botões de opção somente; opcional)</p> 
       <ol> 
        <li> <p>Clique em <b>Opções</b>, ative uma das opções a seguir:</p> 
           <ul> 
            <li><strong>Mostrar valores</strong>: mostra os valores de cada escolha no campo. O rótulo de cada opção é exibido por padrão.</li> 
            <li><strong>Classificar seleções de A a Z</strong>: classifica as opções adicionadas em ordem alfabética no campo.</li> 
           </ul> 
        </li> 
        <li> <p>Para cada opção adicionada para o usuário, clique no ícone de engrenagem <img src="assets/gear-icon-settings.png">, em seguida, selecione uma das seguintes opções:</p> 
           <ul> 
            <li><strong>Selecionar por padrão</strong>: selecione a opção por padrão no campo.</li> 
            <li> <p><strong>Ocultar seleção</strong>: oculte a escolha no campo. As opções ocultas permanecem acessíveis nos relatórios.</p> </li> 
            <li> <p><strong>Remover seleção</strong>: remova a escolha do campo.</p> <p><b>AVISO</b>: se você tiver objetos atuais usando essa opção, não remova-a do campo. Sua remoção fará com que os dados do histórico sejam perdidos. Em vez disso, selecione a opção para ocultá-la, o que impede que os usuários a selecionem no futuro.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Para alterar o tipo de exibição de um campo no formulário personalizado, clique no **Tipo de exibição** e, em seguida, clique no tipo desejado.

   Você pode alternar entre os seguintes tipos de exibição de campo:

   * **Campos do tipo seleção**: Caixas De Seleção, Lista Suspensa, Botões De Opção.
   * **Campos do tipo texto**: Campo De Texto De Linha Única, Campo De Texto De Parágrafo. (Você não pode alternar um Campo de texto com Formatação para um tipo de exibição diferente. No entanto, você pode removê-lo e adicionar outro tipo de campo.)

   Por exemplo, se você criou um campo Checkboxes, é possível alterá-lo para um campo Suspenso ou um campo Radio Buttons. Ou, se você tiver criado um Campo de texto de linha única, poderá alterá-lo para um campo de texto de parágrafo.

   >[!NOTE]
   >
   >Considere o seguinte quando quiser alterar o tipo de exibição de um campo de caixa de seleção ou de um campo suspenso de várias seleções (uma lista suspensa que permite que mais de uma opção seja selecionada) para um tipo de campo de seleção única:
   >
   >* Se você alterar para Botões de opção, o Workfront manterá quaisquer valores de seleção múltipla que um usuário possa ter inserido no campo até que o usuário altere e salve dados em qualquer parte do formulário. Nesse ponto, todos os valores que foram selecionados usando o campo do tipo de seleção múltipla são substituídos pelo valor do Botão de opção selecionado.
   >* Se você alterar para uma lista suspensa de seleção única, o Workfront manterá todos os valores de seleção múltipla que um usuário pode ter inserido no campo até que o usuário altere e salve os valores no campo. Nesse ponto, todos os valores que foram selecionados usando o campo do tipo de seleção múltipla são substituídos pelo valor selecionado na lista suspensa.


1. (Opcional) Repita as etapas 2 a 6 para adicionar outros campos personalizados.

   Ou

   Adicione campos que já foram criados para sua organização, conforme explicado em [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >Você pode adicionar até 500 campos e widgets em um único formulário personalizado. No entanto, a degradação do desempenho pode ocorrer quando existem mais de 100 em um formulário, dependendo de sua complexidade. Exemplos de formulários complexos incluem formulários com parâmetros em cascata, campos de dados personalizados calculados e várias opções de valor em um único campo.

1. Clique em **Aplicar**.
1. Se quiser continuar criando seu formulário personalizado de outras maneiras, continue com um dos seguintes artigos:

   * [Posicionar campos e widgets personalizados em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Adicionar uma quebra de seção a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Reutilizar um campo personalizado calculado existente em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Adicionar lógica de exibição e lógica de salto a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Pré-visualizar e preencher um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
