---
title: Criar campos
description: No Adobe Maestri, você pode criar campos personalizados para cada tipo de tipo de registro operacional ou taxonomia. Você pode então associar o campo com registros Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7e2bb0ee-5f25-4307-9fec-876590c0ae1a
source-git-commit: 6f026590f0030b564f0d110afead9ade1acd7896
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Formula fields
description: In Adobe Maestro, you can create custom fields for each kind of operational record type or taxonomy. You can then associate the field with Maestro records.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

<!--Should the structure of this article be like this one: https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/customize/custom-forms/custom-form-builder/use-the-custom-form-builder/add-a-custom-field-to-a-custom-form.html?lang=en ??-->

<!--will they add a way to create fields elsewhere than in a table?! - how will that change the structure of this article? -->

# Criar campos

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

No Adobe Maestri, você pode criar campos personalizados para tipos de registros operacionais ou taxonomias. Você pode associar os campos aos registros do Maestro para aprimorar as informações dos registros.

Você deve criar tipos de registro antes de criar campos para associar a eles. Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

Você pode criar campos das seguintes maneiras no Maestro:

* Do zero
* Conectando tipos de registro
* Importando tipos de registro usando um arquivo Excel e CSV
* Criando um tipo de registro
* Criando um espaço de trabalho a partir de um modelo

Para obter mais informações sobre campos Maestro, consulte [Visão geral do campo](../fields/fields-overview.md)

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
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Modelo de layout</td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/grant-access.md">Conceder acesso ao Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Criar campos do zero {#create-fields-from-scratch}

<!--in a table (not sure if this can be done elsewhere?!-->

{{step1-to-maestro}}

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
   * [Pessoas](#people)
   * [Criado por](#created-by)
   * [Data de criação](#created-date)
   * [Modificado pela última vez por](#last-modified-by)
   * [Data da última modificação](#last-modified-date)

   >[!IMPORTANT]
   >
   >    Não é possível alterar o tipo Field do campo depois de salvá-lo.

1. Continue adicionando cada campo, conforme descrito nas seções abaixo.

### Texto de linha única {#single-line-text}

Os campos de texto de linha única capturam informações alfanuméricas limitadas. Por exemplo, você pode capturar as informações de Proprietário, Participante, Equipe ou Unidade organizacional em um campo de texto de linha única. O conteúdo de um campo de texto de linha única pode ter até 250 caracteres. <!-- asked Lilit if we can change this to "Single-line" since this can have numbers and text.-->

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Texto em linha única** tipo de campo.

   ![](assets/single-line-text-field-type.png)

1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida ao passar o mouse sobre o cabeçalho da coluna do campo em uma tabela.
1. Clique em **Criar**.

   O novo campo de linha única é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.


### Parágrafo {#paragraph}

Os campos de parágrafo capturam informações alfanuméricas adicionais sobre um registro, semelhantes ao campo Descrição.

>[!TIP]
>
>* O conteúdo de um campo de parágrafo pode ter até 1.000 caracteres.
>
>* Você pode usar a formatação Rich Text para aprimorar o conteúdo de campos de parágrafo quando eles são exibidos na exibição de tabela ou na página Detalhes de um registro.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Parágrafo** tipo de campo.

   ![](assets/paragraph-field-type.png)


1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
1. Clique em **Criar**.

   O novo campo de parágrafo é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.


### Seleção múltipla {#multi-select}

Você pode usar um campo de seleção múltipla para capturar informações adicionais em qualquer formato selecionando mais de uma opção em um menu suspenso.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Multisseleção** tipo de campo.

   ![](assets/multi-select-field-type.png)


1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Opções**: as opções disponíveis para seleção no menu suspenso após salvar o campo. Você pode ter números e letras para o nome de cada escolha.
1. Clique em **Adicionar opção** para adicionar quantas opções forem necessárias. Não há limite para quantas opções você pode adicionar a um campo de seleção múltipla.
1. (Opcional) Arraste e solte manualmente cada escolha na ordem desejada ou selecione a opção
   **Classificar seleções de A a Z** opção se desejar que as opções sejam listadas automaticamente em ordem alfabética. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Clique em **x** ícone à direita de uma opção para removê-lo.
1. Clique na amostra de cores à esquerda de uma opção para expandir o seletor de cores e personalizar a cor de cada opção.
1. Clique em **Criar**.

   O novo campo de seleção múltipla é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.

### Seleção única {#single-select}

Os campos de seleção única capturam informações adicionais em qualquer formato ao selecionar uma opção em um menu suspenso.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Seleção única** tipo de campo.

   ![](assets/single-select-field-type.png)


1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Opções**: as opções disponíveis para seleção no menu suspenso após salvar o campo. Você pode ter números e letras para o nome de cada escolha.

1. Clique em **Adicionar opção** para adicionar quantas opções forem necessárias. Não há limite para quantas opções você pode adicionar a um campo de seleção única.
1. (Opcional) Arraste e solte manualmente cada escolha na ordem desejada ou selecione a opção **Classificar seleções de A a Z** opção se desejar que as opções sejam listadas automaticamente em ordem alfabética. <!--Add this if they added this functionality: You cannot edit this option after you save the field.-->
1. Clique em **x** ícone à direita de uma opção para removê-lo.
1. Clique na amostra de cores à esquerda de uma opção para expandir o seletor de cores e personalizar a cor de cada opção.
1. Clique em **Criar**.

   O novo campo de seleção única é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.

### Data {#date}

Você pode usar um campo de data para capturar informações adicionais no formato de data e hora.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Data** tipo de campo.

   ![](assets/date-field-type.png)


1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Formato de data**: o tipo de formato de data que você deseja exibir nesse campo. <!--update this casing - submitted bug for it-->

     Selecione entre os seguintes formatos:
      * **Localidade**: corresponde à localidade do seu navegador.
      * **Padrão**: 16/05/2023
      * **Longo**: 16 de maio de 2023
      * **Europeu**: 05/16/2023
      * **ISO**: 16/05/2023
   * **Incluir um campo de tempo**: selecione essa opção se desejar incluir um carimbo de data e hora. Essa opção não está selecionada por padrão. <!--update this setting name - submitted bug for it to be changed-->

     Selecione entre as seguintes opções:

      * **24h**: Por exemplo: 18:00
      * **12 h**: Por exemplo: 18:00

1. Clique em **Criar**.

   O novo campo de data é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.

### Número {#number}

Os tipos de campo de número capturam informações em um formato de número.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Número** tipo de campo.

   ![](assets/number-field-type.png)
1. Adicione as seguintes informações no **Novo campo** guia:

   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro.
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Precisão**: o número de decimais que você deseja gravar para o campo. É possível exibir até 6 decimais.
   * **Permitir números negativos**: selecione essa opção se desejar permitir números negativos nesse campo. Essa opção não está selecionada por padrão.

   >[!NOTE]
   >
   >    Se você selecionar Permitir números negativos e valores negativos forem armazenados nos registros aos quais o campo está anexado, não será mais possível desmarcar a configuração no futuro.

1. Clique em **Criar**.

   O novo campo de número é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.

### Percentagem {#percentage}

Os tipos de campo Porcentagem capturam informações em um formato de número seguido por um sinal de porcentagem.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Porcentagem** tipo de campo.

   ![](assets/percentage-field-type.png)

1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro.
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Precisão**: o número de decimais que você deseja gravar para o campo. É possível exibir até 6 decimais.
   * **Permitir números negativos**: selecione esta opção se desejar permitir valores percentuais negativos neste campo. Essa opção não está selecionada por padrão.

   >[!NOTE]
   >
   >    Se você selecionar Permitir números negativos e valores negativos forem armazenados nos registros aos quais o campo está anexado, não será mais possível desmarcar a configuração no futuro.

1. Clique em **Criar**.

   O novo campo de porcentagem é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.

### Moeda {#currency}

Os tipos de campo Moeda capturam as informações em um formato de número precedido por um símbolo de moeda.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Moeda** tipo de campo.

   ![](assets/currency-field-type.png)

1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Moeda**: o tipo de moeda que você deseja exibir neste campo. Esta é uma lista de moedas de acordo com a Organização Internacional de Normalização (ISO).
   * **Precisão**: o número de decimais que você deseja gravar para o campo. É possível exibir até 6 decimais.
   * **Permitir números negativos**: selecione esta opção se desejar permitir valores de moeda negativos neste campo. Essa opção não está selecionada por padrão.

   >[!NOTE]
   >
   >    Se você selecionar Permitir números negativos e valores negativos forem armazenados nos registros aos quais o campo está anexado, não será mais possível desmarcar a configuração no futuro.

1. Clique em **Criar**.

   O novo campo de moeda é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.

### Caixa de seleção

Você pode usar o tipo de campo Caixa de seleção para adicionar uma única opção de caixa de seleção a um registro. Você pode usar esse campo para indicar um atributo ou status específico para esse registro específico. Por exemplo, você pode usá-lo como um sinalizador para rastrear a conclusão, a aprovação ou qualquer outro atributo binário para cada registro.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Caixa de seleção** tipo de campo.

   ![](assets/checkbox-field-type.png)

1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
1. Clique em **Criar**.

   O novo campo de caixa de seleção é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.

### Pessoas

Você pode usar o tipo de campo Pessoas para adicionar um usuário <!--, job role, or team--> para um registro. Este campo é do tipo digitação antecipada e só é possível adicionar usuários<!--, roles, or teams--> que já existem no Workfront.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Pessoas** tipo de campo.

   ![](assets/people-field-type.png)

1. Adicione as seguintes informações no **Novo campo** guia:
   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro.
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Permitir valores múltiplos**: selecione essa opção se desejar permitir que os usuários adicionem mais de um usuário nesse campo. Essa opção não está selecionada por padrão.

   >[!NOTE]
   >
   >    Se você selecionar Permitir vários valores e vários usuários forem armazenados nos registros aos quais o campo está anexado, não será mais possível desmarcar a configuração no futuro, ao editar esse campo.

1. Clique em **Criar**.

   O novo campo do tipo Pessoas é adicionado como uma coluna ao tipo de registro e seus valores podem ser associados a registros.

### Criado por

Você pode usar o tipo de campo Criado por para adicionar o usuário que criou o registro a um registro. Este campo é somente leitura e é preenchido automaticamente com o nome do usuário que estava conectado quando o registro foi criado.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Criado por** tipo de campo.

   ![](assets/created-by-field-type.png)

1. Adicione as seguintes informações no **Novo campo** guia:

   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--this might change and they might prepopulate it with "Created by"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.

1. Clique em **Criar**.

   O novo campo Created by-type é adicionado como uma coluna ao tipo de registro e seus valores são pré-preenchidos com o nome do usuário que criou cada registro.


### Data de criação

Você pode usar o tipo de campo Data de criação para adicionar a data em que um registro foi criado a um registro. Este campo é somente leitura e é preenchido automaticamente com a data (e, opcionalmente, com a hora) em que o registro foi criado.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Data de criação** tipo de campo.

   ![](assets/created-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Adicione as seguintes informações no **Novo campo** guia:

   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--this might change and they might prepopulate it with "Created date"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Formato de data**: selecione nos seguintes formatos:

      * **Localidade**: corresponde à localidade do seu navegador.
      * **Padrão**: 16/05/2023
      * **Longo**: 16 de maio de 2023
      * **Europeu**: 05/16/2023
      * **ISO**: 16/05/2023
   * **Incluir um campo de tempo**: selecione essa opção se desejar incluir um carimbo de data e hora. Essa opção não está selecionada por padrão. <!--submitted a UI text change for this - check the UI-->

     Selecione entre as seguintes opções:

      * **24h**: Por exemplo: 18:00
      * **12 h**: Por exemplo: 18:00

1. Clique em **Criar**.

   O novo campo de tipo de data Created é adicionado como uma coluna ao tipo de registro e seus valores são preenchidos previamente com a data (ou data e hora) em que o registro foi criado.


### Modificado pela última vez por

Você pode usar o tipo de campo Última modificação por para adicionar o usuário que modificou o registro por último a um registro. Este campo é somente leitura e é preenchido automaticamente com o nome do usuário que fez logon quando o registro foi atualizado pela última vez.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Última modificação por** tipo de campo.

   ![](assets/last-modified-by-field-type.png)

1. Adicione as seguintes informações no **Novo campo** guia:

   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--this might change and they might prepopulate it with "Created by"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.

1. Clique em **Criar**.

   O novo campo Última modificação por tipo é adicionado como uma coluna ao tipo de registro e seus valores são pré-preenchidos com o nome do usuário que modificou cada registro pela última vez.


### Data da última modificação

Você pode usar o tipo de campo Data da última modificação para adicionar a data em que um registro foi modificado pela última vez a um registro. Este campo é somente leitura e é preenchido automaticamente com a data (e, opcionalmente, com a hora) em que o registro foi modificado pela última vez.

1. Comece a criar um campo conforme descrito na seção [Criar campos do zero](#create-fields-from-scratch) neste artigo, selecione a variável **Data de criação** tipo de campo.

   ![](assets/last-modified-date-field-type.png)

   <!--check the image above - added bug fix for UI text changes-->

1. Adicione as seguintes informações no **Novo campo** guia:

   * **Nome**: O nome do tipo de campo, como ele aparecerá em uma tabela ou na página Detalhes do registro. <!--this might change and they might prepopulate it with "Created date"-->
   * **Descrição**: informações adicionais sobre o campo. A descrição de um campo é exibida quando você passa o mouse sobre a coluna do campo em uma tabela.
   * **Formato de data**: selecione nos seguintes formatos:

      * **Localidade**: corresponde à localidade do seu navegador.
      * **Padrão**: 16/05/2023
      * **Longo**: 16 de maio de 2023
      * **Europeu**: 05/16/2023
      * **ISO**: 16/05/2023
   * **Incluir um campo de tempo**: selecione essa opção se desejar incluir um carimbo de data e hora. Essa opção não está selecionada por padrão. <!--submitted a UI text change for this - check the UI-->

     Selecione entre as seguintes opções:

      * **24h**: Por exemplo: 18:00
      * **12 h**: Por exemplo: 18:00

1. Clique em **Criar**.

   O novo campo de tipo de data Última modificação é adicionado como uma coluna ao tipo de registro e seus valores são pré-preenchidos com a data (ou data e hora) em que o registro foi modificado pela última vez.

## Criar campos conectando tipos de registro

Você pode criar campos de registro vinculados ao adicionar uma nova conexão entre dois tipos de registro Maestri ou um tipo de registro e tipos de objeto de outras aplicações.

Para obter informações sobre como conectar tipos de registros Maestri, consulte [Conectar tipos de registro](../architecture/connect-record-types.md)

## Criar campos importando tipos de registro usando um arquivo Excel e CSV

Para obter mais informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

## Criar campos criando um tipo de registro

Ao criar um tipo de registro, vários campos associados ao novo tipo de registro também são criados por padrão. Para obter mais informações, consulte [Criar tipos de registro operacional](../architecture/create-record-types.md).

## Criar campos criando um espaço de trabalho a partir de um modelo

O Maestri cria campos para tipos de registros operacionais e taxonomias quando você cria um espaço de trabalho a partir de um modelo.

Para obter informações, consulte [Criar espaços de trabalho operacionais](../architecture/create-workspaces.md).