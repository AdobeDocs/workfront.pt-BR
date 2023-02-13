---
title: Copiar e enviar solicitações
description: Copiar e enviar solicitações
author: Alina
draft: Probably
feature: Work Management
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# Copiar e enviar solicitações

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is NWE only - hard code it in classic articles!)</p>
-->

Quando você envia solicitações similares frequentemente, é possível copiar uma solicitação enviada existente. Nesse caso, você pode copiar uma solicitação existente, fazer alterações mínimas nela e ressubmetê-la como uma nova solicitação.

## Requisitos de acesso

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso para adicionar solicitações a uma fila de solicitações</p> <p>Exibir permissões ou permissões superiores na solicitação existente</p> <p>Para obter informações sobre como configurar uma fila de solicitações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve ter uma solicitação que você ou alguém em sua organização enviou anteriormente para poder copiá-la e reenviá-la. Se a solicitação pertencer a outra pessoa, você deverá ter pelo menos acesso a Exibi-la para poder copiá-la e enviá-la como nova.

## Considerações sobre cópia e envio de solicitações como novas

* Você só pode copiar e enviar solicitações enviadas. Não é possível copiar solicitações elaboradas.
* Você pode copiar e enviar solicitações que você enviou originalmente ou solicitações que outras pessoas enviaram e que você tem acesso a, pelo menos, Exibir.
* Você sempre tem acesso para copiar e enviar uma cópia de suas próprias solicitações, a menos que alguém tenha removido suas permissões para elas.
* O acesso a copiar e enviar solicitações originalmente enviadas por outras pessoas pode ser concedido automaticamente para pessoas na mesma empresa quando o criador da fila de solicitações ativar o **Pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações** nas áreas Detalhes da fila ou Editar projeto . Desativar essa configuração permite que somente o solicitante original exiba suas próprias solicitações.

   Para obter mais informações, consulte os seguintes artigos:

   * [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md)

* Você pode atualizar a cópia da solicitação original antes de enviá-la novamente como uma nova solicitação.
* Se as seguintes alterações ocorrerem após o envio da solicitação original, você não poderá mais copiá-la e reenviá-la:

   * A fila de solicitações foi excluída.
   * O tópico da fila foi excluído.

      >[!TIP]
      >
      >Se o tópico da fila for o único na fila de solicitações, você ainda poderá copiar e enviar a solicitação e ela será salva sob a própria fila de solicitações.

   * A fila de solicitações não é mais publicada como uma Fila de solicitações de ajuda. Para obter mais informações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Se a fila de solicitações não tiver um tópico na fila e a solicitação original tiver sido enviada antes de janeiro de 2022.

   * O Status do projeto associado à fila de solicitações não é mais Atual.

* Você pode copiar e enviar uma cópia de uma solicitação convertida se ela tiver sido preservada no processo de conversão. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   >[!TIP]
   >
   >A solicitação copiada não está vinculada a um objeto de resolução.

## Copiar e enviar solicitações

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Solicitações**.
1. (Condicional) Se a seção Enviada não for exibida por padrão, clique em **Enviado** no painel esquerdo.
1. Localize a solicitação que você deseja copiar e enviar como nova e siga um destes procedimentos:

   * Selecione-o e clique no botão **Copiar e enviar como novo** ícone ![](assets/copy-and-submit-as-new-requests-area-nwe.png) no canto superior esquerdo da lista de solicitações enviadas.
   * Clique no botão **Mais** menu ![](assets/more-icon.png) à direita do nome da solicitação, em seguida, clique em **Copiar e enviar como novo**

      Ou

      Clique com o botão direito do mouse na solicitação selecionada e depois clique em **Copiar e enviar como novo**.

      ![](assets/request-selected-more-menu-options-nwe-350x191.png)

      >[!TIP]
      >
      >Quando não tem acesso para criar problemas, você recebe um aviso de que o administrador o restringiu a criar solicitações.

1. (Opcional) Atualize as seguintes informações, se necessário:

   * **Tipo de solicitação**: a fila de solicitações na qual a solicitação copiada é salva. Por padrão, a solicitação copiada é salva na fila de solicitações da solicitação original.
   * **Grupos de tópicos** e **Tópicos da fila**, se estiverem selecionadas. Os nomes ou grupos de tópicos e tópicos da fila são personalizados para o seu ambiente. Por padrão, a solicitação copiada é salva nos grupos de tópicos e nos tópicos da fila da solicitação original.

      >[!TIP]
      >
      >Se o caminho mudar do caminho da solicitação original, então o criador da fila de solicitações modificou a fila.

1. (Opcional) Atualize quaisquer informações da solicitação copiada. Dependendo de quais campos o criador da fila de solicitações ativou no **Campos da nova edição** da seção **Detalhes da fila** na subguia do projeto, é possível encontrar um dos seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Assunto</strong> </td> 
      <td>Exibe o nome da solicitação original. Atualize-o, se necessário. Caso contrário, o Workfront nomeia a solicitação copiada <b>Cópia de &lt;name of="" original="" request=""&gt;</b>. Este é um campo obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td>Exibe a descrição da solicitação original. Atualize-o, se necessário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Exibe o URL da solicitação original. Atualize-o, se necessário.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridade</strong> </td> 
      <td> <p>Especifique a prioridade da sua solicitação. A prioridade deve definir a velocidade com que você acha que essa solicitação deve ser resolvida. As opções padrão são:</p> 
       <ul> 
        <li>Nenhum(a)</li> 
        <li>Baixa</li> 
        <li>Normal</li> 
        <li>Alta</li> 
        <li>Urgente</li> 
       </ul> <p>O administrador do Workfront pode modificar os nomes das prioridades.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Severidade</strong> </td> 
      <td> <p>Especifique a gravidade da sua solicitação. A severidade deve definir o impacto que essa solicitação tem em seu trabalho, caso ele não seja resolvido a tempo. As opções padrão são:</p> 
       <ul> 
        <li>Cosmética</li> 
        <li>Causa Confusão</li> 
        <li>Problema com Solução</li> 
        <li>Problema Sem Solução</li> 
        <li>Erro Fatal</li> 
       </ul> <p>O administrador do Workfront pode modificar os nomes das severidades.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contato Primário</strong> </td> 
      <td>O Contato Principal de uma solicitação é padronizado para você, pois você é a pessoa-ponto para tratar de qualquer pergunta relacionada à solicitação. No entanto, é possível alterar para qualquer outro usuário do Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Atribuições</strong></span> </td> 
      <td> <p>Indique o nome de um usuário ativo, função de trabalho ou equipe ao qual a solicitação deve ser atribuída. </p> <p> Você pode especificar mais de um usuário, função de trabalho ou equipe. </p> <p>Dependendo de como a fila de solicitações foi configurada, você pode atribuir a solicitação somente a um ou dois tipos de recursos, em vez de todos os três. </p> <p>Recomendamos o uso das Regras de roteamento para suas Filas de solicitação para que elas possam ser encaminhadas automaticamente para os recursos apropriados. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Dependendo de como a fila de solicitações foi configurada, você pode atribuir apenas um tipo de recurso à solicitação (por exemplo, usuários). Se uma regra de roteamento também estiver associada à fila de solicitações e ela encaminhar automaticamente a solicitação a um tipo diferente de recurso (por exemplo, uma equipe), sua solicitação será atribuída à entidade que você especificar manualmente ao enviar a solicitação (usuários) e ao recurso especificado na regra de roteamento (a equipe).</p> <p style="font-weight: normal;">Para obter mais informações, consulte os seguintes artigos:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar regras de roteamento</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Horas planejadas</strong> </td> 
      <td> <p>Estime quantas horas levaria para essa solicitação ser concluída.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de início planejado</strong> </td> 
      <td> <p>A data em que o trabalho nessa solicitação deve ser iniciado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de conclusão planejada</strong> </td> 
      <td>A data em que deseja que essa solicitação seja resolvida.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>O status padrão de uma nova solicitação é "Novo". O administrador do Workfront pode ter alterado o nome desse status. Também é possível alterar o status para outro item no menu suspenso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documentos</strong> </td> 
      <td> <p>Adicione documentos a sua solicitação. Os documentos anexados ao pedido original não são transferidos para o pedido copiado.</p> <p><b>DICA</b>

   Dependendo de como a fila de solicitações foi configurada, a seção Documentos pode ser exibida antes ou depois dos campos personalizados.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Opcional) Atualize quaisquer informações nos formulários personalizados anexados, se necessário.

   >[!TIP]
   >
   >* Todos os formulários personalizados anexados à solicitação original e os valores incluídos nos campos personalizados são transferidos para a solicitação copiada. Isso inclui campos que contêm lógica.
   >* Não é possível remover formulários personalizados da solicitação copiada.


1. Clique em **Enviar**.

   A solicitação copiada é enviada como uma nova solicitação na fila de solicitações que você especificou.
