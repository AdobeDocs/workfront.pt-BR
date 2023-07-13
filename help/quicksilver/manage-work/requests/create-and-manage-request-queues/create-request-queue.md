---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar uma fila de solicitações
description: Você pode configurar uma Fila de solicitações onde os usuários podem inserir solicitações ocasionais que não são trabalhos planejados em um projeto.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: ddb8f39e3ef400b02b443230f237b6a563d99d5f
workflow-type: tm+mt
source-wordcount: '2571'
ht-degree: 2%

---

# Criar uma fila de solicitações

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

Você pode configurar uma Fila de solicitações onde os usuários podem inserir solicitações ocasionais que não são trabalhos planejados em um projeto. Por exemplo, uma fila de solicitações de Help Desk pode ser configurada para capturar todas as solicitações de usuário que chegam a um departamento de TI.

## Requisitos de acesso

<!--drafted for P&P: replace the table below with this:

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
   <td> 
   <p>Current license: Stadard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator
-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront

## Visão geral das filas de solicitações

Configurar uma fila de solicitações como um projeto. Ao designar o projeto como uma Fila de solicitações, a fila torna-se acessível a partir da área Solicitações do Adobe Workfront. Ao personalizar a Fila de solicitações, você também personaliza o formulário que os usuários preenchem ao enviarem as solicitações.

Este artigo descreve como criar uma fila de solicitações a partir de um projeto existente. No entanto, para criar consistência para o processo de entrada de solicitação ou para adicionar várias camadas a ele para fins de relatório e melhor gerenciamento, também é possível configurar blocos de construção adicionais de uma fila de solicitações, que são descritos na tabela a seguir.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Detalhes da fila</td> 
   <td> <p>Você deve configurar um projeto como uma fila de solicitações na área Detalhes da fila. Esta etapa é obrigatória. </p> <p>Para obter mais informações, consulte <a href="#create-a-request-queue" class="MCXref xref">Criar uma fila de solicitações</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Grupos de Tópicos</td> 
   <td> <p>São menus adicionais que classificam solicitações com base em recursos comuns. Por exemplo, para uma Fila de solicitação de TI, você pode querer ter grupos de tópicos "No local" e "Remoto". </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Criar Grupos de Tópicos</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enfileirar tópicos</td> 
   <td> <p>São menus adicionais que classificam solicitações que pertencem ao mesmo Grupo de tópicos com base em recursos comuns. Um grupo de tópicos pode conter vários tópicos da fila. </p> <p>Por exemplo, o grupo de tópicos "No local" da Fila de solicitação de TI pode conter os tópicos "Hardware", "Software" e "Rede" da fila. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar Tópicos de Fila</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Regras de Encaminhamento</td> 
   <td> <p>Eles permitem encaminhar cada solicitação a um usuário, função de trabalho, equipe ou projeto. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar Regras de Encaminhamento</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar uma fila de solicitações

Ao configurar um projeto como uma Fila de solicitações, o status do projeto deve ser Atual para ser exibido na área Solicitações do Workfront.

Para criar uma Fila de solicitações:

1. Vá para o projeto que você deseja configurar como uma Fila de solicitações.
1. (Opcional) Clique em **Detalhes do projeto** no painel esquerdo e adicione uma **Descrição** ao projeto na **Visão geral** área. Essas informações são exibidas em todas as novas solicitações.
1. Clique em **Detalhes da fila** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, depois **Detalhes da fila**.

   Isso abre a seção Detalhes da fila .

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Especifique as seguintes informações:

   * **Publicar como Fila de solicitação de ajuda:** Selecione esta opção para identificar este projeto como uma fila de solicitações. Todos os problemas recebidos são considerados Solicitações.\
     Quando essa opção não está selecionada, o projeto se comporta como um projeto padrão no Workfront e todos os problemas recebidos são problemas.

   * **Quem pode adicionar solicitações a esta fila:** Selecione quais usuários têm acesso para adicionar solicitações a esta fila. Você pode permitir que os seguintes grupos de pessoas vejam a Fila de solicitações em sua área Solicitações da Barra de navegação global:

     | Quem pode inserir solicitações | Descrição |
     |---|---|
     | Todos | Qualquer usuário do Workfront com uma conta ativa pode visualizar essa fila de solicitações e adicionar solicitações a ela |
     | Pessoas com acesso de visualização a este projeto | Usuários com permissões de Visualização no projeto podem visualizar e adicionar solicitações a esta fila |
     | Pessoas da empresa deste projeto  | Os usuários que pertencem à empresa associada a este projeto podem exibir e adicionar solicitações a esta fila. Se houver uma empresa associada ao projeto, o nome da empresa será listado entre parênteses após essa configuração. |
     | Pessoas do grupo deste projeto  | Os usuários que pertencem ao grupo associado a este projeto podem exibir e adicionar solicitações a esta fila. Se houver um grupo associado ao projeto, o nome do grupo será listado entre parênteses após essa configuração. |

     {style="table-layout:auto"}

   * **Compartilhe com estes links:** As opções a seguir permitem fornecer acesso direto à Fila de solicitações e aos formulários associados a ela a usuários fora do Workfront ou a usuários do Workfront usando uma página externa. Para obter informações sobre como incorporar uma fila de solicitações em um painel como uma página externa, consulte [Incorporar uma fila de solicitações em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Os usuários já devem ter direitos de acesso à Fila de solicitações para obter acesso direto. O uso de qualquer das opções descritas aqui não concede acesso aos usuários automaticamente.

     >[!TIP]
     >
     >Os usuários devem primeiro fazer logon no Workfront antes de obter acesso à fila de solicitações quando acessam a página Fila de solicitações de outro aplicativo.

      * **URL de acesso direto:** Quando um usuário acessa esse URL de um navegador, o usuário é levado diretamente para a seção Nova solicitação na área Solicitações e essa solicitação é selecionada por padrão para ele.

        ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >Você pode exibir uma Fila de solicitações em um painel como uma página externa. Nesse caso, a fila de solicitações é pré-selecionada, mas você pode selecionar qualquer outra fila de solicitações no campo Tipo de solicitação. usuários podem alterar o Tipo de solicitação. Os componentes de navegação das Solicitações também são exibidos.

      * **Código de inserção:** Use esse código HTML para incorporar o formulário de fila de solicitações como um iframe em qualquer página HTML.\
        Se os usuários ainda não estiverem autenticados no Workfront quando visualizarem a página em que o código está incorporado, a caixa de diálogo de logon do Workfront será exibida. Depois que os usuários fazem logon, o formulário Fila de solicitações é exibido.

        >[!NOTE]
        >
        Ao exibir uma Fila de solicitações em um iframe, somente o formulário de solicitação é exibido, o nome da solicitação é pré-selecionado e esmaecido. O usuário não pode alterar o tipo de Solicitação. Os componentes de navegação da área Solicitações não são exibidos.

        Para que o formulário da fila de solicitações seja exibido ao usar esse código incorporado, você deve ativar a configuração &quot;Permitir incorporação do Workfront em um iframe&quot; na configuração do sistema. Para obter mais informações sobre como ativar a incorporação do Workfront em um iframe, consulte [Configurar preferências de segurança do sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Se essa configuração não estiver ativada, o iframe será exibido em branco.

        Você pode ajustar vários aspectos de como o formulário incorporado é exibido, da seguinte maneira:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funcionalidade</strong> </p> </th> 
           <th> <p><strong>Solução</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Ajustar o tamanho do quadro</p> </td> 
           <td> <p>Modifique os atributos "width" e "height".</p> <p>A largura padrão é "500" e a altura é "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direcione usuários para um Tópico de Fila ou Grupo de Tópicos específico</p> </td> 
           <td> <p>Adicione o parâmetro "path" ao URL src. Você pode encontrar o parâmetro de caminho navegando até o Tópico da fila ou Grupo de tópicos desejado no formulário não incorporado e inspecionando o URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Mostrar e permitir que os usuários alterem a lista suspensa pré-configurada Grupo de tópicos</p> </td> 
           <td> <p>Use o parâmetro "path" adicionando o <code>showPreSelectedOptions=true</code> parâmetro para o <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detectar quando o formulário foi enviado</p> </td> 
           <td> <p>Adicione um ouvinte de eventos de "mensagem" à janela da página da Web e verifique se <code>event.data.type</code> é <code>requestSubmitted</code>. <code>event.data.newIssueID</code> será definida como a ID do problema criado.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Tipos de solicitação:** Selecione entre as opções padrão abaixo.

     O administrador do Workfront pode renomear os tipos de solicitação padrão. Para obter mais informações sobre como renomear os tipos de solicitação, consulte [Personalizar tipos de problemas padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Registro de Defeito
      * Pedido de alteração
      * Problema
      * Solicitar

        Este campo é obrigatório e você deve selecionar pelo menos uma opção.

     >[!NOTE]
     >
     Os Tipos de solicitação são exibidos como uma seleção na área Solicitações somente se o Tipo de solicitação for selecionado nas páginas Detalhes da fila e Tópico da fila. Para obter informações sobre como configurar a área Detalhes da fila de um projeto, consulte [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Cada tipo selecionado aqui estará disponível no formulário (você pode selecionar mais de um). Selecionar mais de um tipo pode ajudar a organizar várias solicitações recebidas.\
     Por exemplo, se você estiver usando o formulário em uma fila de solicitações para um projeto de TI, os seguintes tipos de solicitações poderão entrar na fila: hardware, software, correções de erros e problemas.

   * **Duração padrão:** A duração padrão é o tempo normalmente necessário para concluir uma ocorrência. Isso se torna o padrão para todas as questões recebidas e pode ser modificado manualmente. A duração geralmente é definida em horas, dias ou semanas. A duração padrão de um problema é a mesma que o horário planejado para o problema. A Data de conclusão planejada do problema é calculada com base nesse campo.\
     O padrão para a Duração do problema é 1 dia ou 8 horas. Se o administrador do Workfront definir as Horas típicas por dia de trabalho como menos de 8 horas, a Duração padrão para problemas ainda será de 8 horas. Por exemplo, se a opção Horas típicas por dia de trabalho estiver definida como 7 horas, a duração padrão para problemas será de 1,14 dia ou 8 horas. Para obter mais informações sobre como configurar o sistema Horas típicas por dia de trabalho, consulte a seção &quot;Cálculos de linha do tempo&quot; no artigo [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **As pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações.:** Quando selecionada, todas as solicitações enviadas para a fila ficam visíveis para usuários na mesma empresa. Os usuários podem exibir essas solicitações na seção Todas as solicitações, localizada na área Solicitações. Quando essa configuração é ativada ou desativada, isso afeta todas as solicitações futuras; não afeta as informações retroativamente.
   * **Quando alguém fizer uma solicitação, conceder automaticamente:** Quando um usuário faz uma solicitação para a fila de solicitações, o usuário recebe automaticamente o nível de permissão que você escolher para essa solicitação. Selecione entre os seguintes níveis de permissões:

      * **Exibir**
      * **Contribuir**. Esta é a seleção padrão.
      * **Gerenciar**

     Para obter informações sobre o modelo de permissões do Workfront, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Definir as permissões aqui economiza tempo, em vez de precisar conceder permissões para cada solicitação recebida individual. A escolha dessa opção afeta todas as solicitações futuras, mas não afeta retroativamente as solicitações existentes.

   * **Aprovação padrão**: associa um processo de aprovação a esta fila de solicitações. Somente os Processos de aprovação de problemas ficam visíveis nesse menu suspenso. Todos os problemas enviados para essa fila serão associados a esse processo de aprovação. O administrador do Workfront deve definir processos de aprovação no nível do sistema antes que você possa associá-los a filas de solicitações. Os usuários com acesso administrativo aos processos de Aprovação também podem criar processos de aprovação específicos do grupo.

     >[!IMPORTANT]
     >
     Se o grupo do projeto mudar, o processo de aprovação específico do grupo anexado a problemas existentes se tornará um processo de aprovação de uso único. Para obter mais informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte [Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Se você tiver vários tópicos da fila associados a uma fila de solicitações, recomendamos que você associe os processos de aprovação aos tópicos da fila. Para obter mais informações sobre como criar tópicos da fila, consulte [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Considere o seguinte ao adicionar processos de aprovação a filas de solicitações:

      * Somente os processos de aprovação ativos são exibidos na lista.
      * Os processos de aprovação específicos do grupo e de todo o sistema são exibidos na lista. Um processo de aprovação associado a um grupo diferente daquele do projeto não é exibido na lista.

   * **Rota Padrão**: Associe uma Regra de Encaminhamento a esta fila de solicitações. Use as Regras de Encaminhamento para atribuir automaticamente novas ocorrências submetidas a uma Fila de Solicitações ao recurso correto (usuário, função de trabalho ou equipe) e ao projeto correto. Todos os problemas enviados para esta fila serão associados a esta Regra de Encaminhamento. Você deve configurar Regras de Roteamento antes de associá-las à fila de solicitações.\
     Se você tiver vários tópicos da fila associados a uma fila de solicitações, recomendamos que você associe regras de roteamento aos tópicos da fila. Para obter mais informações sobre como criar regras de roteamento, consulte [Criar Regras de Encaminhamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Campos do novo problema:** Na seção Mostrar os seguintes campos selecionados a todos os usuários, selecione os campos que você deseja que fiquem visíveis para todos os usuários que enviam uma solicitação para o projeto ou adicionam um problema ao projeto ou às tarefas.

     >[!TIP]
     >
     Novos campos de problema selecionados na seção Detalhes da fila também são associados a qualquer novo problema adicionado ao projeto ou às tarefas na seção Problemas.

     Quando você habilita qualquer um dos campos Atribuído a, Função de trabalho ou Equipe, eles são sempre renomeados para Atribuições no formulário de solicitação, mas você só pode especificar o tipo de atribuição selecionado aqui.

     >[!NOTE]
     >
     Se você selecionou Atribuído a na área Detalhes da fila, é possível informar somente usuários no campo Atribuições no formulário de solicitação. Nesse caso, não é possível inserir funções de trabalho ou uma equipe.


   * **Documentos**: se você optar por exibir a seção Documentos no novo formulário de solicitação, selecione onde a seção de upload de documento deve ser posicionada. Selecione entre as seguintes opções:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Depois de formulários personalizados</td> 
        <td><span>A seção Documentos é exibida na parte inferior do formulário de solicitação.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Antes dos formulários personalizados</td> 
        <td> <p><span>A seção Documentos é exibida entre os campos do Workfront e os campos personalizados do formulário de solicitação.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Mostrar todos os campos selecionados e não selecionados para:** Selecione quais usuários você deseja ver todos os campos no formulário. As opções a seguir controlam o acesso aos campos no formulário.

     | Quais usuários podem ver todos os campos no formulário de solicitação | Descrição |
     |---|---| 
     | Todos os usuários (planejar licenças) | Todos os usuários que têm uma licença de Plano podem ver os campos selecionados, bem como os campos não selecionados. |
     | Pessoas com direito de acesso de visualização neste projeto (Planejar Licença) | Os usuários com uma licença de Plano que também têm direitos de Exibição para este projeto podem ver os campos selecionados, bem como os campos não selecionados. O restante dos usuários que podem enviar solicitações para esse projeto pode ver apenas os campos selecionados. |
     | Sem usuário | Nenhum usuário pode visualizar os campos não selecionados. Todos os usuários que podem enviar solicitações para este projeto só podem ver os campos selecionados. |

   * **Forms personalizado**: selecione um formulário personalizado para associar à Fila de solicitações. Somente Emitir Forms personalizadas estão disponíveis para seleção nesse menu suspenso. Todos os problemas enviados para a Fila de solicitações terão os formulários selecionados associados a eles.\
     Se você tiver vários Tópicos de fila associados a uma Fila de solicitação, recomendamos que você associe formulários personalizados aos Tópicos de fila. Para obter mais informações sobre como criar subseções para a Fila de solicitações, consulte [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![](assets/custom-forms-on-queue-details.png)

     Se você tiver vários formulários personalizados associados à Fila de solicitações, arraste e solte os formulários para classificá-los na ordem desejada, na **Reordenar Forms** seção.

     >[!TIP]
     >
     Os formulários personalizados adicionados à seção Detalhes da fila também são associados a qualquer novo problema adicionado ao projeto ou às tarefas na seção Problemas.

1. Continue selecionando informações para as configurações no **Configurações da fila de emails** para permitir que os usuários enviem solicitações por email para o projeto da fila de solicitações.

   Para obter mais informações, consulte [Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Clique em **Salvar**.\
   Seu projeto foi configurado para ser uma Fila de solicitações, e os usuários agora podem adicionar solicitações a ela.

1. (Opcional) Para aprimorar a funcionalidade Fila de solicitações, crie subseções adicionais para sua fila, bem como regras para rotear as solicitações recebidas para a equipe, destinatário ou projeto correto.

   * Para obter informações sobre como criar subseções para a Fila de solicitações, consulte os artigos [Criar Tópicos de Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) e [Criar Grupos de Tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * Para obter informações sobre como rotear as solicitações para o responsável, a equipe e o projeto apropriado, consulte [Criar Regras de Encaminhamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
