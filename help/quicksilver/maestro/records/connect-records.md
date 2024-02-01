---
title: Conectar registros
description: Depois de criar conexões entre tipos de registro, você pode conectar registros individuais uns aos outros.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 17796cdc-6de8-4209-a5af-b255dc64d70a
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '2847'
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
<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--if you change steps here, also update steps in the "Connect records" article-->

# Conectar registros

{{maestro-important-intro}}

Você pode conectar registros do Adobe Maestro uns aos outros ou a objetos de outras aplicações.

Primeiro, você deve conectar dois tipos de registro juntos ou um tipo de registro a um tipo de objeto de outro aplicativo e, em seguida, usar a exibição Tabela do tipo de registro para conectar registros uns aos outros ou registros a outros objetos.

Para obter informações sobre como conectar tipos de registro entre si ou a tipos de objeto de outros aplicativos, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).

Para obter um exemplo de conexão de tipos de registro, consulte [Exemplo de conexão de tipos de registro e registros](../architecture/example-connect-record-types-and-records.md).

Você pode conectar o seguinte:

* Registros operacionais principais
* Maestri registros operacionais para registros de taxonomia
* Gerenciar registros operacionais e objetos de outras aplicações.

  Você pode conectar registros do Maestro a objetos dos tipos listados abaixo a partir das seguintes aplicações:

   * Adobe Workfront

      * Projetos
      * Portfólios
      * Programas
      * Empresa
      * Grupo

   * Adobe Experience Manager Assets

      * Arquivos de imagem
      * Pastas



  <!--when you add more objects, fix the Access Requirements below which right now refer only to projects-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>Para conectar registros do Maestri com a Experience Manager Assets, você deve ter uma licença da Adobe Experience Manager Assets e a instância da Workfront de sua organização deve ser integrada à Adobe Business Platform ou à Adobe Admin Console.</p>
   </td>
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
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Gerenciar permissões em um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Maestri no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Conectar registros

### Considerações sobre a conexão de registros

* Depois de conectar os tipos de registro, os tipos de registro conectados são exibidos como campos de registro vinculados na tabela dos tipos de registro dos quais estão vinculados.
* Você pode procurar e adicionar registros e objetos do registro vinculado e tipos de objeto a partir dos campos de registro vinculados.
* É possível adicionar campos dos tipos de registro vinculados à tabela do tipo de registro a partir do qual você está vinculando.
* Não é possível atualizar manualmente os valores de campos vinculados nos registros a partir dos quais você está vinculando.

  Os valores dos campos vinculados dos registros vinculados preenchem o registro Maestro que você está vinculando automaticamente a partir do espaço de trabalho Maestro que você configura ou a partir do aplicativo de terceiros.

* Qualquer pessoa com acesso ao Maestro e Gerenciar permissões para o espaço de trabalho pode ver as conexões que você faz entre registros do Maestro ou entre registros do Maestri e objetos de outras aplicações. Eles podem exibir registros e objetos conectados independentemente de suas permissões nos aplicativos de terceiros aos quais você está se conectando. <!--check with PM-->
* Você poderá exibir e editar as conexões de todos os outros usuários se tiver permissões de Gerenciamento para o espaço de trabalho em que os registros conectados estão.
* Você pode conectar um registro do Maestro a um ou vários objetos de outro aplicativo.
* Para vincular registros do Maestro a outros registros ou objetos, você deve ter o seguinte:

   * Pelo menos um espaço de trabalho do Maestro, tipo de registro e registro.

     Para obter mais informações, consulte os seguintes artigos:

      * [Criar espaços de trabalho](../architecture/create-workspaces.md)
      * [Criar tipos de registro](../architecture/create-record-types.md)
      * [Criar registros](../records/create-records.md)

   * Conexões entre tipos de registro ou entre tipos de registro e objetos de outros aplicativos. Para obter informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md)

### Conectar registros do Maestro

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho do qual deseja conectar registros.
1. Clique no cartão de um tipo de registro para abrir a página do tipo de registro.
1. Selecione um **Tabela** exibir do **Exibir** no canto superior direito da página tipo de registro.
1. (Opcional) Adicione registros ao tipo de registro selecionado adicionando uma nova linha à tabela. Para obter informações, consulte [Criar registros](../../maestro/records/create-records.md).
1. Em um registro listado na exibição de tabela, vá para a coluna de registro vinculado e passe o mouse sobre a célula correspondente ao registro que deseja vincular a outros registros, em seguida, clique no **+** ícone.

   A variável **Conectar objetos** é exibida.

   ![](assets/connected-objects-table-for-records.png)

1. Comece a digitar o nome de um registro na caixa de pesquisa e selecione-o quando ele for exibido na lista

   Ou

   Selecione o nome de um ou vários registros na caixa e clique em **Conectar objetos** no canto superior direito da caixa Conectar objetos.

   São aditados os seguintes pontos:

   * Os registros vinculados são exibidos no campo do registro vinculado selecionado na etapa 5. <!--accurate?--> A atualização dos registros vinculados atualiza automaticamente os campos vinculados para os registros a partir dos quais você está vinculando. Não é possível editar manualmente campos vinculados.

     >[!TIP]
     >
     >* Usamos &quot;campos vinculados&quot; e &quot;campos de pesquisa&quot; alternadamente.
     >
     >* Se você ativou o **Permitir vários registros** definindo quando você conectou os tipos de registro, os valores dos campos para os vários objetos selecionados serão exibidos separados por vírgulas ou agregados de acordo com o agregador escolhido.

1. (Opcional) Feche a página do tipo de registro Maestro e vá para o espaço de trabalho selecionado.
1. Clique no cartão do tipo de registro ao qual você está vinculado.

   Por exemplo, se você conectou o **Campaign** com o registro Produto, clique no botão **Produto** cartão.

   O cartão de tipo de registro deve ser aberto na exibição Tabela. Caso contrário, selecione uma exibição de tabela.

   Observe que **Campaign** o campo linked record exibe os nomes das campanhas vinculadas aos produtos na página Product record type. Atualizar as informações de Campanha atualiza automaticamente o campo de registro vinculado Campanha para o tipo de registro Produto.

### Conectar registros do Maestri a objetos do Workfront

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

Depois de criar uma conexão entre um tipo de registro Maestro e um tipo de objeto Workfront, você pode conectar registros Maestri individuais a objetos no Workfront. Os campos do Workfront que você conectou são automaticamente preenchidos nos registros do Maestro que você está vinculando os objetos do.

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho do qual deseja conectar registros.
1. Clique no cartão de um tipo de registro para abrir a página do tipo de registro.
1. Selecione um **Tabela** exibir do **Exibir** no canto superior direito da página tipo de registro.

1. (Opcional) Adicione registros individuais ao tipo de registro selecionado adicionando uma nova linha à tabela. Para obter informações, consulte [Criar registros](../../maestro/records/create-records.md).
1. (Condicional) Se você conectou o tipo de registro selecionado a um objeto do Workfront, vá para a coluna de objetos vinculados e passe o mouse sobre a célula correspondente ao registro que deseja vincular com os objetos do Workfront, em seguida, clique na **+** ícone.

   A variável **Conectar objetos** é exibida.

   ![](assets/connect-objects-box-to-select-projects.png)

   Para obter mais informações sobre como conectar tipos de registro a objetos de um aplicativo de terceiros, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).

1. Comece digitando o nome de um objeto Workfront na caixa de pesquisa e selecione-o quando ele for exibido na lista

   Ou

   Selecione o nome de um ou vários objetos na caixa e clique em **Conectar objetos** no canto superior direito da caixa Conectar objetos.

   São aditados os seguintes pontos:

   * Os objetos Workfront selecionados são adicionados ao campo de registro vinculado.
   * Se você os tiver adicionado ao conectar o tipo de registro ao Workfront, os campos vinculados (ou os campos de pesquisa) serão automaticamente preenchidos com informações do Workfront.
   * Um novo tipo de registro chamado &quot;&lt; Nome do tipo de objeto do Workfront >&quot; é criado no mesmo espaço de trabalho que o registro Maestro do qual você está vinculando. O nome do objeto faz parte do nome desse tipo de registro. Por exemplo, vincular a projetos do Workfront cria a variável **Projeto** tipo de registro no Maestro.

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
     >* Um campo de registro vinculado aos registros vinculados Maestro não é criado para os objetos vinculados do Workfront no Workfront.


1. (Opcional) Feche a página do tipo de registro Maestro e vá para o Espaço de trabalho selecionado.
1. (Opcional) Clique no cartão para o tipo de registro do objeto do Workfront. Por exemplo, clique no link **Projeto** , se você vinculou a projetos do Workfront. O cartão de tipo de registro do Workfront somente leitura deve abrir na exibição de tabela.

   Os registros listados na página de tipo de registro do Workfront são objetos somente leitura do Workfront que foram vinculados a partir dos registros do Maestro. Os campos vinculados do tipo de registro do Workfront também são exibidos como colunas somente leitura e são preenchidos automaticamente quando são preenchidos no Workfront.

1. (Opcional) Para abrir a página Detalhes do registro de objeto do Workfront no Maestri, siga um destes procedimentos:

   * No tipo de registro vinculado, vá para o campo Workfront object linked record e clique no nome do objeto do Workfront.
   * No **Tabela** da página tipo de registro do Workfront, clique no nome do objeto Workfront

     Ou

     Clique em **Mais** à direita do nome do objeto do Workfront e clique em **Exibir**.

     ![](assets/workfront-object-more-menu-in-table-with-go-to-source-link.png)

   Isso abre a página Detalhes do mestre do objeto vinculado do Workfront. Esta página é somente leitura.

1. (Opcional) Para abrir o objeto Workfront vinculado no Workfront, siga um destes procedimentos:

   * No **Tabela** Na exibição da página tipo de registro do Workfront, clique no nome do objeto do Workfront para abrir o registro do Projeto no Maestro

   Ou

   Clique em **Mais** à direita do nome do objeto do Workfront e clique em **Ir para origem**.

   ![](assets/workfront-project-maestro-details-page-with-go-to-source-link.png)

   Isso abre a página do objeto do Workfront. Você pode editar informações sobre o objeto do Workfront, se tiver permissões para isso.

1. (Opcional) Na página de registro de objeto do Workfront somente leitura no Maestro, clique no link **Adicionar campos** ícone ![](assets/add-fields-icon.png) no canto superior direito da exibição de tabela, para adicionar ou remover campos do Workfront do tipo de registro do Workfront.

   >[!NOTE]
   >
   >  Os campos que você adiciona ou remove na página tipo de registro de objeto do Workfront não são adicionados nem removidos do tipo de registro Maestro que se vincula ao tipo de objeto do Workfront. Os campos só são visíveis na página do tipo de registro somente leitura do Workfront, portanto, você pode analisá-los no Maestro.

1. (Opcional e condicional) Se você tiver adicionado pelo menos dois campos de data ao objeto do Workfront, clique no **Exibir** menu suspenso na página tipo de registro de objeto do Workfront e selecione o **Linha do tempo** exibir ou **Criar visualização** para criar uma visualização de linha do tempo.  Para obter informações, consulte [Gerenciar a exibição de linha do tempo](/help/quicksilver/maestro/views/manage-the-timeline-view.md).

   Os objetos vinculados ao Workfront são exibidos na visualização de linha do tempo.


### Conectar registros do Maestri a objetos do Adobe Experience Manager

<!--when we will have more applications to link to from Maestro, change the title to soemthing like: Connect Maestro records to objects from other applications-->

>[!IMPORTANT]
>
>Você deve ter uma licença do Adobe Experience Manager Assets e a instância da Workfront de sua organização deve estar integrada à Plataforma de negócios Adobe ou à Adobe Admin Console para poder conectar os registros Maestri à Adobe Experience Manager Assets.
>
>Em caso de dúvidas sobre a integração com a Adobe Admin Console, consulte [Perguntas frequentes sobre a experiência unificada do Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

Depois de criar uma conexão entre um tipo de registro Maestro e o Adobe Experience Manager Assets, você pode conectar registros Maestri individuais a ativos Experience Manager. Os campos de ativos que você conectou a partir do Experience Manager Assets ao criar a conexão são preenchidos automaticamente no tipo de registro Mestre que você vinculou.

{{step1-to-maestro}}

O espaço de trabalho acessado por último deve ser aberto por padrão.

1. (Opcional) Expanda a seta apontando para baixo à direita de um nome de espaço de trabalho existente e selecione o espaço de trabalho do qual deseja conectar registros.
1. Clique no cartão de um tipo de registro para abrir a página do tipo de registro.
1. Selecione um **Tabela** exibir do **Exibir** no canto superior direito da página tipo de registro.

1. (Opcional) Adicione registros individuais ao tipo de registro selecionado adicionando uma nova linha à tabela. Para obter informações, consulte [Criar registros](../../maestro/records/create-records.md).
1. (Condicional) Se você conectou o tipo de registro selecionado ao Experience Manager Assets, vá para a coluna de objetos vinculados e passe o mouse sobre a célula correspondente ao registro que deseja vincular com outros objetos do Experience Manager e clique no botão **+** ícone.

   A variável **Selecionar ativos** é exibida. <!--update screen shot with actual assets-->

   ![](assets/select-assets-box-for-aem-record-connections.png)

   Para obter mais informações sobre como conectar tipos de registro a objetos de um aplicativo de terceiros, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).

1. Clique em para selecionar alguns dos seguintes tipos de ativos:

   * Imagens
   * Pastas

   É possível selecionar vários ativos.

   >[!IMPORTANT]
   >
   > Você pode conectar somente ativos que você tenha acesso para visualizar no Experience Manager. Uma vez conectado, todos os usuários do Maestro podem visualizar os ativos no Maestro, independentemente do acesso deles ao Experience Manager Assets.

1. Clique em **Selecionar**.

   São aditados os seguintes pontos:

   * Os ativos de Experience Manager selecionados são adicionados ao campo de registro vinculado.
   * Os campos vinculados (ou campos de pesquisa) são preenchidos com informações dos ativos conectados ao Experience Manager.
   * Um novo tipo de registro chamado &quot;Experience Manager Assets&quot; é criado no mesmo espaço de trabalho do registro Maestro que você está vinculando. <!--is this still added?-->

     Este é um tipo de registro somente leitura e exibe ativos de Experience Manager que estão selecionados no novo campo de objeto vinculado que você criou a partir do registro Maestro. Os campos vinculados do objeto vinculado também são exibidos nos registros de Experience Manager vinculados somente leitura.

     >[!IMPORTANT]
     >
     > O tipo de registro Experience Manager Assets somente leitura é criado somente quando ativos individuais são adicionados aos registros Maestri. Simplesmente criar uma conexão entre um tipo de registro Maestro e o Experience Manager Assets não cria o tipo de registro Experience Manager Assets.

     Todas as informações existentes nos campos dos ativos de Experience Manager são exibidas nos campos vinculados ou de pesquisa.

     >[!TIP]
     >
     >
     >* Se você ativou a configuração Permitir vários registros, os valores dos vários objetos serão exibidos separados por vírgulas.
     >
     >* Um campo de registro vinculado aos registros vinculados Maestro não é criado para os ativos de Experience Manager vinculados no aplicativo do Experience Manager Assets.


1. (Opcional) Feche a página do tipo de registro Maestro e vá para o espaço de trabalho selecionado.
1. Clique no cartão para o tipo de registro Experience Manager Assets. O cartão de tipo de registro do Experience Manager Assets somente leitura deve abrir na exibição Tabela.

   Os registros listados na página de tipo de registro do Experience Manager Assets são ativos somente leitura. Os campos vinculados do tipo de registro Experience Manager Assets também são exibidos como colunas somente leitura e são preenchidos automaticamente quando são preenchidos no Experience Manager.

1. (Opcional) Vá para o tipo de registro vinculado ao Experience Manager Assets a partir de e clique no nome de um ativo no campo de registro vinculado. Os detalhes do Experience Manager do ativo são exibidos em uma janela pop-up. <!--update screen shot with hi-rez picture-->

   ![](assets/asset-pop-up-window-with-aem-details-and-thumbnail.png)

   Os seguintes campos são exibidos para um arquivo de imagem:

   * Uma miniatura da imagem
   * O nome do arquivo de imagem
   * Dimensões
   * Tamanho
   * Descrição
   * O caminho do arquivo no Experience Manager
   * O tipo de ativo
   * Data de criação
   * Data de modificação

1. (Opcional) Para abrir a página Detalhes do registro do Experience Manager Assets no Maestro, faça o seguinte:

   1. Vá para a **Experience Manager Assets** Maestro cartão de tipo de registro no mesmo espaço de trabalho que você selecionou originalmente e clique em para abrir a página de tipo de registro.
A página do tipo de registro Experience Manager Assets Maestri é somente leitura.
   1. Na exibição de tabela, clique no nome de um ativo

      Ou

      Passe o mouse sobre o nome de um ativo, clique no ícone **Mais** menu ![](assets/more-menu.png) à direita do nome do ativo e clique em **Exibir**.\
      Isso abre o mestre do ativo **Detalhes** página. Esta página é somente leitura.
1. (Opcional) Para abrir a página Detalhes do registro de ativos de Experience Manager no Experience Manager, siga um destes procedimentos:

   * Vá para a página Tipo de registro Maestro do registro que você está vinculando, clique no nome de um ativo no campo de registro vinculado para abrir a janela pop-up e, em seguida, clique no **Abertura** ícone ![](assets/open-asset-icon.png) para abrir o ativo.
   * Vá para a **Experience Manager Assets** Cartão do tipo de registro Maestri no mesmo espaço de trabalho selecionado originalmente e clique em para abrir a página do tipo de registro, clique no nome de um ativo para abrir o Maestro **Detalhes** e clique em **Ir para origem** no canto superior direito da tela.

     ![](assets/go-to-source-asset-maestro-details-page.png)
   * Vá para a **Experience Manager Assets** Maestri record type card no mesmo espaço de trabalho selecionado originalmente e clique no cartão para abrir a página Experience Manager Assets record type, passe o mouse sobre o nome de um ativo, clique em **Mais** e clique em **Ir para origem**.

     ![](assets/go-to-source-option-on-table-view.png)

   O ativo é aberto no Experience Manager Assets.

1. (Opcional) Clique no link **Adicionar campos** ícone ![](assets/add-fields-icon.png) no canto superior direito da exibição de tabela na página tipo de registro do Experience Manager Assets, para adicionar ou remover campos Experience Manager.

   >[!NOTE]
   >
   >  Os campos adicionados ou removidos na página Tipo de registro do Experience Manager Assets não são adicionados nem removidos do tipo de registro Maestro vinculado ao ativo Experience Manager. Os campos só são visíveis na página do tipo de registro somente leitura do Experience Manager Assets, portanto, você pode analisá-los no Maestro.

1. (Opcional e condicional) Se você adicionou pelo menos dois campos de data ao ativo vinculado por Experience Manager, clique no link **Exibir** menu suspenso na página tipo de registro do Experience Manager Assets e selecione o **Linha do tempo** exibir ou **Criar visualização** para criar uma visualização de linha do tempo.  Para obter informações, consulte [Gerenciar a exibição de linha do tempo](/help/quicksilver/maestro/views/manage-the-timeline-view.md).
Os ativos vinculados ao Experience Manager Assets são exibidos na visualização de linha do tempo.