---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Melhorias no gerenciamento de recursos
description: Esta página descreve todos os aprimoramentos do Gerenciamento de recursos feitos com a versão 20.3 para o ambiente Produção. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 10 de agosto de 2020.
author: Luke
feature: Product Announcements
exl-id: a2c34117-e03c-4394-9b81-7c18433531d1
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# 20.3 Melhorias no gerenciamento de recursos

Esta página descreve todos os aprimoramentos do Gerenciamento de recursos feitos com a versão 20.3 para o ambiente Produção. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 10 de agosto de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.3, consulte [Visão geral da versão 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Incluir horas de problemas na área Trabalho Atribuído do Balanceador de Carga de Trabalho

Para permitir que você veja uma imagem completa de todas as cargas de trabalho de suas pessoas, introduzimos uma configuração que permite incluir horas de problemas na área de Trabalho Atribuído do Balanceador de Carga de Trabalho.

Para obter informações sobre como trabalhar no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajustar alocações para dias não úteis no Balanceador de Carga de Trabalho

Você pode ajustar alocações para seus recursos para dias que não sejam úteis usando o Balanceador de Carga de Trabalho.

Para obter informações sobre o gerenciamento de alocações no Balanceador de Carga de Trabalho, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Filtros de variável disponíveis no Balanceador de carga de trabalho

Para melhorar sua experiência e proporcionar mais flexibilidade ao compartilhar informações, agora implementamos filtros variáveis para o Balanceador de carga de trabalho. Os seguintes filtros foram adicionados ao Balanceador de Carga de Trabalho:

* &quot;Me&quot; (ao filtrar por usuários)
* &quot;Minha função principal&quot; (ao filtrar por funções)
* &quot;Minha equipe inicial&quot; ou &quot;Todas as minhas equipes&quot; (ao filtrar por equipes).

Esses filtros substituem as variáveis de filtro curinga de $$USER.ID, $$USER.roleID, $$USER.homeTeamID e $$USER.TeamIDs

Ao aplicar um desses filtros e compartilhar o Balanceador de carga de trabalho ou colocá-lo em um painel, todos os outros usuários verão suas próprias informações.

Para obter informações sobre como aplicar filtros ao Balanceador de Carga de Trabalho, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Nova classificação para projetos no Balanceador de Carga de Trabalho

O Balanceador de Carga de Trabalho agora classifica os projetos com base primeiro na Data Inicial Planejada mais antiga e, em segundo lugar, na Data de Conclusão Planejada mais recente das tarefas no projeto que ocorrem durante o período que o usuário exibe na tela. Isso permite organizar o trabalho em uma hierarquia em árvore, o que ajuda a identificar o trabalho com mais facilidade por um dia.

Para obter informações sobre como visualizar projetos e itens de trabalho no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Exibir o progresso do trabalho real no Balanceador de Carga de Trabalho

Para lhe dar uma perspectiva precisa do progresso da sua carga de trabalho, introduzimos uma nova configuração no Balanceador de Carga de Trabalho que mostra a linha do tempo de tarefas e problemas de acordo com suas Datas Projetadas. Você pode ativar a configuração Mostrar datas projetadas para exibir a linha do tempo projetada do item de trabalho, além da linha do tempo planejada.

Além disso, com essa melhoria, se uma tarefa ou um problema for concluído antes da Data de Conclusão Planejada, as horas alocadas dos dias restantes serão atingidas para indicar que não contam na alocação geral do usuário.

Para obter informações sobre como navegar no Balanceador de Carga de Trabalho e ativar configurações, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Recursos do Balanceador de carga de trabalho previamente comunicados como lançamento com a versão 20.2

* [Ajustar a alocação diária e semanal no Balanceador de carga de trabalho](#adjust-daily-and-weekly-allocation-in-the-workload-balancer)
* [Atualizar Horas Planejadas da Tarefa no Balanceador de Carga de Trabalho](#update-task-planned-hours-in-the-workload-balancer)
* [Uma maneira mais conveniente de atualizar alocações no Balanceador de Carga de Trabalho](#a-more-convenient-way-to-update-allocations-in-the-workload-balancer)

### Ajustar a alocação diária e semanal no Balanceador de carga de trabalho {#adjust-daily-and-weekly-allocation-in-the-workload-balancer}

Para evitar o esgotamento dos recursos, agora é possível ajustar a alocação diária e semanal dos usuários para funcionar usando o Balanceador de carga de trabalho.

Antes desse aprimoramento, isso só era possível usando as ferramentas de Agendamento de recursos.

Para obter informações sobre o gerenciamento de alocações no Balanceador de Carga de Trabalho, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

### Atualizar Horas Planejadas da Tarefa no Balanceador de Carga de Trabalho {#update-task-planned-hours-in-the-workload-balancer}

>[!NOTE]
>
>Esse aprimoramento estará disponível em Produção logo após a versão 2020.2.

Uma nova opção na área Gerenciamento de Recursos do nível de acesso agora permite que usuários com esse acesso editem Horas Planejadas do Balanceador de Carga de Trabalho. Quando você ajusta alocações no Balanceador de Carga de Trabalho, o total de alocações diárias não precisa corresponder ao número de Horas Planejadas das tarefas. Depois de salvar suas alocações, o total de horas de alocação se tornará o Horário Planejado da tarefa. Isso só é possível para tarefas com um Tipo de duração simples.

Para obter informações sobre o gerenciamento de alocações no Balanceador de Carga de Trabalho, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Para obter informações sobre a concessão de acesso ao Gerenciamento de Recursos, consulte [Conceder acesso ao gerenciamento de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

### Uma maneira mais conveniente de atualizar alocações no Balanceador de Carga de Trabalho {#a-more-convenient-way-to-update-allocations-in-the-workload-balancer}

Para tornar mais conveniente gerenciar as alocações de um usuário para um item de trabalho no Balanceador de Carga de Trabalho, agora é possível clicar duas vezes no item de trabalho. Também é possível usar a opção de menu Editar alocações existente. Além disso, não é mais necessário ativar a exibição de alocações para atualizá-las.

Para obter informações sobre o gerenciamento de alocações no Balanceador de Carga de Trabalho, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).
