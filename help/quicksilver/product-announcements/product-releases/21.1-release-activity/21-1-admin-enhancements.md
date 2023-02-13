---
content-type: release-notes
keywords: notas,trimestral,atualizar
navigation-topic: product-releases
title: 21.1 Aprimoramentos do administrador
description: Esta página descreve todas as melhorias do Administrador feitas com a versão 21.1 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 15 de fevereiro de 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# 21.1 Aprimoramentos do administrador

Esta página descreve todas as melhorias do Administrador feitas com a versão 21.1 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 15 de fevereiro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.1, consulte [Visão geral da versão 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Introduza a nova configuração Nível de Acesso para copiar projetos

Para fornecer mais controle, como administrador de sistema, sobre o que os Planejadores podem fazer com um projeto, tornamos o nível de acesso Editar aos projetos mais granular, introduzindo uma nova configuração que permite habilitar ou desabilitar a capacidade de copiar projetos. Antes dessa alteração, quando você ativava o acesso dos usuários a Editar projetos, eles tinham acesso automático para copiá-los. Com o novo recurso, é possível conceder a alguém acesso para editar projetos sem ter necessariamente acesso para copiá-los, desativando a nova configuração Copiar .

Se os usuários tiverem acesso a Editar projetos em seu nível de acesso antes dessa alteração, eles terão essa configuração ativada automaticamente quando esse recurso for lançado.

Para obter informações sobre o nível de acesso do Plano, consulte [Conceder acesso aos projetos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obter informações sobre cópia de um projeto, consulte [Copiar um projeto](../../../manage-work/projects/manage-projects/copy-project.md).

Esse recurso agora está incluído na variável [Fundamentos do administrador na nova experiência do Workfront, Parte 1: Organização do usuário](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) caminho de aprendizagem no Workfront One.

## Em um Formulário personalizado em um objeto, selecione todos os itens em um campo suspenso de várias seleções

>[!NOTE]
>
>Essa funcionalidade não está disponível no momento quando você está enviando uma nova Solicitação.

Na página Detalhes de um objeto, ao preencher um campo suspenso de várias seleções em um Formulário personalizado, você pode clicar em Selecionar tudo se precisar selecionar todas as opções disponíveis.

Para obter informações sobre como editar dados em um Formulário personalizado, consulte [Editar informações em campos de formulário personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Recalcular todos os campos do Formulário personalizado em um objeto

Agora é mais fácil garantir que todos os dados em campos personalizados calculados estejam atualizados para um objeto. Uma nova opção de menu Recalcular expressões permite recalcular rapidamente todos os dados nesses campos.

Isso é especialmente útil depois que alguém edita dados em outro objeto referenciado por um campo personalizado calculado em seu objeto.

Anteriormente, os usuários precisavam usar soluções alternativas para garantir que todos os dados nos campos personalizados calculados estivessem atualizados. Por exemplo, eles editaram o objeto junto com outros objetos para usar a opção de recálculo que está disponível para edição em massa.

Para obter mais informações, consulte [Editar informações em campos de formulário personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Desbloquear preferências de tarefa e emissão para Administradores de Grupo

>[!NOTE]
>
>Até 24 de junho de 2021, isso estava disponível como parte de uma implementação em fases somente para clientes que têm a capacidade de desbloquear preferências de projeto para grupos. Agora ele está disponível para todos os clientes.

Os administradores do Adobe Workfront agora podem dar mais autonomia aos administradores de grupo ao desbloquear tarefas individuais e emitir preferências. Quando uma preferência é desbloqueada, os Administradores de grupo podem configurá-la para seus grupos para atender às necessidades exclusivas de cada grupo e aos processos internos.

Para obter mais informações, consulte [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Esse recurso agora está incluído na variável [Fundamentos do administrador na nova experiência do Workfront, Parte 2: Configuração do projeto](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) caminho de aprendizagem no Workfront One.

## Definir configurações de nível de acesso para portfólios e programas separadamente

Agora é mais fácil gerenciar o acesso dos usuários a portfólios e programas, pois você pode definir suas configurações de nível de acesso separadamente.

Anteriormente, as configurações de nível de acesso para portfólios e programas eram combinadas. Isso significava que você não podia definir configurações de acesso para programas sem configurá-los da mesma forma para portfólios, e o mesmo era verdade em sentido inverso.

Para obter informações sobre como configurar um nível de acesso, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Para obter informações sobre configurações de acesso que você pode configurar para programas e portfólios, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Esse recurso agora está incluído na variável [Fundamentos do administrador na nova experiência do Workfront, Parte 1: Organização do usuário](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) caminho de aprendizagem no Workfront One.

## Marque todas as caixas de seleção em uma série ao editar informações em um formulário personalizado

>[!NOTE]
>
>Essa funcionalidade não está disponível no momento quando você está enviando uma nova Solicitação.

Na página Detalhes de um objeto, ao preencher um campo Formulário personalizado contendo caixas de seleção, você pode clicar em Selecionar tudo se precisar selecionar todas as caixas de seleção disponíveis.

Essa opção é exibida somente se o campo contiver mais de 2 caixas de seleção.

Para obter mais informações, consulte [Editar informações em campos de formulário personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Configurar a Workfront de lista de permissões de email do

Para proteger melhor seus dados, agora você pode usar um domínio de email lista de permissões para:

* Controle para onde os emails do Workfront podem ir se contiverem relatórios ou documentos armazenados no Workfront
* Controlar domínios de email podem estar no endereço de email que os usuários podem especificar em seu perfil de usuário

Por exemplo, se você quiser proteger dados confidenciais, como um relatório que lista seus clientes de risco, poderá incluir somente seu domínio de email interno ou domínios na  de lista de permissões de email. Dessa forma, os usuários não podem enviar esse relatório (ou qualquer outro relatório do Workfront) para um endereço de email externo.

Para obter mais informações, consulte a seção [Configurar a  lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) no artigo [Configurar a  lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Atribuir um Administrador de Grupo a um subgrupo

Para facilitar o funcionamento independente dos níveis de sua organização, adicionamos a capacidade de atribuir um Administrador de grupo a um subgrupo. Agora é possível delegar o gerenciamento de subgrupos às pessoas certas.

Anteriormente, somente um grupo de nível superior podia ter Administradores de grupo e esses administradores gerenciavam todos os subgrupos abaixo do grupo de nível superior.

Para obter mais informações, consulte a seção [Administradores de grupo para subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) no artigo [Visão geral de subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Esse recurso agora está incluído na variável [Fundamentos do administrador na nova experiência do Workfront, Parte 1: Organização do usuário](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) caminho de aprendizagem no Workfront One.

## Configurar notificações de evento para grupos

>[!NOTE]
>
>Disponível como parte de uma implantação em fases somente para clientes que têm a capacidade de desbloquear preferências de projeto para grupos. Isso inclui todos os clientes no Cluster 4 e 6 e um pequeno número de clientes em outros clusters. Essa nota será atualizada à medida que a funcionalidade for disponibilizada para mais clusters.

Os administradores do Workfront agora podem dar mais autonomia aos administradores de grupo, permitindo que eles configurem notificações de eventos para seus grupos de nível superior. Os subgrupos herdam as configurações de notificação de evento do grupo pai principal.

Anteriormente, as notificações de eventos eram configuráveis somente por um administrador do Workfront no nível do sistema, o que significa que todos os grupos tinham que usar o mesmo conjunto de notificações de eventos.

Para obter mais informações, consulte os seguintes artigos:

* [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Exibir e configurar notificações de evento para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

Esse recurso agora está incluído na variável [Fundamentos do administrador na nova experiência do Workfront, Parte 1: Organização do usuário](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) caminho de aprendizagem no Workfront One.

Esse recurso agora está incluído na variável [Notificações por email e no aplicativo na nova experiência do Workfront](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) caminho de aprendizagem no Workfront One.

## Trabalhar com projetos de grupos e processos de aprovação na área Grupos

Se você for um Administrador de grupo, é fácil visualizar e trabalhar com os projetos do seu grupo e os processos de aprovação, agora que estão listados na área Grupos . Na página principal de um grupo, é possível:

* Clique em Projetos no menu à esquerda para ver os projetos do grupo e criar novos para o grupo. Se um projeto selecionado foi compartilhado com você, é possível usar os botões na barra de ferramentas para editá-lo, exportá-lo, copiá-lo ou excluí-lo.

   Para obter mais informações, consulte [Criar e modificar projetos de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Clique em Aprovações no menu esquerdo para ver e gerenciar todos os processos de aprovação associados ao grupo.

   Para obter mais informações, consulte [Processos de aprovação no nível do grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Essa funcionalidade também está disponível para administradores do Workfront.

## Exibir o número de licenças usadas e alocadas em um grupo

Para determinar o grau de distribuição de suas licenças, agora é possível visualizar o número de licenças usadas em um grupo e em qualquer subgrupo abaixo dele.

Se você gerenciar um grupo de nível superior, é possível visualizar o número de licenças usadas em um grupo (e seus subgrupos) e o número máximo de licenças alocadas para o grupo.

Para obter mais informações, consulte [Exibir o número de licenças alocadas e usadas em um grupo na nova experiência do Adobe Workfront](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

