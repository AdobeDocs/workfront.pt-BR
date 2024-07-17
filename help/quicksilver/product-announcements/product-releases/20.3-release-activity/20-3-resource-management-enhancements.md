---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Aprimoramentos no gerenciamento de recursos
description: Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 20.3 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 10 de agosto de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 20.3 Aprimoramentos no gerenciamento de recursos

Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 20.3 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 10 de agosto de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.3, consulte a [visão geral da versão 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Incluir horas de problemas na área Trabalho atribuído do Balanceador de carga de trabalho

Para permitir que você veja uma imagem completa de todas as cargas de trabalho do seu pessoal, introduzimos uma configuração que permite incluir horas de problemas na área Trabalho atribuído do Balanceador de carga de trabalho.

Para obter informações sobre como trabalhar no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajustar alocações para dias não úteis no Balanceador de carga de trabalho

Você pode ajustar alocações para seus recursos para dias não úteis usando o Balanceador de carga de trabalho.

Para obter informações sobre como gerenciar alocações no Balanceador de carga de trabalho, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Filtros variáveis disponíveis no Balanceador de carga de trabalho

Para melhorar sua experiência e fornecer mais flexibilidade ao compartilhar informações, implementamos filtros de variável para o Balanceador de carga de trabalho. Os seguintes filtros foram adicionados ao Balanceador de carga de trabalho:

* &quot;Me&quot; (ao filtrar por usuários)
* &quot;Minha função principal&quot; (ao filtrar por funções)
* &quot;Minha equipe inicial&quot; ou &quot;Todas as minhas equipes&quot; (ao filtrar por equipes).

Esses filtros substituem as variáveis de filtro curinga de $$USER.ID, $$USER.roleID, $$USER.homeTeamID e $$USER.teamIDs

Ao aplicar um desses filtros e, em seguida, compartilhar o Balanceador de carga de trabalho ou colocá-lo em um painel, todos os outros usuários verão suas próprias informações.

Para obter informações sobre como aplicar filtros ao Balanceador de carga de trabalho, consulte [Informações de filtro no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nova classificação para projetos no Balanceador de carga de trabalho

O Balanceador de carga de trabalho agora classifica os projetos com base primeiro na Data de início planejada mais antiga e depois na Data de conclusão planejada mais recente das tarefas no projeto que ocorrem durante o período de tempo que o usuário exibe na tela. Isso permite organizar o trabalho em uma hierarquia em árvore, o que ajuda a identificar mais facilmente o trabalho de um dia.

Para obter informações sobre como exibir projetos e itens de trabalho no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Exibir o progresso real do trabalho no Balanceador de carga de trabalho

Para fornecer uma perspectiva precisa do progresso da carga de trabalho, introduzimos uma nova configuração no Balanceador de carga de trabalho que mostra a linha do tempo de tarefas e problemas de acordo com suas Datas projetadas. Você pode ativar a configuração Mostrar Datas Projetadas para exibir a linha do tempo projetada do item de trabalho, além da linha do tempo planejada.

Além disso, com essa melhoria, se uma tarefa ou um problema for concluído antes da Data de conclusão planejada, as horas alocadas dos dias restantes serão eliminadas para indicar que elas não contam para a alocação geral do usuário.

Para obter informações sobre como navegar no Balanceador de carga de trabalho e habilitar configurações, consulte [Navegar no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Os recursos do Balanceador de carga de trabalho anteriormente comunicados como lançados com a versão 20.2

* [Ajustar a alocação diária e semanal no Balanceador de Carga de Trabalho](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Atualizar horas planejadas da tarefa no Balanceador de carga de trabalho](#update-task-planned-hours-in-the-workload-balancer)
* [Uma maneira mais conveniente de atualizar alocações no Balanceador de carga de trabalho](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Ajustar a alocação diária e semanal no Balanceador de carga de trabalho {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Para evitar o esgotamento de seus recursos, agora é possível ajustar a alocação diária e semanal de seus usuários para trabalhar usando o Balanceador de carga de trabalho.

Antes desse aprimoramento, isso só era possível usando as ferramentas de Agendamento de recursos.

Para obter informações sobre como gerenciar alocações no Balanceador de carga de trabalho, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

### Atualizar horas planejadas da tarefa no Balanceador de carga de trabalho {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Esse aprimoramento estará disponível na Produção logo após a versão 2020.2.

Uma nova opção na área Gerenciamento de recursos do nível de acesso agora permite que os usuários com esse acesso editem Horas planejadas no Balanceador de carga de trabalho. Quando você ajusta alocações no Balanceador de carga de trabalho, o total de alocações diárias não precisa corresponder ao número de Horas planejadas das tarefas. Depois que você salvar as alocações, o total de horas de alocação se tornará as Horas planejadas da tarefa. Isso só é possível para tarefas que tenham um Tipo de duração simples.

Para obter informações sobre como gerenciar alocações no Balanceador de carga de trabalho, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Para obter informações sobre como conceder acesso ao Gerenciamento de Recursos, consulte [Conceder acesso ao Gerenciamento de Recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Uma maneira mais conveniente de atualizar alocações no Balanceador de carga de trabalho {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Para facilitar o gerenciamento das alocações de um usuário para um item de trabalho no Balanceador de carga de trabalho, clique duas vezes no item de trabalho. Você também pode usar a opção existente do menu Editar alocações. Além disso, não é mais necessário ativar a exibição de alocações para poder atualizá-las.

Para obter informações sobre como gerenciar alocações no Balanceador de carga de trabalho, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
