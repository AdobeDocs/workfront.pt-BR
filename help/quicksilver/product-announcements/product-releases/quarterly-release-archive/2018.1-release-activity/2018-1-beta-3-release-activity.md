---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão 2018.1 do Beta 3
description: Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.1 do Beta 3. A funcionalidade foi disponibilizada no ambiente de Pré-visualização em 7 de janeiro de 2018. Ele será disponibilizado no ambiente de Produção no início de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 0%

---

# Atividade da versão 2018.1 do Beta 3

Esta página descreve todas as alterações disponíveis mais recentemente no ambiente de Pré-visualização com a versão 2018.1 do Beta 3. A funcionalidade foi disponibilizada no ambiente de Pré-visualização em 7 de janeiro de 2018. Ele será disponibilizado no ambiente de Produção no início de 2018.

>[!IMPORTANT]
>
> A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

Para obter uma lista de todas as alterações feitas em 2018.1, consulte  Visão geral da atividade da versão [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

A versão 2018.1 do Beta 3 contém melhorias para administradores do Workfront e outros usuários:

**Para Administradores**

* [Melhorias no administrador de grupo](#group-administrator-improvements)

**Para Todos Os Usuários**

* [Melhorias do visualizador de provas do HTML5](#html5-proofing-viewer-improvements)
* [Melhorias na revisão no Workfront](#proofing-improvements-within-workfront)
* [Melhorias na Área Residencial](#home-area-improvements) 
* [Melhorias Agile](#agile-improvements)
* [Melhorias no Gráfico de Gantt](#gantt-chart-improvements)
* [Melhorias no planejamento de recursos](#resource-planner-improvements)

## Melhorias no administrador de grupo {#group-administrator-improvements}

* [Redefinição da IU de senha atualizada para administradores de grupo](#reset-password-ui-updated-for-group-administrators)
* [Opções de Configuração de Nível de Acesso para administradores de grupo](#access-level-setup-options-for-group-administrators)
* [Criar perfis de planilha de horas para grupos](#create-timesheet-profiles-for-groups)
* [Recuperar itens excluídos para usuários como um administrador de grupo](#recover-deleted-items-for-users-as-a-group-administrator)

### Redefinição da interface de usuário de senha atualizada para administradores de grupo {#reset-password-ui-updated-for-group-administrators}

Como administrador de grupo, ao redefinir a senha de outro usuário, você será solicitado a fornecer sua própria senha antes de alterar a deles. A interface do usuário foi atualizada para refletir essa funcionalidade. Antes dessa alteração, a interface do usuário mostrava que a senha de administrador do Workfront era necessária.

Para obter mais informações sobre como redefinir senhas para outros usuários, consulte [Editar perfil de um usuário](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Para obter mais informações sobre os recursos de um administrador de grupo, consulte a seção &quot;Recursos de administradores de grupo&quot; em [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Opções de configuração de nível de acesso para administradores de grupo {#access-level-setup-options-for-group-administrators}

Como administrador do Workfront, agora você pode controlar se os administradores de grupo podem fazer logon como outros usuários ou se podem redefinir as senhas de outros usuários. Adicionamos uma nova configuração no Nível de acesso para ativar ou desativar esse acesso. Antes dessa alteração, todos os administradores de grupo podiam fazer logon como outros usuários e redefinir as senhas de outros usuários por padrão. Essa alteração afeta somente o Nível de Acesso do Planejador.

Para obter mais informações sobre como configurar o nível de acesso para usuários, consulte [Conceder acesso aos usuários](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

Para obter mais informações sobre os recursos de um administrador de grupo, consulte a seção &quot;Recursos de administradores de grupo&quot; em [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Criar perfis de planilha de horas para grupos {#create-timesheet-profiles-for-groups}

Como administrador de grupo, agora você pode criar Perfis de planilha de horas para os grupos que administra e associá-los aos grupos que administra ou aos usuários desses grupos. Os perfis de planilha de horas garantem que as planilhas de horas sejam criadas automaticamente para os usuários associados a elas.

Antes dessa alteração, somente um administrador do Workfront poderia criar Perfis de folha de horas.

Para obter mais informações sobre como criar Perfis de Planilha de Horas, consulte [Criar, editar e atribuir perfis de planilha de horas](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Para obter mais informações sobre os recursos de um administrador de grupo, consulte a seção &quot;Recursos de administradores de grupo&quot; em [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

### Recuperar itens excluídos para usuários como um administrador de grupo {#recover-deleted-items-for-users-as-a-group-administrator}

Se um projeto estiver associado a um Grupo para o qual você é o administrador do grupo, você poderá recuperar o projeto ou qualquer uma de suas tarefas, problemas ou documentos excluídos da Lixeira. Antes dessa alteração, somente um administrador do Workfront poderia recuperar itens da Lixeira.

Para obter mais informações sobre como recuperar itens excluídos no Workfront, consulte [Restaurar itens excluídos](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

Para obter mais informações sobre os recursos de um administrador de grupo, consulte a seção &quot;Recursos de administradores de grupo&quot; em [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

## Melhorias no visualizador de provas do HTML5  {#html5-proofing-viewer-improvements}

* [Comparar Modo](#compare-mode)
* [Filtrar a Lista de Comentários](#filter-the-comment-list)
* [A lista de comentários é pesquisada depois que o primeiro caractere é inserido](#comment-list-is-searched-after-the-first-character-is-entered)

### Modo de comparação {#compare-mode}

Agora você pode usar o modo de comparação no visualizador de provas de HTML5 ao exibir provas estáticas e de vídeo. 

O modo Comparar no visualizador de provas HTML5 difere do visualizador de provas herdado das seguintes maneiras:

* Ao iniciar o modo Comparar, a versão mais recente passa para o lado direito, com a versão que você está comparando abrindo à esquerda.

  Anteriormente, a versão mais recente era movida para o lado esquerdo, com a versão que você está comparando abrindo à direita.

* Você pode escolher qual versão de uma prova deseja comparar diretamente no visualizador de provas. 
* O nível de zoom atual e a posição das provas no visualizador de provas são mantidos ao inserir a navegação simultânea.
* Nova opção Redefinir ao usar navegação simultânea.
* Ao sair do modo de comparação, você pode escolher qual prova deseja fechar. 

  Anteriormente, a versão mais antiga era sempre fechada.

* Várias melhorias de aparência e usabilidade.

Para obter mais informações, consulte [Comparar provas no visualizador de provas](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md).

### Filtrar a lista de comentários {#filter-the-comment-list}

Agora é possível filtrar comentários na lista de comentários. Você pode filtrar por usuário, ações, não lidos e muito mais.

### A lista de comentários é pesquisada depois que o primeiro caractere é inserido {#comment-list-is-searched-after-the-first-character-is-entered}

Agora, ao pesquisar a lista de comentários, ela é automaticamente filtrada depois que você digita o primeiro caractere.

Antes dessa alteração, você tinha que digitar pelo menos 3 caracteres no campo de pesquisa antes da lista de comentários ser filtrada.

Para obter mais informações, consulte em .

## Aprimoramentos de provas no Workfront {#proofing-improvements-within-workfront}

* [Vincular Provas do Workfront Proof ao Workfront](#link-proofs-from-workfront-proof-to-workfront)
* [Não é mais possível remover uma prova de um documento](#can-no-longer-remove-a-proof-from-a-document)
* [Aparência atualizada ao gerar e abrir provas](#updated-look-and-feel-when-generating-and-opening-proofs)

### Vincular provas do Workfront Proof ao Workfront {#link-proofs-from-workfront-proof-to-workfront}

Agora você pode vincular provas de documentos que já existem em sua conta do Workfront Proof ao Workfront.

Antes dessa alteração, não era possível acessar provas que já existiam no Workfront Proof no Workfront. 

Para obter mais informações, consulte [Vincular documentos de aplicativos externos](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md) em [Vincular documentos de aplicativos externos](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Não é mais possível remover uma prova de um documento {#can-no-longer-remove-a-proof-from-a-document}

Não é mais possível remover uma prova de um documento. Em vez disso, para remover uma prova, você deve excluir o documento inteiro.

Esse aprimoramento reduz o risco de os usuários excluírem inadvertidamente todas as versões de um documento comprovado. 

Para obter informações sobre como excluir um documento, consulte [Excluir uma prova](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md) em [Excluir uma prova](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md).

### Aparência atualizada ao gerar e abrir provas {#updated-look-and-feel-when-generating-and-opening-proofs}

Agora há um ponteiro de animação atualizado quando uma prova está sendo gerada.

## Melhorias na área inicial {#home-area-improvements}

As seguintes melhorias foram feitas na área Página inicial:

* [Exibir aprovações de provas da área inicial](#view-proof-approvals-from-the-home-area)
* [Os campos padrão são exibidos ao configurar o modelo de layout para itens na área da página inicial](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### Exibir aprovações de provas na área inicial {#view-proof-approvals-from-the-home-area}

Agora você pode visualizar aprovações de prova na área Página inicial, além de aprovações padrão.

Anteriormente, era possível visualizar as aprovações do Workfront, mas não as aprovações de uma prova.  

Para obter mais informações, consulte [Usar a área da Página Inicial](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

### Os campos padrão são exibidos ao configurar o modelo de layout para itens na área da página inicial {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

Anteriormente, os campos padrão não estavam visíveis no modelo de layout.

Para obter mais informações, consulte &quot;Criar e gerenciar modelos de layout&quot;.

## Melhorias Agile {#agile-improvements}

* [Adicionar Tarefas e Problemas à Iteração Diretamente da Página de Detalhes da Tarefa ou Problema](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [Incluir problemas no Backlog Scrum e no Story Board de uma Equipe Agile](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [Aplicar Agrupamentos e Filtros ao Backlog de uma Equipe Agile](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [Criar uma Iteração em Branco e Atualizá-la Mais Tarde](#create-a-blank-iteration-and-update-it-later)
* [Os campos &quot;Foco&quot; e &quot;Capacidade&quot; são preenchidos previamente ao criar uma iteração](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### Adicionar tarefas e problemas à iteração diretamente da página Detalhes da tarefa ou problema {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

Agora é possível adicionar tarefas e problemas que estão atribuídos a uma Equipe Ágil a uma iteração diretamente da tarefa ou problema.

Anteriormente, só era possível adicionar tarefas a uma iteração a partir do backlog. 

Para obter mais informações, consulte [Criar uma iteração](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md) em [Criar uma iteração](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Incluir problemas no backlog de Scrum e no Storyboard de uma Equipe Ágil {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

Agora os problemas são incluídos por padrão no backlog da sua equipe ágil ao usar a metodologia ágil de Scrum (os problemas não são exibidos no backlog de uma equipe ágil ao usar a metodologia Kanban).

Antes dessa alteração, somente tarefas podiam ser adicionadas ao backlog. Se você quiser adicionar um problema, primeiro é necessário converter o problema em uma tarefa antes que ele possa ser adicionado.

Para obter informações sobre problemas no backlog, consulte  [Gerenciar o backlog ágil](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Aplicar agrupamentos e filtros ao backlog de uma equipe Agile {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

As opções de Agrupamento e Filtro agora estão disponíveis no backlog ágil, permitindo organizar o backlog por agrupamentos, bem como filtrar tarefas e problemas específicos.

Antes dessa alteração, você poderia aplicar em exibições ao backlog ágil.

Para obter mais informações, consulte  [Gerenciar a lista de pendências ágil](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md) no  [Gerenciar o backlog ágil](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md).

### Criar uma iteração em Branco e Atualizar Mais Tarde {#create-a-blank-iteration-and-update-it-later}

Não é mais necessário adicionar uma tarefa ou um problema a uma iteração para criá-la. Você pode criar uma iteração em branco e adicionar tarefas e problemas posteriormente.

Para obter mais informações, consulte [Criar uma iteração](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

### Os campos &quot;Foco&quot; e &quot;Capacidade&quot; são preenchidos previamente ao criar uma iteração {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

Agora, ao criar uma iteração, os campos &quot;Foco&quot; e &quot;Capacidade&quot; são pré-preenchidos com os valores médios para todas as iterações anteriores criadas pela sua equipe. Se sua equipe não criou iterações anteriores, esses campos aparecerão como 0.

Anteriormente, esses campos sempre eram definidos como 0.

Para obter mais informações, consulte [Criar uma iteração](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Melhorias no Gráfico de Gantt {#gantt-chart-improvements}

* [Habilitar Modo de Edição no Gráfico de Gantt](#enable-edit-mode-in-the-gantt-chart)
* [Remover predecessores ao editar o gráfico de Gantt](#remove-predecessors-when-editing-the-gantt-chart)

### Ativar modo de edição no gráfico de Gantt {#enable-edit-mode-in-the-gantt-chart}

Ao ativar o modo de edição no gráfico de Gantt, você pode fazer alterações nas informações dentro do gráfico. Antes dessa alteração, não era possível editar as informações no gráfico de Gantt. Só é possível editar informações de tarefas na lista de tarefas.

Para obter mais informações sobre a edição do Gráfico de Gantt, consulte [Atualizar informações na lista de tarefas Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

### Remover predecessores ao editar o gráfico de Gantt {#remove-predecessors-when-editing-the-gantt-chart}

Usando o modo Editar para o Diagrama de Gantt, agora é possível remover os relacionamentos de predecessores entre tarefas no Diagrama de Gantt de um projeto. Antes dessa melhoria, você poderia remover a relação de predecessora somente na lista de tarefas ou no nível da tarefa.

Para obter mais informações sobre a edição do Gráfico de Gantt, consulte [Atualizar informações na lista de tarefas Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md).

## Melhorias no planejamento de recursos {#resource-planner-improvements}

* [Orçamento com Duração Zero no Planejador de Recursos](#budget-with-zero-duration-in-the-resource-planner)

* [Mostrar dados por custo no Planejador de recursos](#show-data-by-cost-in-the-resource-planner)

### Orçamento com Duração Zero no Planejador de Recursos {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>Esse recurso foi removido do ambiente de Pré-visualização e está sendo lançado com a versão 18.1.

Agora você pode fazer o orçamento de seus recursos no Planejador de recursos para qualquer data, dentro ou fora do período do projeto. Antes dessa melhoria, você poderia estimar seus recursos somente para as datas dentro do período do projeto.

Para obter mais informações sobre recursos de orçamento no Planejador de recursos, consulte a seção &quot;Recursos de orçamento no Planejador de recursos&quot; na [Visão geral do Planejador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

### Mostrar dados por custo no Planejador de recursos {#show-data-by-cost-in-the-resource-planner}

Agora você pode exibir as informações no Planejador de recursos por custo, além dos valores de Horas e FTE. Você pode exibir Custos no Planejador de Recursos quando você o estiver visualizando nas visualizações Visualizar por Projeto ou Visualizar por Função. Você não pode exibir Custos quando está exibindo o Planejador de Recursos na view Exibir por Usuário.

Para obter mais informações sobre como exibir o Planejador de Recursos por valores de Horas, FTE ou Custo, consulte [Visão geral da navegação do Planejador de Recursos](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md).
