---
product-area: requests
navigation-topic: create-requests
title: Criar e enviar solicitações do Adobe Workfront
description: O trabalho planejado é representado no Adobe Workfront por projetos e tarefas. No entanto, você pode trabalhar em um ambiente em que um trabalho não planejado, na forma de solicitações aleatórias, possa entrar a qualquer momento. O Workfront fornece um fluxo de trabalho para acomodar esse tipo de ambiente por meio do uso de Filas de solicitação.
author: Alina
feature: Work Management
exl-id: 8b023a3d-326d-4d63-9e1e-8171553a9e23
source-git-commit: b40ade1f1d7a9b81c654a274c5e8c872bf74b180
workflow-type: tm+mt
source-wordcount: '2337'
ht-degree: 2%

---

# Criar e enviar solicitações do Adobe Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Linked to the UI - do not change/ remove; THIS IS NOW SPLIT IN THREE ARTICLES>> MAKE SURE THE TRANSITION TO THE OTHER TWO IS CLEAR SINCE THIS IS LINKED TO UI)</p>
<p>(NOTE:&nbsp;If they come out with templates AND drafts, consider splitting this article to keep Create in one and Working with Drafts and Requests in another??)</p>
<p>(NOTE: this article is linked from Submitting Workfront Requests from Salesforce) </p>
</div>
-->

O trabalho planejado é representado no Adobe Workfront por projetos e tarefas. No entanto, você pode trabalhar em um ambiente em que um trabalho não planejado, na forma de solicitações aleatórias, possa entrar a qualquer momento. O Workfront fornece um fluxo de trabalho para acomodar esse tipo de ambiente por meio do uso de Filas de solicitação. 

Após criar uma solicitação em uma Fila de solicitações, é possível atribuí-la para ser concluída ou convertê-la em uma tarefa ou projeto.\
Para obter mais informações sobre conversão de problemas em uma tarefa ou projeto, consulte o artigo [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Você pode criar uma solicitação das seguintes maneiras:

* Do zero, conforme descrito neste artigo.
* De rascunhos. Para obter mais informações, consulte [Criar solicitações de rascunhos](../../../manage-work/requests/create-requests/create-requests-from-drafts.md).
* A partir de uma solicitação existente, copiando e enviando uma cópia. Para obter mais informações, consulte [Copiar e enviar solicitações](../../../manage-work/requests/create-requests/copy-and-submit-requests.md).

## Requisitos de acesso

<!--drafted for P&P - replace table: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos para usar as filas de solicitação

Como administrador do Workfront, você deve criar Filas de solicitação e disponibilizá-las aos usuários antes que eles possam usar essa funcionalidade. Um usuário com uma licença do Planejador e com permissões Editar acesso a Projetos e Gerenciar para um projeto específico também pode criar Filas de solicitação. 

Para obter informações sobre como criar Filas de Solicitações, consulte o artigo [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Você deve criar os seguintes componentes de uma Fila de solicitações:

* Um projeto no status Atual, publicado como uma Fila de solicitações de ajuda.
* Enfileirar tópicos.\
   Para obter mais informações, consulte o artigo [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

* Regras de Encaminhamento.\
   Para obter mais informações, consulte o artigo [Criar regras de roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

* (Opcional) Grupos de tópicos.\
   Para obter mais informações, consulte o artigo [Criar grupos de tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

* (Opcional) Solicite um formulário personalizado.\
   Para obter mais informações, consulte o artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* (Opcional) Solicitar processo de aprovação.\
   Para obter mais informações, consulte o artigo [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Criar solicitações e gerar rascunhos no aplicativo Web do Workfront

Ao criar uma solicitação no aplicativo Web do Workfront, o Workfront salva a solicitação como rascunho antes de enviá-la. O Workfront cria um rascunho assim que você seleciona a fila de solicitações e começa a inserir informações para ele.

Você pode continuar enviando a solicitação ou pode concluir quantas informações tiver disponível e navegar até ela para finalizá-la mais tarde. O Workfront salva a solicitação elaborada que você iniciou na pasta Rascunhos .

>[!IMPORTANT]
>
>Considere o seguinte ao trabalhar com rascunhos:
>
>* O Workfront não cria solicitações de rascunho quando você as envia de um aplicativo de terceiros, como enviá-las por email para o Workfront ou criá-las usando qualquer outro aplicativo. Quando você envia uma solicitação de fora do aplicativo Web Workfront, a solicitação é salva na seção Enviada .
>* Se a estrutura de uma fila de solicitações for alterada, não será mais possível acessar rascunhos existentes. Por exemplo, se um tópico da fila for removido ou um grupo de tópicos for adicionado, os rascunhos salvos não estarão mais acessíveis.
>


Para obter informações sobre como criar solicitações a partir de rascunhos existentes, consulte [Criar solicitações de rascunhos](../../../manage-work/requests/create-requests/create-requests-from-drafts.md). Para obter informações sobre como excluir rascunhos de solicitação, consulte também [Excluir um rascunho de solicitação](../../../manage-work/requests/create-requests/delete-request-draft.md).

Para criar uma solicitação no aplicativo Web do Workfront: 

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   </MadCap:conditionalText>
   -->

1. Clique em  **Solicitações**, depois clique em **Nova solicitação** no canto superior direito da página.

   >[!TIP]
   >
   >* Você pode acessar a opção Nova solicitação em qualquer seção da área Solicitações .
   >* A opção Nova solicitação fica esmaecida quando você não tem acesso para criar problemas.


1. (Condicional) Clique dentro do **Tipo de solicitação** e siga um destes procedimentos:

   * No **Caminhos recentes** selecione um caminho usado recentemente para abrir uma fila de solicitações. Um caminho inclui a fila de solicitações, os grupos de tópicos e o tópico da fila que você enviou recentemente. Os três últimos caminhos são exibidos por padrão.

      >[!NOTE]
      >
      >O Workfront salva um caminho somente quando você realmente enviou uma solicitação a ele. Não cria caminhos para solicitações redigidas.

      ![](assets/list-of-recent-paths-and-request-queues-when-entering-new-request-nwe-350x295.png)

   * No **Solicitar filas** selecione uma fila de solicitações.
   * Insira uma palavra-chave que pertença a um caminho acessado anteriormente para procurar uma fila de solicitações.

      Por exemplo, se você tiver uma fila de solicitações chamada &quot;Help Desk&quot; com um Grupo de tópicos chamado &quot;Localização&quot; e um tópico da fila chamado &quot;Remoto&quot;, poderá digitar &quot;remoto&quot; e todas as filas de solicitações que contêm &quot;remoto&quot; em qualquer elemento de exibição de caminho.

      >[!TIP]
      >
      >Quando você digita um nome que contém um caractere especial, a fila de solicitações, o tópico da fila ou o grupo de tópicos são exibidos mesmo quando você omite digitar o caractere.

      ![](assets/request-queue-search-findings-with-highlighted-results-350x210.png)

      A lista de filas de solicitação disponíveis e caminhos recentes é atualizada dinamicamente para incluir somente caminhos que contêm a palavra-chave realçada nos resultados.

      Os resultados da pesquisa são exibidos nas seguintes áreas:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Filas de solicitações</td> 
        <td>Solicitar filas que contêm a palavra-chave em seu nome</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Caminhos de solicitação</td> 
        <td> <p>Caminhos (que incluem filas de solicitações, grupos de tópicos, tópicos da fila) que contêm a palavra-chave em qualquer um dos nomes de seus elementos</p> </td> 
       </tr> 
      </tbody> 
     </table>
   >[!TIP]
   >
   >* As primeiras 200 filas de solicitações são exibidas por padrão, em ordem alfabética.
   >* O nome da fila de solicitações é o nome do projeto que foi publicado como uma Fila de solicitações de ajuda.
   >* A descrição do projeto configurado como a fila de solicitações selecionada é exibida à direita do nome da fila de solicitações.

   >   
   >Para obter mais informações sobre como publicar um projeto como uma fila de solicitações de ajuda, consulte o artigo [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. No **Nova solicitação** , siga um destes procedimentos:

   * (Condicional) Selecione um rascunho disponível na mensagem de notificação exibida no campo Tipo de solicitação .

      Essa área é exibida somente se você tiver salvo rascunhos antes sem enviá-los.

      Os três rascunhos mais recentes de três tópicos diferentes da fila são exibidos por padrão.

      ![](assets/new-drafts-after-new-request-area-was-removed-350x162.png)

   * Comece a inserir uma nova solicitação na fila selecionada.

      Um novo rascunho salva automaticamente para você na seção Rascunhos depois que você começa a inserir informações para a nova solicitação e dá um nome à solicitação no campo Assunto .

1. (Opcional) Se a Fila de solicitações incluir Grupos de tópicos, selecione o nome do Grupo de tópicos no primeiro campo suspenso. Caso contrário, selecione um Tópico da fila.

   >[!TIP]
   Quando você passa o mouse sobre um Grupo de tópicos ou um Tópico da fila, o campo Descrição é exibido à direita. Ele contém informações adicionais sobre o tópico do grupo ou tópico da fila.
   ![](assets/show-description-on-queue-topic-when-submitting-request-nwe-350x81.png)   >

   Você pode ter até 10 camadas de Grupos de tópicos incorporados à Fila de solicitações.\
   Para obter mais informações sobre como criar Grupos de tópicos, consulte o artigo [Criar grupos de tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obter mais informações sobre como criar tópicos da fila, consulte o artigo [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   >[!TIP]
   Se você selecionou um rascunho ou um caminho anterior, os grupos de tópicos e os tópicos da fila já estão selecionados. Você pode selecionar um diferente, se necessário.

1. Dependendo de quais campos o administrador do Workfront tiver ativado o **Campos da nova edição** da seção **Detalhes da fila** na subguia do projeto, é possível encontrar qualquer um dos seguintes campos ao enviar uma nova solicitação:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Assunto</strong> </td> 
      <td>Especifique um nome para sua solicitação. Este é um campo obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td>Especifique uma descrição para sua solicitação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Especifique um URL que possa estar relacionado a sua solicitação.</p> </td> 
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
      <td> <p>Especifique uma severidade para sua solicitação. A severidade deve definir o impacto que essa solicitação tem em seu trabalho, caso ele não seja resolvido a tempo. As opções padrão são:</p> 
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
      <td>O Contato Principal de uma solicitação é padronizado para você, pois você é a pessoa-ponto para tratar de qualquer pergunta relacionada à solicitação. No entanto, é possível alterar para qualquer outro usuário do Workfront.</td> 
     </tr> 
     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>Atribuições</strong> </td> 
      <td> <p><span>Especifique o nome de um usuário ativo, função de trabalho ou equipe à qual a solicitação deve ser atribuída.</span> </p> <p>Você pode especificar apenas uma equipe.</p>

   <p> Dependendo de como a fila de solicitações foi configurada, você pode atribuir apenas um ou dois tipos de recurso à solicitação, em vez de todos os três (por exemplo, você só pode atribuir a solicitação aos usuários).</p>

   <p>Se uma regra de roteamento também estiver associada à fila de solicitações e ela encaminhar automaticamente a solicitação a um tipo diferente de recurso (por exemplo, uma equipe), sua solicitação será atribuída à entidade que você especificar manualmente ao enviar a solicitação (usuários) e ao recurso especificado na regra de roteamento (a equipe). </p>

   <p> Para obter mais informações, consulte os seguintes artigos:</p> 
      <ul> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma fila de solicitações</a> </p> </li> 
      <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar regras de roteamento</a> <br> </p> </li> 
      </ul> </p>

   <p><span>Recomendamos o uso das Regras de roteamento para suas Filas de solicitação para que elas possam ser encaminhadas automaticamente para os recursos apropriados.</span> </p> </td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>Horas planejadas</strong> </td> 
      <td> <p>Estime quantas horas levaria para essa solicitação ser concluída.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de início planejado</strong> </td> 
      <td> <p>Especifique a data em que o trabalho nesta solicitação deve ser iniciado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Data de conclusão planejada</strong> </td> 
      <td>Especifique a data em que deseja que esta solicitação seja resolvida.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>O status padrão de uma nova solicitação é "Novo". O administrador do sistema pode ter alterado o nome deste status. Também é possível alterar o status para outro item no menu suspenso.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Documentos</strong> </td> 
      <td> <p>Adicione documentos a sua solicitação. </p> <p> Dependendo de como a fila de solicitações foi configurada, a seção Documentos pode ser exibida antes ou depois dos campos personalizados. </p> <p>Os documentos carregados no Workfront são armazenados por 24 horas em uma solicitação redigida. Depois disso, você deverá reanexá-las ao retornar para editar e enviar o rascunho. Os documentos vinculados de outras unidades são salvos no rascunho permanentemente. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Se o administrador do Workfront associou um formulário personalizado à Fila de solicitações ou ao Tópico de fila, especifique os campos dentro do formulário personalizado.\
   Os formulários personalizados são diferentes para cada instância do Workfront. 
1. (Opcional e condicional) Em qualquer ponto durante a inserção da solicitação, clique em [!UICONTROL **Descartar rascunho**] se desejar excluir o rascunho criado automaticamente. Isso exclui o rascunho que não pode ser recuperado. Uma mensagem de confirmação é exibida para confirmar que você está excluindo o rascunho.

1. (Opcional) Clique em [!UICONTROL **Desfazer**] na mensagem de confirmação, caso deseje reverter a ação e manter o rascunho.

1. Siga um destes procedimentos:

   * Clique em **Enviar** se você estiver pronto para enviar a solicitação. A solicitação é salva na seção Enviada . Dependendo da Regra de Roteamento da Fila de Solicitações, essa solicitação pode ser roteada para um projeto diferente daquele designado como Fila de Solicitações. Para obter informações sobre regras de roteamento, consulte [Criar regras de roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

      Ou

      Clique em **Fechar** se você não estiver pronto para enviá-lo, poderá voltar e finalizá-lo mais tarde. Sua solicitação é salva na seção Rascunhos e estará disponível na próxima vez que você enviar uma solicitação para essa fila de solicitações.

      ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)
   Quando você envia a solicitação, o rascunho é automaticamente excluído e não pode ser restaurado.

   Para obter informações sobre como abordar solicitações recebidas, consulte o artigo [Gerenciar solicitações de trabalho e de equipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

   Para obter informações sobre como localizar solicitações enviadas ou redigidas, consulte também [Localizar solicitações enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).

## Criar solicitações de fora do Workfront

É possível compartilhar um link direto para uma fila de solicitações ao enviar uma nova solicitação e incorporá-la a outros aplicativos. Os usuários que acessam esse link da Web ou de outros aplicativos também devem estar conectados com uma conta ativa do Workfront para poder acessar essa fila e enviar solicitações a ela. Para obter mais informações, consulte [Compartilhar um link para uma fila de solicitações](../../../manage-work/requests/create-requests/share-link-to-request-queue.md).

## Criar solicitações ao enviar um email para o Workfront

Se a Fila de solicitações estiver habilitada para receber solicitações por email, você poderá enviar suas solicitações por email diretamente para o email associado à Fila de solicitações.

O texto do corpo do email é adicionado como a descrição da solicitação.

>[!NOTE]
A formatação de HTML é removida quando a solicitação entra no Workfront, mas as assinaturas e o conteúdo existente do thread de Responder para não são removidos e aparecem na descrição da solicitação.

Para obter informações sobre como habilitar uma Fila de solicitações para receber solicitações por email, consulte [Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Criar solicitações usando o cliente do Outlook

Você pode enviar solicitações usando o cliente do Outlook. Você pode criar uma nova solicitação ou converter um email em uma solicitação. 

Para obter informações sobre como enviar solicitações usando o cliente Outlook, consulte o artigo [Criar uma solicitação do Adobe Workfront a partir de um email do Outlook](../../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).

## Criar solicitações usando o aplicativo móvel do Workfront

Você pode enviar solicitações usando o aplicativo móvel em seu smartphone. Você pode criar uma nova solicitação e enviá-la às Filas de solicitação que você tem acesso para ver no aplicativo Web. 

Para obter informações sobre como enviar solicitações por meio do aplicativo móvel, consulte o [Solicitações](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md#requests) nos artigos:

* [Adobe Workfront para Android](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)
* [Adobe Workfront para iOS](../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)

## Criar solicitações de outros aplicativos

Você pode enviar solicitações usando qualquer aplicativo que tenha sido integrado ao Workfront: 

* Você pode criar uma integração personalizada entre o Workfront e outro aplicativo que permite enviar solicitações ao Workfront a partir de outro aplicativo.\
   Para obter mais informações sobre integrações personalizadas do Workfront, consulte o artigo [Integrações do Adobe Workfront](../../../administration-and-setup/configure-integrations/workfront-integrations-1.md).

* Você pode enviar solicitações do Salesforce se tiver instalado o aplicativo Workfront para Salesforce.\
   Para obter informações sobre como enviar solicitações do Salesforce usando nosso aplicativo Workfront para Salesforce, consulte o artigo [Enviar solicitações do Adobe Workfront de objetos do Salesforce](../../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

## Localizar solicitações enviadas

Para obter informações sobre como localizar solicitações enviadas ou redigidas, consulte [Localizar solicitações enviadas](../../../manage-work/requests/create-requests/locate-submitted-requests.md).
