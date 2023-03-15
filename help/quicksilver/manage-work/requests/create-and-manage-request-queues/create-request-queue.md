---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar uma fila de solicitações
description: Você pode configurar uma Fila de solicitações em que os usuários possam inserir solicitações ocasionais que não sejam planejadas para trabalhar em um projeto.
author: Alina
feature: Work Management
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: e83d4742106bc3cb5adb939040997959315dd1e2
workflow-type: tm+mt
source-wordcount: '2545'
ht-degree: 2%

---

# Criar uma fila de solicitações

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

Você pode configurar uma Fila de solicitações em que os usuários possam inserir solicitações ocasionais que não sejam planejadas para trabalhar em um projeto. Por exemplo, uma fila de solicitações de suporte técnico pode ser configurada para capturar todas as solicitações de usuários enviadas a um departamento de TI.

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront

## Visão geral das filas de solicitação

Você configura uma fila de solicitações como um projeto. Quando você designa o projeto como uma Fila de solicitações, a fila fica acessível a partir da área Solicitações do Adobe Workfront. Ao personalizar a Fila de solicitações, você também está personalizando o formulário que os usuários preenchem ao enviarem as solicitações.

Este artigo descreve como criar uma fila de solicitações a partir de um projeto existente. No entanto, para criar consistência para o processo de entrada de solicitação ou para adicionar várias camadas a ele para fins de relatório e melhor gerenciamento, também é possível configurar blocos de construção adicionais de uma fila de solicitações, descritos na tabela a seguir.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Detalhes da fila</td> 
   <td> <p>Você deve configurar um projeto como uma fila de solicitações na área Detalhes da fila. Esta etapa é obrigatória. </p> <p>Para obter mais informações, consulte o <a href="#create-a-request-queue" class="MCXref xref">Criar uma fila de solicitações</a> neste artigo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Grupos de Tópicos</td> 
   <td> <p>São menus adicionais que classificam solicitações com base em recursos comuns. Por exemplo, para uma fila de solicitações de TI, você pode querer grupos de tópicos "No site" e "Remoto". </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Criar grupos de tópicos</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enfileirar tópicos</td> 
   <td> <p>São menus adicionais que classificam solicitações que pertencem ao mesmo Grupo de tópicos com base em recursos comuns. Um grupo de tópicos pode conter vários tópicos da fila. </p> <p>Por exemplo, o grupo de tópicos "No site" para a fila de solicitações de TI pode conter os tópicos da fila "Hardware", "Software" e "Rede". </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Criar Tópicos da Fila</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Regras de Encaminhamento</td> 
   <td> <p>Eles permitem rotear cada solicitação para um usuário, função de trabalho, equipe ou para um projeto. </p> <p>Para obter mais informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Criar regras de roteamento</a>. </p> <p>Isso é opcional.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar uma fila de solicitações

Quando você configura um projeto como uma Fila de solicitações, o status do projeto deve ser Atual para ser exibido na área Solicitações do Workfront.

Para criar uma Fila de solicitações:

1. Vá para o projeto que deseja configurar como uma Fila de solicitações.
1. (Opcional) Clique em **Detalhes do projeto** no painel esquerdo e adicione um **Descrição** para o projeto no **Visão geral** área. Essas informações são exibidas em todas as novas solicitações.
1. Clique em **Detalhes da fila** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, em seguida **Detalhes da fila**.

   Isso abre a seção Detalhes da fila .

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. Especifique as seguintes informações:

   * **Publicar como fila de solicitações de ajuda:** Selecione essa opção para identificar esse projeto como uma fila de solicitações. Todos os problemas recebidos são considerados Solicitações.\
      Quando essa opção não está selecionada, o projeto se comporta como um projeto padrão no Workfront e todos os problemas recebidos são problemas.

   * **Quem pode adicionar solicitações a esta fila:** Selecione quais usuários têm acesso para adicionar solicitações a esta fila. Você pode permitir que os seguintes grupos de pessoas vejam a Fila de Solicitações em sua área de Solicitações da Barra de Navegação Global:

      | Todos | Qualquer usuário do Workfront com uma conta ativa pode visualizar essa fila de solicitações e adicionar solicitações a ela |
      |---|---|
      | Pessoas com acesso de visualização a este projeto | Os usuários com permissões de Exibição do projeto podem exibir e adicionar solicitações a esta fila |
      | Pessoas da empresa deste projeto  | Os usuários que pertencem à empresa associada a este projeto podem visualizar e adicionar solicitações a esta fila. Se houver uma empresa associada ao projeto, o nome da empresa será listado entre parênteses após essa configuração. |
      | Pessoas do grupo deste projeto  | Os usuários que pertencem ao grupo associado a este projeto podem visualizar e adicionar solicitações a esta fila. Se houver um grupo associado ao projeto, o nome do grupo será listado entre parênteses após essa configuração. |

      {style="table-layout:auto"}

   * **Compartilhe com estes links:** As opções a seguir permitem fornecer acesso direto à Fila de solicitações e aos formulários associados a ela a usuários fora do Workfront ou a usuários do Workfront usando uma página externa. Para obter informações sobre como incorporar uma fila de solicitações em um painel como uma página externa, consulte [Incorporar uma fila de solicitações em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

      Os usuários já devem ter direitos de acesso à Fila de solicitações para obter acesso direto. Usar qualquer uma das opções descritas aqui não concede acesso automático aos usuários.

      >[!TIP]
      >
      >Os usuários devem primeiro fazer logon no Workfront antes de obter acesso à fila de solicitações quando acessarem a página Fila de solicitações de outro aplicativo.

      * **URL de acesso direto:** Quando um usuário acessa esse URL a partir de um navegador, o usuário é levado diretamente para a seção Nova solicitação na área Solicitações e essa solicitação é selecionada por padrão para eles.

         ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

         >[!NOTE]
         >
         >Você pode exibir uma Fila de solicitações em um painel como uma página externa. Nesse caso, a fila de solicitações é pré-selecionada, mas você pode selecionar qualquer outra fila de solicitações no campo Tipo de solicitação . Os usuários do podem alterar o Tipo de solicitação. Os componentes de navegação das Solicitações também são exibidos.

      * **Código incorporado:** Use esse código de HTML para incorporar o formulário de fila de solicitações como um iframe em qualquer página de HTML.\
         Se os usuários ainda não estiverem autenticados no Workfront quando visualizarem a página onde o código está incorporado, a caixa de diálogo de logon do Workfront será exibida. Depois que os usuários fizerem logon, o formulário Fila de solicitações será exibido.

         ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

         >[!NOTE]
         Ao exibir uma Fila de solicitações em um iframe, somente o formulário de solicitação é exibido, o nome da solicitação é pré-selecionado e esmaecido. O usuário não pode alterar o tipo de Solicitação. Os componentes de navegação da área Solicitações não são exibidos.

         Para que o formulário da fila de solicitações seja exibido ao usar esse código incorporado, você deve ativar a configuração &quot;Permitir incorporação do Workfront em um iframe&quot; na configuração do sistema. Para obter mais informações sobre como habilitar a incorporação do Workfront em um iframe, consulte [Configurar preferências de segurança do sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Se essa configuração não estiver ativada, o iframe será exibido como em branco.

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
           <td> <p>Ajuste o tamanho do quadro</p> </td> 
           <td> <p>Modifique os atributos "largura" e "altura".</p> <p>Por padrão, a largura é "500" e a altura é "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direcionar usuários para um tópico da fila ou grupo de tópicos específico</p> </td> 
           <td> <p>Adicione o parâmetro "path" ao URL src. Você pode encontrar o parâmetro de caminho navegando até o Tópico da fila ou Grupo de tópicos desejado no formulário não incorporado e inspecionando o URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Mostrar e permitir que os usuários alterem a lista suspensa Grupo de Tópicos pré-configurado</p> </td> 
           <td> <p>Use o parâmetro "path" ao adicionar a variável <code>showPreSelectedOptions=true</code> para <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detectar quando o formulário foi enviado</p> </td> 
           <td> <p>Adicione um ouvinte de evento "message" à janela da página da Web e verifique se <code>event.data.type</code> é <code>requestSubmitted</code>. <code>event.data.newIssueID</code> será definida como a ID do problema criado.</p> </td> 
          </tr> 
         </tbody> 
        </table>
   * **Tipos de solicitação:** Selecione dentre as opções padrão abaixo.

      O administrador do Workfront pode renomear os tipos de solicitação padrão. Para obter mais informações sobre como renomear os tipos de solicitação, consulte [Personalizar tipos de problemas padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Alterar ordem
      * Problema
      * Solicitações
      * Risco

         Este é um campo obrigatório e você deve selecionar pelo menos uma opção.
      >[!NOTE]
      Os Tipos de Solicitação são exibidos como uma seleção na área Solicitações somente se o Tipo de Solicitação estiver selecionado nas páginas Detalhes da Fila e Tópico da Fila. Para obter informações sobre como configurar a área Detalhes da fila de um projeto, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Cada tipo selecionado aqui estará disponível no formulário (você pode selecionar mais de um). Selecionar mais de um tipo pode ajudar a organizar várias solicitações.\
      Por exemplo, se você estiver usando o formulário em uma fila de solicitações para um projeto de TI, os seguintes tipos de solicitação podem entrar na fila: hardware, software, correções de erros e problemas.

   * **Duração padrão:** A duração padrão é o tempo necessário para concluir um problema. Isso se torna o padrão para todos os problemas recebidos e pode ser modificado manualmente. A duração é geralmente definida em horas, dias ou semanas. A Duração padrão de um problema é a mesma que as Horas planejadas do problema. A Data de conclusão planejada do problema é calculada com base nesse campo.\
      O padrão para a Duração do problema é 1 dia ou 8 horas. Se o administrador do Workfront definir as Horas típicas por dia de trabalho como menos de 8 horas, a Duração padrão para problemas ainda será de 8 horas. Por exemplo, se as Horas típicas por dia de trabalho forem definidas como 7 horas, a Duração padrão para problemas será de 1,14 dia ou 8 horas. Para obter mais informações sobre como configurar o sistema Horas típicas por dia de trabalho, consulte a seção &quot;Cálculos de linha do tempo&quot; no artigo [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **As pessoas da mesma empresa herdarão as mesmas permissões para todas as solicitações.:** Quando selecionadas, todas as solicitações enviadas para a fila do ficam visíveis para usuários na mesma empresa. Os usuários podem exibir essas solicitações na seção Todas as solicitações , localizada na área Solicitações . No momento em que essa configuração é ativada ou desativada, isso afeta todas as solicitações futuras; não tem impacto retroativo nas informações.
   * **Quando alguém faz uma solicitação, concede automaticamente:** Quando um usuário faz uma solicitação na fila de solicitações, o usuário recebe automaticamente o nível de permissão que você escolher para essa solicitação. Selecione entre os seguintes níveis de permissões:\
      **- Exibir**

      **- Contribuir**
      **- Gerenciar**

      Para obter informações sobre o modelo de permissões do Workfront, consulte [Visão geral do compartilhamento de permissões em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
      Definir permissões aqui economiza tempo, em vez de precisar conceder permissões para cada solicitação de entrada individual. A escolha dessa opção afeta todas as solicitações futuras, mas não afeta as solicitações existentes retroativamente.

   * **Aprovação padrão**: Associe um processo de aprovação a esta fila de solicitações. Somente Processos de aprovação de problemas estão visíveis neste menu suspenso. Todos os problemas enviados para esta fila serão associados a este processo de aprovação. O administrador do Workfront deve definir processos de aprovação no nível do sistema antes de associá-los às filas de solicitação. Os usuários com acesso administrativo a processos de aprovação também podem criar processos de aprovação específicos do grupo.

      >[!IMPORTANT]
      Se o grupo do projeto mudar, o processo de aprovação específico do grupo anexado às questões existentes se tornará um processo de aprovação de uso único. Para obter mais informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte [Como as alterações de grupo e processo de aprovação afetam os processos de aprovação atribuídos](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

      Se você tiver vários tópicos de fila associados a uma fila de solicitações, recomendamos que associe processos de aprovação aos tópicos da fila. Para obter mais informações sobre como criar tópicos de fila, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Considere o seguinte ao adicionar processos de aprovação a filas de solicitação:

      * Somente os processos de aprovação ativos são exibidos na lista.
      * Os processos de aprovação em todo o sistema e específicos do grupo são exibidos na lista. Um processo de aprovação associado a um grupo diferente do do projeto não é exibido na lista.
   * **Rota padrão**: Associe uma Regra de Roteamento a esta fila de solicitações. Use Regras de Roteamento para atribuir automaticamente novos problemas enviados a uma Fila de Solicitações ao recurso correto (usuário, função de trabalho ou equipe) e ao projeto correto. Todos os problemas enviados para esta fila serão associados a esta Regra de Roteamento. Você deve configurar Regras de roteamento antes de associá-las à fila de solicitações.\
      Se você tiver vários tópicos de fila associados a uma fila de solicitações, recomendamos que associe as regras de roteamento aos tópicos da fila. Para obter mais informações sobre como criar regras de roteamento, consulte [Criar regras de roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Campos da nova edição:** Na seção Mostrar os seguintes campos selecionados para todos os usuários , selecione quaisquer campos que deseja que fiquem visíveis para todos os usuários que enviam uma solicitação para o projeto ou adicionam um problema ao projeto ou às tarefas.

      >[!TIP]
      Os novos campos de ocorrência selecionados na seção Detalhes da fila também são associados a qualquer novo problema adicionado ao projeto ou às tarefas na seção Problemas .

      Quando você ativa qualquer um dos campos Atribuído a, Função de Trabalho ou Equipe, eles são sempre renomeados para Atribuições no formulário de solicitação, mas você só pode especificar o tipo de atribuição selecionado aqui.

      **Exemplo:** Se tiver selecionado Atribuído a na área Detalhes da fila, você poderá inserir somente usuários no campo Atribuições no formulário de solicitação. Nesse caso, não é possível inserir funções de cargo ou uma equipe.

   * **Documentos**: Se você optar por exibir a seção Documentos no novo formulário de solicitação, selecione onde a seção de upload de documento deve ser posicionada. Selecione uma das opções a seguir:

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
        <td> <p><span>A seção Documents é exibida entre os campos Workfront e os campos personalizados do formulário de solicitação.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

      ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Mostrar todos os campos selecionados e não selecionados para:** Selecione quais usuários deseja visualizar todos os campos do formulário. As opções a seguir controlam o acesso aos campos no formulário.

      | Todos os Usuários (Licenças do Plano) | Todos os usuários que têm uma licença de Plano podem ver os campos selecionados e não selecionados. |
      |---|---|
      | Pessoas com direito de acesso de visualização neste projeto (Planejar Licença) | Os usuários com uma licença do Plano que também têm direitos de Exibição para este projeto podem ver os campos selecionados, bem como os campos não selecionados. O restante dos usuários que podem enviar solicitações para este projeto podem ver apenas os campos selecionados. |
      | Sem usuário | Nenhum usuário pode ver os campos não selecionados. Todos os usuários que podem enviar solicitações para este projeto só podem ver os campos selecionados. |

      {style="table-layout:auto"}

   * **Forms personalizada**: Selecione um formulário personalizado para associar à Fila de solicitações. Somente Emitir Forms Personalizado estão disponíveis para seleção no menu suspenso. Todos os problemas enviados para a Fila de solicitações terão os formulários selecionados associados a eles.\
      Se você tiver vários Tópicos da fila associados a uma Fila de solicitação, recomendamos que associe formulários personalizados aos Tópicos da fila. Para obter mais informações sobre como criar subseções para a Fila de solicitações, consulte [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

      Se você tiver vários formulários personalizados associados à Fila de solicitações, arraste e solte os formulários para classificá-los na ordem desejada, na **Reordenar o Forms** seção.

      >[!TIP]
      Os formulários personalizados adicionados à seção Detalhes da fila também são associados a qualquer novo problema adicionado ao projeto ou às tarefas na seção Problemas .

   * **Permitir que Problemas sejam adicionados por email:** Selecione essa opção para permitir que as solicitações sejam enviadas por email.\
      Para obter mais informações, consulte [Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).




1. Clique em **Salvar**.\
   Seu projeto foi configurado para ser uma Fila de solicitações e os usuários agora podem adicionar solicitações a ele.

1. (Opcional) Para aprimorar a funcionalidade Fila de solicitações , crie subseções adicionais para sua fila, bem como regras para rotear as solicitações recebidas para a equipe, o destinatário ou o projeto correto.

   Para obter informações sobre como criar subseções para a Fila de solicitações, consulte os artigos [Criar Tópicos da Fila](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) e [Criar grupos de tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).\
   Para obter informações sobre como rotear as solicitações para o destinatário, a equipe e o projeto apropriado, consulte [Criar regras de roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
