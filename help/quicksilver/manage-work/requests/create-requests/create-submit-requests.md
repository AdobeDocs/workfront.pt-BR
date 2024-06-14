---
product-area: requests
navigation-topic: create-requests
title: Criar e enviar solicitações do Adobe Workfront
description: O trabalho planejado é representado na Adobe Workfront por projetos e tarefas. No entanto, você pode trabalhar em um ambiente em que o trabalho não planejado, na forma de solicitações aleatórias, pode entrar a qualquer momento. O Workfront fornece um fluxo de trabalho para acomodar esse tipo de ambiente por meio do uso de Filas de solicitações.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 1%

---

# Criar e enviar solicitações do Adobe Workfront

<!--Audited: 12/2023-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE: If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

O trabalho planejado é representado na Adobe Workfront por projetos e tarefas. No entanto, você pode trabalhar em um ambiente em que o trabalho não planejado, na forma de solicitações, pode entrar a qualquer momento. O Workfront fornece um fluxo de trabalho para acomodar esse tipo de ambiente por meio do uso de Filas de solicitações.

Depois de criar uma solicitação em uma Fila de solicitações, você pode atribuí-la para ser concluída ou convertê-la em uma tarefa ou projeto.\
Para obter mais informações sobre como converter problemas em uma tarefa ou projeto, consulte o artigo [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Você pode criar uma solicitação das seguintes maneiras:

* Do zero, conforme descrito neste artigo.
* De rascunhos. Para obter informações, consulte [Criar solicitações a partir de rascunhos](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* De uma solicitação existente, copiando e submetendo uma cópia. Para obter informações, consulte [Copiar e enviar solicitações](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Colaborador ou superior</p>
   Ou
   <p>Atual: solicitação ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a ocorrências</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos para usar as Filas de solicitações

Um administrador do Workfront deve criar Filas de solicitações e disponibilizá-las aos usuários antes que eles possam usar essa funcionalidade. Um usuário com uma licença de Planejador e com acesso para Editar a Projetos e Gerenciar permissões para um projeto específico também pode criar Filas de solicitações.

Para obter informações sobre como criar Filas de solicitações, consulte o artigo [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Um administrador do Workfront deve criar os seguintes componentes de uma Fila de solicitações:

* Um projeto com o status Atual, publicado como uma Fila de solicitação de ajuda.
* Enfileirar tópicos.\
  Para obter mais informações, consulte o artigo [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Regras de Encaminhamento.\
  Para obter mais informações, consulte o artigo [Criar Regras de Encaminhamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Opcional) Grupos de tópicos.\
  Para obter mais informações, consulte o artigo [Criar Grupos de Tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Opcional) Solicitar formulário personalizado.\
  Para obter mais informações, consulte o artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* (Opcional) Solicite o processo de aprovação.\
  Para obter mais informações, consulte o artigo [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Criar solicitações e gerar rascunhos no aplicativo web do Workfront

Ao criar uma solicitação no aplicativo Web do Workfront, o Workfront salva a solicitação como rascunho antes de você enviá-la. O Workfront cria um rascunho assim que você seleciona sua fila de solicitações e começa a inserir informações nela.

Você pode continuar enviando a solicitação ou preencher quantas informações estiverem disponíveis e sair dela para concluí-la posteriormente. O Workfront salva a solicitação em rascunho que você iniciou na pasta Rascunhos.

>[!IMPORTANT]
>
>Considere o seguinte ao trabalhar com rascunhos:
>
>* O Workfront não cria rascunhos de solicitações ao enviá-los por meio de um aplicativo de terceiros, como enviá-los por email para o Workfront ou criá-los usando outro aplicativo. Ao enviar uma solicitação de fora do aplicativo Web Workfront, ela é salva na seção Enviado.
>* Se a estrutura de uma fila de solicitações mudar, você não poderá mais acessar rascunhos existentes. Por exemplo, se um tópico da fila for removido ou um grupo de tópicos for adicionado, os rascunhos salvos não estarão mais acessíveis.
>

Para obter informações sobre como criar solicitações a partir de rascunhos existentes, consulte [Criar solicitações a partir de rascunhos](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). Para obter informações sobre como excluir rascunhos de solicitações, consulte também [Excluir um rascunho de solicitação](../../../manage-work/requests/create-requests/delete-request-draft.md).

Para criar uma solicitação no aplicativo Web do Workfront:

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. Clique em  **Solicitações** e, em seguida, clique em **Nova solicitação** no canto superior direito da página.

   >[!TIP]
   >
   >* Você pode acessar a opção Nova solicitação em qualquer seção na área Solicitações.
   >* A opção Nova solicitação fica esmaecida quando você não tem acesso para criar problemas.

1. (Condicional) Clique dentro da **Tipo de solicitação** e execute um dos procedimentos a seguir:

   * No **Caminhos recentes** , selecione um caminho usado recentemente para abrir uma fila de solicitações. Um caminho inclui a fila de solicitações, os grupos de tópicos e o tópico da fila que você enviou recentemente. Os três últimos caminhos são exibidos por padrão.

     >[!NOTE]
     >
     >O Workfront salva um caminho somente quando você realmente submeteu uma solicitação a ele. Ele não cria caminhos para solicitações em rascunho.

     ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * No **Filas de solicitações** selecione uma fila de solicitações.
   * Insira uma palavra-chave que pertença a um caminho acessado anteriormente para procurar uma fila de solicitações.

     Por exemplo, se você tiver uma fila de solicitações chamada &quot;Help Desk&quot; com um Grupo de tópicos chamado &quot;Local&quot; e um Tópico da fila chamado &quot;Remoto&quot;, poderá digitar &quot;remoto&quot; e todas as filas de solicitações que contêm &quot;remoto&quot; em qualquer elemento de seu caminho serão exibidas.

     >[!TIP]
     >
     >Quando você digita um nome que contém um caractere especial, a fila de solicitações, o tópico da fila ou o grupo de tópicos são exibidos mesmo quando você omite a digitação do caractere.

     ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

     A lista de filas de solicitações e caminhos recentes disponíveis é atualizada dinamicamente para incluir apenas caminhos que contêm a palavra-chave que está destacada nos resultados.

     Os resultados da pesquisa são exibidos nas seguintes áreas:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Filas de solicitações</td> 
        <td>Filas de solicitações que contêm a palavra-chave em seu nome</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Caminhos de solicitação</td> 
        <td> <p>Caminhos (que incluem filas de solicitações, grupos de tópicos, tópicos de fila) que contêm a palavra-chave em qualquer um dos nomes de seus elementos</p> </td> 
       </tr> 
      </tbody> 
     </table>

   >[!TIP]
   >
   >* As primeiras 200 filas de solicitações são exibidas por padrão, em ordem alfabética.
   >* O nome da fila de solicitações é o nome do projeto que foi publicado como uma Fila de solicitações de ajuda.
   >* A descrição do projeto configurado como a fila de solicitações selecionada é exibida à direita do nome da fila de solicitações.
   >   
   >Para obter mais informações sobre como publicar um projeto como uma Fila de solicitação de ajuda, consulte o artigo [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. No **Nova solicitação** formulário, execute um dos procedimentos a seguir:

   * (Condicional) Selecione um rascunho disponível na mensagem de notificação exibida sob o campo Tipo de solicitação.

     Esta área é exibida somente se você tiver salvado rascunhos antes sem enviá-los.

     Os três rascunhos mais recentes de três tópicos diferentes da fila são exibidos por padrão.

     ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Comece a inserir uma nova solicitação na fila selecionada.

     Um novo rascunho é salvo automaticamente na seção Rascunhos depois que você começa a especificar informações para a nova solicitação e dá um nome à solicitação no campo Assunto.

1. (Opcional) Se sua Fila de solicitações incluir Grupos de tópicos, selecione o nome do Grupo de tópicos no primeiro campo suspenso. Caso contrário, selecione um Tópico da Fila.

   >[!TIP]
   >
   >Quando você passa o mouse sobre um Grupo de tópicos ou um Tópico da fila, o campo Descrição é exibido à direita. Contém informações adicionais sobre o grupo de tópicos ou o tópico da fila.
   >
   >
   >![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >
   >

   Você pode ter até 10 camadas de Grupos de tópicos incorporados à sua Fila de solicitações.\
   Para obter mais informações sobre como criar Grupos de Tópicos, consulte o artigo [Criar Grupos de Tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obter mais informações sobre como criar Tópicos da fila, consulte o artigo [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   >
   >Se você tiver selecionado um rascunho ou um caminho anterior, os tópicos de grupos de tópicos e de fila já estarão selecionados. Você pode selecionar um diferente, se necessário.

1. Dependendo dos campos que o administrador do Workfront ativou na variável **Campos do novo problema** seção do **Detalhes da fila** no projeto, você poderá encontrar qualquer um dos seguintes campos ao enviar uma nova solicitação:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Assunto</strong> </td> 
      <td>Especifique um nome para a solicitação. Este campo é obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td>Especifique uma descrição para a solicitação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Especifique um URL que possa estar relacionado à sua solicitação.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridade</strong> </td> 
      <td> <p>Especifique uma prioridade para a solicitação. A prioridade deve definir a velocidade com que você acha que essa solicitação deve ser resolvida. As opções padrão são: </p> 
       <ul> 
        <li>Nenhum(a)</li> 
        <li>Baixa </li> 
        <li>Normal</li> 
        <li>Alta</li> 
        <li>Urgente</li> 
       </ul> <p>O administrador do sistema pode modificar os nomes das prioridades.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Severidade</strong> </td> 
      <td> <p>Especifique uma severidade para a solicitação. A severidade deve definir o impacto que essa solicitação terá no seu trabalho se não for resolvida a tempo. As opções padrão são:</p> 
       <ul> 
        <li>Cosmética</li> 
        <li>Causa Confusão</li> 
        <li>Problema com Solução</li> 
        <li>Problema Sem Solução</li> 
        <li>Erro Fatal</li> 
       </ul> <p>O administrador do sistema pode modificar os nomes das severidades.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Contato Primário</strong> </td> 
      <td>O contato principal de uma solicitação é assumido como padrão por você, já que você é a pessoa certa para responder a qualquer pergunta relacionada à solicitação. No entanto, é possível alterá-lo para qualquer outro usuário do Workfront.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Atribuições</strong> </td> 
      <td> <p><span>Especifique o nome de um usuário ativo, função de trabalho ou equipe à qual a solicitação deve ser atribuída.</span> </p> <p>Você pode especificar apenas um grupo.</p>

   <p> Dependendo de como a fila de solicitações foi configurada, você pode atribuir apenas um ou dois tipos de recursos à solicitação, em vez de todos os três (por exemplo, você só pode atribuir a solicitação aos usuários).</p>

   <p>Se uma regra de roteamento também estiver associada à fila de solicitações e ela rotear automaticamente a solicitação para um tipo diferente de recurso (por exemplo, uma equipe), sua solicitação será atribuída à entidade especificada manualmente ao enviar a solicitação (usuários) e ao recurso especificado na regra de roteamento (a equipe). </p>

   <p> Para obter mais informações, consulte os seguintes artigos:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar Regras de Encaminhamento</a> <br> </p> </li> 
      </ul> </p>

   <p><span>Recomendamos o uso das Regras de roteamento para suas Filas de solicitações, para que elas possam ser roteadas automaticamente para os recursos apropriados.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Horas planejadas</strong> </td> 
      <td> <p>Estime quantas horas levaria para essa solicitação ser concluída.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de Início Planejada</strong> </td> 
      <td> <p>Especifique a data em que o trabalho nesta solicitação deve começar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de Término Planejada</strong> </td> 
      <td>Especifique a data em que deseja que esta solicitação seja resolvida.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>O status padrão de uma nova solicitação é "Novo". O administrador do sistema pode ter alterado o nome deste status. Você também pode alterar o status para algo diferente nesse menu suspenso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documentos</strong> </td> 
      <td> <p>Adicione documentos à sua solicitação. </p> <p> Dependendo de como a fila de solicitações foi configurada, a seção Documentos pode ser exibida antes ou depois dos campos personalizados. </p> <p>Os documentos que você carrega no Workfront são armazenados por 24 horas em uma solicitação em rascunho. Depois disso, você deverá reanexá-los quando retornar para editar e submeter o rascunho. Os documentos vinculados a partir de outras unidades são salvos no rascunho permanentemente. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Se o administrador do Workfront associou um formulário personalizado à Fila de solicitação ou ao Tópico da fila, especifique os campos dentro do formulário personalizado.\
   Os formulários personalizados são diferentes para cada instância do Workfront.
1. (Opcional e condicional) Em qualquer momento durante a inserção da solicitação, clique em [!UICONTROL **Descartar rascunho**] se quiser excluir o rascunho criado automaticamente. Isso exclui o rascunho que não pode ser recuperado. Uma mensagem de confirmação é exibida para confirmar que você está excluindo o rascunho.

1. (Opcional) Clique em [!UICONTROL **Desfazer**] na mensagem de confirmação se quiser reverter a ação e manter o rascunho.

1. Siga um destes procedimentos:

   * Clique em **Enviar** se estiver pronto para enviar a solicitação. A solicitação é salva na seção Enviado . Dependendo da Regra de Encaminhamento da Fila de Solicitações, essa solicitação pode ser encaminhada para um projeto diferente daquele designado como Fila de Solicitações. Para obter informações sobre regras de roteamento, consulte [Criar Regras de Encaminhamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Ou

     Clique em **Fechar** se você não estiver pronto para enviá-lo e puder voltar e concluí-lo mais tarde. Sua solicitação é salva na seção Rascunhos e estará disponível para você na próxima vez que enviar uma solicitação para essa fila de solicitações.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

   Ao enviar a solicitação, o rascunho é excluído automaticamente e não pode ser restaurado.

   Para obter informações sobre como endereçar solicitações recebidas, consulte o artigo [Gerenciar solicitações de trabalho e de equipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   Para obter informações sobre como localizar solicitações enviadas ou rascunhadas, consulte também [Localizar solicitações enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Criar solicitações de fora do Workfront

Você pode compartilhar um link direto para uma fila de solicitações ao enviar uma nova solicitação e incorporá-la a outros aplicativos. Os usuários que acessam este link pela web ou por outros aplicativos também devem estar conectados com uma conta ativa do Workfront para poderem acessar esta fila e enviar solicitações a ela. Para obter informações, consulte [Compartilhar um link para uma fila de solicitações](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Criar solicitações ao enviar por email para o Workfront

Se a Fila de solicitação estiver habilitada para receber solicitações por email, você poderá enviar suas solicitações por email diretamente para o endereço de email associado à Fila de solicitação.

O texto do corpo do email é adicionado como a descrição da solicitação.

>[!NOTE]
>
>A formatação de HTML é removida quando a solicitação entra no Workfront, mas as assinaturas e o conteúdo existente do thread de Responder para não são removidos e aparecem na descrição da solicitação.

Para obter informações sobre como habilitar uma Fila de solicitações para receber solicitações por email, consulte [Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Criar solicitações usando o cliente Outlook

Você pode enviar solicitações usando o cliente Outlook. Você pode criar uma nova solicitação ou converter um email em uma solicitação.

Para obter informações sobre como enviar solicitações usando o cliente Outlook, consulte o artigo [Criar uma solicitação Adobe Workfront a partir de um email do Outlook](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Criar solicitações usando o aplicativo móvel do Workfront

Você pode enviar solicitações usando o aplicativo móvel em seu smartphone. Você pode criar uma nova solicitação e enviá-la às Filas de solicitações que você tem acesso para ver no aplicativo web.

Para obter informações sobre como enviar solicitações por meio do aplicativo móvel, consulte a seção Solicitações nos artigos:

* [Adobe Workfront para Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests)
* [Adobe Workfront para iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md#requests)

## Criar solicitações de outros aplicativos

É possível enviar solicitações usando qualquer aplicativo que tenha sido integrado ao Workfront:

* Você pode criar uma integração personalizada entre o Workfront e outro aplicativo que permite enviar solicitações para o Workfront a partir do outro aplicativo.\
  Para obter mais informações sobre integrações personalizadas do Workfront, consulte o artigo [Integrações do Adobe Workfront](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* Você pode enviar solicitações do Salesforce se tiver instalado o aplicativo Workfront para Salesforce.\
  Para obter informações sobre como enviar solicitações do Salesforce usando nosso aplicativo Workfront para Salesforce, consulte o artigo [Enviar solicitações do Adobe Workfront de objetos do Salesforce](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## Localizar solicitações enviadas

Para obter informações sobre como localizar solicitações enviadas ou rascunhadas, consulte [Localizar solicitações enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
