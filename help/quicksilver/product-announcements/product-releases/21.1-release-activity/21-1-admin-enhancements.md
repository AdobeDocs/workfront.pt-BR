---
content-type: release-notes
keywords: notas,trimestral,atualizar
navigation-topic: product-releases
title: 21.1 Aprimoramentos do administrador
description: Esta página descreve todas as melhorias de Administrador feitas com a versão 21.1 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 15 de fevereiro de 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 6fe1a2c71f53d6b314c2b1402a547f9c934bfbea
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 0%

---

# 21.1 Aprimoramentos do administrador

Esta página descreve todas as melhorias de Administrador feitas com a versão 21.1 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 15 de fevereiro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.1, consulte a [visão geral da versão 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Introduzir nova configuração de Nível de acesso para copiar projetos

Para dar a você mais controle, como administrador do sistema, sobre o que os planejadores podem fazer com um projeto, tornamos o acesso de Edição a projetos no nível de acesso mais granular, introduzindo uma nova configuração que permite ativar ou desativar a capacidade de copiar projetos. Antes dessa alteração, quando você ativava o acesso dos usuários à Edição de projetos, eles tinham acesso automático à cópia dos projetos. Com o novo recurso, é possível conceder a alguém acesso para editar projetos sem ter necessariamente acesso para copiá-los, desativando a nova configuração Copiar.

Se os usuários tiverem acesso a Editar projetos em seu nível de acesso antes dessa alteração, eles terão essa configuração ativada automaticamente quando esse recurso for lançado.

Para obter informações sobre o nível de acesso Plano, consulte [Conceder acesso aos projetos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obter informações sobre como copiar um projeto, consulte [Copiar um projeto](../../../manage-work/projects/manage-projects/copy-project.md).

Este recurso agora está incluído nos [Fundamentos do administrador na nova experiência do Workfront, Parte 1: caminho de aprendizado Organização de usuários](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) no Workfront One.

## Em um Formulário personalizado em um objeto, selecione todos os itens em um campo suspenso de várias seleções

>[!NOTE]
>
>No momento, essa funcionalidade não está disponível quando você está enviando uma nova solicitação.

Na página Detalhes de um objeto, ao preencher um campo suspenso de várias seleções em um Formulário personalizado, você pode clicar em Selecionar tudo se precisar selecionar todas as opções disponíveis.

Para obter informações sobre como editar dados em um Formulário personalizado, consulte [Editar informações em campos de formulário personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Recalcular todos os campos de formulário personalizado de um objeto

Agora é mais fácil garantir que todos os dados em campos personalizados calculados estejam atualizados para um objeto. Uma nova opção de menu Recalcular Expressões permite recalcular rapidamente todos os dados nesses campos.

Isso é especialmente útil depois que alguém edita dados em outro objeto que é referenciado por um campo personalizado calculado em seu objeto.

Anteriormente, os usuários precisavam usar soluções alternativas para garantir que todos os dados em campos personalizados calculados estivessem atualizados. Por exemplo, eles editaram o objeto junto com outros objetos para usar a opção de recálculo que está disponível para edição em massa.

Para obter mais informações, consulte [Editar informações em campos de formulário personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Desbloqueie preferências de tarefas e problemas para Administradores de Grupos

>[!NOTE]
>
>Até 24 de junho de 2021, isso estava disponível como parte de uma implantação em fases somente para clientes que têm a capacidade de desbloquear as preferências do projeto para grupos. Agora está disponível para todos os clientes.

Os administradores do Adobe Workfront agora podem dar mais autonomia aos administradores de grupo, desbloqueando preferências individuais de tarefas e problemas. Quando uma preferência é desbloqueada, os administradores de grupos podem configurá-la para que seus grupos atendam às necessidades exclusivas e aos processos internos de cada grupo.

Para obter mais informações, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Este recurso agora está incluído nos [Fundamentos do administrador na nova experiência do Workfront, Parte 2: Caminho de Aprendizado da Instalação do Projeto](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) no Workfront One.

## Definir configurações de nível de acesso para portfólios e programas separadamente

Agora é mais fácil gerenciar o acesso de usuários a portfólios e programas, pois você pode definir suas configurações de nível de acesso separadamente.

Anteriormente, as configurações de nível de acesso para portfólios e programas eram combinadas. Isso significava que você não poderia definir as configurações de acesso para programas sem configurá-las da mesma maneira para portfólios, e o mesmo era verdadeiro na ordem inversa.

Para obter informações sobre como configurar um nível de acesso, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Para obter informações sobre configurações de acesso que você pode definir para programas e portfólios, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Este recurso agora está incluído nos [Fundamentos do administrador na nova experiência do Workfront, Parte 1: caminho de aprendizado Organização de usuários](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) no Workfront One.

## Marcar todas as caixas de seleção em uma série ao editar informações em um Formulário personalizado

>[!NOTE]
>
>No momento, essa funcionalidade não está disponível quando você está enviando uma nova solicitação.

Na página Detalhes de um objeto, ao preencher um campo Formulário personalizado contendo caixas de seleção, você pode clicar em Selecionar tudo se precisar marcar todas as caixas de seleção disponíveis.

Essa opção será exibida somente se o campo contiver mais de duas caixas de seleção.

Para obter mais informações, consulte [Editar informações em campos de formulário personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Configurar a pesquisa de email do Workfront incluir na lista de permissões

Incluir na lista de permissões Para proteger melhor seus dados, agora é possível usar uma pesquisa de domínio de email para:

* Controle para onde os emails do Workfront podem ir se contiverem relatórios ou documentos armazenados no Workfront
* Controlar domínios de email pode estar no endereço de email que os usuários podem especificar em seus perfis de usuário

Incluir na lista de permissões Por exemplo, se você quiser proteger dados confidenciais, como um relatório que lista os clientes em risco, poderá incluir somente o(s) domínio(s) de email interno(s) na pesquisa de email. Dessa forma, os usuários não podem enviar esse relatório (ou qualquer outro relatório do Workfront) para um endereço de email externo.

Incluir na lista de permissões incluir na lista de permissões Para obter mais informações, consulte a seção [Configurar o arquivo de firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) no artigo [Configurar o arquivo de firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Atribuir um Administrador de Grupo a um subgrupo

Para facilitar a operação independente dos níveis de sua organização, adicionamos a capacidade de atribuir um Administrador de grupo a um subgrupo. Agora você pode delegar o gerenciamento de subgrupos às pessoas certas.

Anteriormente, somente um grupo de nível superior poderia ter Administradores de grupo, e esses administradores gerenciavam todos os subgrupos abaixo do grupo de nível superior.

Para obter mais informações, consulte a seção [Administradores de grupos para subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) no artigo [Visão geral dos subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Este recurso agora está incluído nos [Fundamentos do administrador na nova experiência do Workfront, Parte 1: caminho de aprendizado Organização de usuários](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) no Workfront One.

## Configurar notificações de eventos para grupos

>[!NOTE]
>
>Disponível como parte de uma implantação em fases somente para clientes que têm a capacidade de desbloquear as preferências do projeto para grupos. Isso inclui todos os clientes nos clusters 4 e 6 e um pequeno número de clientes em outros clusters. Esta nota será atualizada à medida que a funcionalidade se tornar disponível para mais clusters.

Os administradores do Workfront agora podem dar mais autonomia aos administradores de grupo, permitindo que eles configurem notificações de evento para seus grupos de nível superior. Os subgrupos herdam configurações de notificação de eventos do grupo principal.

Anteriormente, as notificações de eventos só podiam ser configuradas por um administrador do Workfront no nível do sistema, o que significa que todos os grupos precisavam usar o mesmo conjunto de notificações de eventos.

Para obter mais informações, consulte os seguintes artigos:

* [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Exibir e configurar notificações de eventos para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

<!--This feature is now included in the [Administrator Fundamentals in the new Workfront experience, Part 1: User Organization](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) learning path on Workfront One.

This feature is now included in the [Email and In-App Notifications in the new Workfront experience](https://experienceleague.adobe.com/en/docs/workfront/using/home://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) learning path on Workfront One.-->

## Trabalhar com projetos de grupo e processos de aprovação na área Grupos

Se você for um Administrador de grupo, é fácil visualizar e trabalhar com os projetos e processos de aprovação do seu grupo, agora que eles estão listados na área Grupos. Na página principal de um grupo, você pode:

* Clique em Projetos no menu esquerdo para ver os projetos do grupo e criar novos projetos para o grupo. Se um projeto selecionado tiver sido compartilhado com você, você poderá usar os botões na barra de ferramentas para editá-lo, exportá-lo, copiá-lo ou excluí-lo.

  Para obter mais informações, consulte [Criar e modificar projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Clique em Approvals no menu esquerdo para ver e gerenciar todos os processos de aprovação associados ao grupo.

  Para obter mais informações, consulte [Processos de aprovação de nível de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Essa funcionalidade também está disponível para administradores do Workfront.

## Exibir o número de licenças usadas e alocadas em um grupo

Para determinar o desempenho de distribuição das licenças, agora é possível visualizar o número de licenças usadas em um grupo e em qualquer subgrupo abaixo dele.

Se você gerenciar um grupo de nível superior, poderá exibir o número de licenças usadas em um grupo (e seus subgrupos) e o número máximo de licenças alocadas para o grupo.

Para obter mais informações, consulte [Exibir o número de licenças alocadas e usadas em um grupo na nova experiência do Adobe Workfront](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

