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
source-git-commit: c4e1961092883f523d04adaacd58129a0379783d
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Visão geral da integração do Frame.io

A integração do Workfront e do Frame.io permite que os coordenadores de projetos gerenciem projetos e planejem o trabalho no Workfront, enquanto os criadores, profissionais de marketing e participantes podem revisar e aprovar ativos no Frame.io.

## Baseado em armazenamento corporativo Adobe

No centro dessa integração está o armazenamento corporativo da Adobe — uma solução de armazenamento baseada em nuvem que serve como repositório central para ativos em produtos corporativos da Adobe, incluindo Workfront, Frame.io e Creative Cloud.

Os principais benefícios do armazenamento corporativo da Adobe incluem:

* Camada de armazenamento unificado para ativos criativos e de gerenciamento de trabalho
* Permissões centralizadas via Adobe IMS para controle de acesso seguro
* Visibilidade completa de ativos nos aplicativos Workfront, Frame.io e Creative Cloud <!--coming soon?-->
* Gerenciamento dimensionável de armazenamento e cotas para as necessidades corporativas

Para obter mais detalhes, consulte [visão geral do armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

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

#### Limites de análise de vídeo

Há um limite anual para solicitações de prova de vídeo definido em 10% do total de licenças de usuário pagas da Workfront de uma organização (Standard e Light). Esse limite é aplicado no nível da organização.

Os administradores do Workfront receberão notificações quando o uso atingir 80% e 100% do limite.

Esse limite não se aplica a clientes do Frame.io Enterprise.

#### Tipos de arquivo compatíveis no visualizador Frame.io

O visualizador Frame.io suporta todos os tipos comuns de vídeo, imagem, áudio, PDF e MS® Office. Para obter uma lista detalhada dos arquivos suportados, consulte [Tipos no Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Acesso e licenciamento para o visualizador Frame.io

O visualizador Frame.io está disponível para todos os usuários do Workfront com uma licença paga. Nenhuma licença adicional do Frame.io é necessária para usar o visualizador do Frame.io para revisões e aprovações com essa integração.

Se a sua organização quiser aproveitar a funcionalidade adicional do Frame.io, como carregar ativos diretamente para projetos no Frame.io, você pode comprar uma licença corporativa do Frame.io. Entre em contato com seu representante de conta da Adobe para agendar uma demonstração e explorar os benefícios da solução Frame.io completa.

A funcionalidade de prova do Workfront não está disponível com essa integração.

## Gerenciamento eficiente de projetos no Workfront

Com a integração do Workfront e do Frame.io, os coordenadores de projetos podem aproveitar os poderosos recursos de gerenciamento de projetos da Workfront para planejar, acompanhar e gerenciar trabalhos.

Para obter mais informações sobre como gerenciar projetos no Workfront, consulte [Projetos: índice do artigo](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

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

<!--* External document providers-->
* Acesso à prova
* Visualizador de documentos no Workfront
* Documentos favoritos
* Solicitar documentos


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->



