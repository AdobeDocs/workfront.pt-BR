---
title: Enviar solicitações do Adobe Workfront Planning
description: Depois que alguém compartilhar um link para um formulário de solicitação com você a partir de uma página de tipo de registro no Adobe Workfront Planning, você poderá adicionar uma solicitação para criar registros para o tipo de registro associado ao formulário de solicitação.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ca8f1375d641531eaf11e3889ccb67a6fbe1788f
workflow-type: tm+mt
source-wordcount: '2460'
ht-degree: 1%

---

# Enviar solicitações do Adobe Workfront Planning para criar registros

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Depois que um gerenciador de espaço de trabalho cria um formulário de solicitação para um tipo de registro no Adobe Workfront Planning, você pode usar o formulário para submeter solicitações que criarão registros para o tipo de registro associado ao formulário.

Você pode submeter uma solicitação do Workfront Planning nas seguintes áreas:

* Na área Solicitações do Workfront ou no widget Minhas solicitações na Página inicial.
* De um link direto para o formulário de solicitação que foi compartilhado.
* Na página tipo de registro, ao adicionar um novo registro enviando uma solicitação. Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).

Este artigo descreve como enviar uma solicitação para adicionar novos registros a um tipo de registro da área Solicitações do Workfront ou de um link compartilhado.

Os gerentes do Workspace podem criar forms de solicitação que você pode usar, como usuário ou pessoa externa, para submeter solicitações aos tipos de registro do Planning. As solicitações criam registros para o tipo de registro associado ao formulário de solicitação.

Para obter informações sobre como um gerenciador de espaço de trabalho pode criar um formulário de solicitação e associá-lo a um tipo de registro, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront ou Workflow</p>
<p>Qualquer pacote do Workfront Planning</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront.</p>
   </td> </tr>
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Qualquer</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Exibir permissões ou mais altas para um espaço de trabalho e tipo de registro, se você for um usuário do Workfront</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Para que você possa enviar uma solicitação para um formulário de solicitação do Workfront Planning, é necessário que o seguinte esteja em vigor:

* Deve existir o seguinte no Workfront Planning:

   * Um espaço de trabalho
   * Um tipo de registro
   * Um formulário de solicitação associado a um tipo de registro.

     Para obter informações, consulte [Criar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* O formulário de solicitação deve ser compartilhado de uma maneira que você possa acessá-lo. Existem os seguintes cenários:

   * Internamente, o formulário deve ser compartilhado com usuários que têm permissões de Exibição ou superiores para o espaço de trabalho.

     Os usuários do Workfront podem acessar o formulário por meio de um link ou localizá-lo na área Solicitações do Workfront.

   * Externamente, compartilhando um link para o formulário de registro com pessoas externas que não têm uma conta do Workfront.

     Os usuários do Workfront também podem acessar o link compartilhado com pessoas externas.

* Se compartilhado com um link, o link para o formulário não deve expirar.

## Considerações sobre o envio de solicitações ao Workfront Planning

* Não é possível editar uma solicitação no Workfront depois de enviá-la.
* Cada solicitação enviada cria um registro para o tipo de registro associado ao form usado, se o form não estiver associado a uma aprovação ou se a aprovação tiver sido concedida por todos os aprovadores.
* Os registros criados ao enviar formulários de solicitação são idênticos aos registros adicionados por qualquer outro método no Workfront Planning.

  Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).
* Os registros criados enviando formulários de solicitação são conectados à solicitação original. Esta conexão não pode ser removida.
* Você pode exibir os registros criados e as solicitações usadas para criá-los nas seguintes áreas:
   * Área de solicitações no Workfront.

  <div class="preview">

   * Em um campo conectado de uma página do tipo de registro no Workfront Planning quando você adiciona a solicitação como um registro conectado.
   * Em um campo conectado da área Detalhes de um registro no Workfront Planning quando você adiciona a solicitação como um registro conectado.

  </div>

  >[!TIP]
  >
  ><span class="preview">Você pode exibir o nome da solicitação no campo Assunto na área Solicitações do Workfront ou no campo Conexão da solicitação original no Workfront Planning. </span>

* As solicitações de Planejamento enviadas estão visíveis somente na nova experiência de solicitação. Não é possível ver as solicitações do Planning na experiência de solicitação herdada.

  Para obter informações, consulte [Criar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).
* Há limitações na forma como determinados tipos de campo são exibidos em um formulário de solicitação ou na página de detalhes da solicitação após o envio de um formulário.

  Para obter informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--
Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.
-->


## Enviar uma solicitação ao Workfront Planning na área Solicitações do Workfront

{{step1-to-requests}}

1. Ative a configuração **Usar nova experiência**, no canto superior direito da tela.
Ativar essa configuração torna os formulários de solicitação do Workfront Planning disponíveis na área **Solicitações** do Workfront.

   >[!TIP]
   >
   >Essa configuração só está disponível quando a instância do Workfront é integrada à Experiência unificada do Adobe.
   >
   >Para poder enviar solicitações do Workfront Planning nessa área, você deve atender às seguintes condições:
   >
   >* Sua empresa adquiriu uma licença do Workfront Planning.
   >
   >* Você tem acesso para exibir pelo menos um espaço de trabalho.

1. Clique na **Que solicitação deseja enviar?Barra** para abrir uma lista de formulários de solicitação.
1. Selecione um formulário de solicitação na lista ou comece a digitar o nome do formulário de solicitação e selecione-o quando ele aparecer na lista.

   Uma janela é aberta com o nome do formulário de solicitação na parte superior.

   >[!TIP]
   >
   >As filas de solicitações do Workfront contêm o nome da fila e o nome do formulário na lista de solicitações. Os formulários de solicitações do Planning exibem somente o nome do formulário na lista de solicitações.

1. Atualize o campo **Assunto**. Este é o nome da solicitação. Este campo é obrigatório.
1. Atualize o campo **Nome**. Este é o nome do registro futuro.

   >[!TIP]
   >
   >O campo **Nome** é exclusivo da sua organização e pode exibir um rótulo diferente na sua instância do Workfront. O campo é o campo principal do registro.

1. Atualize os campos restantes no formulário de solicitação. Os campos com um asterisco vermelho são obrigatórios.
1. (Condicional) Se sua organização permitir o **Preenchimento de formulário** ativado por IA, você poderá carregar documentos como prompts. A IA usa esses documentos para preencher o formulário e você pode aceitar ou rejeitar as sugestões de IA antes de enviar a solicitação.


   Para obter instruções, consulte [Usar preenchimento de formulário fornecido pela IA para preencher uma solicitação usando prompts ou documentos](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).
1. Clique em **Enviar**.

   O formulário de solicitação é fechado e você retorna à área **Solicitações**.

   Seu formulário é enviado e os seguintes itens ocorrem:

   * Se o formulário de solicitação não estava associado a uma aprovação, a solicitação é adicionada à lista Solicitações na área Solicitações do Workfront e o widget Minhas solicitações na Página inicial, e um novo registro é adicionado ao tipo de registro associado ao formulário.

     Os campos a seguir exibem informações de solicitação e registro na área Solicitações e o widget Minhas solicitações na Página inicial:

      * **Assunto**: o nome da solicitação original como adicionado na área Solicitações. Você não pode ocultar ou remover o campo **Assunto** da lista de solicitações. O nome tem um link que abre a página de solicitação no Planning.
      * **Objeto criado**: o nome do registro que foi criado a partir da solicitação como ele é exibido no Planning. O nome do objeto criado tem um link que abre o registro criado a partir da solicitação.
      * **Tipo de objeto**: o nome do espaço de trabalho e o tipo de registro em que foram criados registros a partir da solicitação no Planning.
      * **Status**: o status do objeto de solicitação.
      * **Formulário de solicitação**: o nome do formulário de solicitação associado ao tipo de registro no Planning.
      * <span class="preview">**Status do objeto criado**: o status do registro criado.</span>

   * Se o formulário de solicitação foi associado a uma aprovação, a solicitação é adicionada à lista Solicitações na área Solicitações do Workfront e ao widget Minhas solicitações com o status **Revisão pendente**. Um novo registro é adicionado à página de tipo de registro somente após ser aprovado pelos aprovadores.

     Para obter informações, consulte [Adicionar uma aprovação a um formulário de solicitação](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * <span class="preview">Você pode adicionar o campo de conexão **Solicitação original** a um tipo de registro no Planning para exibir o nome da solicitação original que criou um registro. Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md). </span>
   * A solicitação é visível somente para o proprietário, aprovador e pessoas que têm pelo menos permissões de Visualização no espaço de trabalho. Os administradores do Workfront podem exibir todas as solicitações enviadas para qualquer espaço de trabalho no sistema.
   * Você recebe uma notificação no aplicativo e uma notificação por email informando que a solicitação foi enviada com êxito ou para revisão.
   * Se o formulário de solicitação foi associado a uma aprovação, os aprovadores recebem uma notificação no aplicativo e uma notificação por email para revisar e aprovar a solicitação.

     >[!NOTE]
     >
     >As notificações por email e no aplicativo ficam visíveis somente quando a instância do Workfront de sua organização é integrada à Adobe Unified Experience.
     >
     >Há um link para a solicitação na notificação de confirmação ou aprovação por email.

1. (Opcional) Clique em **Exibir sua solicitação** na mensagem de confirmação para abrir a solicitação ou clique no ícone **X** para fechar a confirmação.
1. (Opcional) Para gerenciar a forma como as informações são exibidas na lista de solicitações, atualize os seguintes elementos de exibição para a lista:

   * Visualizar
   * Filtro
   * Colunas

   <div class="preview">

   * Agrupamento
   * Formatar células
   * Altura da linha

   </div>


   Para obter informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   <!-- 
   Removing this as this is covered at a higher level in the Use enhanced lists article: 
   1. (Optional) From the requests list, do any of the following:
      * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 
         ![Editing filters in the Requests area](assets/filters-editing-box-in-requests-planning-tab.png)
         You can filter by the following fields:  
         * **Workspace**: The workspace the request form is associated with.
         * **Object type**: The record type the request form is associated with.
         * **Entry date**: The date when the request was submitted.
         * **Request form**: The name of the request form used to submit the request.
         * **Status**: The status of the request.
         * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.
        You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
      * Click **Columns** to open the **Fields visibility and order** box, then hide, show, or rearrange the columns in the request list. 
         >[!TIP]
         >
         >You cannot add any more columns. 
         ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)
      * Click the **+** icon in the upper-right corner of the request list to open the **Column manager** and add or remove columns in the requests list. 
   -->

1. Clique no nome de uma solicitação na lista.

   A página de detalhes da solicitação é aberta.

   ![Solicitar página com comentário](assets/new-request-page-with-comment.png)

1. (Opcional) Insira um comentário na área **Comentários**.
1. (Condicional) Se o formulário de solicitação não estiver associado a uma aprovação ou se a solicitação tiver sido aprovada, clique no nome da solicitação e, em seguida, clique no nome do registro no campo **Objeto criado**.

   A página do registro é aberta no Workfront Planning.

   >[!TIP]
   >
   >* Se o campo principal do registro não foi atualizado no formulário de solicitação, o nome do registro no campo Registro da solicitação será exibido como **Sem título**.
   >
   >* Se o formulário de solicitação estiver associado a uma aprovação, a aprovação deverá ser concedida antes que você possa acessar o registro da página de solicitação. O registro não é criado até que a aprovação seja concedida.

1. (Opcional) Clique no nome do **Tipo de registro**.

   A página de tipo de registro é aberta no Workfront Planning.

## Enviar uma solicitação ao Workfront Planning a partir de um link compartilhado para um formulário de solicitação

As informações nesta seção se aplicam apenas às pessoas que enviam uma solicitação de um link compartilhado e que podem não ter uma conta do Workfront.

Pessoas externas não podem acessar áreas internas da Workfront, como **Solicitações** ou **Residência**.

1. Acesse o link compartilhado com você a partir de um tipo de registro do Workfront Planning.

1. Atualize os campos disponíveis no formulário. Os campos com um asterisco são obrigatórios.

   >[!TIP]
   >
   >   Se o campo **Assunto** estiver disponível, ele não estará visível no Workfront Planning após o envio da solicitação.
   >
   >Recomendamos que você atualize o máximo possível de campos em sua solicitação para tornar o novo registro identificável quando ele for adicionado ao tipo de registro no Workfront Planning.

1. Clique em **Enviar**.

   Seu formulário será enviado e você receberá uma confirmação.

   Se o formulário estiver associado a uma aprovação, ele deverá ser aprovado antes de criar um registro.

1. (Opcional) Clique em **Enviar outra solicitação** para adicionar outra solicitação usando o mesmo link compartilhado.

   * Se o formulário de solicitação não estava associado a uma aprovação, a solicitação é adicionada à lista Solicitações na área Solicitações do Workfront e o widget Minhas solicitações na Página inicial, e um novo registro é adicionado ao tipo de registro associado ao formulário. Isso está disponível somente quando você faz logon no Workfront.

   * Se o formulário de solicitação foi associado a uma aprovação, a solicitação é adicionada à lista Solicitações na área Solicitações do Workfront e o widget Minhas solicitações com um status Revisão pendente. Um novo registro é adicionado à página de tipo de registro somente após ser aprovado por todos os aprovadores. Isso está disponível somente quando você faz logon no Workfront.

     Para obter informações, consulte [Adicionar uma aprovação a um formulário de solicitação](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     >[!IMPORTANT]
     >
     >Você pode exibir somente as solicitações submetidas por você ou por qualquer outra pessoa aos espaços de trabalho para os quais você tem pelo menos permissões. Os administradores do Workfront podem exibir todas as solicitações enviadas para qualquer espaço de trabalho no sistema.

   * Você recebe uma notificação no aplicativo e uma notificação por email informando que a solicitação foi enviada com êxito ou para revisão.
   * Se o formulário de solicitação foi associado a uma aprovação, os aprovadores recebem uma notificação no aplicativo e uma notificação por email para revisar e aprovar a solicitação.

     >[!NOTE]
     >
     >As notificações por email e no aplicativo ficam visíveis somente quando a instância do Workfront de sua organização é integrada à Adobe Unified Experience.

   <span class="preview"> Depois que a solicitação foi aprovada e o registro foi criado, os campos Approved by e Approved date exibem informações sobre a aprovação no registro.</span>

1. (Opcional) Clique em **Exibir sua solicitação** para abrir a solicitação no Workfront.

Ou

Clique em [Enviar outra solicitação](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) para abrir o formulário e adicionar uma nova solicitação.

A página de detalhes da solicitação é aberta.

![Solicitar página com comentário](assets/new-request-page-with-comment.png)

1. (Opcional) Insira um comentário na área **Comentários**.
1. (Condicional) Se o formulário de solicitação não estiver associado a uma aprovação ou se a solicitação tiver sido aprovada, clique no nome da solicitação e, em seguida, clique no nome do registro no campo **Objeto criado**.

   A página do registro é aberta no Workfront Planning.

   >[!TIP]
   >
   >* Se o nome do registro não foi adicionado ao formulário de solicitação, o nome do registro no campo Registro da solicitação será exibido como **Sem título**.
   >
   >* Se o formulário de solicitação estiver associado a uma aprovação, a aprovação deverá ser concedida antes que você possa acessar o registro da página de solicitação.

1. (Opcional) Clique no nome do **Tipo de objeto**.

   A página de tipo de registro é aberta no Workfront Planning.

## Criar uma solicitação copiando uma solicitação existente

Você pode copiar uma solicitação na lista de solicitações no Workfront e, em seguida, editar os detalhes e enviá-la como uma nova solicitação.

Isso está disponível somente na nova experiência de solicitação.

Copiar uma solicitação de Planejamento existente e submetê-la como uma nova é semelhante a copiar uma solicitação Workfront existente.

Para obter mais informações, consulte [Copiar e enviar solicitações](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Criar rascunhos e solicitações a partir de rascunhos existentes

Você pode criar um rascunho de uma solicitação, voltar ao rascunho e submetê-lo posteriormente como uma solicitação.

Isso está disponível somente na nova experiência de solicitação. A criação de rascunhos e solicitações a partir de rascunhos existentes no Workfront Planning é idêntica à criação a partir do Adobe Workfront.

Para obter mais informações, consulte [Criar solicitações de rascunhos](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).

## Excluir rascunhos ou solicitações enviadas

É possível excluir solicitações enviadas ou seus rascunhos ao usar a nova experiência de solicitações.

Quando você exclui uma solicitação do Planning, as seguintes situações ocorrem:

* A solicitação não pode ser recuperada.
* O registro criado da solicitação não é excluído.
* Os rascunhos excluídos não podem ser recuperados. Não há registros associados a rascunhos.

Excluir solicitações do Planning é semelhante a excluir solicitações do Workfront.

Para obter informações, consulte [Excluir uma solicitação enviada ou rascunho da solicitação](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md).







