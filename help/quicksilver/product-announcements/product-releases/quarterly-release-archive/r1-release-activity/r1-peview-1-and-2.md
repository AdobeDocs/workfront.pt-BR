---
content-type: release-notes
navigation-topic: product-releases-archive
title: Visualização 1 e 2 do R1
description: Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com as versões R1.1 e R1.2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 19 de janeiro de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 2%

---

# Visualização 1 e 2 do R1

Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com as versões R1.1 e R1.2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 19 de janeiro de 2017.

Para obter uma lista de todas as alterações feitas em R1, consulte [Visão geral da atividade de versão R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Restaurar Projetos, Tarefas e Problemas da Lixeira 

Os administradores do Workfront agora podem restaurar projetos, tarefas e problemas que foram excluídos nos últimos 30 dias. Todas as informações associadas ao projeto, tarefa ou problema são restauradas, incluindo documentos e dados personalizados.

Novas opções também estão disponíveis para configurar o que acontece com as horas registradas em um projeto, tarefa ou problema excluído. Para obter mais informações, consulte [Configurar efeito em horas quando um objeto for excluído e restaurado](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Para obter mais informações sobre como restaurar objetos no Workfront, consulte [Restaurar itens excluídos](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Para obter informações sobre como exibir projetos, tarefas e problemas restaurados recentemente, consulte [Exibir item restaurado](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## O diagrama de aprovação mostra a representação visual das etapas de aprovação anterior, atual e futura

Agora, quando uma aprovação está pendente em um projeto, tarefa ou problema, um diagrama é exibido. O diagrama de aprovação mostra a etapa atual no processo de aprovação (que está pendente) e também permite visualizar rapidamente as etapas de aprovação anteriores e futuras sem navegar até a guia Aprovações.

Antes dessa alteração, as informações sobre as etapas de aprovação estavam disponíveis somente na guia Aprovações do projeto, tarefa ou problema e eram exibidas somente em uma exibição de lista em vez de em uma exibição de diagrama. (Essas informações ainda estão disponíveis e inalteradas na guia Aprovações .)

Em projetos, as informações de aprovação são exibidas no cabeçalho ao lado do título do projeto. Em tarefas e problemas, as informações de aprovação são exibidas no painel direito.

Para obter mais informações, consulte [Aprovando trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md) em  [Aprovando trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configurar Objetos a Serem Atualizados que Estão Pendentes de Aprovação

Quando um projeto, tarefa ou problema está com aprovação pendente, é possível configurar se os usuários podem:

* Edite o formulário personalizado de um projeto, tarefa ou problema que esteja pendente de aprovação.\
  Para obter informações sobre como configurar projetos, tarefas e problemas a serem editados quando a aprovação estiver pendente, consulte [Definir configurações de aprovação globais](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Adicionar problemas a um projeto com aprovação pendente.\
  Para obter informações sobre como configurar projetos para permitir que os usuários adicionem problemas quando o projeto estiver com aprovação pendente, consulte [Configurar preferências de projeto do sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Editar tarefas e problemas em um projeto que está pendente de aprovação.\
  Para obter informações sobre como configurar projetos para permitir que os usuários editem tarefas e problemas quando o projeto estiver pendente de aprovação, consulte [Configurar preferências de projeto do sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Antes dessa alteração, não era possível editar projetos, tarefas e problemas com aprovação pendente; além disso, não era possível adicionar problemas a projetos com aprovação pendente e tarefas e problemas não podiam ser editados dentro de projetos com aprovação pendente.

## Atribuir modelos de layout a grupos

Agora você pode atribuir modelos de layout a grupos.

Antes dessa alteração, você poderia atribuir modelos de layout a usuários, equipes e funções de trabalho. A atribuição de um modelo de layout a grupos tem a classificação mais baixa na prioridade de atribuição do modelo de layout. 

Para obter mais informações, consulte &quot;Criar e gerenciar modelos de layout&quot;.

## Alterações nas notificações do usuário de edição em massa

A funcionalidade mudou com a edição de configurações de notificação por email de usuário em massa. Quando você seleciona vários usuários para editar suas configurações de email de notificação, somente as notificações específicas que você está atualizando são alteradas para todos os usuários selecionados. Todas as configurações de notificação por email inalteradas permanecem as mesmas para todos os usuários selecionados, mesmo que sejam diferentes de usuário para usuário. 

Antes dessa alteração, as configurações de notificação por email selecionadas eram salvas e todas as outras configurações de notificação inalteradas eram desmarcadas quando você salvava as alterações. 

Para obter mais informações, consulte &quot;Modificando Configurações de Notificação do Usuário em Massa&quot; em [Modificar suas próprias notificações por email](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Aparência e funcionalidade atualizadas de várias notificações por email

A aparência das seguintes notificações por email foi atualizada com uma nova interface:

* Atribuição de problema
* Alterações na data de confirmação
* Quando uma status de projeto for alterada de ideia/aprovado/solicitado/em planejamento para atual, enviar email para a equipe
* Decisão de aprovação às partes interessadas
* Uma conclusão de tarefa predecessora para dependentes de tarefa
* Aprovação pendente (projeto, tarefa, problemas)
* Alteração de status em projetos, tarefas, problemas

Lembre-se de atualizar o endereço de email associado à sua conta para testar essa funcionalidade, pois a Sandbox de visualização apaga os endereços de email de todos os usuários.    Para obter mais informações sobre notificações por email, consulte [notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Novas opções de resumo de email para várias áreas de notificação

As áreas de notificações a seguir tiveram a opção &quot;Resumo diário&quot; adicionada:

* Informações sobre Projetos em que estou trabalhando
* Informações sobre Projetos que estou patrocinando
* Informações sobre Aprovações
* Informações sobre Trabalho atribuído a mim
* Comunicação

Para obter mais informações, consulte [notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  Lembre-se de atualizar o endereço de email associado à sua conta para testar essa funcionalidade, pois a Sandbox de visualização apaga os endereços de email de todos os usuários. 

## Tornar um grupo público

Ao tornar um grupo público, agora é possível adicioná-lo aos usuários sem ser um proprietário de grupo. Será necessário ter acesso administrativo do usuário para editar os usuários.

Para obter mais informações sobre como tornar um grupo público, consulte a seção [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) em [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Compartilhar o URL de um objeto no aplicativo móvel 

Agora você pode compartilhar o URL nos seguintes objetos no aplicativo móvel do Workfront:

* Projetos
* Tarefas
* Problemas
* Planilhas de horas
* Documentos

Você pode compartilhar um URL de um objeto nos seguintes aplicativos:

* Mensagem de texto
* Email
* Unidade de armazenamento (por exemplo, iCloud Drive)
* Outro aplicativo instalado (por exemplo, Notes, Facebook)
* Você pode copiar um link para o objeto na área de transferência e colá-lo posteriormente em qualquer outro aplicativo. 

## Ajuda contextual na configuração

Todas as áreas no menu Configurar foram atualizadas com um ícone Ajuda no canto superior direito da área. Esse ícone fornece um link para um artigo de Site de ajuda sobre essa área. Algumas seções dentro das áreas de Configuração também foram atualizadas com o ícone Ajuda. 

## Adicionar taxas de despesas mais precisas

Agora você pode adicionar taxas de despesas mais exatas ao criar tipos de despesas. As taxas de despesa podem conter até 4 caracteres após a casa decimal (por exemplo, 1,0375). Isso significa que qualquer campo que use essa taxa pode ser mais preciso.

Antes dessa alteração, as taxas de despesa podiam conter apenas até 2 caracteres após a casa decimal (por exemplo, 1,03).

Para obter mais informações sobre como criar taxas de despesas, consulte [Criar tipos de despesas personalizados](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Gravação do webinário de versão 1 e 2 da visualização R1

Este webinário foi apresentado pela equipe de Preparação para versão do Workfront em 19 de janeiro de 2017. Esse webinário foi focado nas alterações de lançamento em 2017 e abordou a nova funcionalidade que está disponível para teste na Pré-visualização.
