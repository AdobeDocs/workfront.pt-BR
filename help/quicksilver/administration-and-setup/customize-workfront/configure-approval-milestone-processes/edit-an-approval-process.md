---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Editar um processo de aprovação
description: Se você for um administrador do Adobe Workfront ou tiver acesso administrativo a processos de aprovação, poderá visualizar e editar todos os processos de aprovação no sistema.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 2%

---

# Editar um processo de aprovação

<!--Audited: 08/2025-->

Se você for um administrador do Adobe Workfront ou tiver acesso administrativo a processos de aprovação, poderá visualizar e editar todos os processos de aprovação no sistema.

Se você for um administrador de grupo, poderá ver e editar os processos de aprovação associados ao grupo ou grupos que gerencia.

Para obter informações sobre como criar processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>* Quando você edita um processo de aprovação global que já está em uso, suas alterações afetam todos os objetos em todo o sistema que já estão associados a ele.
>* Se você adicionar um novo aprovador ao estágio atual em um processo de aprovação que já foi iniciado em um objeto, o processo para esse objeto será redefinido e os aprovadores terão que começar novamente.
>
>  No entanto, se você fizer as seguintes alterações em um processo de aprovação já iniciado em um objeto, esse processo continuará sem interrupção:
>
>* Adicionar um estágio além do estágio atual
>* Adicionar um aprovador adicional antes do estágio atual

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront*</td> 
   <td><p>Para o processo de aprovação de nível de sistema ou de uso único:</p><ul><li><p>Qualquer pacote</p></li></ul>
   <p>Para o processo de aprovação em nível de grupo:</p>
   <ul><li><p>Fluxo de trabalho Prime ou Ultimate</p></li>
   <li><p>Workfront Prime ou Ultimate</p></li></ul>
   </td>

</tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p>
 <p>Plano</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Se você for um administrador do sistema ou tiver acesso administrativo aos processos de Aprovação, poderá criar um processo de aprovação no nível do sistema ou um processo de aprovação no nível do grupo para um grupo específico.</p> 
   <p>Se você for um administrador de grupo e tiver acesso administrativo aos processos de Aprovação, poderá criar processos de aprovação de nível de grupo para grupos gerenciados.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação da Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

I made the above match what we had for Create approval process - seemed more complete; 
For this article, the old access was: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to Approval Processes if you are not a System Administrator</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Editar um processo de aprovação existente

{{step-1-to-setup}}

1. (Condicional) Se você estiver editando um processo de aprovação no nível do sistema, clique em **Processos** > **Aprovações** no painel esquerdo.

   Ou

   Se você estiver editando um processo de aprovação em nível de grupo, faça o seguinte:

   1. No painel esquerdo, clique em **Grupos** ![Ícone Grupos](assets/groups-icon.png).
   1. Clique no nome do grupo para o qual deseja listar ou gerenciar processos de aprovação de grupo.
   1. No painel esquerdo, clique em **Aprovações**. Talvez seja necessário clicar em **Mostrar mais** primeiro.

1. Clique na guia **Aprovações de projetos**, **Aprovações de tarefas** ou **Aprovações de problemas**, dependendo do tipo de processo de aprovação que deseja editar.

1. Selecione o processo de aprovação que deseja editar e clique em **Editar** na parte superior da lista. A caixa Edit approval process é exibida.

   ![Editar processo de aprovação](assets/edit-approval-process-global-area-new.png)

1. Especifique as seguintes informações na caixa que é exibida:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do processo de aprovação</td> 
      <td><p>Digite um nome descritivo para o processo de aprovação. Os usuários veem esse nome ao aplicar o processo de aprovação a um objeto, conforme descrito em <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associar um processo de aprovação novo ou existente ao trabalho</a>.</p>
      <p>Este campo é obrigatório.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição do processo de aprovação. Isso é exibido na seção <b>Aprovações</b> na área <b>Configuração</b> ao lado do nome do processo de aprovação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Está ativo</td> 
      <td> <p>Mantenha essa opção ativada se quiser que outros usuários possam anexar o processo de aprovação a projetos, tarefas e problemas que eles criarem. </p> <p>Essa opção está ativada por padrão.</p> <p>Dica: marcar um processo de aprovação como inativo é útil quando sua organização não precisa mais usá-lo, mas você deseja preservar as informações históricas sobre seu uso.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Este processo de aprovação pode ser usado por </td> 
      <td> <p>Se quiser que o processo de aprovação esteja disponível para projetos, tarefas, problemas e modelos pertencentes apenas a um grupo específico, comece digitando o nome do grupo e, em seguida, selecione o nome quando ele for exibido:</p> 
       <ul> 
        <li>Se você for um administrador do sistema ou tiver acesso administrativo a processos de aprovação, poderá ver qualquer grupo no sistema ao digitar seu nome. <b>Todos os grupos</b> está selecionado por padrão. </li> 
        <li>Se você for um administrador de grupo sem acesso administrativo a processos de aprovação, poderá atribuir o processo de aprovação a qualquer grupo gerenciado ao digitar seu nome. A opção <b>Todos os Grupos</b> não está disponível.</li> 
       </ul> 
       <p>Este campo é obrigatório.</p>
       <p>Esta opção não está disponível para processos de aprovação de uso único.</p> <p><b>AVISO</b>: quando você faz alterações ao processo de aprovação específico do grupo, os processos de aprovação existentes que já foram associados a itens de trabalho podem mudar. Para obter informações sobre essas alterações, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos</a>.</p> <p>Para obter informações sobre como listar e gerenciar os processos de aprovação do seu grupo na página do seu grupo, consulte <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processos de aprovação de nível de grupo</a>. </p> <p>Para obter informações sobre acesso administrativo a processos de aprovação, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Configure um caminho para o processo de aprovação usando as opções a seguir.

   Um caminho é onde você especifica o que precisa acontecer no processo de aprovação. Crie estágios em um caminho para indicar quem precisa fazer o trabalho de aprovação e em que ordem.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Iniciar o processo de aprovação quando o status estiver configurado como</p> </td> 
      <td> <p>Selecione o status que acionará o processo de aprovação em itens de trabalho. Quando alguém atualiza um item de trabalho para esse status, seu processo de aprovação é iniciado. </p> 
      <p>Este campo é obrigatório.</p>
      <p>O mesmo status não pode ser selecionado para vários caminhos de processo de aprovação.</p> <p>Os status disponíveis baseiam-se no que está selecionado na opção <b>Esta aprovação pode ser usada por</b> (explicado na tabela acima):</p> 
      <ul> 
      <li> Se <b>Todos os grupos</b> estiver selecionado, somente os status bloqueados do sistema estarão disponíveis. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Se um grupo específico for selecionado, somente os status disponíveis para esse grupo estarão disponíveis</p> </li> 
      </ul> <p>Para obter informações sobre como o processo de aprovação funciona com status, consulte a seção <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Como os processos de aprovação dependem dos status</a> no artigo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome do estágio</td> 
      <td>(Opcional) Digite um nome que descreva o primeiro estágio do caminho. Se você não especificar um nome de estágio, o nome padrão será <b>Estágio 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprovadores</td> 
      <td> <p>Comece digitando o nome do usuário, da equipe ou da função de trabalho que deseja designar como aprovador para esse estágio e clique no nome quando ele aparecer na lista suspensa. Você pode adicionar somente usuários, funções de trabalho e equipes ativos. </p>

   <p>Este campo é obrigatório.</p>

   <p><b>DICA</b></p>

   <p>Ao adicionar um usuário como aprovador, observe o avatar, a função principal do usuário ou o endereço de email dele para distinguir entre usuários com nomes idênticos. Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.</p>
      <p>Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Conceder acesso aos usuários</a></p>.

   <p><b>Nota</b>

   Adicionar um usuário, equipe ou função como aprovador não lhes dá permissões automaticamente para o objeto associado a essa aprovação. Eles recebem permissões para o objeto quando a etapa de aprovação é acionada. Caso contrário, os objetos devem ser compartilhados com eles antes que possam tomar uma decisão de aprovação. </p>
   <p>Você também pode designar um indivíduo como um aprovador especificando a função do indivíduo. Por exemplo, você pode atribuir um Proprietário do projeto, Patrocinador do projeto, Proprietário do Portfolio, Proprietário do programa ou Gerente como aprovador. Essas opções são exibidas automaticamente quando você começa a digitar.</p> 
      <p><b>IMPORTANTE</b>
      <ul> 
      <li> Quando você atribui uma aprovação ao Patrocinador do Projeto e ninguém é designado como patrocinador de um projeto, a aprovação é reatribuída ao Proprietário do Projeto. Se ninguém for designado como o proprietário do projeto, a aprovação será atribuída ao administrador do Workfront. </li> 
      <li> Quando você atribui uma aprovação a uma função e a opção <b>Aprovador que não precisa estar na equipe do projeto</b> está desabilitada, mas nenhuma função na equipe do projeto corresponde à função na aprovação, a aprovação é reatribuída ao Proprietário do projeto. Para obter informações sobre configurações de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação globais</a>.
      </li> 
      <li>Quando você atribui uma aprovação ao Proprietário do projeto e ninguém é designado como o proprietário de um projeto, a aprovação é reatribuída ao administrador principal do Workfront, conforme indicado na seção Informações do cliente na área Configuração. Para obter informações, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurar informações básicas do sistema</a>.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>Quando você atribui funções de trabalho como aprovadores, todos os usuários associados a essa função de trabalho que também estão na equipe do projeto podem tomar uma decisão sobre a aprovação. </p> 
      <p>Quando você atribui uma equipe como um aprovador, qualquer usuário nessa equipe pode tomar uma decisão sobre a aprovação. </p> 
      <p>Para obter mais informações sobre a equipe de criação, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da Equipe de Criação</a>. Para obter mais informações sobre aprovação de trabalho, consulte <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Aprovando trabalho </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">É necessária somente uma decisão</td> 
      <td>(Exibido somente se você adicionar vários aprovadores ao estágio) Selecione essa opção se qualquer um dos aprovadores no estágio puder aprovar ou rejeitar o item de trabalho durante esse estágio. Essa ação permite que o item de trabalho saia do estágio.  
      <p>Quando essa opção não está selecionada, todos os aprovadores identificados devem aprovar ou rejeitar o estágio (em qualquer ordem) antes que o item saia do estágio. Se qualquer um dos aprovadores rejeitar o estágio, o processo será interrompido e iniciado novamente para que as alterações necessárias possam ser feitas. Em seguida, os aprovadores podem aprovar ou rejeitar o estágio novamente.</p> 
      <p>Quando uma equipe é designada como aprovador, qualquer membro da equipe pode conceder ou rejeitar um estágio.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Adicionar estágio</p> </td> 
      <td>(Opcional) Adicione outro estágio ao caminho, usando as opções explicadas nas três linhas acima. Você pode adicionar quantos estágios forem necessários ao caminho.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Escolha o que acontece quando a aprovação é rejeitada</td> 
      <td> <p>Selecione a ação que deseja realizar se o item de trabalho for rejeitado em qualquer estágio do caminho:</p> 
      <ul> <li><strong>Criar um Problema</strong>: (Disponível somente para processos de aprovação de projetos e tarefas) Um problema é criado no projeto ou tarefa em que o processo de aprovação está em execução. O recurso padrão atribuído na tarefa ou o proprietário do projeto é atribuído ao problema. Por padrão, o nome do problema criado é <strong>Aprovação rejeitada (Nome do Projeto ou da Tarefa)</strong>. Esse é um Problema de rejeição, inserido na tarefa ou no projeto, dependendo do processo de aprovação em que a rejeição aconteceu.</li> 
      <li> <p><strong>Definir Status como</strong>: escolha uma das seguintes opções:</p> 
      <ul> <li><strong>Status Anterior</strong>: o projeto, tarefa ou problema rejeitado reverte para o status anterior ao status que ativa o processo de aprovação.</li> 
      <li> <p><strong>Qualquer outro status na lista</strong>: o objeto rejeitado é movido para o status escolhido, como Em Espera. Você pode escolher um dos status padrão ou um status personalizado adicionado ao sistema do Workfront.</p> <p>Se você selecionar um status associado a um processo de aprovação como status de rejeição para um caminho de aprovação, o objeto rejeitado será movido para o status selecionado e será marcado como "Aprovação pendente".</p>
      <p>Por exemplo, se você selecionar Em espera para o status de rejeição e o status Em espera estiver associado a um processo de aprovação, o objeto rejeitado será colocado no status "Em espera - Aprovação pendente", exigindo a aprovação.</p>    <p>Para um processo de aprovação em todo o sistema, somente os status de todo o sistema estão disponíveis.</p> <p>Para um processo de aprovação específico de grupo, todos os status de grupo estão disponíveis. Isso inclui todos os status personalizados que o administrador do grupo criou especificamente para o grupo, bem como quaisquer status de todo o sistema. </p> <p>Para obter informações sobre como o processo de aprovação funciona com status, consulte a seção <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Como os processos de aprovação dependem dos status</a> no artigo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Clique em **Adicionar caminho** para adicionar outro caminho ao processo de aprovação, referindo-se à lista de opções na etapa anterior.

   O novo caminho deve ser associado a outro status. O caminho dispara quando o item é atualizado para mostrar este status. Você não pode ter dois caminhos para o mesmo status.

1. Clique em **Salvar**.
1. (Opcional) Siga qualquer um destes procedimentos:

   * Associe o processo de aprovação a projetos, tarefas ou problemas específicos em todo o sistema, conforme descrito em [Associe um processo de aprovação novo ou existente a um trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Fora da Workfront, notifique os usuários de que o processo de aprovação está disponível para eles associarem a seus projetos, tarefas ou problemas, conforme descrito em [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Crie outro processo de aprovação que será acionado se esse processo de aprovação for rejeitado e o item receber outro status. Isso oferece uma maneira de vincular processos de aprovação.
