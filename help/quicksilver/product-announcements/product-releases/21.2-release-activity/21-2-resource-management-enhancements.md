---
content-type: release-notes
keywords: notas,trimestral,atualizar,versão
navigation-topic: 2021-2-release-activity
title: Aprimoramentos no gerenciamento de recursos na 21.2
description: Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 21.2 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte Visão geral da versão 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
TQID: https://experienceleague.adobe.com/cAM0R2azvfhRW25brnRKCUXZ5f2ZLGeBVd19okbdBpU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 575
ht-degree: 3%

---

# Aprimoramentos no gerenciamento de recursos na 21.2

Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 21.2 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 10 de maio de 2021. Para obter uma lista de todas as alterações disponíveis com a versão 21.2, consulte a [Visão geral da versão 21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Visualização em nível de mês no Balanceador de carga de trabalho

Para ajudar você a gerenciar a alocação de recursos por períodos maiores, implementamos uma visualização em nível de mês para o Balanceador de carga de trabalho. É possível exibir até três meses por vez e atualizar alocações mensais de recursos. Antes dessa alteração, você poderia visualizar o Balanceador de carga de trabalho somente por dia ou semana.

Para obter informações, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Conexão entre o Planejador de cenários, o Balanceador de carga de trabalho e a lista de tarefas

>[!NOTE]
>
>Disponível somente na nova experiência do Adobe Workfront.

Para ajudá-lo com o planejamento estratégico de seus projetos e garantir que eles se alinhem às iniciativas de visão geral do Planejador de cenários, criamos uma nova área no projeto que exibe os requisitos de função de trabalho das iniciativas, bem como as horas planejadas estimadas nos itens de trabalho do projeto. Essa área está disponível para o Balanceador de carga de trabalho no nível do projeto, bem como para a lista de tarefas na nova experiência do Workfront. Na experiência clássica, isso está disponível somente para o Balanceador de carga de trabalho do projeto.

Para obter informações, consulte os seguintes artigos:

* [Visão geral da reconciliação de alocações de recursos entre projetos e iniciativas](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navegar no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Essa nova funcionalidade é visível para todos os usuários, tanto na experiência do Workfront nova quanto na clássica. Isso também é visível para clientes que não compraram uma licença do Planejador de cenários do Workfront.

## Use as Horas planejadas ao calcular os Valores líquidos no Planejador de recursos

Uma nova configuração no Planejador de recursos permite que você use as Horas planejadas ao calcular os Valores líquidos.

Antes desse aprimoramento, a Workfront calculava valores líquidos somente usando as horas orçadas. Os valores líquidos exibem a diferença entre Horas disponíveis e Orçadas ou Planejadas, FTE ou custo. As horas orçadas ainda são a configuração padrão ao calcular valores Líquidos.

Para obter informações, consulte [Visão geral de horas, FTE e informações de custo nas exibições de Projeto e Função do Planejador de Recursos](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## Visualização de 12 semanas no Balanceador de carga de trabalho

Agora você pode visualizar até 12 semanas de informações no Balanceador de carga de trabalho. Antes desse aprimoramento, você poderia visualizar 2, 4 e 6 semanas de informações.

Para obter informações sobre como visualizar o Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Navegar pelo Balanceador de carga de trabalho.

## Alteração na forma como o filtro Função de trabalho funciona na área Não atribuído do Balanceador de carga de trabalho

Para melhorar o funcionamento do filtro Função de trabalho no Balanceador de carga de trabalho e corresponder às expectativas dos usuários, modificamos a funcionalidade do filtro na área Não atribuído. Agora você pode exibir somente as horas alocadas para as funções de trabalho especificadas no filtro.

Antes desse aprimoramento, ao aplicar o filtro Função de trabalho à área Não atribuído, o Balanceador de carga de trabalho exibia todas as horas associadas aos itens de trabalho atribuídos às funções de trabalho.

Para obter informações sobre como filtrar informações no Balanceador de carga de trabalho, consulte [Gerenciar filtros no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
