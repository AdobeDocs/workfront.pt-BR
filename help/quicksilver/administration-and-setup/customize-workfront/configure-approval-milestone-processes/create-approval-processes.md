---
title: Criar um Processo de Aprovação para Itens de Trabalho
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Você pode criar um processo de aprovação que os usuários podem anexar a um item de trabalho (projeto, tarefa, problema, modelo ou tarefa de modelo), um documento ou uma prova. Um processo de aprovação garante que os designados atribuídos ao objeto revisem determinadas alterações antes que o objeto avance no sistema.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 1709e285-51a5-49a1-a03a-743a334fbe4d
source-git-commit: a1ead3895afaf8b601a9c53e08d41b1cab51cb48
workflow-type: tm+mt
source-wordcount: '2191'
ht-degree: 1%

---

# Criar um processo de aprovação para itens de trabalho

<!-- Audited: 12/2023 -->

<!--see below the "hidden" content for the redesigned tabs - August 2023-->

Você pode criar um processo de aprovação que os usuários podem anexar a um item de trabalho (projeto, tarefa, problema, modelo ou tarefa de modelo), um documento ou uma prova. Um processo de aprovação garante que os designados atribuídos ao objeto revisem determinadas alterações antes que o objeto avance no sistema.

Este artigo descreve como criar processos de aprovação global em nível de sistema ou de grupo para itens de trabalho (projeto, tarefa, problema, modelo ou tarefa de modelo).

Para obter informações sobre aprovações associadas a documentos ou provas, consulte os seguintes artigos:

* [Solicitar aprovações de documentos](../../../review-and-approve-work/manage-approvals/request-document-approvals.md)
* [Visão geral do fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md)

>[!NOTE]
>
>Os usuários também podem criar processos de aprovação de uso único para um projeto, tarefa, problema, modelo ou tarefa de modelo em que têm permissões de Gerenciamento.
>
>Este artigo usa o termo &quot;processo de aprovação global&quot; para se diferenciar do processo de aprovação de uso único. Um processo de aprovação global pode ser usado repetidamente.
>
>No nível do grupo, um processo de aprovação global é restrito a itens de trabalho e status que pertencem ao grupo.
>
>Para obter informações sobre processos de aprovação de uso único, consulte [Visão geral do processo de aprovação](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md) e [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td><p>Processo de aprovação em nível de sistema ou de uso único: qualquer</p>
   <p>Processo de aprovação em nível de grupo: Prime ou Ultimate</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Padrão </p>
 <p>ou</p> 
<p>Atual: Plano </p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Se você for um administrador do sistema ou tiver acesso administrativo a processos de aprovação, poderá criar um processo de aprovação no nível do sistema ou um processo de aprovação no nível do grupo para um grupo específico.</p> 
   <p>Se você for um administrador de grupo, poderá criar processos de aprovação de nível de grupo para grupos gerenciados.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um processo de aprovação global de nível de sistema ou de grupo para itens de trabalho

{{step-1-to-setup}}

1. (Condicional) Se você estiver criando um processo de aprovação no nível do sistema, clique em **Processos** > **Aprovações** no painel esquerdo.

   Ou

   Se você estiver criando um processo de aprovação em nível de grupo, clique em **Grupos** ![](assets/groups-icon.png), clique no nome do grupo e em **Aprovações**.

   <!--hidden for the new tab redesign - August 2023: 
   ![](assets/approvals-area-in-setup-processes.png)
   -->

1. Escolha a guia **Aprovações de Projetos**, **Aprovações de Tarefas** ou **Aprovações de Problemas**.

1. Clique em **Novo processo de aprovação**.
1. Especifique as seguintes informações na caixa que é exibida:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do processo de aprovação</td> 
      <td><p>Digite um nome descritivo para o processo de aprovação. Os usuários veem esse nome ao aplicar o processo de aprovação a um objeto, conforme descrito em <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref">Associar um processo de aprovação novo ou existente ao trabalho</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td><p>Digite uma descrição do processo de aprovação. Isso é exibido na seção <b>Aprovações</b> na área <b>Configuração</b> ao lado do nome do processo de aprovação.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Está ativo</td> 
      <td> <p>Mantenha essa opção ativada se quiser que outros usuários possam anexar o processo de aprovação a projetos, tarefas e problemas que eles criarem. </p> <p>Essa opção está ativada por padrão.</p> <p> Dica: marcar um processo de aprovação como inativo é útil quando sua organização não precisa mais usá-lo, mas você deseja preservar as informações históricas sobre seu uso.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Este processo de aprovação pode ser usado por </td> 
      <td> <p>Se quiser que o processo de aprovação esteja disponível para projetos, tarefas, problemas e modelos pertencentes apenas a um grupo específico, comece digitando o nome do grupo e, em seguida, selecione o nome quando ele for exibido:</p> 
       <ul> 
       <li>Se você for um administrador do sistema ou tiver acesso administrativo a processos de aprovação, poderá ver qualquer grupo no sistema ao digitar seu nome. <b>Todos os grupos</b> está selecionado por padrão. </li> 
       <li>Se você for um administrador de grupo sem acesso administrativo a processos de aprovação, poderá atribuir o processo de aprovação a qualquer grupo gerenciado ao digitar seu nome. A opção <b>Todos os Grupos</b> não está disponível.</li> 
       </ul> 
       <p>Esta opção não está disponível para processos de aprovação de uso único.</p> 
       <p><b>AVISO</b>: quando você faz alterações ao processo de aprovação específico do grupo, os processos de aprovação existentes que já foram associados a itens de trabalho podem mudar. Para obter informações sobre essas alterações, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos</a>.</p> 
       <p>Para obter informações sobre como listar e gerenciar os processos de aprovação do seu grupo na página do seu grupo, consulte <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref">Processos de aprovação de nível de grupo</a>. </p> 
       <p>Para obter informações sobre acesso administrativo a processos de aprovação, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
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
      <td> <p>Selecione o status que acionará o processo de aprovação em itens de trabalho. Quando alguém atualiza um item de trabalho para esse status, seu processo de aprovação é iniciado. </p> <p>O mesmo status não pode ser selecionado para vários caminhos de processo de aprovação.</p> <p>Os status disponíveis baseiam-se no que está selecionado na opção <b>Esta aprovação pode ser usada por</b> (explicado na tabela acima):</p> 
       <ul> 
       <li> Se <b>Todos os grupos</b> estiver selecionado, somente os status do sistema estarão disponíveis
       <li> <p>Se um grupo específico for selecionado, somente os status disponíveis para esse grupo estarão disponíveis</p> </li> 
       </ul> <p>Para obter informações sobre como o processo de aprovação funciona com status, consulte a seção <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref">Como os processos de aprovação dependem dos status</a> no artigo <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref">Visão geral do processo de aprovação</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome do estágio</td> 
      <td>(Opcional) Digite um nome que descreva o primeiro estágio do caminho. Se você não especificar um nome de estágio, o nome padrão será <b>Estágio 1</b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aprovadores</td> 
      <td> <p>Comece digitando o nome do usuário, da equipe ou da função de trabalho que deseja designar como aprovador para esse estágio e clique no nome quando ele aparecer na lista suspensa. Você pode adicionar somente usuários ativos, <span>funções de trabalho</span> e equipes. </p>

   <p><b>DICA</b>:</p>

   <p>Ao adicionar um usuário como aprovador, observe o avatar, a função principal do usuário ou o endereço de email dele para distinguir entre usuários com nomes idênticos. Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.</p>
      <p>Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md">Conceder acesso aos usuários</a>. </p>

   <p><b>NOTA</b>:

   Adicionar um usuário, equipe ou função como aprovador não lhes dá permissões automaticamente para o objeto associado a essa aprovação. Eles recebem permissões para o objeto quando a etapa de aprovação é acionada. Caso contrário, os objetos devem ser compartilhados com eles antes que possam tomar uma decisão de aprovação. </p> <p>Você também pode designar um indivíduo como um aprovador especificando a função do indivíduo. Por exemplo, você pode atribuir um Proprietário do projeto, Patrocinador do projeto, Proprietário do Portfolio, Proprietário do programa ou Gerente como aprovador. Essas opções são exibidas automaticamente quando você começa a digitar.</p>

   <p><b>IMPORTANTE</b>:  
       <ul> 
       <li> <p>Quando você atribui uma aprovação ao Patrocinador do Projeto e ninguém é designado como patrocinador de um projeto, a aprovação é reatribuída ao Proprietário do Projeto. Se ninguém for designado como o proprietário do projeto, a aprovação será atribuída ao administrador do Workfront. </p> </li> 
      </ul> 
       <ul> 
       <li> <p>Quando você atribui uma aprovação a uma função e o <b>Aprovador que não precisa estar na equipe do projeto (para processos de aprovação que incluem uma função)</b> está desabilitado, mas não há funções na equipe do projeto que correspondam à função na aprovação, a aprovação é reatribuída ao Proprietário do projeto. Para obter informações sobre configurações de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação globais</a>.</p> </li> 
       </ul> 
       <ul> 
       <li> <p>Quando você atribui uma aprovação ao Proprietário do projeto e ninguém é designado como o proprietário de um projeto, a aprovação é reatribuída ao administrador principal do Workfront, conforme indicado na seção Informações do cliente na área Configuração. Para obter informações, consulte <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref">Configurar informações básicas do sistema</a>.  </p> </li> 
       </ul> <p> <img src="assets/approval-create-add-users-nwe-350x304.png" style="width: 350;height: 304;"> </p> </p> <p>Você pode repetir esse processo para adicionar vários aprovadores ao estágio. Um único estágio pode incluir uma combinação de usuários, equipes e funções de trabalho como aprovadores. Não há limite para o número de aprovadores que podem ser adicionados a um estágio.</p> <p><b>IMPORTANTE</b>:  <p>Quando você atribui funções de trabalho como aprovadores, todos os usuários associados a essa função de trabalho que também estão na equipe do projeto podem tomar uma decisão sobre a aprovação. </p> <p>Quando você atribui uma equipe como um aprovador, qualquer usuário nessa equipe pode tomar uma decisão sobre a aprovação. </p> <p>Para obter mais informações sobre a equipe de criação, consulte <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref">Visão geral da Equipe de Criação</a>. Para obter mais informações sobre aprovação de trabalho, consulte <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref">Aprovando trabalho </a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Somente uma decisão é necessária <br> <br> (é exibida somente se você adicionar vários aprovadores ao estágio) </td> 
      <td> <p>Selecione esta opção se qualquer um dos aprovadores no estágio puder aprovar ou rejeitar o item de trabalho durante este estágio. Essa ação permite que o item de trabalho saia do estágio. </p> <p>Quando essa opção não está selecionada, todos os aprovadores identificados devem aprovar ou rejeitar o estágio (em qualquer ordem) antes que o item saia do estágio. Se qualquer um dos aprovadores rejeitar o estágio, o processo será interrompido e iniciado novamente para que as alterações necessárias possam ser feitas. Em seguida, os aprovadores podem aprovar ou rejeitar o estágio novamente.</p> <p>Quando uma equipe é designada como aprovador, qualquer membro da equipe pode conceder ou rejeitar um estágio.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Adicionar estágio</p> </td> 
      <td><p>(Opcional) Adicione outro estágio ao caminho, usando as opções explicadas nas três linhas acima. Você pode adicionar quantos estágios forem necessários ao caminho.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Escolha o que acontece quando a aprovação é rejeitada</p> </td> 
      <td> <p>Selecione a ação que deseja realizar se o item de trabalho for rejeitado em qualquer estágio do caminho:</p> 
       <ul> 
       <li><b>Criar um Problema</b>: (Disponível somente para processos de aprovação de projetos e tarefas) Um problema é criado no projeto ou tarefa em que o processo de aprovação está em execução. O recurso padrão atribuído na tarefa ou o proprietário do projeto é atribuído ao problema. Por padrão, o nome do problema criado é <b>Aprovação rejeitada (&lt;Nome do Projeto ou da Tarefa&gt;)</b>. Esse é um Problema de rejeição, inserido na tarefa ou no projeto, dependendo do processo de aprovação em que a rejeição aconteceu.</li> 
       <li> <p><b>Definir Status como</b>: escolha uma das seguintes opções:</p> 
       <ul> 
       <li><b>Status Anterior</b>: o projeto, tarefa ou problema rejeitado reverte para o status anterior ao status que ativa o processo de aprovação.</li> 
       <li><p><b>Qualquer outro status na lista</b>: o objeto rejeitado é movido para o status escolhido, como Em Espera. Você pode escolher um dos status padrão ou um status personalizado adicionado ao sistema do Workfront.</p>
       <p>Se você selecionar um status associado a um processo de aprovação como status de rejeição, o objeto rejeitado será movido para o status selecionado e será marcado como "Aprovação pendente".</p> 
       <p> Por exemplo, se você selecionar Em espera para o status de rejeição e o status Em espera estiver associado a um processo de aprovação, o objeto rejeitado será colocado no status "Em espera - Aprovação pendente", exigindo a aprovação.</p>

   </tr> 
    </tbody> 
   </table>

1. (Opcional) Clique em **Adicionar caminho** para adicionar outro caminho ao processo de aprovação, referindo-se à lista de opções na etapa anterior.

   O novo caminho deve ser associado a outro status. O caminho dispara quando o item é atualizado para mostrar este status. Você não pode ter dois caminhos para o mesmo status.

1. Clique em **Salvar**.
1. Agora que o processo de aprovação foi criado, continue com qualquer um dos seguintes:

   * Associe o processo de aprovação a projetos, tarefas ou problemas específicos em todo o sistema, conforme descrito em [Associe um processo de aprovação novo ou existente a um trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Fora da Workfront, notifique os usuários de que o processo de aprovação está disponível para eles associarem a seus projetos, tarefas ou problemas, conforme descrito em [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Crie outro processo de aprovação que será acionado se esse processo de aprovação for rejeitado e o item receber outro status. Isso oferece uma maneira de vincular processos de aprovação.

Para obter informações sobre como editar um processo de aprovação, consulte [Editar um processo de aprovação](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

## Associando um processo de aprovação a um item de trabalho

Quando quiser criar um processo de aprovação para um item de trabalho (projeto, tarefa ou problema), você

1. Criar o processo de aprovação primeiro
1. Criar o item de trabalho
1. Associar o processo de aprovação ao item de trabalho

Para obter instruções sobre como associar um processo de aprovação a um item de trabalho, consulte [Associar um processo de aprovação novo ou existente a um trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Qualquer usuário do Workfront com permissões de gerenciamento para um projeto, tarefa ou problema pode criar processos de aprovação de uso único para uso somente no objeto em que foi criado. Para obter mais informações, consulte [Associar um processo de aprovação novo ou existente a um trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Permitir que os usuários modifiquem processos de aprovação global para um único item de trabalho

Por padrão, os usuários que gerenciam permissões em projetos, tarefas e problemas podem criar processos de aprovação de uso único neles. Para obter informações sobre como adicionar processos de aprovação de uso único a projetos, tarefas e problemas, consulte a seção [Associar um processo de aprovação de uso único a um projeto, tarefa, problema, modelo ou tarefa de modelo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#creating-a-single-use-approval-process) no artigo [Associar um processo de aprovação novo ou existente a trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

Os usuários também podem alterar as configurações de um processo de aprovação global associado a um item de trabalho. Essas alterações afetam somente o projeto, tarefa ou problema associado ao processo de aprovação no nível do sistema. Para obter mais informações, consulte a seção [Modificar um processo de aprovação global para uso em um objeto específico](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md#modifying-a-global-approval-process) no artigo [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)).
