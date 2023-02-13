---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Editar um processo de aprovação
description: Se você for um administrador da Adobe Workfront ou tiver acesso administrativo aos processos de aprovação, poderá ver e editar todos os processos de aprovação no sistema.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: 4440fc50e988da6e446fd9a3195ae94f978b4b74
workflow-type: tm+mt
source-wordcount: '1927'
ht-degree: 6%

---

# Editar um processo de aprovação

Se você for um administrador da Adobe Workfront ou tiver acesso administrativo aos processos de aprovação, poderá ver e editar todos os processos de aprovação no sistema.

Se você for um administrador de grupo, poderá ver e editar os processos de aprovação associados ao grupo ou grupos que você gerencia.

Para obter informações sobre a criação de processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* Ao editar um processo de aprovação global que já está em uso, suas alterações afetam todos os objetos em todo o sistema que já estão associados a ele.
>* Se você adicionar um novo aprovador ao estágio atual em um processo de aprovação que já tenha sido iniciado em um objeto, o processo para esse objeto será redefinido e os aprovadores terão que começar de novo.
>
>  No entanto, se você fizer as seguintes alterações em um processo de aprovação que já foi iniciado em um objeto, esse processo continuará sem interrupção:
>
>* Adicionar um estágio além do estágio atual
>* Adicionar um aprovador adicional antes do estágio atual


## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo aos Processos de aprovação se você não for um administrador do sistema</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Editar um processo de aprovação existente

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).
1. (Condicional) Se você estiver editando um processo de aprovação em nível de sistema, clique em **Processos** > **Aprovações** no painel esquerdo.

   Ou

   Se você estiver editando um processo de aprovação em nível de grupo, faça o seguinte:

   1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).
   1. Clique no nome do grupo para o qual você deseja listar ou gerenciar os processos de aprovação de grupo.
   1. No painel esquerdo, clique em **Aprovações**. Talvez seja necessário clicar em **Mostrar mais** primeiro.

1. Clique no botão **Aprovações de projeto**, **Aprovações de tarefa** ou **Aprovações de edição** , dependendo do tipo de processo de aprovação que deseja editar.

1. Selecione o processo de aprovação que deseja editar e clique em **Editar** na parte superior da lista. A caixa Edit approval process é exibida.

   ![](assets/edit-approval-process-global-area-new.png)

1. Especifique as seguintes informações na caixa que é exibida:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do processo de aprovação</td> 
      <td>Digite um nome descritivo para o processo de aprovação. Os usuários veem esse nome ao aplicar o processo de aprovação a um objeto, conforme descrito em <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associar um processo de aprovação novo ou existente ao trabalho</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição do processo de aprovação. Isso é exibido na <b>Aprovações</b> na seção <b>Configuração</b> ao lado do nome do processo de aprovação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Está ativo</td> 
      <td> <p>Mantenha essa opção habilitada se quiser que outros usuários possam anexar o processo de aprovação a projetos, tarefas e problemas que criarem. </p> <p>Essa opção é ativada por padrão.</p> <p>Dica: Marcar um processo de aprovação como inativo é útil quando sua organização não precisa mais usá-lo, mas você deseja preservar as informações históricas sobre seu uso.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Este processo de aprovação pode ser usado por </td> 
      <td> <p>Se desejar que o processo de aprovação esteja disponível para projetos, tarefas, problemas e modelos pertencentes a um grupo específico, comece a digitar o nome do grupo e selecione o nome quando ele for exibido:</p> 
       <ul> 
        <li>Se você for um administrador do sistema ou tiver acesso administrativo aos processos de aprovação, poderá ver qualquer grupo no sistema ao digitar o nome. <b>Todos os grupos</b> é selecionada por padrão. </li> 
        <li>Se você for um administrador de grupo sem acesso administrativo aos processos de aprovação, poderá atribuir o processo de aprovação a qualquer grupo que gerencie ao digitar o nome. O <b>Todos os Grupos</b> não está disponível.</li> 
       </ul> <p>Essa opção não está disponível para processos de aprovação de uso único.</p> <p><b>AVISO</b>: Quando você faz alterações no processo de aprovação específico do grupo, os processos de aprovação existentes que já foram associados a itens de trabalho podem ser alterados. Para obter informações sobre essas alterações, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Como as alterações de grupo e processo de aprovação afetam os processos de aprovação atribuídos</a>.</p> <p>Para obter informações sobre como listar e gerenciar os processos de aprovação do seu grupo na página do seu grupo, consulte <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processos de aprovação no nível do grupo</a>. </p> <p>Para obter informações sobre o acesso administrativo aos processos de aprovação, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configure um caminho para o processo de aprovação usando as seguintes opções.

   Um caminho é onde você especifica o que precisa acontecer no processo de aprovação. Crie estágios em um caminho para indicar quem precisa fazer o trabalho de aprovação e em que ordem.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Iniciar o processo de aprovação quando o status estiver configurado como</p> </td> 
      <td> <p>Selecione o status que acionará o processo de aprovação em itens de trabalho. Quando alguém atualiza um item de trabalho para esse status, seu processo de aprovação é iniciado. </p> <p>O mesmo status não pode ser selecionado para vários caminhos do processo de aprovação.</p> <p>Os status disponíveis são baseados no que é selecionado na opção . <b>Essa aprovação pode ser usada por</b> (explicado no quadro acima):</p> 
      <ul> 
      <li> If <b>Todos os grupos</b> for selecionado, somente os status bloqueados do sistema estarão disponíveis. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Se um grupo específico for selecionado, somente os status disponíveis para esse grupo estarão disponíveis</p> </li> 
      </ul> <p>Para obter informações sobre como o processo de aprovação funciona com status, consulte a seção <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Como os processos de aprovação dependem dos status</a> no artigo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome do estágio</td> 
      <td>(Opcional) Digite um nome descrevendo o primeiro estágio do caminho. Se você não especificar um nome de estágio, o nome padrão será <b>Fase 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprovadores</td> 
      <td> <p>Comece digitando o nome do usuário, da equipe ou da função de trabalho que deseja designar como aprovador para esse estágio e clique no nome quando ele for exibido na lista suspensa. Você pode adicionar somente usuários ativos, funções de trabalho e equipes. </p>

   <p><b>DICA</b>:</p>

   <p>Ao adicionar um usuário como aprovador, observe o avatar, a função primária do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os adiciona.</p>

   <p><b>Nota</b>:

   Adicionar um usuário, equipe ou função como aprovador não concede automaticamente permissões ao objeto associado à aprovação. Eles recebem permissões do objeto quando a etapa de aprovação é acionada. Caso contrário, os objetos devem ser compartilhados com eles antes que possam tomar uma decisão de aprovação. </p>
   <p>Também é possível designar um indivíduo como aprovador ao especificar a função dele. Por exemplo, você pode atribuir um Proprietário do projeto, Patrocinador do projeto, Proprietário do Portfolio, Proprietário do programa ou Gerente como aprovador. Essas opções são exibidas automaticamente quando você começa a digitar.</p> 
      <p><b>IMPORTANTE</b>:  
      <ul> 
      <li> Quando você atribui uma aprovação ao Patrocinador do Projeto e ninguém é designado como patrocinador de um projeto, a aprovação é reatribuída ao Proprietário do Projeto. Se ninguém for designado como proprietário do projeto, a aprovação será atribuída ao administrador do Workfront. </li> 
      <li> Ao atribuir uma aprovação a uma função e à opção <b>Aprovador não é necessário estar na equipe do projeto</b> estiver desabilitada, mas nenhuma função na equipe do projeto corresponder à função na aprovação, a aprovação será reatribuída ao Proprietário do projeto. Para obter informações sobre configurações de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>.
      </li> 
      <li>Quando você atribui uma aprovação ao Proprietário do projeto e ninguém é designado como o proprietário de um projeto, a aprovação é reatribuída ao administrador principal do Workfront, conforme indicado na seção Informações do cliente na área Configuração . Para obter mais informações, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurar informações básicas para seu sistema</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>Quando você atribui funções de trabalho como aprovadores, todos os usuários associados a essa função de trabalho que também estão na equipe do projeto podem tomar uma decisão sobre a aprovação. </p> 
      <p>Quando você atribui uma equipe como aprovador, qualquer usuário nessa equipe pode tomar uma decisão sobre a aprovação. </p> 
      <p>Para obter mais informações sobre a equipe do projeto, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da equipe do projeto</a>. Para obter mais informações sobre aprovação de trabalho, consulte <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Aprovar trabalho </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">É necessária somente uma decisão</td> 
      <td>(Exibe apenas se você adicionar vários aprovadores ao palco) Selecione essa opção se qualquer um dos aprovadores do palco puder aprovar ou rejeitar o item de trabalho durante esse estágio. Essa ação permite que o item de trabalho saia do palco.  
      <p>Quando essa opção não está selecionada, todos os aprovadores identificados devem aprovar ou rejeitar o estágio (em qualquer ordem) antes que o item saia do palco. Se qualquer um dos aprovadores rejeitar o palco, o processo será interrompido e reiniciado para que as alterações necessárias possam ser feitas. Em seguida, os aprovadores podem aprovar ou rejeitar o palco novamente.</p> 
      <p>Quando uma equipe é designada como aprovadora, qualquer membro da equipe pode conceder ou rejeitar um estágio.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Adicionar estágio</p> </td> 
      <td>(Opcional) Adicione outro estágio ao caminho, usando as opções explicadas nas três linhas acima. Você pode adicionar quantos estágios forem necessários ao caminho.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Escolha o que acontece quando a aprovação é rejeitada</td> 
      <td> <p>Selecione a ação que deseja tomar se o item de trabalho for rejeitado em qualquer estágio do caminho:</p> 
      <ul> <li><strong>Criar um problema</strong>: (Disponível somente para processos de aprovação de projeto e tarefa) Um problema é criado no projeto ou tarefa em que o processo de aprovação está em execução. O recurso atribuído padrão na tarefa ou o proprietário do projeto é atribuído ao problema. Por padrão, o nome do problema criado é <strong>Aprovação Rejeitada (Nome do Projeto ou da Tarefa)</strong>. Trata-se de um Problema de Rejeição, inserido na tarefa ou no projeto, dependendo do processo de aprovação em que a rejeição ocorreu.</li> 
      <li> <p><strong>Definir Status como</strong>: Escolha uma das opções a seguir:</p> 
      <ul> <li><strong>Status anterior</strong>: O projeto, a tarefa ou o problema rejeitado reverte para o status anterior ao status que ativa o processo de aprovação.</li> 
      <li> <p><strong>Qualquer outro status na lista</strong>: O objeto rejeitado é movido para o status escolhido, como Em Retenção. Você pode escolher um dos status padrão ou um status personalizado adicionado ao sistema do Workfront.</p> <p>Se você selecionar um status associado a um processo de aprovação como status de rejeição para um caminho de aprovação, o objeto rejeitado será movido para o status selecionado e será marcado como “Aprovação pendente”. </p>
      <p>Por exemplo, se você selecionar Em espera para o status de rejeição e o status Em espera estiver associado a um processo de aprovação, o objeto rejeitado será colocado no status “Em espera - Aprovação pendente”, exigindo a aprovação.</p>    <p>Para um processo de aprovação em todo o sistema, somente os status em todo o sistema estão disponíveis.</p> <p>Para um processo de aprovação específico de grupo, todos os status de grupo estão disponíveis. Isso inclui todos os status personalizados criados pelo administrador do grupo especificamente para o grupo, bem como todos os status do sistema. </p> <p>Para obter informações sobre como o processo de aprovação funciona com status, consulte a seção <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Como os processos de aprovação dependem dos status</a> no artigo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Clique em **Adicionar caminho** para adicionar outro caminho ao processo de aprovação, consulte a lista de opções na etapa anterior.

   O novo caminho deve ser associado a outro status. O caminho dispara quando o item é atualizado para mostrar esse status. Não é possível ter dois caminhos para o mesmo status.

1. Clique em **Salvar**.
1. (Opcional) Siga um destes procedimentos:

   * Associe o processo de aprovação a projetos, tarefas ou problemas específicos em seu sistema, conforme descrito em [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Fora da Workfront, notifique os usuários de que o processo de aprovação está disponível para eles associarem-se a seus projetos, tarefas ou problemas, conforme descrito em [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Crie outro processo de aprovação que será acionado se esse processo de aprovação for rejeitado e o item assumir outro status. Isso oferece uma maneira de vincular processos de aprovação.
