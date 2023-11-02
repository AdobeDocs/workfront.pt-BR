---
title: Criar registros
description: Em Adobe Maestro, um registro é uma instância de um tipo de registro. Você deve criar tipos de registro antes de criar registros individuais.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 0699740f8ef0932316843d9aec0008ccdeb319f5
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# Criar registros

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta do Adobe.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Em Adobe Maestro, um registro é uma instância de um tipo de registro.

Você pode ter os seguintes tipos de registros:

* **Registros operacionais**: elas representam objetos relacionados ao trabalho. Por exemplo, para um registro operacional chamado &quot;Campanha&quot;, é possível nomear registros como &quot;Informativo mensal&quot; ou &quot;Vendas de verão&quot;.
* **Registros de taxonomia**: eles representam atributos que podem ser associados a registros operacionais. Por exemplo, para um tipo de registro de taxonomia chamado &quot;Canal&quot;, é possível nomear taxonomias como &quot;Email&quot;, &quot;Mídia social&quot; ou &quot;Publicidade&quot;.

A criação de registros operacionais é idêntica à criação de registros de taxonomia ou taxonomias.

Você pode criar registros no Maestro seguindo um destes procedimentos:

* Criá-los manualmente para os tipos de registro do Maestro
* Conecte-os aos registros do Maestro a partir de aplicativos de terceiros.

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

## Criar registros adicionando-os manualmente a um tipo de registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Você pode criar registros na exibição de tabela de uma página do tipo de registro.

1. Clique em **Menu principal** ícone ![](assets/main-menu-workfront.png) no canto superior direito <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->e, em seguida, clique em **Maestro** ![](assets/maestro-icon.png).
O espaço de trabalho acessado pela última vez é aberto por padrão. Para obter informações sobre como criar espaços de trabalho, consulte [Criar espaços de trabalho](../architecture-and-fields/create-workspaces.md).
1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.
Todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. (Condicional) Se a página do tipo de registro não abrir na exibição de tabela, clique no link **Exibir** e selecione um existente **Visualização em tabela** ![](assets/table-view-icon.png) ou clique em **Criar visualização > Tabela** para criar uma visualização de tabela.

1. Para adicionar novos registros, clique em **Novo &lt; Nome do tipo de registro >** na última linha da tabela

   Ou

   Clique em **Shift + Enter** no teclado a partir de qualquer coluna ou linha da tabela. Isso adiciona uma linha vazia.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Comece a digitar informações na nova linha sobre o novo registro.

   >[!NOTE]
   >
   >  * O campo Nome não é obrigatório. No entanto, recomendamos que você adicione um nome para o registro, pois é útil para identificar registros ao vincular registros uns aos outros.
   >
   >  * Os campos que se referem a outros tipos de registro ou campos calculados são campos somente leitura.

1. Continue adicionando informações em cada linha e clique em **Enter** no teclado para salvar as alterações.

## Criar registros conectando-os de outro aplicativo

Você pode importar registros de outros aplicativos vinculando-os aos registros vinculados Maestri.

1. Crie um tipo de registro Maestri, conforme descrito na seção [Criar tipos de registro](../architecture-and-fields/create-record-types.md).

1. Crie registros Maestri para o tipo de registro criado na etapa anterior. Para obter informações, consulte a seção [Criar registros adicionando-os manualmente a um tipo de registro](#create-records-by-manually-adding-them-to-a-record-type) neste artigo.

1. Crie uma conexão com um tipo de objeto de um aplicativo de terceiros para o tipo de registro Maestri que você criou. Para obter informações, consulte [Conectar tipos de registro](../architecture-and-fields/connect-record-types.md).

1. Adicione registros do aplicativo de terceiros aos registros Maestri criados acima usando o campo de registro vinculado criado na etapa anterior. Para obter informações, consulte [Conectar registros](../records/connect-records.md).

   Os seguintes itens são criados no Maestro:

   * Um tipo de registro Maestro somente leitura que se refere ao tipo de registro de terceiros ao qual você vinculou no campo de registro conectado.

     Por exemplo, se você conectar um tipo de registro Maestro a projetos Workfront, um tipo de registro somente leitura chamado &quot;projetos Workfront&quot; será criado no mesmo espaço de trabalho.
   * Registros somente leitura na página de tipo de registro de terceiros. Os registros importados do aplicativo de terceiros permanecem como somente leitura e só podem ser atualizados no aplicativo original.


## Criar registros copiando e colando informações de uma lista externa

1. No Maestri, comece criando registros na exibição Tabela, conforme descrito na seção [Criar registros adicionando-os manualmente a um tipo de registro](#create-records-by-manually-adding-them-to-a-record-type) neste artigo.

   Certifique-se de que a exibição de tabela Maestro tenha as colunas (ou os campos) que você deseja preencher com as novas informações de registro.

1. Clique em **Novo &lt; Nome do tipo de registro >** na última linha da tabela para adicionar quantas linhas novas desejar aos novos registros.

   Por exemplo, adicione 10 linhas à exibição de tabela se desejar colar as informações de 10 novos registros de outro aplicativo.

1. Em outro aplicativo, crie uma lista de registros que deseja importar no Maestri.

   Por exemplo, você pode usar uma planilha do Excel para criar sua lista.

   A lista deve conter informações em formato de tabela.

   >[!TIP]
   >
   > As colunas da lista devem conter informações para os campos existentes que você tem no Maestro.
   >
   > Certifique-se de que você tem os campos desejados já criados em Maestro e que as informações em sua folha exibe no formato correto que corresponde ao de cada campo em Maestri.

1. No aplicativo de terceiros, selecione várias linhas e colunas e cole as informações na exibição de tabela do tipo de registro, começando com o primeiro novo registro.

   As seguintes informações são importadas no Maestro:

   * As linhas contêm os novos registros
   * As colunas preenchem informações para os campos dos registros.
