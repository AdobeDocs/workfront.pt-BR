---
title: Copiar e enviar solicitações
description: Ao submeter solicitações semelhantes com frequência, você pode copiar uma solicitação submetida existente. Nesse caso, você pode copiar uma solicitação existente, fazer alterações mínimas nela e reenviá-la como uma nova solicitação.
author: Becky
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 59a53f7355032810a05fce2d3f0dfe30d64bbd40
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 2%

---

# Copiar e enviar solicitações


<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Ao submeter solicitações semelhantes com frequência, você pode copiar uma solicitação submetida existente. Nesse caso, você pode copiar uma solicitação existente, fazer alterações mínimas nela e reenviá-la como uma nova solicitação.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Editar acesso a ocorrências</p>  </td> 
  </tr> 
  <tr>
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>Acesso para adicionar solicitações a uma fila de solicitações</p> <p>Exibir permissões ou mais altas na solicitação existente</p> <p>Para obter informações sobre como configurar uma fila de solicitações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a>. </p> </td> 
  </tr>
  <tr> 
   <td role="rowheader"> Produto</td> 
   <td> <ul><li>Adobe Workfront</li><li>Você precisa ter o Adobe Workfront Planning para exibir solicitações ou formulários de solicitação do Planning</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve ter uma solicitação enviada anteriormente por você ou por alguém em sua organização para poder copiá-la e reenviá-la. Se a solicitação pertencer a outra pessoa, você deverá ter pelo menos acesso para Visualizá-la para poder copiá-la e enviá-la como nova.

## Considerações sobre a cópia e o envio de solicitações como novas

* Você só pode copiar e enviar solicitações enviadas. Não é possível copiar solicitações em rascunho.
* Você pode copiar e submeter solicitações que submeteu originalmente ou solicitações que outras pessoas submeteram e que você tem acesso a pelo menos Exibir.
* Você sempre tem acesso para copiar e enviar uma cópia de suas próprias solicitações, a menos que alguém tenha removido suas permissões.
* O acesso para copiar e enviar solicitações originalmente enviadas por outras pessoas pode ser concedido automaticamente a pessoas na mesma empresa quando o criador da fila de solicitações habilitar a **Pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações** nas áreas Detalhes da fila ou Editar projeto. Desativar essa configuração permite que somente o solicitante original visualize suas próprias solicitações.

  Para obter mais informações, consulte os seguintes artigos:

   * [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md)

* Você pode atualizar a cópia da solicitação original antes de reenviá-la como uma nova solicitação.
* Se as seguintes alterações ocorrerem depois que a solicitação original for enviada, você não poderá mais copiá-la e reenviá-la:

   * A fila de solicitações foi excluída.
   * O tópico da fila foi excluído.

     >[!TIP]
     >
     >Se o tópico da fila for o único na fila de solicitações, você ainda poderá copiar e enviar a solicitação e ela será salva na própria fila de solicitações.

   * A fila de solicitações não é mais publicada como uma Fila de solicitações de ajuda. Para obter informações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Se a fila de solicitações não tiver um tópico da fila e a solicitação original tiver sido enviada antes de janeiro de 2022.

   * O status do projeto associado à fila de solicitações não é mais atual.

* Você poderá copiar e enviar uma cópia de uma solicitação convertida se ela tiver sido preservada no processo de conversão. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >A solicitação copiada não está vinculada a um objeto de resolução.

## Copiar e enviar solicitações na experiência herdada de solicitação

{{step1-to-requests}}

1. (Condicional) Se a seção Enviado não for exibida por padrão, clique em **Enviado** no painel esquerdo.

   >[!TIP]
   >
   >   O administrador do Workfront ou de grupo pode personalizar o modelo de layout e remover áreas do menu Principal ou do painel esquerdo do ambiente. Nesse caso, elas podem não estar disponíveis para você.

1. Localize a solicitação que você deseja copiar e submeter como nova e siga um destes procedimentos:

   * Selecione-a e clique em **Copiar** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) no canto superior esquerdo da lista de solicitações enviadas.

   >[!TIP]
   >
   > Se você não tiver selecionado uma solicitação primeiro, o ícone Copiar ficará esmaecido.

   * Clique no menu **Mais** ![](assets/more-icon.png) à direita do nome da solicitação e clique em **Copiar e enviar como novo**

     Ou

     Clique com o botão direito do mouse na solicitação selecionada, em seguida clique em **Copiar e enviar como novo**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Quando você não tem acesso para criar problemas, você recebe um aviso de que o administrador restringiu você de criar solicitações.

1. (Opcional) Atualize as seguintes informações, se necessário:

   * **Tipo de Solicitação**: a fila de solicitações na qual a solicitação copiada é salva. Por padrão, a solicitação copiada é salva na fila de solicitações da solicitação original.
   * **Grupos de Tópicos** e **Tópicos da Fila**, se estiverem selecionados. Os nomes ou grupos de tópicos e tópicos da fila são personalizados para o seu ambiente. Por padrão, a solicitação copiada é salva nos grupos de tópicos e nos tópicos da fila da solicitação original.

     >[!TIP]
     >
     >Se o caminho mudar do caminho da solicitação original, o criador da fila de solicitações modificará a fila.

1. (Opcional) Atualize quaisquer informações da solicitação copiada. Dependendo dos campos que o criador da fila de solicitações habilitou na seção **Novos Campos de Problema** da subguia **Detalhes da Fila** no projeto, você poderá encontrar qualquer um dos seguintes campos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Assunto</strong> </td> 
      <td>Exibe o nome da solicitação original. Atualize-a, se necessário. Caso contrário, o Workfront nomeia a solicitação copiada <b>Cópia de &lt;Nome da solicitação original&gt;</b>. Este campo é obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td>Exibe a descrição da solicitação original. Atualize-a, se necessário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Exibe o URL da solicitação original. Atualize-a, se necessário.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridade</strong> </td> 
      <td> <p>Especifique a prioridade da solicitação. A prioridade deve definir a velocidade com que você acha que essa solicitação deve ser resolvida. As opções padrão são:</p> 
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
      <td> <p>Especifique a severidade da solicitação. A severidade deve definir o impacto que essa solicitação terá no seu trabalho se não for resolvida a tempo. As opções padrão são:</p> 
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
      <td>O contato principal de uma solicitação é assumido como padrão por você, já que você é a pessoa certa para responder a qualquer pergunta relacionada à solicitação. No entanto, é possível alterá-lo para qualquer outro usuário do Workfront.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Atribuições</strong></span> </td> 
      <td> <p>Indique o nome de um usuário, função de trabalho ou equipe ativa à qual a solicitação deve ser atribuída. </p> <p> Você pode especificar mais de um usuário, função de trabalho ou equipe. </p> <p>Dependendo de como a fila de solicitações foi configurada, você pode atribuir a solicitação somente a um ou dois tipos de recursos, em vez de todos os três. </p> <p>Recomendamos o uso das Regras de roteamento para suas Filas de solicitações, para que elas possam ser roteadas automaticamente para os recursos apropriados. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Dependendo de como a fila de solicitações foi configurada, você pode atribuir apenas um tipo de recurso à solicitação (por exemplo, usuários). Se uma regra de roteamento também estiver associada à fila de solicitações e ela rotear automaticamente a solicitação para um tipo diferente de recurso (por exemplo, uma equipe), sua solicitação será atribuída à entidade especificada manualmente ao enviar a solicitação (usuários) e ao recurso especificado na regra de roteamento (a equipe).</p> <p style="font-weight: normal;">Para obter mais informações, consulte os seguintes artigos:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma Fila de Solicitações</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar Regras de Roteamento</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Horas planejadas</strong> </td> 
      <td> <p>Estime quantas horas levaria para essa solicitação ser concluída.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de Início Planejada</strong> </td> 
      <td> <p>A data em que o trabalho nesta solicitação deve começar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de Término Planejada</strong> </td> 
      <td>A data em que você deseja que esta solicitação seja resolvida.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>O status padrão de uma nova solicitação é "Novo". O administrador do Workfront pode ter alterado o nome desse status. Você também pode alterar o status para algo diferente nesse menu suspenso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documentos</strong> </td> 
      <td> <p>Adicione documentos à sua solicitação. Os documentos anexados à solicitação original não são transferidos para a solicitação copiada.</p> <p><b>DICA</b>

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

   A solicitação copiada é submetida como uma nova solicitação na fila de solicitações especificada.

<div class="preview">

## Copiar e enviar solicitações na nova experiência de solicitação

Você pode copiar e enviar solicitações na área Solicitações do Workfront ou a partir do widget Minhas solicitações na Página inicial.

1. Para acessar a lista Solicitações, clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Solicitações]**.

1. Para acessar o widget Minhas solicitações na Página inicial:

   1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Início]**.
   1. Localize o widget Minhas solicitações.

      Para obter mais informações sobre o widget Minhas solicitações, consulte [Usar o widget Minhas solicitações](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Na lista Solicitações ou no widget Minhas solicitações, passe o mouse sobre a solicitação que você deseja copiar.

   Um menu de três pontos Mais é exibido.
   ![](assets/more-menu.png)

1. Clique no menu **Mais** à direita do nome da solicitação e clique em **Copiar**.

   Ou

   Clique com o botão direito do mouse na solicitação selecionada e clique em **Copiar**.

   >[!TIP]
   >
   >Quando você não tem acesso para criar problemas, você recebe um aviso de que o administrador restringiu você de criar solicitações.

1. (Opcional) Atualize quaisquer informações da solicitação copiada. Os campos disponíveis dependem da Fila de solicitações ou do Formulário de solicitações usado para a solicitação.

   <!--When you enter or change any field values in the copied request, it is saved as a draft.-->

1. Clique em **Enviar**.

   A solicitação copiada é enviada como uma nova solicitação.

</div>

