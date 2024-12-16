---
title: Criar e Gerenciar um Formulário de Solicitação no Adobe Workfront Planning
description: Depois de selecionar um tipo de registro na área Adobe Workfront Planning, você pode criar um formulário de solicitação e associá-lo a esse tipo de registro. Em seguida, você pode compartilhar um link com outros usuários internos ou externos. Os usuários com um link para o formulário podem preencher os valores de campo nele e, ao enviá-lo, podem adicionar um novo registro para o tipo de registro associado a ele.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 9b5ba629fa2f50f0425f4afbfd4faa891d917845
workflow-type: tm+mt
source-wordcount: '1557'
ht-degree: 2%

---

# Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode criar um formulário de solicitação e associá-lo a um tipo de registro no Adobe Workfront Planning. Em seguida, você pode compartilhar um link com outros usuários internos ou externos.

Os usuários com um link para o formulário podem atualizar os valores de campo nele e adicionar novos registros enviando-o.

Este artigo descreve como um gerenciador de espaço de trabalho pode criar um formulário de solicitação associado a um tipo de registro.

Para obter informações sobre como enviar uma solicitação a um tipo de registro para criar um registro, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produtos</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td>
   <td>
<p>Qualquer um dos seguintes planos da Workfront:</p>
<ul><li>Selecionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p>
   </td>

<tr>
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td>
   <td>
<p>Qualquer </p>  
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </td>

<tr>
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td>
   <td>
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões de objeto</p></td>
   <td>
   <ul>
   <li><p>Gerenciar permissões em um espaço de trabalho</p></li>
    <li><p>Os administradores do sistema podem gerenciar espaços de trabalho que não criaram. </p></li>
    </ul>
   <p>Para obter informações sobre o compartilhamento de permissões para objetos do Workfront Planning, consulte  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Visão geral das permissões de compartilhamento no Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um formulário de solicitação para um tipo de registro

{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.

1. Clique no menu **Mais** ![](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho da página e clique em **Criar formulário de solicitação**.
1. Atualize o nome do formulário de solicitação. Por padrão, o nome do formulário é **Formulário sem título**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Opcional) Adicione uma **Descrição** para o formulário de solicitação.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Clique em **Criar**. O formulário de solicitação para o tipo de registro selecionado abre <span class="preview"> na guia Formulário </span>.

   ![](assets/campaigns-request-form-edit-mode.png)

   O formulário de solicitação contém as seguintes informações, por padrão:

   * Campos de registro disponíveis na exibição de tabela do tipo de registro selecionado. <!--they are working on removing the limitation below-->

   >[!IMPORTANT]
   >
   > Dependendo do ambiente usado para criar um formulário de solicitação, os seguintes cenários existem:
   >
   >* Campos dos seguintes tipos não são exibidos no formulário de solicitação <span class="preview"> nos ambientes de Pré-visualização </span> ou Produção:
   >
   >    * Criado por e Modificado pela última vez por
   >    * Fórmula
   >    * Data de criação e data da última modificação
   >    * Campos de pesquisa de objetos do Workfront
   >    * Campos de pesquisa de registros conectados do Workfront Planning
   >    * Campos conectados do AEM Assets
   >* Os campos dos seguintes tipos não são exibidos no formulário de solicitação no ambiente de Produção. <span class="preview">Eles são exibidos no ambiente de Visualização:</span>
   >    * <span class="preview"> campos conectados de registros do Workfront Planning</span>
   >    * <span class="preview">Pessoas </span>
   >    * <span class="preview">Campos conectados de objetos do Workfront</span>
   >    * <span class="preview">Campos conectados do AEM Assets </span>


   * **Seção padrão**: esta é a quebra de seção padrão que o Workfront aplica ao formulário de solicitação. A seção Padrão não pode ser renomeada ou removida.
   * Campo **Assunto**: o campo que identificará a solicitação no Workfront. Esse recurso ainda não está disponível no ambiente de produção. <span class="preview">Está disponível no ambiente de visualização.</span> A configuração e o valor do campo Assunto não são editáveis.

     >[!TIP]
     >
     >O campo **Assunto** exige um valor quando está visível no formulário de solicitação. No entanto, você pode remover o campo **Assunto**, se necessário, e os solicitantes não o verão no formulário.

   * Todos os campos associados ao tipo de registro.

     Os campos contidos no formulário de solicitação estarão visíveis para todos que enviarem uma solicitação para esse tipo de registro.

1. (Opcional) Passe o mouse sobre qualquer campo no formulário que deseja remover, em seguida, clique no ícone **x** para removê-los. Eles são adicionados à guia **Campos** à esquerda do formulário.

   Por exemplo, remova o campo **Assunto**, pois ele não está visível no Workfront Planning. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Clique em qualquer campo e use os controles no painel direito no formulário para definir seu tamanho ou qualquer uma das seguintes informações:

   * **Rótulo**: este é o nome do campo como ele aparecerá no formulário de solicitação. Isso não altera o nome do campo de registro.
   * **Instruções**: adicione mais informações sobre o campo.
   * **Criar um campo obrigatório**: quando selecionado, o campo deve ter um valor. Caso contrário, o formulário não poderá ser enviado.
   * **Adicionar lógica**: defina quais condições devem ser atendidas para que o campo seja exibido ou fique oculto.

   >[!NOTE]
   >
   >   O tipo de campo de cada campo é exibido na parte superior do painel direito, depois que você seleciona o campo no formulário.
   >   
   >
   >   Os campos Moeda, Número e Porcentagem são exibidos como um tipo de campo de texto de linha única. No entanto, o formato do campo é preservado e os valores dentro desses campos serão exibidos como valores de Moeda, Número e Porcentagem.

1. (Opcional) Clique na guia **Elementos de conteúdo** no lado esquerdo do formulário e adicione qualquer um dos seguintes elementos:

   * **Texto descritivo**
   * **Quebra de seção**

   Para obter mais informações sobre como criar um formulário personalizado, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Opcional) Clique em **Visualizar** para ver como o formulário será exibido para outros usuários quando eles o usarem para enviar um novo registro.

1. 
   <div class="preview">(Opcional) Clique na guia **Configuração** e adicione pelo menos um usuário ao campo **Aprovadores** para aprovar novas solicitações para esse formulário de registro.

   ![](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Quando você associa um formulário de solicitação a aprovadores, qualquer nova solicitação deve primeiro ser aprovada por todos os aprovadores antes de gerar um novo registro.
   * Você pode adicionar um ou vários aprovadores a um formulário de solicitação.
   * Se pelo menos um aprovador rejeitar a solicitação, ela será rejeitada e o registro não será criado.
   * Todos os aprovadores devem tomar uma decisão antes que uma solicitação seja aprovada ou rejeitada.

     Para obter mais informações sobre como adicionar aprovações a formulários de solicitação, consulte [Adicionar aprovação a um formulário de solicitação](/help/quicksilver/planning/requests/add-approval-to-request-form.md). </div>

1. (Opcional) Clique no menu **Mais** ![](assets/more-menu.png) à direita do nome do formulário no cabeçalho e clique em **Editar** para atualizar o nome do formulário.
1. Clique em **Publish** para publicar o formulário e obter um link exclusivo para ele.

   As seguintes situações ocorrem:

   * O botão **Publish** foi removido.
   * O botão **Cancelar publicação** é adicionado ao formulário. Clicar nele impedirá que o formulário seja acessível.
   * Um botão **Compartilhar** é adicionado ao formulário.

1. Clique em **Compartilhar** para compartilhar o formulário com outras pessoas.

   ![](assets/share-box-for-request-form.png)

1. Selecione entre as seguintes opções para indicar quais tipos de usuários podem acessar este formulário:

   * Qualquer pessoa com acesso de exibição ou superior ao espaço de trabalho
   * Qualquer pessoa com acesso de contribuição ou superior ao espaço de trabalho
   * Qualquer pessoa com o link

   >[!WARNING]
   >
   >
   >* Quando você seleciona **Qualquer pessoa com o link**, qualquer pessoa pode acessar o formulário e enviar um novo registro, mesmo pessoas fora da sua organização que não tenham uma conta do Workfront.
   >
   > * <span class="preview">Um formulário que contém os seguintes tipos de campo não pode ser compartilhado publicamente:</span>
   >
   >     * <span class="preview">Fórmula</span>
   >     * <span class="preview">Conexões do Workfront ou AEM Assets</span>
   >     * <span class="preview">Campos de pesquisa</span>
   >     * <span class="preview">Pessoas</span>
   >

1. (Condicional) Se você selecionou **Qualquer pessoa com o link** na etapa anterior, selecione a **Data de expiração do link** no calendário disponível. As pessoas receberão um erro depois que o link expirar e você deverá atualizar a data do link e gerar um novo link para compartilhar antes que as pessoas possam acessar o formulário novamente.

   Você pode selecionar datas futuras dentro de 180 dias a partir da data atual.

1. Clique em **Salvar e copiar link** para salvar os detalhes de compartilhamento do formulário.

   As opções de compartilhamento de formulário são salvas e o link é copiado para a área de transferência. Agora você pode compartilhá-lo com outras pessoas.

   Para obter informações sobre como criar registros usando um link para um formulário de solicitação, consulte [Enviar solicitações do Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Clique em **Salvar** no canto inferior direito da guia **Formulário** para salvar o formulário.
1. Clique na seta à esquerda do nome do formulário no cabeçalho para fechar o formulário.

   A página de tipo de registro é aberta.
1. (Opcional) Clique no menu **Mais** ![](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho e siga um destes procedimentos:
   * Clique em **Atualizar formulário de solicitação** para fazer alterações no formulário de solicitação.
   * Clique em **Copiar link para o formulário de solicitação** para compartilhar o link para o formulário com outras pessoas.

   >[!TIP]
   >
   >Há uma indicação de que o link é compartilhado publicamente quando isso ocorre.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
