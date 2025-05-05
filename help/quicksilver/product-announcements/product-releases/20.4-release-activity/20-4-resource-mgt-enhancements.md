---
title: 20.4 Aprimoramentos no gerenciamento de recursos
description: 20.4 Aprimoramentos no gerenciamento de recursos
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# 20.4 Aprimoramentos no gerenciamento de recursos

Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 20.4 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 9 de novembro de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.4, consulte a [visão geral da versão 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Planeje o trabalho usando o esforço do trabalho em vez das horas planejadas

Para oferecer flexibilidade ao planejar um trabalho em seus projetos, introduzimos o novo conceito de Esforço de trabalho para tarefas. Você pode estimar se o Esforço de trabalho de uma tarefa é pequeno, médio ou grande sem estimar manualmente as Horas planejadas da tarefa. Cada nível de esforço é calculado com base em uma porcentagem de tempo das horas típicas por dia, conforme configurado em sua instância.

As seguintes melhorias estão disponíveis com este novo recurso:

* Habilitar esta configuração para projetos e modelos para torná-la disponível para tarefas e tarefas de modelo
* Atualizar esta configuração para cada tarefa com um Tipo de Duração Simples que atualiza automaticamente as Horas Planejadas da tarefa
* Desabilite esta configuração usando um Modelo de layout para usuários que preferem continuar usando as Horas planejadas.
* Exibir o valor deste novo campo em uma lista de tarefas ou relatório.

Para obter informações sobre Esforço de trabalho, consulte [Visão geral do Esforço de trabalho](../../../manage-work/tasks/task-information/work-effort.md).

Este recurso agora está incluído no [Fundamentos do planejador, Parte 2 do caminho de aprendizado](https://experienceleague.adobe.com/pt-br/docs/workfront/using/home) no Workfront One.

## Cores baseadas no status do projeto para itens de trabalho no Balanceador de carga de trabalho

Para melhor visibilidade e maior personalização de sua experiência no Balanceador de carga de trabalho, agora é possível alterar as cores dos projetos e seus itens de trabalho para corresponder ao status dos projetos. As cores correspondem aos status de projeto de nível de grupo ou de sistema. As cores exibidas podem corresponder aos status do sistema e do projeto personalizado.

Para obter informações sobre como personalizar a exibição no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ajustar a alocação de usuários usando valores percentuais no Balanceador de carga de trabalho

Agora é possível gerenciar as alocações dos usuários no Balanceador de carga de trabalho usando porcentagens em vez de horas.

Para obter informações sobre como gerenciar alocações no Balanceador de carga de trabalho, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Mostrar ou ocultar o trabalho concluído no Balanceador de carga de trabalho

Uma nova configuração agora permite mostrar ou ocultar itens de trabalho concluídos no Balanceador de carga de trabalho. A configuração é ativada por padrão e itens de trabalho concluídos que correspondem aos critérios de filtragem e ao período selecionado são exibidos no Balanceador de carga de trabalho.

Antes dessa melhoria, os itens de trabalho concluídos sempre eram exibidos no Balanceador de carga de trabalho.

Para obter mais informações sobre como ajustar configurações no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Melhorias de usabilidade no Balanceador de carga de trabalho

Para garantir uma experiência simplificada e amigável ao gerenciar os recursos no Balanceador de carga de trabalho, as seguintes melhorias de usabilidade estão disponíveis:

* Agora você pode abrir o Resumo de problemas e tarefas no ícone Resumo em vez do menu Mais. Essa experiência agora é consistente com a de listas.

  >[!NOTE]
  >
  >Essa opção está disponível somente na nova experiência do Adobe Workfront.

* Você pode acessar o menu Mais à esquerda de uma barra de objetos em vez de no final de uma barra de objetos. Isso facilita a localização quando os objetos abrangem um longo período de tempo.
* Você pode acessar os recursos de atribuição com um atalho de teclado. Anteriormente, isso estava disponível somente no menu Mais.
* Você pode carregar todos os itens restantes com o nome de um usuário em vez de apenas os 20 itens a seguir clicando em Carregar mais.

Para obter mais informações sobre como navegar no Balanceador de carga de trabalho, consulte [Navegar no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Gráfico de alocação de usuários no Balanceador de carga de trabalho

Para permitir que você tenha uma representação visual de alto nível da alocação de usuários em um determinado período, uma nova configuração agora permite uma visualização de gráfico de como as alocações são exibidas no Balanceador de carga de trabalho. Ativar essa configuração exibe a alocação dos usuários em um gráfico de linhas que indica as superalocações em blocos vermelhos e as subalocações em azul.

Para obter mais informações sobre como definir configurações no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualizar trabalho concluído no Balanceador de carga de trabalho

Para permitir que você identifique facilmente o trabalho que já foi concluído e gerencie as atribuições de usuário corretamente, ativamos um indicador visual no Balanceador de carga de trabalho que mostra quando os itens de um período selecionado foram concluídos. Agora você pode ver uma marca de seleção verde para tarefas, problemas quando são concluídas. O projeto também exibe a marca de seleção verde quando há itens de trabalho concluídos durante o período exibido na tela.

Para obter informações sobre como exibir informações no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Novo filtro padrão para a área Trabalho atribuído no Balanceador de carga de trabalho

O filtro Padrão da área Trabalho atribuído no Balanceador de carga de trabalho agora exibe somente os usuários que são membros de todas as equipes às quais você, como usuário conectado, está associado. O novo filtro agora exibe as informações mais relevantes para você, por padrão.

Antes dessa melhoria, todos os usuários que você tinha acesso para visualizar eram exibidos nessa área.

Para obter informações sobre como usar filtros no Balanceador de carga de trabalho, consulte [Gerenciar filtros no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Novo ícone para alternar entre horas e valores percentuais ou tempo alocado e restante no Balanceador de carga de trabalho

Adicionamos uma nova configuração que permite alternar entre Horas e Porcentagens alocadas à medida que você visualiza o Balanceador de carga de trabalho. Com esse novo ícone, também eliminamos a seção Carga de trabalho do usuário no painel Configurações. O Balanceador de carga de trabalho mostra o tempo alocado por padrão e movemos a configuração Horas restantes para o novo ícone Porcentagem ou Horas.

Essa melhoria elimina cliques e torna a navegação no Balanceador de carga de trabalho mais fácil e eficiente.

Para obter informações sobre como gerenciar configurações para o Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Um novo filtro integrado para o Balanceador de carga de trabalho: Usuários em projetos

Para tornar sua experiência de filtragem no Balanceador de carga de trabalho mais eficiente, adicionamos um novo filtro incorporado na área Trabalho atribuído. Agora é possível aplicar o filtro Usuários em projetos, que exibe os usuários atribuídos a tarefas e problemas nos projetos especificados.

Para obter informações sobre como usar filtros no Balanceador de carga de trabalho, consulte [Informações de filtro no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

