---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Visão geral do processo de aprovação
description: Você pode criar um processo de aprovação e anexá-lo a um objeto para garantir que os usuários designados revisem determinadas alterações antes que o objeto avance.
author: Courtney
feature: Work Management
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# Visão geral do processo de aprovação

Você pode criar um processo de aprovação e anexá-lo a um objeto para garantir que os usuários designados revisem determinadas alterações antes que o objeto avance.

Isso está disponível para os seguintes tipos de objetos no Adobe Workfront:

* Item de trabalho (projeto, tarefa ou emissão, modelo, tarefa do modelo)
* Documento
*  Prova

Para obter instruções sobre como criar um processo de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Este artigo contém informações gerais sobre processos de aprovação associados a itens de trabalho.

## Tipos de processos de aprovação

Se você for um administrador da Adobe Workfront ou um usuário com acesso administrativo aos processos de aprovação, poderá criar os seguintes processos de aprovação para projetos, tarefas e problemas:

* **Um processo de aprovação global em nível de sistema**: Os usuários podem anexá-los a qualquer um dos seguintes procedimentos:

   * Um projeto, tarefa ou problema na seção Aprovações
   * Na caixa Editar projeto, na área Processo de Aprovação Padrão da Tarefa
   * Na seção Detalhes da fila ou Tópico da fila de um projeto, nas áreas Processo de aprovação padrão. O projeto deve ser habilitado como uma fila de solicitações.

* **Um processo de aprovação global em nível de grupo**: Os usuários podem anexá-los ao seguinte:

   * Um projeto, tarefa ou problema pertencente ao grupo que esteja associado ao processo de aprovação na seção Aprovações
   * Na caixa Editar projeto, na área Processo de aprovação padrão da tarefa para um projeto pertencente ao grupo associado ao processo de aprovação
   * Na seção Detalhes da fila ou Tópico da fila de um projeto, nas áreas Processo de aprovação padrão. O projeto deve ser habilitado como uma fila de solicitações e deve pertencer ao grupo associado ao processo de aprovação.

   Para obter informações sobre como criar o processo de aprovação no nível do sistema ou de grupo, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Um processo de aprovação de uso único**: Para uso com um único projeto, tarefa, problema, modelo ou tarefa de modelo. Esse tipo de processo de aprovação afeta apenas o objeto associado a ele e não está disponível para ser associado a nenhum outro objeto.

   Para obter informações sobre como criar um processo de aprovação de uso único, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Este artigo usa o termo &quot;processo de aprovação global&quot; para diferenciar do &quot;processo de aprovação de uso único&quot;. Um processo de aprovação global pode ser usado repetidamente.
>
>O termo &quot;processo de aprovação global a nível de grupo&quot; refere-se a um processo de aprovação que pode ser utilizado repetidamente em itens e com status associados apenas a um grupo específico.

Para obter informações sobre como criar um processo de aprovação de nível de sistema ou um processo de aprovação de nível de grupo, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Considerações sobre os processos de aprovação

* Você deve criar o projeto, a tarefa, a emissão, o modelo ou a tarefa do modelo antes que o processo de aprovação possa ser associado a eles.
* Um processo de aprovação está sempre associado a dois itens essenciais:

   * Cada processo de aprovação corresponde a um determinado status de item de trabalho no sistema Workfront. Quando você altera o status de um item de trabalho, uma aprovação anexada para esse status requer que a alteração de status seja confirmada antes que o novo status possa ser atribuído ao item.

      >[!TIP]
      >
      >
      >   
      >   
      >   * Você pode associar uma aprovação de nível de grupo a um status global ou de nível de grupo.
      >   * Não é possível alterar o status de um item usando um processo de aprovação para um status diferente daquele associado ao processo de aprovação.

         >   
         >   
         >     Por exemplo, se você tiver uma aprovação de tarefa associada ao status Em andamento, a tarefa alterará automaticamente seu status para Em andamento quando a aprovação for concedida. Ele não pode alterar automaticamente seu status para Completed ou qualquer outro status que não esteja associado à aprovação.


   * As entidades associadas a um processo de aprovação podem ser usuários, funções de trabalho ou equipes. Os usuários são responsáveis por aceitar ou rejeitar a aprovação. É possível atribuir aprovações a usuários que cumprem uma determinada função no projeto. Por exemplo, você pode atribuir uma aprovação a um Proprietário do projeto ou Patrocinador. Para obter mais informações, consulte [Criar um processo de aprovação para itens de trabalho](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

      Os seguintes cenários existem:

      * Quando você atribui uma aprovação a funções de cargo, qualquer usuário na Equipe do Projeto que esteja associado à função de cargo pode tomar uma decisão sobre a aprovação. A função associada à aprovação pode ser a Função principal ou qualquer Outra função.

         Para obter informações sobre a Equipe do projeto, consulte [Visão geral da equipe do projeto](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Ao atribuir uma aprovação a uma equipe, qualquer membro dessa equipe pode tomar uma decisão sobre a aprovação. A equipe associada à aprovação pode ser a Equipe inicial ou qualquer outra equipe.

         Para obter informações sobre funções e equipes de um usuário, consulte [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Quando você cria um item de trabalho, ele não tem um processo de aprovação anexado automaticamente. Você deve anexar um manualmente se quiser usar um. Para obter informações sobre como anexar um processo de aprovação a um item, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* O administrador do Workfront ou um usuário com acesso administrativo aos processos de aprovação pode criar processos de aprovação global no nível do sistema para uso em todo o sistema. Um administrador de grupo com acesso administrativo a processos de aprovação pode criar um processo de aprovação global em nível de grupo para uso somente por um determinado grupo que ele gerencia.
* Se você não quiser usar um processo de aprovação global predefinido de nível de sistema ou de grupo para um item de trabalho, poderá criar e anexar um processo de aprovação de uso único a ele quando tiver permissões de gerenciamento no objeto para o qual deseja anexar o processo de aprovação.

   >[!NOTE]
   Você pode usar um processo de aprovação de uso único apenas uma vez para o item específico para o qual ele foi criado. Você pode associar status globais, bem como status de nível de grupo para processos de aprovação de uso único para projetos, tarefas, problemas, modelos e tarefas de modelo.

* Ao anexar um processo de aprovação em nível de grupo a um item usando status personalizados em nível de grupo, alterar o Grupo do projeto pode criar um conflito entre os status de aprovação do grupo anterior e aqueles existentes no nível do sistema. Considere remover os processos de aprovação em nível de grupo no projeto, ou suas tarefas ou problemas antes de atualizar o grupo. Para obter informações sobre como criar processos de aprovação em nível de grupo, consulte [Processos de aprovação no nível do grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Para obter informações sobre como criar status de grupo personalizado, consulte [Criar ou editar um status de grupo](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Para obter informações sobre como atualizar o Grupo de um projeto, consulte [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

## O fluxo de trabalho do processo de aprovação

Esta seção explica o seguinte sobre a aprovação de itens de trabalho:

* [Como os processos de aprovação dependem dos status](#how-approval-processes-rely-on-statuses)
* [Como um fluxo de trabalho típico usa um processo de aprovação](#how-a-typical-workflow-uses-an-approval-process)

### Como os processos de aprovação dependem dos status {#how-approval-processes-rely-on-statuses}

Anexar um status a um processo de aprovação garante que o item passe pelos departamentos na ordem correta.

**Exemplo:** Você pode anexar um processo de aprovação ao status de Departamento de marketing que requer aprovação pelo departamento de finanças. Em seguida, quando alguém altera o status de um item de trabalho para &quot;Departamento de Marketing&quot;, o item não pode ser movido para esse departamento até que o Departamento de Finanças se desconecte dele.

Para obter mais informações sobre status para itens de trabalho, consulte os seguintes artigos:

* [Acessar a lista de status de projeto do sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Acessar a lista de status de tarefas do sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Acesse a lista de status de problemas do sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Como um fluxo de trabalho típico usa um processo de aprovação {#how-a-typical-workflow-uses-an-approval-process}

O cenário a seguir ilustra como um processo de aprovação ajuda os usuários a aprovar o trabalho como um objeto do Workfront progride por meio de um fluxo de trabalho de várias etapas nesta ordem:

1. O administrador do Workfront ou um usuário com acesso administrativo a Processos de Aprovação cria um processo de aprovação para um projeto, tarefa ou problema.

   >[!NOTE]
   Você pode anexar processos de aprovação de projeto a um modelo e processos de aprovação de tarefa a uma tarefa de modelo. Depois disso, quando alguém usa o modelo para criar um projeto, o processo de aprovação se torna um processo de aprovação de projeto ou tarefa, respectivamente. Um processo de aprovação de uso único anexado a uma tarefa de modelo ou modelo permanece um processo de aprovação de uso único para projetos e tarefas.

1. Um usuário com permissão Gerenciar ao projeto, tarefa ou problema anexa o processo de aprovação ao item ou cria uma aprovação de uso único para o item.
1. Um usuário atribuído ao item de trabalho altera seu status para o status que inicia o processo de aprovação e ele é iniciado. (A pessoa que criou o processo de aprovação definiu a relação entre o status e o processo de aprovação.)
1. Os aprovadores designados recebem uma notificação sobre o processo de aprovação pendente e revisam o item de trabalho.
1. O processo de aprovação termina depois que os aprovadores designados aprovarem todas as etapas do processo. Ou, se rejeitarem uma etapa, o status será redefinido para um status predefinido ou um problema será criado. (A pessoa que criou o processo de aprovação definiu quais dessas etapas automatizadas ocorrem após uma rejeição.)

**Exemplo:** Uma equipe de publicidade criou um status chamado Pronto para impressão e um processo de aprovação chamado Designer/Copywriter Signoff que ela associou a esse status. Esse processo de aprovação é configurado para:

* Exigir aprovação do designer e do redator da equipe
* Iniciar sempre que alguém alterar o status de um item de trabalho para Pronto para Impressão

Um proprietário de projeto de panfleto anexa o processo de aprovação de Assinatura do Designer/Cópia ao projeto de panfleto.

Quando alguém no projeto altera o status para Pronto para Impressão, o redator e designer recebem notificações pedindo sua aprovação ou rejeição. Durante o processo de aprovação, quando estiverem deliberando se a aprovam ou não, o status dos projetos será exibido como Pronto para impressão - Aprovação pendente.

Depois que ambos aprovarem o folheto no Workfront, o status do projeto será alterado para Pronto para Impressão.

## Processos de aprovação de documentos

Aprovações de documentos são usadas para uma aprovação mais geral. Os comentários são capturados no formato de chat na guia Atualizações . Você pode usar os botões de aprovação para aprovar, rejeitar ou aprovar com alterações.

Para adicionar aprovadores a um documento depois que ele for carregado no Workfront, consulte [Solicitar aprovações de documento](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Processos de aprovação de prova

Aprovações de prova são usadas para uma análise mais profunda e geralmente incluem fluxos de trabalho mais complicados. O feedback é capturado com ferramentas de marcação no visualizador de prova. Você pode usar os botões de aprovação para aprovar, rejeitar ou aprovar com alterações.

Para adicionar um Fluxo de trabalho automatizado a uma prova de documento e designar determinados usuários no fluxo de trabalho como aprovadores da prova, consulte [Criar uma prova avançada com um fluxo de trabalho Automatizado](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Definir configurações para processos de aprovação de item de trabalho

Como administrador do Workfront, você pode definir configurações globais para processos de aprovação de itens de trabalho em seu sistema. Essas configurações determinam várias regras para processos de aprovação, como por quanto tempo uma decisão de aprovação deve permanecer aberta ou como você gerencia a delegação de aprovação em seu sistema. Para obter mais informações sobre configurações do processo de aprovação, consulte [Definir configurações de aprovação global](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
