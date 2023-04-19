---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Adicionar um campo personalizado a um formulário personalizado com o construtor de formulários herdado
description: Ao trabalhar em um formulário personalizado, você pode criar um novo campo personalizado e adicioná-lo a um formulário personalizado. Também é possível adicionar um campo personalizado que já foi adicionado a outro formulário personalizado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: f9fce2715cad3e2ea2bf16de5f4ba457f981725c
workflow-type: tm+mt
source-wordcount: '2264'
ht-degree: 3%

---

# Adicionar um campo personalizado a um formulário personalizado com o construtor de formulários herdado

Ao trabalhar em um formulário personalizado, você pode criar um novo campo personalizado e adicioná-lo a um formulário personalizado.

Também é possível adicionar um campo personalizado que já foi adicionado a outro formulário personalizado. Para obter instruções, consulte [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Para obter informações sobre como adicionar um widget de ativo a um formulário personalizado, que é um processo semelhante à adição de um campo personalizado, consulte [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>Em um formulário personalizado que contém vários campos personalizados ou várias opções de seleção múltipla em campos personalizados, os usuários podem experimentar um desempenho mais lento ao adicionar ou alterar valores nesses campos. Por exemplo, um formulário contendo 100 campos personalizados ou vários campos personalizados com mais de 200 opções podem ser mais lentos quando os usuários interagem com ele.

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

## Adicionar um campo personalizado a um formulário personalizado

1. Comece a criar ou editar um formulário personalizado, conforme descrito em [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Abra o **Adicionar um campo** guia .

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
      <td>Permite que os usuários digitem várias linhas de texto no campo e formatem o texto com negrito, itálico, sublinhado, marcadores, numeração, hiperlinks e aspas de bloco. Isso está disponível na Página inicial, na área Atualizações, nas listas e na área Detalhes para objetos Workfront. Um limite de 15.000 caracteres permite bastante texto e formatação.</p> <p>Para obter informações sobre como acessar esse campo por meio da API, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Armazenamento de campo de texto formatado na API</a>.</p> <p><b>OBSERVAÇÃO</b>: Campos de texto com formatação não estão disponíveis para aplicativos móveis Workfront (disponíveis em próximas versões). </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Suspenso</td> 
      <td>Fornece uma lista de opções suspensas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typeahead </td> 
      <td>Permite que os usuários digitem o nome de um objeto existente no Workfront. Uma lista de sugestões é exibida quando o usuário começa a digitar.
      Esse tipo de campo oferece suporte para os seguintes objetos:
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
      <td>Exibe um calendário em que os usuários podem selecionar uma data e hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Caixa de Seleção</td> 
      <td>Permite que os usuários selecionem várias opções.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botões de seleção</td> 
      <td>Requer que os usuários selecionem apenas uma opção.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto descritivo</td> 
      <td>Permite incluir instruções e vincular a páginas fora do Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Quebra de seção</td> 
      <td>Na verdade, uma quebra de seção não é um campo. Você pode usar uma quebra de seção para organizar os campos e widgets personalizados em seções e, se necessário, configurar diferentes permissões de visualização e edição para cada seção. Para obter informações sobre adicionar e configurar quebras de seção, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Adicionar uma quebra de seção a um formulário personalizado</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. No **Configurações de campo** , configure as opções disponíveis para o tipo de campo personalizado que você está adicionando:

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
      <td> <p>(Obrigatório) Esse nome é como o sistema identifica o campo personalizado quando você o adiciona a várias áreas em todo o Workfront, como relatórios, Início e interações da API.</p> <p>Ao configurar o campo personalizado pela primeira vez e digitar o rótulo, o campo Nome é preenchido automaticamente para correspondência. Mas os campos Rótulo e Nome não são sincronizados — isso dá a você a liberdade de alterar o rótulo que seus usuários veem sem precisar alterar o nome que o sistema vê.</p> 
      <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Embora seja possível fazer isso, recomendamos que você não altere esse nome depois que você ou outros usuários começarem a usar o formulário personalizado no Workfront. Nesse caso, o sistema não reconhecerá mais o campo personalizado, onde agora pode ser referenciado em outras áreas do Workfront. <p>Por exemplo, se você adicionar o campo personalizado a um relatório e depois alterar seu nome, o Workfront não o reconhecerá no relatório e ele deixará de funcionar corretamente lá, a menos que você o adicione novamente ao relatório usando o novo nome.</p> </li>
      <li> <p>Recomendamos que você não digite um nome que já esteja sendo usado em campos integrados do Workfront.</p> </li>
      <li><p>Recomendamos que você não use o caractere ponto/ponto no nome do campo personalizado para evitar erros ao usar o campo em diferentes áreas do Workfront.</p></li>
      </ul> <p>Cada nome de campo personalizado deve ser exclusivo na instância do Workfront de sua organização. Dessa forma, é possível reutilizar um que já foi criado para outro formulário personalizado. Para obter mais informações, consulte <a href="#Add" class="MCXref xref">Adicionar um campo personalizado a um formulário personalizado</a> neste artigo.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Instruções</td> 
      <td> <p>Digite quaisquer informações adicionais sobre o campo personalizado. Quando os usuários preenchem o formulário personalizado, eles podem passar o mouse sobre o ícone de ponto de interrogação para visualizar uma dica de ferramenta com as informações digitadas aqui.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formatar</td> 
      <td> <p>Selecione o tipo de dados que será capturado no campo personalizado. É possível alterar a seleção de formato após salvar o formulário, mas o novo formato deve oferecer suporte ao valor inserido.</p>

   <p><strong>Exemplo:</strong> Se você salvar um valor numérico para um campo com formato Text em pelo menos um objeto e depois alterar o formato para Number ou Currency, um erro não será encontrado. </p>
      <p>No entanto, se você salvar um valor alfanumérico em um campo com formato de Texto em pelo menos um objeto e tentar alterar o formato para Número ou Moeda, ocorrerá um erro, pois o valor alfanumérico salvo não é compatível com os formatos Número ou Moeda. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Exibição</td> 
      <td>(Somente para botões de opção, caixas de seleção e botões de opção) Alterne o tipo de seleção de opção desejada para o campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamanho</td> 
      <td>(Somente campos de texto) Selecione uma largura para o campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir horário</td> 
      <td>(Somente campos de data) Selecione essa opção se desejar mostrar a hora do dia junto com a data no campo .</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto referenciado</td> 
      <td> <p>(Somente campos Digitar) Selecione o tipo de objeto que deseja associar ao campo.</p> <p>Depois de clicar em Aplicar ou Salvar+Fechar, não será possível alterar o tipo de objeto do campo.</p> <p><b>Nota</b>:   
        <ul> 
         <li>Se o administrador do Workfront personalizou o nome de Portfolio, Programas ou Projetos na interface do usuário do Workfront, o nome padrão do Workfront para o objeto será exibido nessa lista suspensa, não no nome personalizado. Consulte o administrador do Workfront se precisar de ajuda com isso.<br></li> 
         <li>Os seguintes tipos de objeto são compatíveis com os aplicativos móveis iOS e Android Workfront: Usuário, Empresa, Grupo, Função do trabalho, Portfolio, Programa, Projeto e Modelo.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Adicionar Filtro</td> 
      <td> <p>(Somente campos Digitar) Adicione um filtro para um tipo de objeto para limitar os objetos que os usuários podem escolher ao usar o campo. </p> <p>Por exemplo, é possível limitar um campo para que os nomes de usuário possam ser selecionados apenas se atenderem aos seguintes critérios:</p> 
       <ul> 
        <li>Eles pertencem a um grupo ou grupos especificados por você</li> 
        <li>Eles estão associados a uma função ou cargo especificado por você</li> 
        <li>Eles pertencem ao mesmo grupo que a pessoa que usa o campo</li> 
       </ul> <p>Você deve definir o filtro para o tipo de objeto selecionado usando a sintaxe do Modo de texto . Para obter informações sobre como criar um filtro usando o Modo de texto, consulte a seção <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">Editar modo de texto em um filtro</a> no artigo <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">Visão geral do modo de texto</a>. </p> <p><b>Nota</b>:   
        <ul> 
         <li>Se você estiver editando um formulário personalizado existente, adicionar um filtro a um campo Digitar não removerá objetos (fora do escopo do filtro) que os usuários já adicionaram usando o campo.</li> 
         <li>Este filtro não está disponível em dispositivos móveis. Se você usar o filtro para um campo Digitar , o campo aparecerá nos dispositivos móveis dos usuários não afetados pelo filtro.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto descritivo</td> 
      <td>(Somente campos de texto descritivo) Digite o texto que deseja exibir para fornecer instruções ou um link no formulário personalizado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hiperlink</td> 
      <td>(Somente campos de Texto descritivo) Se quiser aplicar um hiperlink ao Texto descritivo digitado, adicione-o aqui.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tornar um campo obrigatório</td> 
      <td>Selecione essa opção se desejar que o campo seja obrigatório para que o usuário preencha o formulário personalizado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rastrear alterações de campo nos campos de atualização</td> 
      <td><p>Clique na lista suspensa e selecione os tipos de objeto nos quais você deseja rastrear automaticamente as alterações de valor do campo.</p> 
      <p><b>OBSERVAÇÃO</b>: Essa opção não está disponível para o seguinte:</p> 
      <ul> 
      <li>Formulários personalizados associados aos seguintes tipos de objetos: Despesa, Empresa, Iteração, Registro de Faturamento e Grupo.</li> 
      <li>Os seguintes tipos de campo: Calculadas , texto descritivo e quebra de seção</li> 
      </ul>
      <p><b>IMPORTANTE</b>: Selecionar ou desmarcar um tipo de objeto aqui afeta todos os formulários personalizados que estão associados ao tipo de objeto selecionado e que contêm esse campo. Por exemplo, se você desmarcar um tipo de objeto aqui e salvar o formulário personalizado, as alterações no valor do campo não serão mais rastreadas para esse tipo de objeto em qualquer formulário personalizado que contenha o campo.</p>
       <p>Depois de selecionar um tipo de objeto aqui para um campo e salvar o formulário personalizado, o campo é exibido na guia Campos personalizados, na área Atualizar feeds, em Configurar.</p> 
       <p>Por outro lado, se esse campo for excluído na área Atualizar feeds da Configuração, o tipo de objeto para essa configuração será desmarcado em todos os formulários personalizados que estão associados ao tipo de objeto e que contêm esse campo.</p> 
       <p>Para obter mais informações, consulte a seção <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">Adicionar campos que você deseja que o Workfront rastreie</a> no artigo <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">Configurar atualizações do sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adicionar Lógica</td> 
      <td>Especifique quais campos devem aparecer no formulário, com base nas seleções que os usuários fazem nos campos existentes. Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Adicionar lógica de exibição e ignorar lógica a um formulário personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seleções </td> 
      <td> <p>(Apenas lista suspensa, caixas de seleção ou botões de opção; opcional)</p> 
       <ol> 
        <li> <p>Clique em <b>Opções</b>, em seguida, ative uma das seguintes opções:</p> 
           <ul> 
            <li><strong>Mostrar valores</strong>: Mostra os valores de cada escolha no campo . O rótulo de cada escolha é exibido por padrão.</li> 
            <li><strong>Classificar opções A-Z</strong>: Classifica as opções adicionadas alfabeticamente no campo .</li> 
           </ul> 
        </li> 
        <li> <p>Para cada escolha que você adicionar para o usuário, clique no ícone de engrenagem <img src="assets/gear-icon-settings.png">e selecione uma das seguintes opções:</p> 
           <ul> 
            <li><strong>Selecionar por padrão</strong>: Selecione a escolha por padrão no campo .</li> 
            <li> <p><strong>Ocultar Escolha</strong>: Oculte a escolha no campo . As opções ocultas permanecem acessíveis nos relatórios.</p> </li> 
            <li> <p><strong>Remover Escolha</strong>: Remova a opção do campo .</p> <p><b>AVISO</b>: Se você tiver objetos atuais usando essa opção, não os remova do campo. A remoção fará com que os dados históricos sejam perdidos. Em vez disso, selecione a opção para ocultá-la, o que impede que os usuários a selecionem no futuro.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Para alterar o tipo de exibição de um campo no formulário personalizado, clique no botão **Tipo de exibição** no menu suspenso e, em seguida, clique no tipo desejado.

   Você pode alternar entre os seguintes tipos de exibição de campo:

   * **Campos do tipo seleção**: Caixas de seleção, Suspensa, Botões de opção.
   * **Campos do tipo texto**: Campo de texto de linha única, Campo de texto do parágrafo. (Não é possível alternar um Campo de texto com Formatação para um tipo de exibição diferente. No entanto, é possível removê-lo e adicionar outro tipo de campo.)

   Por exemplo, se você criou um campo Caixas de seleção, é possível alterá-lo para um campo Suspenso ou para um campo Botões de opção. Ou, se você tiver criado um Campo de texto de linha única, poderá alterá-lo para um campo de Texto de parágrafo.

   >[!NOTE]
   >
   >Considere o seguinte quando quiser alterar o tipo de exibição de um campo de caixa de seleção ou de um campo suspenso de várias seleções (uma lista suspensa que permite a seleção de mais de uma opção) para um tipo de campo de seleção única:
   >
   >* Se você alterar para Botões de opção, o Workfront retém quaisquer valores de seleção múltipla que um usuário possa ter inserido no campo até que o usuário altere e salve os dados em qualquer parte do formulário. Neste ponto, os valores que foram selecionados usando o campo de tipo multisseleção são substituídos pelo valor do botão de opção selecionado.
   >* Se você alterar para uma lista suspensa de seleção única, o Workfront retém quaisquer valores de seleção múltipla que um usuário possa ter inserido no campo até que o usuário altere e salve os valores no campo. Neste ponto, qualquer valor que tenha sido selecionado usando o campo de tipo multiseleção é substituído pelo valor Suspenso selecionado.


1. (Opcional) Repita as etapas 2 a 6 para adicionar outros campos personalizados.

   Ou

   Adicione campos que já foram criados para sua organização, como explicado em [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >É possível adicionar até 500 campos e widgets em um único formulário personalizado. No entanto, pode ocorrer degradação do desempenho quando houver mais de 100 em um formulário, dependendo de sua complexidade. Exemplos de formulários complexos incluem formulários com parâmetros em cascata, campos de dados personalizados calculados e várias opções de valor em um único campo.

1. Clique em **Aplicar**.
1. Se quiser continuar criando seu formulário personalizado de outras maneiras, continue com um dos seguintes artigos:

   * [Posicionar campos e widgets personalizados em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Adicionar uma quebra de seção a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Reutilizar um campo personalizado calculado existente em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Adicionar lógica de exibição e ignorar lógica a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Visualizar e preencher um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
