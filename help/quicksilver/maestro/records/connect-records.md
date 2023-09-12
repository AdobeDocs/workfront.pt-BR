---
title: Conectar registros
description: Depois de criar conexões entre tipos de registro, você pode conectar registros individuais uns aos outros.
hidefromtoc: true
hide: true
source-git-commit: 71ce412ead1590b8511ec4219d3ba72fbf32b98d
workflow-type: tm+mt
source-wordcount: '1804'
ht-degree: 0%

---


<!--when you make this live, update the metadata above to this: 
---
title: Connect records and objects
description: In addition to connecting Maestro records to one another, you can also connect Maestro records to objects from other applications.  
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->
<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Conectar registros

>[!IMPORTANT]
>
>Atualmente, o Adobe Maestro faz parte de um programa beta fechado que está aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode conectar registros do Adobe Maestro uns aos outros ou a objetos de outras aplicações.

Primeiro, você deve conectar dois tipos de registro juntos ou um tipo de registro a um tipo de objeto de outro aplicativo e, em seguida, usar a exibição Tabela do tipo de registro para conectar registros uns aos outros ou registros a outros objetos.

Para obter informações sobre como conectar tipos de registro entre si ou a tipos de objeto de outros aplicativos, consulte [Conectar tipos de registro](../architecture-and-fields/connect-record-types.md).

Para obter um exemplo de conexão de tipos de registro, consulte [Exemplo de conexão de tipos de registro e registros](../architecture-and-fields/example-connect-record-types-and-records.md).

Você pode conectar o seguinte:

* Registros operacionais principais
* Maestri registros operacionais para registros de taxonomia
* Gerenciar registros operacionais e objetos de outras aplicações.

  Os seguintes aplicativos e tipos de objeto são suportados no momento:

   * Adobe Workfront

      * Projetos
      * Portfólios
      * Programas
      * Empresa
      * Grupo

  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

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
   <td><p>Qualquer um, para criar registros Maestro</p> 
<p>Trabalhe ou mais para visualizar projetos no Workfront</p>
  <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Visão geral das licenças do Adobe Workfront</a>.</p> 
  </td>
  </tr>
  <tr>
   <td role="rowheader">Nível de acesso</td>
   <td> <p>Qualquer um, para criar registros Maestro</p>
<p>Acesso igual ou superior a projetos, Portfolio, programas</p> 
<p>Acesso adicional a Grupos e Empresas, ao visualizar grupos ou empresas aos quais os usuários não pertencem</p>   
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões de objeto</p></td>
   <td> <p>Exibir ou ter permissões mais altas para os objetos que você deseja vincular com registros Maestro  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do sistema deve adicionar a área Maestro no modelo de layout. Para obter informações, consulte <a href="../access/grant-access.md">Conceder acesso ao Adobe Maestro</a>. </p></td>
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

## Conectar registros

### Considerações sobre a conexão de registros

* Depois que a conexão entre os tipos de registro for estabelecida, os tipos de registro conectados serão exibidos como campos de registro vinculados na tabela dos tipos de registro dos quais estão vinculados.
* Você pode procurar e adicionar registros e objetos do registro vinculado e tipos de objeto a partir dos campos de registro vinculados.
* É possível adicionar campos dos tipos de registro vinculados à tabela do tipo de registro a partir do qual você está vinculando.
* Não é possível atualizar manualmente os valores de campos vinculados nos registros a partir dos quais você está vinculando.

  Os valores dos campos vinculados dos registros vinculados preenchem o registro Maestro do qual você está vinculando automaticamente.

* Qualquer pessoa com acesso ao Maestro pode ver as conexões que você faz entre registros do Maestro ou entre registros do Maestro e objetos do Workfront. Além disso, você pode exibir e editar as conexões de todas as outras pessoas. <!--add that this is based on your permissions in both Maestro and Workfront (or, later, any other application)-->
* Você pode conectar um registro do Maestro a um ou vários objetos de outro aplicativo.
* Não é possível conectar taxonomias a tipos de registro ou a objetos de outro aplicativo. <!-- this is temporary; there will be certain objects (teams, etc) that will be linked to taxonomies, per Lilit-->
* Atualmente, você pode vincular registros Maestro somente a objetos Workfront. Para vincular registros do Maestro a objetos do Workfront, você deve ter o seguinte:

   * Objetos do Workfront. Por exemplo, primeiro você deve criar projetos, portfólios, programas, empresas ou grupos no Workfront.
   * Espaços de trabalho, tipos de registros e registros do mestre. Para obter mais informações, consulte os seguintes artigos:

      * [Criar espaços de trabalho](../architecture-and-fields/create-workspaces.md)
      * [Criar tipos de registro](../architecture-and-fields/create-record-types.md)
      * [Criar registros](../records/create-records.md)

   * Conexões entre tipos de registro ou entre tipos de registro e objetos de outros aplicativos. Para obter informações, consulte [Conectar tipos de registro](../architecture-and-fields/connect-record-types.md).

### Conectar registros do Maestro

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito do Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> e clique em **Maestro** ![](assets/maestro-icon.png).

   O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho do qual deseja conectar registros.
1. Clique no cartão de um tipo de registro para abrir a página do tipo de registro.
1. Selecione uma exibição de Tabela na **Exibir** no canto superior direito da página tipo de registro.
1. Adicionar uma conexão com outro tipo de registro ou objeto do tipo de registro selecionado. Para obter informações, consulte [Conectar tipos de registro](../architecture-and-fields/connect-record-types.md).

Uma nova coluna é adicionada à tabela para exibir o tipo de registro vinculado.

1. Adicione registros ao tipo de registro selecionado adicionando uma nova linha à tabela. Para obter informações, consulte [Criar registros](../../maestro/records/create-records.md).
1. A partir de um registro listado na exibição de tabela, vá para a coluna de registro vinculado e passe o mouse sobre a célula correspondente ao registro que você deseja vincular com outros registros Maestri, em seguida, clique no **+** ícone.

   A variável **Conectar objetos** é exibida.

   ![](assets/connected-objects-table-for-records.png)

1. Comece a digitar o nome de um registro na caixa de pesquisa e selecione-o quando ele for exibido na lista

   Ou

   Selecione o nome de um ou vários registros na caixa e clique em **Conectar objetos** no canto superior direito da caixa Conectar objetos.

   São aditados os seguintes pontos:

   * Os registros vinculados são exibidos no campo do registro vinculado selecionado na etapa 3. A atualização dos registros vinculados atualiza automaticamente os campos de registro vinculados para os registros a partir dos quais você está vinculando. <!--ensure the number of the step stays accurate-->
   * Os campos vinculados que pertencem aos registros vinculados são automaticamente preenchidos com as informações dos registros vinculados originais. Não é possível editar manualmente campos vinculados.

     >[!TIP]
     >
     >* Usamos &quot;campos vinculados&quot; e &quot;campos de pesquisa&quot; alternadamente.
     >
     >* Se você ativou a configuração Permitir vários registros quando conectou os tipos de registro, os valores dos campos dos vários objetos selecionados serão exibidos separados por vírgulas ou agregados de acordo com o agregador escolhido.

1. (Opcional) Feche a página do tipo de registro Maestro e vá para o Espaço de trabalho selecionado.
1. Clique no cartão do tipo de registro ao qual você está vinculado.

   Por exemplo, se você conectou o registro de Campanha ao registro de Produto, clique no botão **Produto** cartão.

   O cartão de tipo de registro deve ser aberto na exibição Tabela.

   Observe que o campo Campaign linked record exibe os nomes das campanhas vinculadas aos produtos na página Product record type. Atualizar as informações de Campanha atualiza automaticamente o campo de registro vinculado Campanha para o tipo de registro Produto.

### Conectar registros do Maestri a objetos do Workfront

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Depois de criar uma conexão entre um tipo de registro Maestro e um tipo de objeto Workfront, você pode conectar registros Maestri individuais a objetos no Workfront. Você também pode conectar campos do objeto Workfront ao tipo de registro Maestro.

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito do Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> e clique em **Maestro** ![](assets/maestro-icon.png).

   O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho do qual deseja conectar registros.
1. Clique no cartão de um tipo de registro para abrir a página do tipo de registro.
1. Selecione uma exibição de Tabela na **Exibir** no canto superior direito da página tipo de registro.
1. Adicionar uma nova conexão a um tipo de objeto do Workfront com o tipo de registro selecionado. Selecione entre os seguintes objetos na seção Workfront:

   * Projeto
   * Portfólio
   * Programa
   * Empresa
   * Grupo

   Para obter mais informações, consulte [Conectar tipos de registro](../architecture-and-fields/connect-record-types.md).

   Uma nova coluna é adicionada à tabela para exibir o tipo de objeto vinculado.

1. Adicione registros individuais ao tipo de registro selecionado adicionando uma nova linha à tabela. Para obter informações, consulte [Criar registros](../../maestro/records/create-records.md).
1. Em um registro listado na exibição de tabela, vá para a coluna de objeto vinculado e passe o mouse sobre a célula correspondente ao registro que deseja vincular a outros objetos do Workfront e clique no **+** ícone. <!--change Workfront to other applications, when this will be possible-->

   A variável **Conectar objetos** é exibida.

   ![](assets/connect-objects-box-to-select-projects.png)

1. Comece digitando o nome de um objeto Workfront na caixa de pesquisa e selecione-o quando ele for exibido na lista

   Ou

   Selecione o nome de um ou vários objetos na caixa e clique em **Conectar objetos** no canto superior direito da caixa Conectar objetos.

   São aditados os seguintes elementos ao Maestro:

   * Os objetos Workfront selecionados são adicionados ao campo de registro vinculado.
   * Um novo campo vinculado (ou um campo de pesquisa) é criado para cada campo vinculado selecionado ao adicionar os campos ao seu registro vinculado.
   * Um novo tipo de registro chamado &quot;objeto Workfront&quot; é criado no mesmo espaço de trabalho do registro Maestro do qual você está vinculando. O nome do objeto faz parte do nome desse tipo de registro. Por exemplo, vincular a projetos do Workfront cria o tipo de registro de projeto do Workfront no Maestro.

     Este é um tipo de registro somente leitura e exibe os objetos do Workfront que estão selecionados no novo campo de objeto vinculado que você criou a partir do registro Maestro. Os campos vinculados do objeto vinculado também são exibidos nos registros somente leitura vinculados do Workfront.

     >[!IMPORTANT]
     >
     > O tipo de registro de objeto do Workfront somente leitura é criado somente quando projetos individuais são adicionados aos registros do Maestro. Simplesmente criar uma conexão entre um tipo de registro Maestro e um tipo de objeto Workfront não cria o tipo de registro Workfront.

     Qualquer informação existente nos campos dos objetos do Workfront é exibida nos campos vinculados ou de pesquisa.

     >[!TIP]
     >
     >
     >* Se você ativou a configuração Permitir vários registros, os valores dos vários objetos serão exibidos separados por vírgulas ou agregados de acordo com o agregador escolhido.
     >
     >* Um campo de registro vinculado aos registros vinculados Maestri não é criado para os objetos vinculados do Workfront.


1. (Opcional) Feche a página do tipo de registro Maestro e vá para o Espaço de trabalho selecionado.
1. Clique no cartão para o tipo de registro de objeto do Workfront. Por exemplo, clique no link **Projeto do Workfront** , se você vinculou a projetos do Workfront. O cartão de tipo de registro do Workfront somente leitura deve abrir na exibição Tabela.

   >[!NOTE]
   >
   >    * Os registros listados na página Tipo de registro do Workfront são objetos somente leitura do Workfront. Os campos vinculados do tipo de registro do Workfront também são exibidos como colunas somente leitura e são preenchidos automaticamente quando são preenchidos no Workfront.
   >    * Não é possível atualizar manualmente os campos do Workfront no Maestro. Os campos de objeto do Workfront devem ser preenchidos no Workfront e os valores de campo são exibidos automaticamente no registro do Workfront no Maestro.
   >
   >    * Para exibir o tipo de registro de objeto do Workfront na exibição Linha do tempo, você deve ter pelo menos dois campos de data exibidos na exibição Tabela da página tipo de registro somente leitura do Workfront.

1. (Opcional) Clique no link **Mais** menu ![](assets/more-menu.png) ao lado do nome do tipo de registro de objeto do Workfront no cabeçalho da página, clique em **Renomear** para editar o nome do registro.

   >[!NOTE]
   >
   >    Não é possível excluir um tipo de registro vinculado do Workfront ou quaisquer objetos da página de tipo de registro do Workfront.

1. (Opcional) Clique no link **Adicionar campos** ícone ![](assets/add-fields-icon.png) no canto superior direito da exibição de tabela na página tipo de registro do Workfront, para adicionar ou remover campos do Workfront do tipo de registro do Workfront.

   >[!NOTE]
   >
   >  Os campos que você adiciona ou remove na página tipo de registro de objeto do Workfront não são adicionados nem removidos do tipo de registro Maestro que se vincula ao tipo de objeto do Workfront. Os campos só são visíveis na página do tipo de registro somente leitura do Workfront, portanto, você pode analisá-los no Maestro.

1. (Opcional) No menu suspenso Exibir na página tipo de registro de objeto do Workfront, escolha a exibição Linha do tempo para exibir os objetos vinculados do Workfront na exibição Linha do tempo.












