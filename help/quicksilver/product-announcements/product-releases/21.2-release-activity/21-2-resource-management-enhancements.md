---
content-type: release-notes
keywords: notas,trimestral,atualização,versão
navigation-topic: 2021-2-release-activity
title: 21.2 Melhorias no gerenciamento de recursos
description: Esta página descreve todas as melhorias no Gerenciamento de recursos realizadas com a versão 21.2 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte Visão geral da versão 21.2.
author: Luke
feature: Product Announcements
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 21.2 Melhorias no gerenciamento de recursos

Esta página descreve todas as melhorias no Gerenciamento de recursos realizadas com a versão 21.2 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte [Visão geral da versão 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Exibição em nível de mês no Balanceador de Carga de Trabalho

Para ajudá-lo a gerenciar a alocação de recursos por períodos maiores, agora implementamos uma visualização no nível do mês para o Balanceador de Carga de Trabalho. É possível exibir até três meses de cada vez e atualizar alocações mensais de recursos. Antes dessa alteração, você podia exibir o Balanceador de Carga de Trabalho somente por dia ou semana.

Para obter mais informações, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Conexão entre o Planejador de Cenário, o Balanceador de Carga de Trabalho e a lista de tarefas

>[!NOTE]
>
>Disponível somente na nova experiência do Adobe Workfront.

Para ajudá-lo com o planejamento estratégico de seus projetos e garantir que eles estejam alinhados com as iniciativas de maior quadro do Planejador de Cenário, criamos uma nova área no projeto que exibe as necessidades de função de cargo das iniciativas, bem como as horas planejadas estimadas nos itens de trabalho do projeto. Essa área está disponível para o Balanceador de carga de trabalho no nível do projeto, bem como para a lista de tarefas na nova experiência do Workfront. Na experiência clássica, isso está disponível somente para o Balanceador de Carga de Trabalho do projeto.

Para obter informações, consulte os seguintes artigos:

* [Visão geral da reconciliação das alocações de recursos entre projetos e iniciativas](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Essa nova funcionalidade é visível para todos os usuários, tanto na experiência nova quanto na experiência clássica do Workfront. Isso também está visível para clientes que não compraram uma licença do Workfront Scenario Planner.

## Usar Horas Planejadas ao calcular valores Líquidos no Planejador de Recursos

Uma nova configuração no Planejador de Recursos permite que você use Horas Planejadas ao calcular Valores Líquidos.

Antes dessa melhoria, o Workfront calculava os valores Líquidos somente usando as Horas Orçadas. Os valores líquidos exibem a diferença entre Horas Disponíveis e Orçamentadas ou Horas Planejadas, FTE ou Custo. Horas Orçadas ainda é a configuração padrão ao calcular valores Líquidos.

Para obter mais informações, consulte [Visão geral de horas, FTE e informações de custo nas exibições Projeto e Função do Planejador de Recursos](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Exibição de 12 semanas no Balanceador de Carga de Trabalho

Agora é possível visualizar até 12 semanas de informações no Balanceador de Carga de Trabalho. Antes desse aprimoramento, você podia visualizar informações de 2,4 e 6 semanas.

Para obter informações sobre como visualizar o Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Navegue pelo Balanceador de Carga de Trabalho.

## Alteração na forma como o filtro Função do trabalho funciona na área Não atribuído do Balanceador de Carga de Trabalho

Para melhorar a forma como o filtro Função do trabalho funciona no Balanceador de carga de trabalho e para corresponder às expectativas dos usuários, modificamos a funcionalidade do filtro na área Não atribuído. Agora é possível exibir apenas as horas alocadas para as funções de job que você especificar no filtro.

Antes dessa melhoria, ao aplicar o filtro Função de trabalho à área Não atribuído , o Balanceador de carga de trabalho exibia todas as horas associadas aos itens de trabalho atribuídos às funções de trabalho .

Para obter informações sobre filtragem no Balanceador de Carga de Trabalho, consulte [Gerenciar filtros no Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
