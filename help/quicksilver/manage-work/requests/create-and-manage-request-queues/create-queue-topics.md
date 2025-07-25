---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Criar Tópicos de Fila
description: Tópicos de fila trabalham em conjunto com Regras de roteamento para atribuir automaticamente o trabalho recebido a um usuário, função de trabalho, equipe ou para colocá-lo em um projeto. Os Tópicos de Fila definem as condições que precisam existir para que a Regra de Encaminhamento seja implementada.
author: Alina
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 3563d5e7136d8bd70504a0b7762c4be06e5a9c56
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 2%

---

# Criar Tópicos de Fila

<!-- Audited: 12/2023 -->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Tópicos de fila trabalham em conjunto com Regras de roteamento para atribuir automaticamente o trabalho recebido a um usuário, função de trabalho, equipe ou para colocá-lo em um projeto. Os Tópicos de Fila definem as condições que precisam existir para que a Regra de Encaminhamento seja implementada.

Não há limite para o número de Tópicos da fila que podem ser atribuídos a um Grupo de tópicos ou a um projeto. Tópicos de fila são um tipo de objeto reportável.

Você pode criar Tópicos de fila para projetos individuais ou para modelos de projeto.

Depois de criado, não é possível mover tópicos da fila de um projeto ou modelo para outro.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<!--drafted - replace table with P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
    <p>Novo: Padrão</p>
    <p>ou</p>
    <p>Atual: Plano</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p> Gerenciar permissões do projeto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um Tópico de Fila

1. Crie uma Regra de Encaminhamento, um Grupo de Tópicos e um formulário personalizado, caso planeje associá-los ao Tópico da Fila.\
   Para obter mais informações sobre como criar Regras de Encaminhamento, Grupos de Tópicos ou formulários personalizados, consulte os seguintes artigos:

   * [Criar Regras de Roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Criar Grupos de Tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. Vá para o projeto ou modelo que você escolheu para ativar como uma Fila de solicitação de ajuda e onde você deseja criar um novo tópico da fila.\
   Para obter mais informações sobre como designar um projeto como uma Fila de Solicitação de Ajuda, consulte [Criar uma Fila de Solicitação](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Você pode organizar Tópicos de fila relacionados em um Grupo de tópicos. Isso fornecerá ao solicitante uma série de menus suspensos ao fazer uma solicitação.

   Ou

   Você pode aninhar os Tópicos da fila diretamente no projeto designado como uma Fila de solicitação de ajuda, sem um Grupo de tópicos.

   Para obter informações sobre como criar Grupos de Tópicos, consulte [Criar Grupos de Tópicos](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Clique em **Enfileirar tópicos** no painel esquerdo.
1. Clique em **Novo tópico da fila**.
1. No formulário **Novo Tópico da Fila**, digite o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Nome</strong> </td> 
      <td> Nome do Tópico da Fila.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Descrição</strong> </td> 
      <td>Descrever a fila de solicitações. A descrição é exibida quando os usuários selecionam o tópico da fila no processo de envio de uma nova solicitação. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Adicionar ao Grupo de Tópicos</strong> </td> 
      <td> Se não houver Grupos de Tópicos no projeto, o nome do projeto será padronizado como Grupo de Tópicos.<br>Se quiser criar Grupos de Tópicos adicionais aqui, selecione <strong>Criar Novo Grupo de Tópicos</strong> no menu suspenso.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Formulários personalizados</strong> </td> 
      <td>Selecione quaisquer formulários personalizados que deseja associar ao tópico da fila. Você deve criar formulários personalizados para ocorrências antes de associá-los a tópicos da fila. Para obter informações sobre como criar formulários personalizados, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Criar um formulário personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aprovação padrão</strong></td> 
      <td> <p>Associar um processo de aprovação a este tópico da fila. Somente os Processos de aprovação de problemas ficam visíveis nesse menu suspenso. Todos os problemas enviados para essa fila serão associados a este processo de aprovação. O administrador do Adobe Workfront deve definir Processos de aprovação no nível do sistema antes de associá-los aos tópicos da fila. <span>Um usuário com acesso administrativo a Processos de Aprovação também pode criar processos de aprovação específicos do grupo.</span> Para obter mais informações sobre como criar Processos de Aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Criar um processo de aprovação para itens de trabalho</a>.<br></p> 
       <div> 
        <p>Importante: se o grupo do projeto for alterado, o processo de aprovação específico do grupo anexado às questões existentes se tornará um processo de aprovação de uso único. Para obter mais informações sobre como as alterações no grupo do projeto ou no processo de aprovação afetam as configurações de aprovação, consulte <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Como as alterações no grupo e no processo de aprovação afetam os processos de aprovação atribuídos</a>.</p> 
        <p>Considere o seguinte ao adicionar processos de aprovação a tópicos da fila: </p> 
        <ul style="list-style-type: circle;"> 
         <li>Somente os processos de aprovação ativos são exibidos na lista. </li> 
         <li> <p>Os processos de aprovação específicos do grupo e de todo o sistema são exibidos na lista. Um processo de aprovação associado a um grupo diferente daquele do projeto não é exibido na lista.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Duração Padrão</strong> </td> 
      <td>Essa é a duração padrão da solicitação, e a Data de conclusão planejada da solicitação é calculada com base nesse valor.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Rota Padrão</strong> </td> 
      <td>Especifique a regra de roteamento que deseja associar ao Tópico da Fila. Você deve criar a regra de roteamento antes de anexá-la a um Tópico da Fila. Para obter informações, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">Criar Regras de Roteamento</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tipos de Solicitação</strong> </td> 
      <td> <p>Escolha que tipo de solicitações este tópico da fila armazena. As opções visíveis estão definidas na guia <strong>Detalhes da fila</strong> do projeto. Este campo é obrigatório. </p> 
       <p><b>NOTA</b>:</p>
      <p>Os tipos são exibidos como uma seleção na área Solicitações somente se o Tipo de solicitação for selecionado nas páginas Detalhes da fila e Tópico da fila. Para obter informações sobre como configurar a área Detalhes da Fila de um projeto, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Criar uma Fila de Solicitações</a>. </p> <p>Selecione entre os seguintes tipos:</p> 
       <ul> 
        <li>Relatório de erro</li> 
        <li>Pedido de alteração</li> 
        <li>Problema</li> 
        <li>Solicitar</li> 
       </ul> <p>O administrador do Workfront pode ter renomeado algumas dessas opções. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Caixa Novo Tópico de Fila](assets/new-queue-topic-box.png)

1. Clique em **Salvar**.\
   O Tópico de fila agora está disponível para uso e está visível na área Solicitações do Workfront, depois que uma Fila de solicitação e um Grupo de tópico são selecionados.

## Editar um Tópico de Fila

Para editar um Tópico de Fila existente:

1. Vá para o projeto ou modelo que contém o Tópico da fila que deseja editar.
1. Clique em **Enfileirar tópicos** no painel esquerdo.
1. No ambiente de Produção, selecione o Tópico da fila que deseja editar. Na página Detalhes que é aberta, clique em **Editar Tópico da Fila**.
1. <span class="preview">No ambiente de Visualização, selecione o Tópico da Fila que deseja editar e clique no ícone Editar ![ícone Editar](assets/edit-icon.png).</span>

