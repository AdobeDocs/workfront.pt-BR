---
title: Criar campos
description: No Adobe Maestri, você pode criar campos personalizados para cada tipo de tipo de registro operacional ou taxonomia. Você pode então associar o campo com registros Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '2555'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# Criar campos

>[!IMPORTANT]
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

No Adobe Maestri, você pode criar campos personalizados para tipos de registros operacionais ou taxonomias. Você pode associar os campos aos registros do Maestro para aprimorar as informações dos registros.

Você deve criar tipos de registro antes de criar campos para associar a eles. Para obter informações, consulte [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> produto Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer Um</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer Um</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer Um</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/grant-access.md">Conceder acesso ao Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Considerações sobre campos Maestro

* Você pode criar campos somente a partir da exibição de tabela de uma página do tipo registro. Os campos são exibidos como colunas na exibição de tabela.

  Para obter informações sobre o gerenciamento de colunas de tabela (ou campos de registro), consulte [Gerenciar a exibição de tabela](../views/manage-the-table-view.md).

  Para obter informações sobre como gerenciar campos, consulte também os seguintes artigos:

   * [Editar campos](../architecture-and-fields/edit-fields.md)
   * [Excluir campos](./delete-fields.md)

* Os campos associados a um tipo de registro estão disponíveis para serem associados a todos os registros desse tipo. <!--will this change and will the fields be available for other record types, too?! Also, the next bullet might need to change too if this one changes -->

* Campos associados a um tipo de registro não podem ser adicionados a outro tipo de registro. <!-- this will change when they open the Field library tab when creating a field-->

* Você pode criar campos manual ou automaticamente das seguintes maneiras:

   * Manual:

      * Adicionando colunas na visualização Tabela de uma página do tipo registro. As colunas da tabela são os campos associados ao tipo de registro. São os mesmos campos exibidos na página Detalhes de um registro.

        Não é possível criar campos a partir da página Detalhes de um registro.

        Este artigo descreve como criar campos manualmente.

      * Vinculando tipos de registro. Você pode criar campos de registro vinculados ao adicionar uma nova conexão entre dois tipos de registro Maestri ou um tipo de registro e tipos de objeto de outras aplicações.

        <!--* Importing record types with fields using a CSV or an Excel file. - this is not available yet-->

        Para obter mais informações sobre como conectar tipos de registros Maestri, consulte [Conectar tipos de registro](../architecture-and-fields/connect-record-types.md).

      * Importando tipos de registro usando um arquivo Excel ou CSV. Para obter mais informações, consulte [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

   * Automaticamente:

      * Por padrão, sempre que você cria um tipo de registro.

        A seguir estão campos padrão criados por padrão para cada novo tipo de registro operacional:

         * Nome
         * Descrição
         * Data de início
         * Data Final
         * Status. Os valores padrão para status de registro são:
            * Desenvolvimento
            * Planejado
            * Ativo
            * Concluídos
            * Em Espera

           É possível adicionar mais valores ou renomear os existentes.

        A seguir estão os campos padrão criados por padrão para cada novo tipo de registro de taxonomia:

         * Nome <!--will more be added? If not, consider rephrasing this bullet-->

      * Ao criar um espaço de trabalho a partir de um modelo. O Maestri cria campos para tipos de registros operacionais e taxonomias quando você cria um espaço de trabalho a partir de um modelo. Para obter informações, consulte [Criar espaços de trabalho](../architecture-and-fields/create-workspaces.md).



* É possível exibir e atualizar as configurações dos campos que você ou qualquer outro usuário criou. <!--this will change with access/ permissions-->

* É possível ter até 500 campos para um tipo de registro.

* Os nomes de campos podem ter até 250 caracteres.

* Ao excluir um tipo de registro operacional, taxonomia ou espaço de trabalho, todos os campos associados a eles e aos valores dos campos também são excluídos e não podem ser recuperados. <!-- this might change with a possible recycle bin solution?!-->


## Criar campos do zero {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito do Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> e clique em **Maestro** ![](assets/maestro-icon.png).

   O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho cujos tipos de registro você deseja criar campos e, em seguida, clique no tipo de registro.

   Todos os registros existentes associados ao tipo de registro são exibidos nas linhas da exibição de tabela.

   >[!TIP]
   >
   >    Se nenhum registro for exibido, talvez você ainda não tenha nenhum registro ou um filtro aplicado que limite o que você vê na tela.

   Todos os campos existentes associados ao tipo de registro são exibidos nas colunas da exibição de tabela. <!--caveat this for when we can hide the fields; mention that they can be hidden if they are not visible by default-->


1. Clique em **+** ícone no canto superior direito da exibição de tabela para adicionar novos campos.
1. No **Novo campo** selecione entre os seguintes tipos de campo:

   * [Texto de linha única](#single-line-text)
   * [Parágrafo](#paragraph)
   * [Seleção múltipla](#multi-select)
   * [Seleção única](#single-select)
   * [Data](#date)
   * [Número](#number)
   * [Percentagem](#percentage)
   * [Moeda](#currency)
   * [Caixa de seleção](#checkbox)

   >[!IMPORTANT]
   >
   >    Não é possível alterar o tipo Field do campo depois de salvá-lo.

1. Continue adicionando cada campo, conforme descrito nas seções abaixo.

### Texto de linha única {#single-line-text}

Os campos de texto de linha única capturam informações alfanuméricas limitadas. Por exemplo, você pode capturar as informações de Proprietário, Participante, Equipe ou Unidade organizacional em um campo de texto de linha única. O conteúdo de um campo de texto de linha única pode ter até 250 caracteres. <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Texto em linha única** tipo de campo.

   ![](assets/single-line-text-field-type.png)

1. Adicione as seguintes informações:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida ao passar o mouse sobre o cabeçalho da coluna do campo em uma tabela.
1. Clique em **Criar**.

   O novo campo de linha única é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.


### Parágrafo {#paragraph}

Os campos de parágrafo capturam informações alfanuméricas adicionais sobre um registro, semelhantes ao campo Descrição. O conteúdo de um campo de parágrafo pode ter até 1.000 caracteres.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Parágrafo** tipo de campo.

   ![](assets/paragraph-field-type.png)


1. Adicione as seguintes informações:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
1. Clique em **Criar**.

   O novo campo de parágrafo é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.


### Seleção múltipla {#multi-select}

Você pode usar um campo de seleção múltipla para capturar informações adicionais em qualquer formato selecionando mais de uma opção em um menu suspenso.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Multisseleção** tipo de campo.

   ![](assets/multi-select-field-type.png)


1. Adicione as seguintes informações:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Opções**: as opções disponíveis para seleção no menu suspenso após salvar o campo. Você pode ter números e letras para o nome de cada escolha.
1. Clique em **Adicionar opção** para adicionar quantas opções forem necessárias. Não há limite para quantas opções você pode adicionar a um campo de seleção múltipla.
1. (Opcional) Arraste e solte manualmente cada escolha na ordem desejada ou selecione a opção
   **Classificar seleções de A a Z** opção se desejar que as opções sejam listadas automaticamente em ordem alfabética. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Clique em **x** ícone à direita de uma opção para removê-lo.
1. Clique na amostra de cores à esquerda de uma opção para expandir o seletor de cores e personalizar a cor de cada opção.
1. Clique em **Criar**.

   O novo campo de seleção múltipla é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.

### Seleção única {#single-select}

Os campos de seleção única capturam informações adicionais em qualquer formato ao selecionar uma opção em um menu suspenso.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Seleção única** tipo de campo.

   ![](assets/single-select-field-type.png)


1. Adicione as seguintes informações:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Opções**: as opções disponíveis para seleção no menu suspenso após salvar o campo. Você pode ter números e letras para o nome de cada escolha.

1. Clique em **Adicionar opção** para adicionar quantas opções forem necessárias. Não há limite para quantas opções você pode adicionar a um campo de seleção única.
1. (Opcional) Arraste e solte manualmente cada escolha na ordem desejada ou selecione a opção **Classificar seleções de A a Z** opção se desejar que as opções sejam listadas automaticamente em ordem alfabética. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Clique em **x** ícone à direita de uma opção para removê-lo.
1. Clique na amostra de cores à esquerda de uma opção para expandir o seletor de cores e personalizar a cor de cada opção.
1. Clique em **Criar**.

   O novo campo de seleção única é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.

### Data {#date}

Você pode usar um campo de data para capturar informações adicionais no formato de data e hora.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Data** tipo de campo.

   ![](assets/date-field-type.png)


1. Adicione as seguintes informações:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Formato de data**: o tipo de formato de data que você deseja exibir nesse campo.

     Selecione entre os seguintes formatos:
      * **Localidade**: corresponde à localidade do seu navegador.
      * **Padrão**: 16/05/2023
      * **Longo**: 16 de maio de 2023
      * **Europeu**: 05/16/2023
      * **ISO**: 16/05/2023
   * **Incluir um campo de tempo**: selecione essa opção se desejar incluir um carimbo de data e hora. Essa opção não está selecionada por padrão.

     Selecione entre as seguintes opções:

      * **24h**: Por exemplo: 18:00
      * **12 h**: Por exemplo: 18:00

1. Clique em **Criar**.

   O novo campo de data é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.

### Número {#number}

Os tipos de campo de número capturam informações em um formato de número.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Número** tipo de campo.

   ![](assets/number-field-type.png)
1. Adicione as seguintes informações:

   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro.
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Precisão**: o número de decimais que você deseja gravar para o campo. É possível exibir até 6 decimais.
   * **Permitir números negativos**: selecione essa opção se desejar permitir números negativos nesse campo. Essa opção não está selecionada por padrão.

   >[!NOTE]
   >
   >    Se você selecionar Permitir números negativos e valores negativos forem armazenados nos registros aos quais o campo está anexado, não será mais possível desmarcar a configuração no futuro.

1. Clique em **Criar**.

   O novo campo de número é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.

### Percentagem {#percentage}

Os tipos de campo Porcentagem capturam informações em um formato de número seguido por um sinal de porcentagem.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Porcentagem** tipo de campo.

   ![](assets/percentage-field-type.png)

1. Adicione as seguintes informações:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro.
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Precisão**: o número de decimais que você deseja gravar para o campo. É possível exibir até 6 decimais.
   * **Permitir números negativos**: selecione esta opção se desejar permitir valores percentuais negativos neste campo. Essa opção não está selecionada por padrão.

   >[!NOTE]
   >
   >    Se você selecionar Permitir números negativos e valores negativos forem armazenados nos registros aos quais o campo está anexado, não será mais possível desmarcar a configuração no futuro.

1. Clique em **Criar**.

   O novo campo de porcentagem é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.

### Moeda {#currency}

Os tipos de campo Moeda capturam as informações em um formato de número precedido por um símbolo de moeda.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Moeda** tipo de campo.

   ![](assets/currency-field-type.png)

1. Adicione as seguintes informações:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Moeda**: o tipo de moeda que você deseja exibir neste campo. Esta é uma lista de moedas de acordo com a Organização Internacional de Normalização (ISO).
   * **Precisão**: o número de decimais que você deseja gravar para o campo. É possível exibir até 6 decimais.
   * **Permitir números negativos**: selecione esta opção se desejar permitir valores de moeda negativos neste campo. Essa opção não está selecionada por padrão.

   >[!NOTE]
   >
   >    Se você selecionar Permitir números negativos e valores negativos forem armazenados nos registros aos quais o campo está anexado, não será mais possível desmarcar a configuração no futuro.

1. Clique em **Criar**.

   O novo campo de moeda é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.

### Caixa de seleção

Você pode usar o tipo de campo Caixa de seleção para adicionar uma única opção de caixa de seleção a um registro. Você pode usar esse campo para indicar um atributo ou status específico para esse registro específico. Por exemplo, você pode usá-lo como um sinalizador para rastrear a conclusão, a aprovação ou qualquer outro atributo binário para cada registro.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Caixa de seleção** tipo de campo.

   ![](assets/checkbox-field-type.png)

1. Adicione as seguintes informações:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
1. Clique em **Criar**.

   O novo campo de caixa de seleção é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros. O campo também é exibido na página Detalhes de um registro.

## Criar campos vinculando tipos de registro

Você pode criar campos de registro vinculados ao adicionar uma nova conexão entre dois tipos de registro Maestri ou um tipo de registro e tipos de objeto de outras aplicações.

Para obter informações sobre como conectar tipos de registros Maestri, consulte [Conectar tipos de registro](../architecture-and-fields/connect-record-types.md).

## Criar campos importando tipos de registro usando um arquivo Excel e CSV

Para obter mais informações, consulte [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

## Criar campos criando um tipo de registro

Ao criar um tipo de registro, vários campos associados ao novo tipo de registro também são criados por padrão. Para obter mais informações, consulte [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

## Criar campos criando um espaço de trabalho a partir de um modelo

O Maestri cria campos para tipos de registros operacionais e taxonomias quando você cria um espaço de trabalho a partir de um modelo.

Para obter informações, consulte [Criar espaços de trabalho](../architecture-and-fields/create-workspaces.md).



