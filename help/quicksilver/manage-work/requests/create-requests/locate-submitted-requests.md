---
product-area: requests
navigation-topic: create-requests
title: Exibir solicitações enviadas
description: Saiba mais sobre as áreas do Adobe Workfront em que você pode visualizar solicitações enviadas por você ou por outra pessoa, ou solicitações que você nunca enviou e que foram salvas como rascunhos.
author: Becky
feature: Requests
topic: Collaboration
role: User
exl-id: cfa2383a-9594-4867-9b48-11b8ea281486
source-git-commit: b0060470156728a7ad98838378a7d963e2b5fd01
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 3%

---

# Visualizar solicitações enviadas

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Você pode exibir as solicitações que você ou outra pessoa submeteu, ou as solicitações que você iniciou, mas que você nunca terminou de submeter. Você pode localizar essas solicitações nas seguintes áreas do Adobe Workfront:

* A guia **Workfront** da área Solicitações do Workfront: Exiba solicitações enviadas às filas de solicitações do Workfront nas seguintes seções:
   * **Seção enviada**: todas as solicitações que você ou outra pessoa enviou e que você tem acesso a pelo menos Exibir.
   * **Seção de rascunho**: todas as solicitações que você iniciou, mas nunca terminou e nunca enviou. Para obter mais informações sobre rascunhos de solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

  >[!NOTE]
  >
  >* Você só pode exibir seus próprios rascunhos de solicitações.
  >* <span class="preview">Na nova experiência de solicitação, rascunhos e solicitações enviadas são encontrados na mesma lista. </span>
  >* <span class="preview">Os rascunhos criados na experiência herdada não aparecem na nova experiência de Solicitação.</span>

* A guia **Planning** da área Solicitações no Workfront: Exibir solicitações enviadas aos formulários de solicitação do Workfront Planning. Sua organização deve comprar um pacote do Workfront Planning. Para obter informações, consulte os seguintes artigos:

   * [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
   * [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md)


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Colaborador ou superior</p>
   <p>Solicitação ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td><p>Editar acesso a ocorrências</p></td> 
  </tr>
  <tr>
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>Exibir permissões ou superiores nas solicitações</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produto</td> 
   <td> <ul><li>Adobe Workfront</li><li>Você precisa ter o Adobe Workfront Planning para exibir solicitações ou formulários de solicitação do Planning</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir solicitações enviadas na área Solicitações

A exibição de solicitações enviadas é diferente dependendo se você está usando a experiência de solicitação nova ou herdada.

* [Exibir solicitações enviadas na nova experiência de solicitação](#view-submitted-requests-in-the-new-requesting-experience)
* [Exibir solicitações enviadas na experiência herdada de solicitação](#view-submitted-requests-in-the-legacy-requesting-experience)

### Exibir solicitações enviadas na nova experiência de solicitação

Você pode exibir solicitações enviadas na área Solicitações, <span class="preview">que inclui links para objetos criados por essas solicitações.</span>

Para exibir solicitações que você ou outros usuários enviaram na nova experiência de solicitação:

{{step1-to-requests}}

1. Verifique se o botão **Usar nova experiência**, no canto superior direito da tela, está habilitado.

   A lista Solicitações é exibida.

1. (Opcional) Para pesquisar uma solicitação, comece digitando na barra de pesquisa no canto superior direito da lista. Os resultados da pesquisa são exibidos à medida que você digita.
1. (Opcional) Clique em **Filtros** e comece a adicionar condições para as solicitações que deseja exibir.

   Você pode filtrar pelos seguintes campos:

   * **Workspace**: o espaço de trabalho ao qual o formulário de solicitação está associado.
   * **Tipo de registro**: o tipo de registro ao qual o formulário de solicitação está associado.
   * **Data de entrada**: a data em que a solicitação foi enviada.
   * **Formulário de solicitação**: o nome do formulário de solicitação usado para enviar a solicitação.
   * **Status**: o status da solicitação.
   * **Inserido por**: o nome do usuário que adicionou a solicitação. Se a solicitação foi adicionada por alguém fora do Workfront, o campo **Informado por** mostrará `N/A`.

   Você pode ter vários filtros unidos por **And** ou **Or**.
A lista de solicitações é filtrada automaticamente ao adicionar as condições de filtro.
1. (Opcional) Use as exibições para se concentrar nas solicitações que você deseja exibir.

   Para obter instruções, consulte [Criar ou editar exibições na área Solicitações](/help/quicksilver/manage-work/requests/create-requests/create-views-for-requests-list.md).
1. (Opcional) Verifique o status de uma solicitação verificando a coluna Status. Os seguintes status estão disponíveis na nova experiência de solicitação:

   * Rascunho: Esta solicitação ainda não foi enviada.
   * Revisão pendente
   * Em revisão
   * Rejeitado
   * Em andamento
   * Completo

>[!NOTE]
>
>* Se você tiver o Workfront Planning, suas solicitações do Workfront e do Planning serão exibidas na mesma lista. As solicitações Workfront exibem o valor `Issue` na coluna Tipo de objeto.
>* A lista Solicitações é exibida com 50 solicitações exibidas. Para visualizar mais solicitações, navegue até a parte inferior da lista.

### Exibir solicitações enviadas na experiência herdada de solicitação

Para exibir solicitações que você ou outros usuários enviaram na experiência de solicitação herdada:

{{step1-to-requests}}

1. (Condicional) Se sua organização adquiriu um pacote do Workfront Planning, clique na guia **Workfront** para exibir as solicitações do Workfront.
1. Clique em **Enviado** no painel esquerdo para exibir todas as solicitações enviadas.

   É possível exibir até 2000 solicitações, que podem ser exibidas em várias páginas.

   >[!TIP]
   >
   >Não é possível personalizar as colunas na lista Solicitação enviada.

   ![](assets/nwe-submitted-requests-new-list-350x57.png)


1. As seguintes colunas são exibidas por padrão:

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
      <tr> 
         <td role="rowheader">Nome</td> 
         <td> <p>O nome da solicitação.</p> <p>Clique no nome de uma solicitação para abri-la. </p> <p><b>DICA</b>

   Se o problema não foi preservado quando foi convertido em uma tarefa ou um projeto, o nome do problema estará esmaecido e não poderá mais ser clicado. Para obter informações sobre a conversão de problemas, consulte <a href="../../../manage-work/issues/convert-issues/convert-issues.md" class="MCXref xref">Visão geral da conversão de problemas no Adobe Workfront</a>. </p> </td>
   </tr> 
      <tr> 
         <td role="rowheader">Convertido para</td> 
         <td> <p>O nome do objeto de resolução que pode ser uma tarefa ou um projeto para o qual a solicitação foi convertida. </p> <p>Clique no nome da tarefa ou do projeto para abri-los. </p> <p>Se a solicitação não foi convertida, esse campo fica vazio. </p> </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Caminho</td> 
         <td>O nome da fila de solicitações, dos grupos de tópicos e dos tópicos da fila em que a solicitação foi originalmente enviada. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Status</td> 
         <td>O status atual da solicitação ou do objeto de resolução (tarefa ou projeto)</td> 
      </tr> 
      <tr> 
         <td role="rowheader">Data de Entrada</td> 
         <td>A data em que a solicitação foi enviada ou a data em que o objeto de resolução foi criado se a solicitação foi excluída quando convertida. </td> 
      </tr> 
      <tr> 
         <td role="rowheader">Data da última atualização</td> 
         <td> <p>A data em que a solicitação foi atualizada pela última vez.</p> <p>Por padrão, a lista Solicitações enviadas é classificada por esse campo. </p> </td> 
      </tr> 
      </tbody> 
      </table>

1. (Opcional) Clique no cabeçalho de uma coluna para classificar por ela.

   >[!TIP]
   >
   >Ao sair da lista Solicitações enviadas, a opção de classificação selecionada é preservada.

1. (Opcional) Selecione uma solicitação na lista e clique no ícone **do** Abrir Resumo![](assets/open-summary-with-text-nwe.png) para abrir o painel Resumo e exibir informações adicionais sobre a solicitação, adicionar comentários, documentos ou atribuí-la. Para obter informações sobre o painel Resumo, consulte [Visão geral do resumo](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

   >[!TIP]
   >
   >Se o painel Resumo já estiver aberto, o ícone Abrir resumo será alterado para Fechar resumo.

1. (Opcional e condicional) Clique no ícone **X** no canto superior direito ou no ícone **de** Fechar Resumo![](assets/close-summary-with-text-nwe.png) para fechar o Painel de Resumo.

   Se um problema tiver sido convertido em uma tarefa ou projeto e tiver sido excluído no processo de conversão, o Painel de resumo ficará em branco. Para obter informações sobre a conversão de problemas, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. No **ícone de Filtro** ![](assets/filter-nwepng.png), na parte superior direita da lista, selecione qualquer um dos filtros listados na tabela abaixo.

   >[!TIP]
   >
   >Não é possível modificar filtros na seção Enviado da área Solicitações.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Todas</td> 
      <td>Todas as solicitações enviadas, independentemente do status ou de quem as enviou.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abrir</td> 
      <td> <p>Todas as solicitações enviadas que estão abertas no momento, independentemente de quem as enviou. Somente as solicitações que você tiver pelo menos permissões para exibir serão exibidas aqui se você não as tiver enviado. </p> <p>As solicitações sem uma Data de Conclusão Real ou cujo objeto de resolução não tem uma Data de Conclusão Real são listadas na subguia Abrir.</p> <p><b>DICA</b>

   As solicitações que estiverem em qualquer status que não seja igual a Fechado serão consideradas abertas.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Minhas solicitações</td> 
      <td>Solicitações que você enviou independentemente do status. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Minhas solicitações abertas</td> 
      <td> <p>Solicitações enviadas que ainda estão abertas. </p> <p>As solicitações sem uma Data de Conclusão Real ou cujo objeto de resolução não tem uma Data de Conclusão Real são listadas na subguia Minhas Solicitações Abertas. </p> <p><b>DICA</b>

   As solicitações que não estiverem em um status igual a Fechado serão consideradas abertas.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Opcional) Clique no ícone **da** Página de filtro![](assets/search-icon.png) na parte superior da lista para procurar uma solicitação por nome. A lista é atualizada com resultados que correspondem aos seus critérios de pesquisa.

1. (Condicional) Para exibir somente as filas de Solicitações Workfront, pesquise ou filtre por `Issue` tipos de objeto.</span>


   <!--
   <li value="9" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Click the <strong>Complete</strong> subtab to view requests that have been completed.</p> <p>(NOTE: this step will stay drafted even after release. We can't see Completed at this time!) <br>Requests with an Actual Completion Date or whose resolving object has an Actual Completion Date are listed in the Complete subtab.<br>Once a request receives an Actual Completion Date, it stays in the Recently Completed area for 10 business days. After that, it is moved to the Completed area. <br>For information about resolving and resolvable objects, see the article <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overview of Resolving and Resolvable Objects </a>.</p> </li>
   -->

   <!--
   <li value="10" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Optional) Select an option from the <strong>Sort by</strong> drop-down menu to sort the requests by the following criteria:   (NOTE: this step will stay drafted even after release. We can't see Completed at this time!)  
   <ul>
   <li><strong>Assigned To</strong>: Requests are sorted alphabetically by the name of the assignee using the following criteria: 
   <ul>
   <li>All requests assigned to users are sorted first, in the order of the users' names.</li>
   <li>Requests assigned to job roles are sorted secondly, in the order of the job roles' names and are listed after all the requests assigned to users.</li>
   <li>Requests that are assigned to teams are sorted last, in the order of the teams' names and are listed after all the requests assigned to users and those assigned to job roles.</li>
   <li>All unassigned requests are listed last, in the order of their Entry Date. </li>
   </ul></li>
   <li><strong>Submitted On</strong>: Requests are sorted chronologically by the date when they were submitted.</li>
   <li><strong>Recently Updated</strong> (this is the default): Requests are sorted chronologically by the date of their last update.</li>
   <li><strong>Name</strong>: Requests are sorted alphabetically by name. </li>
   <li><strong>Priority</strong>: Requests are sorted in the order of their priority.</li>
   <li><strong>Queue</strong>: Requests are sorted alphabetically by the name of the requests queue where they were submitted. </li>
   <li><strong>Status</strong>: Requests are sorted alphabetically by their status. </li>
   </ul></li>
   -->

1. Clique em **Rascunhos** para exibir todas as solicitações em rascunho. O Workfront salva um número ilimitado de rascunhos para cada fila de solicitações nesta pasta. Ao informar uma nova solicitação para um tópico da fila que já tem um rascunho, você será solicitado a usar um rascunho existente. Para obter mais informações, consulte [Criar solicitações de rascunhos](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).

1. (Opcional e condicional) Se sua organização adquiriu um pacote do Workfront Planning, clique na guia **Planning** e em **Enviado** no painel esquerdo para exibir as solicitações do Workfront Planning.

   Use **Filtros** e **Colunas** para atualizar as informações na lista de solicitações do Planning.

   ![](assets/workfront-planning-tab-submitted-section-in-requests-area.png)

   Para obter informações, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).


1. (Opcional) Verifique o status de uma solicitação verificando a coluna Status. Os seguintes status estão disponíveis na nova experiência de solicitação:

   * Rascunho: Esta solicitação ainda não foi enviada.
   * Em andamento
   * Completo


