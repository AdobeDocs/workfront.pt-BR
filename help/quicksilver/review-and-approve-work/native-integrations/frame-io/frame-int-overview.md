---
product-area: documents
navigation-topic: approvals
title: Visão geral da integração do Frame.io
description: Visão geral da integração do Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Visão geral da integração do Frame.io

A integração do Workfront e do Frame.io permite que os coordenadores de projetos gerenciem projetos e planejem o trabalho no Workfront, enquanto os criadores, profissionais de marketing e participantes podem revisar e aprovar ativos no Frame.io.

## Baseado no gerenciamento de armazenamento corporativo da Adobe

No centro dessa integração está o Adobe Enterprise Storage Management (ESM) — uma solução de armazenamento em nuvem que serve como repositório central para ativos em produtos corporativos da Adobe, incluindo Workfront e Frame.io.

Os principais benefícios do gerenciamento de armazenamento corporativo da Adobe incluem:

* Camada de armazenamento unificado para ativos criativos e de gerenciamento de trabalho
* Permissões centralizadas via Adobe IMS para controle de acesso seguro
* Visibilidade completa de ativos nos aplicativos Workfront, Frame.io e Creative Cloud <!--coming soon?-->
* Gerenciamento dimensionável de armazenamento e cotas para as necessidades corporativas

Para obter mais detalhes, consulte [visão geral do Adobe Enterprise Storage Management](help/quicksilver/review-and-approve-work/esm-overview.md).

## Revisão e aprovação unificadas

A integração Workfront e Frame.io usa a funcionalidade de aprovação unificada da Workfront para gerenciar revisões e aprovações. Com aprovações unificadas, você pode:

* Criar e gerenciar revisões e aprovações diretamente da Workfront
* Rastrear o status de revisões e aprovações em tempo real
* Centralizar feedback e aprovações em um único local
* Garantir que todas as partes interessadas tenham acesso às versões mais recentes dos ativos
* Utilizar Revisores de IA para automatizar revisões de conformidade da marca
* e mais

Para obter mais informações, consulte [Aprovações de documentos unificados: índice do artigo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Usar o visualizador do Frame.io

A integração também se conecta com o visualizador Frame.io. O visualizador Frame.io fornece

* Ferramentas de marcação e comentários
* Histórico e comparação de versões
* Comentários com carimbo de data e hora para análises de vídeo
* Acesso móvel para revisões e aprovações em qualquer lugar

Para obter mais informações, consulte [Introdução à integração do Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Limitações da análise de vídeo

<!--need to confirm these-->

#### Tipos de arquivo compatíveis no visualizador Frame.io

O visualizador Frame.io suporta todos os tipos comuns de vídeo, imagem, áudio, PDF e MS® Office. Para obter uma lista detalhada dos arquivos suportados, consulte [Tipos no Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Acesso e licenciamento para o visualizador Frame.io

O visualizador Frame.io está disponível para todos os usuários do Workfront com uma licença paga. Nenhuma licença adicional do Frame.io é necessária para usar o visualizador do Frame.io para revisões e aprovações com essa integração.

Se a sua organização quiser aproveitar a funcionalidade adicional do Frame.io, como carregar ativos diretamente para projetos no Frame.io, você pode comprar uma licença corporativa do Frame.io. <!--link to Frame.io enterprise license info or who to contacT?-->

A funcionalidade de prova do Workfront não está disponível com essa integração.

## Gerenciamento eficiente de projetos no Workfront

Com a integração do Workfront e do Frame.io, os coordenadores de projetos podem aproveitar os poderosos recursos de gerenciamento de projetos da Workfront para planejar, acompanhar e gerenciar trabalhos.

Para obter mais informações sobre como gerenciar projetos no Workfront, consulte [Projetos: índice do artigo](/help/quicksilver/manage-work/projects/projects-toc.md).

### Convenções de nomenclatura e estrutura impostas

Como essa integração é criada usando o ESM, há algumas convenções de estrutura e nomenclatura aplicadas que devem ser consideradas ao gerenciar projetos e documentos.

* Os nomes dos objetos devem ser exclusivos e não podem ser duplicados
* O ESM requer nomes exclusivos para objetos de mesmo nível com o mesmo pai na árvore hierárquica
* Os documentos não podem ter o mesmo nome se pertencerem ao mesmo projeto

Com essas limitações em mente, o Workfront renomeia automaticamente objetos ou documentos conforme necessário para evitar conflitos.

### Gerenciamento de documentos no Workfront

Os documentos são gerenciados no nível do projeto com essa integração e não podem ser carregados para tarefas ou problemas no momento.

O acesso a documentos também é gerenciado no nível do projeto. Se um usuário tiver acesso a um projeto, ele poderá acessar todos os documentos associados a esse projeto.

<!--Documents can't be dragged as full folders.-->

### Limitações da experiência de documento

Como essa integração é criada usando o ESM, há algumas limitações para a experiência do documento original no Workfront:

#### Limitações

Os seguintes recursos não serão incluídos nesta integração:

* Provedores de documentos externos
* Acesso à prova
* Visualizador de documentos no Workfront


#### Limitações temporários

Por enquanto, os seguintes recursos não estão disponíveis:

* Documentos favoritos
* Solicitar documentos
* Enviar documentos para o Adobe Experience Manager Assets
* Aprovações em vários estágios
* Fazer upload de documentos para comentários ou atualizações no Workfront
* Faça upload de documentos para tarefas ou problemas no Workfront



