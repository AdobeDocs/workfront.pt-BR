---
title: 20.4 Melhorias no gerenciamento de recursos
description: 20.4 Melhorias no gerenciamento de recursos
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 0%

---

# 20.4 Melhorias no gerenciamento de recursos

Esta página descreve todos os aprimoramentos do Gerenciamento de recursos feitos com a versão 20.4 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 9 de novembro de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.4, consulte [Visão geral da versão 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Planejar o trabalho usando o esforço de trabalho em vez das horas planejadas

Para lhe dar flexibilidade quando você planeja trabalhar em seus projetos, introduzimos o novo conceito de Esforço do Trabalho para tarefas. Você pode estimar se o Esforço de trabalho para uma tarefa é pequeno, médio ou grande sem estimar manualmente as Horas Planejadas para a tarefa. Cada nível de esforço é calculado com base em uma porcentagem de tempo das horas diárias normais, conforme configurado na sua instância.

As seguintes melhorias estão disponíveis com este novo recurso:

* Ativar esta configuração para projetos e modelos para torná-la disponível para tarefas e tarefas de modelo
* Atualize essa configuração para cada tarefa com um Tipo de duração simples que atualiza automaticamente as Horas planejadas da tarefa
* Desative essa configuração usando um modelo de layout para usuários que preferem continuar usando as Horas planejadas.
* Exibe o valor desse novo campo em uma lista de tarefas ou relatório.

Para obter informações sobre Esforço de Trabalho, consulte [Visão geral do esforço de trabalho](../../../manage-work/tasks/task-information/work-effort.md).

Esse recurso agora está incluído na variável [Fundamentos do Planejador, caminho de aprendizagem da Parte 2](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-20Y0z000000bm79EAA) no Workfront One.

## Cores baseadas no status do projeto para itens de trabalho no Balanceador de Carga de Trabalho

Para melhor visibilidade e maior personalização de sua experiência no Balanceador de Carga de Trabalho, agora você pode alterar as cores dos projetos e seus itens de trabalho para corresponder ao status dos projetos. As cores correspondem aos status do projeto no nível do grupo ou no nível do sistema. As cores exibidas podem corresponder aos status do sistema e do projeto personalizado.

Para obter informações sobre como personalizar a exibição no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajustar a alocação do usuário usando valores de porcentagem no Balanceador de Carga de Trabalho

Agora você pode gerenciar as alocações de seus usuários no Balanceador de Carga de Trabalho usando porcentagens em vez de horas.

Para obter informações sobre o gerenciamento de alocações no Balanceador de Carga de Trabalho, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Mostrar ou ocultar trabalho concluído no Balanceador de Carga de Trabalho

Uma nova configuração agora permite mostrar ou ocultar itens de trabalho concluídos no Balanceador de Carga de Trabalho. A configuração é ativada por padrão e os itens de trabalho concluídos que correspondem aos critérios de filtragem e o período selecionado são exibidos no Balanceador de Carga de Trabalho.

Antes desse aprimoramento, os itens de trabalho concluídos eram sempre exibidos no Balanceador de Carga de Trabalho.

Para obter mais informações sobre como ajustar configurações no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Melhorias de usabilidade no Balanceador de Carga de Trabalho

Para garantir uma experiência simplificada e amigável ao gerenciar seus recursos no Balanceador de carga de trabalho, as seguintes melhorias de usabilidade agora estão disponíveis:

* Agora é possível abrir o Resumo de problemas e tarefas no ícone Resumo em vez do menu Mais . Essa experiência agora é consistente com a de listas.

   >[!NOTE]
   >
   >Essa opção está disponível somente na nova experiência do Adobe Workfront.

* Você pode acessar o menu Mais à esquerda de uma barra de objetos em vez de no final de uma barra de objetos. Isso facilita a localização de objetos que abrangem um longo período de tempo.
* Você pode acessar os recursos de atribuição com um atalho de teclado. Anteriormente, estava disponível somente no menu Mais .
* Você pode carregar todos os itens restantes sob o nome de um usuário em vez de apenas os 20 itens a seguir clicando em Carregar mais.

Para obter mais informações sobre como navegar no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Gráfico de alocação de usuários no Balanceador de Carga de Trabalho

Para permitir que você tenha uma representação visual de alto nível da alocação dos usuários em um determinado período, uma nova configuração agora ativa uma exibição de gráfico de como as alocações são exibidas no Balanceador de Carga de Trabalho. Ativar essa configuração exibe a alocação dos usuários em um gráfico de linha que indica as sobrealocações em blocos vermelhos e as subalocações em azul.

Para obter mais informações sobre como definir configurações no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualizar trabalho concluído no Balanceador de Carga de Trabalho

Para permitir que você identifique facilmente o trabalho que já foi concluído para que possa gerenciar as atribuições do usuário corretamente, ativamos um indicador visual no Balanceador de Carga de Trabalho que mostra quando os itens de um período selecionado foram concluídos. Agora você pode ver uma marca de seleção verde para tarefas, problemas quando elas são concluídas. O projeto também exibe a marca de seleção verde quando houver itens de trabalho concluídos durante o período exibido na tela.

Para obter informações sobre a exibição de informações no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Novo filtro Padrão para a área de Trabalho Atribuída no Balanceador de Carga de Trabalho

O filtro Padrão para a área de Trabalho Atribuído no Balanceador de Carga de Trabalho agora exibe somente os usuários que são membros de todas as equipes às quais você, como usuário conectado, está associado. O novo filtro agora exibe as informações mais relevantes para você, por padrão.

Antes desse aprimoramento, todos os usuários que você tinha acesso para visualizar eram exibidos nessa área.

Para obter informações sobre o uso de filtros no Balanceador de Carga de Trabalho, consulte [Gerenciar filtros no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Novo ícone para alternar entre horas e valores de porcentagem, ou tempo alocado e restante no Balanceador de Carga de Trabalho

Adicionamos uma nova configuração que permite alternar entre Horas e Porcentagens alocadas conforme você exibe o Balanceador de Carga de Trabalho. Com esse novo ícone, também eliminamos a seção Carga de trabalho do usuário no painel Configurações . O Balanceador de Carga de Trabalho mostra o tempo alocado por padrão e movemos a configuração de Horas Restantes para o novo ícone Porcentagem ou Horas.

Essa melhoria elimina os cliques e torna a navegação no balanceador de carga de trabalho mais fácil e eficiente.

Para obter informações sobre como gerenciar configurações para o Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Um novo filtro integrado para o Balanceador de Carga de Trabalho: Usuários em projetos

Para tornar sua experiência de filtragem no Balanceador de carga de trabalho mais eficiente, adicionamos um novo filtro integrado na área de trabalho atribuído. Agora é possível aplicar o filtro Usuários em projetos , que exibe os usuários atribuídos a tarefas e problemas nos projetos que você especificar.

Para obter informações sobre o uso de filtros no Balanceador de Carga de Trabalho, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

