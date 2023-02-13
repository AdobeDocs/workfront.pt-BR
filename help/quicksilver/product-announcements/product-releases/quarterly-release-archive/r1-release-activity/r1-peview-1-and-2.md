---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Visualização 1 e 2
description: Esta página descreve todas as alterações disponíveis no ambiente de Visualização com as versões R1.1 e R1.2. A funcionalidade nesta página foi disponibilizada no ambiente de Visualização em 19 de janeiro de 2017.
author: Luke
feature: Product Announcements
exl-id: 65219cf1-809f-4d8e-a858-01f7881064d7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 2%

---

# R1 Visualização 1 e 2

Esta página descreve todas as alterações disponíveis no ambiente de Visualização com as versões R1.1 e R1.2. A funcionalidade nesta página foi disponibilizada no ambiente de Visualização em 19 de janeiro de 2017.

Para obter uma lista de todas as alterações feitas em R1, consulte [Visão geral da atividade de versão do R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Restaurar projetos, tarefas e problemas da Lixeira 

Os administradores do Workfront agora podem restaurar projetos, tarefas e problemas que foram excluídos nos últimos 30 dias. Todas as informações associadas ao projeto, tarefa ou problema são restauradas, incluindo documentos e dados personalizados.

Novas opções também estão disponíveis para configurar o que acontece com as horas registradas em um projeto, tarefa ou problema que é excluído. Para obter mais informações, consulte [Configurar o efeito em horas quando um objeto é excluído e restaurado](../../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

Para obter mais informações sobre como restaurar objetos no Workfront, consulte [Restaurar itens excluídos](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Para obter informações sobre como visualizar projetos, tarefas e problemas que foram restaurados recentemente, consulte [Exibir item restaurado](../../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

## Diagrama de Aprovação Mostra a Representação Visual das Etapas de Aprovação Anterior, Atual e Futura

Agora, quando uma aprovação está pendente em um projeto, tarefa ou problema, um diagrama é exibido. O diagrama de aprovação mostra a etapa atual do processo de aprovação (que está pendente) e também permite visualizar rapidamente as etapas de aprovação anteriores e futuras sem navegar até a guia Aprovações .

Antes dessa alteração, as informações sobre as etapas de aprovação estavam disponíveis somente na guia Aprovações do projeto, tarefa ou problema, e eram exibidas somente em uma exibição de lista, em vez de em uma exibição de diagrama. (Essas informações ainda estão disponíveis e inalteradas na guia Aprovações .)

Em projetos, as informações de aprovação são exibidas no cabeçalho ao lado do título do projeto. Em tarefas e problemas, as informações de aprovação são exibidas no painel direito.

Para obter mais informações, consulte [Aprovar trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md) em  [Aprovar trabalho](../../../../review-and-approve-work/manage-approvals/approving-work.md).

## Configurar objetos a serem atualizados que estão pendentes de aprovação

Quando um projeto, tarefa ou problema está pendente de aprovação, agora você pode configurar se os usuários podem:

* Edite o formulário personalizado de um projeto, tarefa ou problema que está pendente de aprovação.\
   Para obter informações sobre como configurar projetos, tarefas e problemas a serem editados durante a aprovação pendente, consulte [Definir configurações de aprovação global](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)

* Adicione problemas a um projeto que está pendente de aprovação.\
   Para obter informações sobre como configurar projetos para permitir que os usuários adicionem problemas quando o projeto estiver pendente de aprovação, consulte [Configurar preferências de projeto em todo o sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Edite tarefas e problemas em um projeto que está pendente de aprovação.\
   Para obter informações sobre como configurar projetos para permitir que usuários editem tarefas e problemas quando o projeto estiver pendente de aprovação, consulte [Configurar preferências de projeto em todo o sistema](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Antes dessa alteração, os projetos, as tarefas e os problemas que estavam pendentes de aprovação não podiam ser editados; além disso, não foi possível adicionar problemas a projetos que estavam pendentes de aprovação e tarefas e problemas não podiam ser editados em projetos que estavam pendentes de aprovação.

## Atribuir modelos de layout a grupos

Agora é possível atribuir modelos de layout a grupos.

Antes dessa alteração, você podia atribuir modelos de layout a usuários, equipes e funções de trabalho. Atribuir um modelo de layout a grupos apresenta a classificação mais baixa na prioridade de atribuição do modelo de layout. 

Para obter mais informações, consulte &quot;Criação e gerenciamento de modelos de layout&quot;.

## Alterações nas notificações do usuário de edição em massa

A funcionalidade foi alterada ao editar as configurações de notificação por email do usuário em massa. Ao selecionar vários usuários para editar suas configurações de email de notificação, somente as notificações específicas que você está atualizando serão alteradas para todos os usuários selecionados. Todas as configurações de notificação de email inalteradas permanecem as mesmas para todos os usuários selecionados, mesmo que sejam diferentes de usuário para usuário. 

Antes dessa alteração, as configurações de notificação por email selecionadas eram salvas e todas as outras configurações de notificação inalteradas eram desmarcadas ao salvar as alterações. 

Para obter mais informações, consulte &quot;Modificando configurações de notificação do usuário em massa&quot; em [Ativar ou desativar suas próprias notificações de evento](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Aparência atualizada de várias notificações por email

A aparência das seguintes notificações por email foi atualizada com uma nova interface do usuário:

* Atribuição de emissão
* Confirmar alterações na data
* Quando uma status de projeto for alterada de ideia/aprovado/solicitado/em planejamento para atual, enviar email para a equipe
* Decisão de aprovação das partes interessadas
* Uma conclusão de tarefa predecessora para dependentes de tarefa
* Aprovação pendente (projeto, tarefa, problemas)
* Alteração de status em projetos, tarefas, problemas

Lembre-se de atualizar o endereço de email associado à sua conta para poder testar essa funcionalidade, já que a sandbox de visualização limpa os endereços de email de todos os usuários.    Para obter mais informações sobre notificações por email, consulte [Notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  

## Novas opções de resumo de email para várias áreas de notificação

As áreas de notificações a seguir tiveram a opção &quot;Resumo diário&quot; adicionada:

* Informações sobre projetos em que estou
* Informações sobre Projetos que estou patrocinando
* Informações sobre Aprovações
* Informações sobre Trabalho atribuído a mim
* Comunicação

Para obter mais informações, consulte [Notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).  Lembre-se de atualizar o endereço de email associado à sua conta para poder testar essa funcionalidade, já que a sandbox de visualização limpa os endereços de email de todos os usuários. 

## Tornar um grupo público

Ao tornar um grupo público, agora é possível adicionar esse grupo aos usuários sem ser proprietário do grupo. Você terá que ter acesso administrativo do usuário para poder editar usuários.

Para obter mais informações sobre como tornar um grupo público, consulte a [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#making-a-group-public) seção em [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Compartilhar o URL de um objeto no aplicativo móvel 

Agora você pode compartilhar o URL nos seguintes objetos no aplicativo móvel do Workfront:

* Projetos
* Tarefas
* Problemas
* Folhas de horas
* Documentos

Você pode compartilhar um URL de um objeto nos seguintes aplicativos:

* Mensagem de texto
* email
* Unidade de armazenamento (por exemplo, iCloud Drive)
* Outro aplicativo instalado (por exemplo, Notes, Facebook)
* Você pode copiar um link para o objeto para a área de transferência e colá-lo posteriormente em qualquer outro aplicativo. 

## Ajuda sensível ao contexto na configuração

Todas as áreas do menu Configuração foram atualizadas com um ícone Ajuda no canto superior direito da área. Este ícone fornece um link para um artigo do Site de Ajuda sobre essa área. Algumas seções dentro das áreas de Configuração também foram atualizadas com o ícone Ajuda. 

## Adicionar Taxas de Despesa Mais Precisas

Agora você pode adicionar taxas de despesas mais exatas ao criar tipos de despesas. As taxas de despesa podem conter até 4 caracteres após o decimal (por exemplo, 1,0375). Isso significa que todos os campos que usam essa taxa podem ser mais precisos.

Antes dessa alteração, as taxas de despesas podiam conter até 2 caracteres após o decimal (por exemplo, 1,03).

Para obter mais informações sobre como criar taxas de despesas, consulte [Criar tipos de despesas personalizadas](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Updated Look and Improved Performance in the Tasks&nbsp;List (by request only)</h2>
-->

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This feature focuses primarily on improving the performance of large lists of tasks. The interface of tasks lists has been updated, but delivers the same functionality as the existing tasks list. You can have access to the new tasks list only if you request it. For more information about how to request access to the new tasks list, see Testing Tasks Lists (Beta).
</MadCap:conditionalText>
-->

 

## Registro do webinar de versão 1 e 2 da visualização R1

Esse Webinar foi apresentado pela equipe de preparação para a versão da Workfront em 19 de janeiro de 2017. Este webinário foi focado nas alterações de versão em 2017 e abordou a nova funcionalidade disponível para teste na Visualização.
