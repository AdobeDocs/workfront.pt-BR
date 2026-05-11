---
product-area: documents
navigation-topic: approvals
title: Atualizar cenários do Workfront Fusion para revisão e aprovação unificadas
description: Inventarie, classifique e corrija cenários do Workfront Fusion criados na revisão herdada do Workfront, à medida que sua organização adota o armazenamento corporativo da Adobe e a revisão e aprovação unificadas.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: 722ba7f6617e3ccc1a1dcbf51f5d539c550617ab
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# Atualizar cenários do Workfront Fusion para revisão e aprovação unificadas

Os cenários do Workfront Fusion criados na revisão herdada do Workfront não funcionam automaticamente em projetos de armazenamento corporativo da Adobe. Módulos específicos de prova, webhooks e endpoints de API têm equivalentes diretos em alguns casos e alterações significativas em outros. Este artigo ajuda você a inventariar os cenários afetados, classificá-los e decidir um caminho de correção antes de trazer equipes que dependem desses cenários para a implantação do armazenamento corporativo da Adobe.

Os cenários com escopo para projetos herdados do Workfront continuam funcionando como atualmente. O trabalho de correção descrito neste artigo aplica-se a cenários que você pretende executar em projetos de armazenamento corporativo da Adobe.

Os conectores de fusão com suporte nativo para revisão e aprovação unificadas devem estar disponíveis no terceiro trimestre de 2026. Planeje a recriação agora, mas recomendamos aguardar os novos conectores antes de criar. Os cenários serão mais simples e confiáveis do que substituirão.

Orientações detalhadas sobre automação serão publicadas juntamente com a versão do conector Fusion do terceiro trimestre de 2026. Use este artigo para inventariar e classificar cenários agora e estar pronto para agir assim que essa orientação estiver disponível.

Para obter um resumo de alto nível sobre o que muda quando sua organização muda para o Workfront no Adobe Enterprise Storage, consulte [Mover para o Workfront no Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).


## O que muda para o Fusion em projetos de armazenamento corporativo da Adobe

Os cenários do Fusion existentes criados no Workfront Proof dependem de módulos específicos de prova, acionadores de webhook e endpoints de API que não fazem parte do modelo de dados de revisão e aprovação unificados. A tabela abaixo mapeia tipos de cenário comuns para o impacto esperado e o caminho a seguir:

| Tipo de cenário | Impacto | Caminho para frente |
|---|---|---|
| Criação e roteamento de prova | Quebras | Recriar usando a API de aprovações unificadas |
| Webhooks de status de prova | Quebras | Recriar com novos acionadores de evento de aprovação |
| Acionadores de upload de documento | Parcial: é necessário testar novamente | Auditoria e teste novamente após a migração |
| Notificações de lembrete de aprovação | Quebras | Substituir pelos prazos finais do modelo de aprovação |
| Encaminhamento de decisão de aprovação | Quebras | Recriar usando novos campos de status de decisão |
| Relatórios de aprovação personalizados | Parcial: os nomes de campo podem mudar | Mapear campos herdados para o novo esquema |


## Classificar cada cenário como Editar, Reconstruir ou Desativar

O trabalho que cada cenário requer depende do que ele faz e do que está disponível na revisão e aprovação unificadas. Use as seguintes classificações:

* **Editar**: a ação relacionada à prova existente tem um equivalente direto na revisão e aprovação unificadas, e você pode atualizar o cenário para usar a nova ação.
* **Recompilar**: as etapas subjacentes foram alteradas significativamente ou há novos recursos que o cenário deve usar, portanto, o cenário precisa ser recompilado do zero.
* **Desativar**: a funcionalidade nativa de revisão e aprovação unificada, como modelos de aprovação de vários estágios com lembretes de prazo, substitui o cenário criado para isso.

Analise cada cenário em relação à sua lógica de negócios específica para decidir sua classificação.

## Abordagem de remediação

Use a seguinte abordagem para planejar e executar a correção do Fusion:

1. **Inventário agora.** Obtenha uma lista completa de cenários ativos do Fusion e marque cada um que faz referência à criação de prova, status da prova, aprovações de documentos ou roteamento de aprovação. Não espere até que o armazenamento corporativo da Adobe esteja habilitado.
1. **Classifique cada cenário** como Editar, Recompilar ou Desativar com base nos critérios da seção anterior.
1. **Pausar cenários dependentes de prova** antes de trazer as equipes que dependem deles para o piloto de armazenamento corporativo da Adobe. A execução de automações obsoletas baseadas em prova no novo modelo pode produzir falhas silenciosas ou ações duplicadas.
1. **Usar modelos de aprovação para substituir a lógica de roteamento simples.** Modelos nativos de aprovação de vários estágios com automação de prazo podem lidar com muitos casos de uso que anteriormente exigiam o Fusion. Para obter mais informações, consulte [Criar um Modelo de Aprovação para ativos e documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Aguarde as atualizações do conector Fusion Q3 2026 antes de recompilar.** Os conectores atualizados expõem módulos criados especificamente para revisão e aprovação unificadas e tornam as reconstruções significativamente mais simples e confiáveis. Não recomendamos a recriação com antecedência em relação à API do Workfront versão 22. Se você continuar com um cenário crítico em termos de tempo, planeje revisitar esse trabalho depois que os novos conectores forem lançados.
1. **Teste os cenários recriados de ponta a ponta em uma instância de sandbox** antes de habilitá-los na produção. Preste atenção especial às cargas de subscrição do evento: os nomes de campo e o esquema são diferentes dos eventos de prova herdados.

>[!TIP]
>
>Muitas organizações acumularam cenários do Fusion que foram soluções alternativas para lacunas na prova de legado. Os recursos nativos de revisão e aprovação unificados — incluindo modelos de aprovação, lembretes de prazo e roteamento de vários estágios — eliminam completamente a necessidade de alguns desses cenários. Conforme você classifica cada cenário, avalie se um recurso nativo pode substituí-lo. Aposentar um cenário geralmente é um resultado de longo prazo mais limpo do que reconstruí-lo.

## Artigos relacionados

* [Migrar para o Workfront no armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [Visão geral unificada de revisão e aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Criar um modelo de aprovação para ativos e documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
