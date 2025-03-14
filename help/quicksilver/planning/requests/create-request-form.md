---
title: Criar e Gerenciar um Formulário de Solicitação no Adobe Workfront Planning
description: Depois de selecionar um tipo de registro na área Adobe Workfront Planning, você pode criar um formulário de solicitação e associá-lo a esse tipo de registro. Em seguida, você pode compartilhar um link com outros usuários internos ou externos. Os usuários com um link para o formulário podem preencher os valores de campo nele e, ao enviá-lo, podem adicionar um novo registro para o tipo de registro associado a ele.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 7c39f54677be746ce6305124026df7df598b3da2
workflow-type: tm+mt
source-wordcount: '2121'
ht-degree: 1%

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
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p>
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
   <li><p>Gerenciar permissões para um espaço de trabalho <!--<span class="preview">and record type</span>--> </p></li>
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

## Limitações de exibição de campo e valor em formulários de solicitação

Há limitações na forma como determinados campos são exibidos no formulário de solicitação e em como seus valores serão exibidos posteriormente nos registros ou na página de detalhes da solicitação, após o envio de uma solicitação.

Para obter informações sobre como enviar solicitações do Workfront Planning, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

* Veja a seguir as limitações de como determinados campos são exibidos em formulários de solicitação, registros criados por um formulário de solicitação ou na página de detalhes da solicitação:

   * Não é possível adicionar campos dos seguintes tipos a um formulário de solicitação:

      * Criado por e Modificado pela última vez por
      * Data de criação e data da última modificação
      * Fórmula. <span class="preview">Campos de fórmula com suporte no ambiente de Visualização.</span>
      * Campos de pesquisa de objetos do Workfront
      * Campos de pesquisa de registros conectados do Workfront Planning

* Veja a seguir as diferenças entre como os formatos de campo são exibidos no construtor de formulários de solicitação e como os valores dos campos são formatados no registro ou na página de detalhes da solicitação:

   * Os campos Moeda, Número e Porcentagem são exibidos como um tipo de campo de texto de linha única no construtor de formulários.

     No entanto, o formato do campo é preservado e os valores dos números nesses campos serão exibidos como Moeda, Número e Valores percentuais no tipo de registro e na página de detalhes da solicitação.

<div class="preview">

* A seguir, descrevemos como alguns valores de campo são exibidos nos formulários de solicitação e nas páginas de detalhes da solicitação:

   * A formatação especial dos campos Moeda, Número e Porcentagem não é preservada. Por exemplo, a precisão decimal não é preservada para os valores desses campos nessas áreas.
   * Os valores do campo Pessoas são exibidos como IDs.
   * Os campos de fórmula que não se referem a outros campos ou cálculos não exibem valores. Por exemplo, um campo com uma fórmula `STRING` exibe um valor &quot;N/A&quot;.
   * Os campos de fórmula que se referem aos campos Moeda exibem os valores sem contabilizar taxas de câmbio.
   * Os valores dos campos de parágrafo exibem um valor &quot;N/A&quot; no formulário de solicitação e exibem tags html em vez do texto formatado na página de detalhes da solicitação.

</div>

## Criar um formulário de solicitação para um tipo de registro

{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.

1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho da página e clique em **Criar formulário de solicitação** <span class="preview">ou **Gerenciar formulários de solicitação**, se você já tiver um formulário e quiser criar outros</span>.
1. <span class="preview">(Condicional) Se quiser adicionar outro formulário, clique em **Novo formulário de solicitação**</span>.
1. Atualize o nome do formulário de solicitação. Por padrão, o nome do formulário é **Formulário sem título**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Opcional) Adicione uma **Descrição** para o formulário de solicitação.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Clique em **Criar**. O formulário de solicitação para o tipo de registro selecionado é aberto na guia Formulário.

   ![Modo de edição do formulário de solicitação de campanhas](assets/campaigns-request-form-edit-mode.png)

   O formulário de solicitação contém as seguintes informações, por padrão:

   * Campos de registro disponíveis na exibição de tabela do tipo de registro selecionado. <!--they are working on removing the limitation below-->

   * **Seção padrão**: esta é a quebra de seção padrão que o Workfront aplica ao formulário de solicitação. Todos os campos de registro são exibidos na área **Seção padrão**.
   * Campo **Assunto**: o campo que identificará a solicitação no Workfront. A configuração e o valor do campo Subject não são editáveis.

     >[!TIP]
     >
     >O campo **Assunto** exige um valor quando está visível no formulário de solicitação. No entanto, você pode remover o campo **Assunto**, se necessário, e os solicitantes não o verão no formulário quando enviarem a solicitação.

   * Todos os campos associados ao tipo de registro.

     Os campos contidos no formulário de solicitação estarão visíveis para todos que enviarem uma solicitação para esse tipo de registro.

1. (Opcional) Passe o mouse sobre qualquer campo no formulário que deseja remover, em seguida, clique no ícone **x** para removê-los. Eles são adicionados à guia **Campos** à esquerda do formulário.

   Por exemplo, remova o campo **Assunto**, pois ele não está visível no Workfront Planning. <!--remove this example if this becomes visible in Planning?-->

1. (Opcional) Para remover a **Seção padrão** do formulário, faça o seguinte:

   1. Remova todos os campos da Seção padrão.
   1. Clique em **Elementos de conteúdo**, adicione uma nova seção e adicione um nome à seção.
   1. Adicione campos à nova seção.
   1. Clique no ícone **x** para remover a **Seção padrão**.
1. Clique em qualquer campo e use os controles no painel direito no formulário para definir seu tamanho ou qualquer uma das seguintes informações:

   * **Rótulo**: este é o nome do campo como ele aparecerá no formulário de solicitação. Isso não altera o nome do campo de registro.
   * **Instruções**: adicione mais informações sobre o campo.
   * **Criar um campo obrigatório**: quando selecionado, o campo deve ter um valor. Caso contrário, o formulário não poderá ser enviado.
   * **Adicionar lógica**: defina quais condições devem ser atendidas para que o campo seja exibido ou fique oculto.

   >[!TIP]
   >
   >   O tipo de campo de cada campo é exibido na parte superior do painel direito, depois que você seleciona o campo no formulário.
   >     

1. (Opcional) Clique na guia **Elementos de conteúdo** no lado esquerdo do formulário e adicione qualquer um dos seguintes elementos:

   * **Texto descritivo**
   * **Quebra de seção**

   Para obter mais informações sobre como criar um formulário personalizado, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Opcional) Clique em **Visualizar** para ver como o formulário será exibido para outros usuários quando eles o usarem para enviar um novo registro.

1. (Opcional) Clique na guia **Configuração** e adicione pelo menos um usuário ao campo **Aprovadores** para aprovar novas solicitações para este formulário de registro.

   ![Guia Configuração](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Quando você associa um formulário de solicitação a aprovadores, qualquer nova solicitação deve primeiro ser aprovada por todos os aprovadores antes de gerar um novo registro.
   * Você pode adicionar um ou vários aprovadores a um formulário de solicitação.
   * Se pelo menos um aprovador rejeitar a solicitação, ela será rejeitada e o registro não será criado.
   * Todos os aprovadores devem tomar uma decisão antes que uma solicitação seja aprovada ou rejeitada.

     Para obter mais informações sobre como adicionar aprovações a formulários de solicitação, consulte [Adicionar aprovação a um formulário de solicitação](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do formulário no cabeçalho e clique em **Editar** para atualizar o nome do formulário.
1. Clique em **Publicar** para publicar o formulário e obter um link exclusivo para ele.

   As seguintes situações ocorrem:

   * O botão **Publicar** foi removido.
   * O botão **Cancelar publicação** é adicionado ao formulário. Clicar nele impedirá que o formulário seja acessível.
   * Um botão **Compartilhar** é adicionado ao formulário.

1. Clique em **Compartilhar** para compartilhar o formulário com outras pessoas.

   ![Compartilhar caixa para o formulário de solicitação](assets/share-box-for-request-form.png)

1. Selecione entre as seguintes opções para indicar quais tipos de usuários podem acessar este formulário:

   * Qualquer pessoa com acesso de exibição ou superior ao espaço de trabalho
   * Qualquer pessoa com acesso de contribuição ou superior ao espaço de trabalho
   * Qualquer pessoa com o link

   >[!WARNING]
   >
   >* Quando você seleciona **Qualquer pessoa com o link**, qualquer pessoa pode acessar o formulário e enviar um novo registro, mesmo pessoas fora da sua organização que não tenham uma conta do Workfront.
   >
   >* Um formulário que contém os seguintes tipos de campo não pode ser compartilhado publicamente:
   >
   >     * Conexões do Workfront ou AEM Assets
   >     * Pessoas
   >

1. (Condicional) Se você selecionou **Qualquer pessoa com o link** na etapa anterior, selecione a **Data de expiração do link** no calendário disponível. <!--take out this tip when we release to production as in multiple forms this is no longer happening-->

   >[!TIP]
   >
   >Há uma indicação de que o link é compartilhado publicamente quando isso ocorre.
   >![Link compartilhado publicamente para formulário no menu de tipo de registro](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)

   As pessoas receberão um erro depois que o link expirar e você deverá atualizar a data do link e gerar um novo link para compartilhar antes que as pessoas possam acessar o formulário novamente.

   Você pode selecionar datas futuras dentro de 180 dias a partir da data atual.

   >[!TIP]
   >
   ><span class="preview">Depois que a data de compartilhamento expirar, o formulário de solicitação não estará mais disponível na área Solicitações do Workfront e os links compartilhados com outros usuários não estarão mais acessíveis.</span>


1. <span class="preview">(Opcional)</span> Clique em **Salvar e copiar link** para salvar os detalhes de compartilhamento do formulário. Se o formulário foi salvo anteriormente, clique em **Copiar link**.

   As opções de compartilhamento de formulário são salvas e o link é copiado para a área de transferência. Agora você pode compartilhá-lo com outras pessoas.

   Para obter informações sobre como criar registros usando um link para um formulário de solicitação, consulte [Enviar solicitações do Adobe Workfront Planning](/help/quicksilver/planning/requests/submit-requests.md).

1. Clique em **Salvar** no canto inferior direito da guia **Formulário** para salvar o formulário.

1. Clique na seta à esquerda do nome do formulário no cabeçalho para fechar o formulário.

   <span class="preview">A exibição de tabela **Formulários de solicitação** é aberta e o formulário é adicionado a ela.</span>

1. <span class="preview">(Opcional) Passe o mouse sobre o nome de um formulário de solicitação na exibição de tabela, em seguida, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do formulário e clique em um dos seguintes:</span>

   * <span class="preview">**Editar formulário**: clique para editar mais informações sobre o formulário. </span>
   * <span class="preview"> **Cancelar publicação**: clique para desfazer a publicação do formulário que o remove da área Solicitações no Workfront. </span>
   * <span class="preview">**Compartilhar**: clique aqui para modificar quem tem acesso ao formulário. </span>
   * <span class="preview">**Copiar link**: clique para copiar rapidamente o link do formulário de solicitação sem abrir o formulário. </span>
   * <span class="preview">**Excluir**: clique aqui para excluir o formulário. Todas as solicitações e registros adicionados usando o formulário não são excluídos. O formulário não pode ser recuperado. </span>

   ![Mais menus no formulário de solicitação da lista de formulários de solicitação](assets/more-menu-on-request-form-from-request-forms-list.png)


1. <span class= "preview">Clique na seta apontando para a esquerda de **Formulários de solicitação** no cabeçalho para fechar a tabela de formulários de solicitação.   </span>

   <span class= "preview">A página de tipo de registro é aberta. </span>
1. (Opcional e condicional) Para editar um formulário existente, siga um destes procedimentos, dependendo do ambiente que você está usando:

   * No ambiente de produção:

      1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho e siga um destes procedimentos:

      1. Clique em **Atualizar formulário de solicitação** para fazer alterações no formulário de solicitação.
      1. Clique em **Copiar link para solicitar o formulário** para compartilhar o link para o formulário com outras pessoas.

   * <span class="preview">No ambiente de Visualização:

      1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho e clique em **Gerenciar formulários de solicitação**. </span>

         <span class="preview">Isso abre a exibição de tabela dos formulários de Solicitação. </span>

      1. <span class="preview">Clique em um formulário de solicitação para abri-lo e editá-lo.</span>
      1. <span class= "preview">(Opcional) Vá para a área **Solicitações** no Workfront e localize o formulário compartilhado para enviar uma solicitação. Para obter informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).</span>
