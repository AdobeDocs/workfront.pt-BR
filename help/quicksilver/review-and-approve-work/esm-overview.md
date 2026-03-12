---
product-area: documents
navigation-topic: approvals
title: Visão geral do armazenamento corporativo da Adobe
description: Visão geral do armazenamento corporativo da Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: 97c351ca38a8b6075634b2f755f2330562bc8b52
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 1%

---

# Visão geral do armazenamento corporativo da Adobe

O armazenamento corporativo da Adobe é uma solução de armazenamento em nuvem que serve como repositório central para ativos em produtos corporativos da Adobe. A integração do Workfront com o Frame.io é baseada no armazenamento corporativo da Adobe, permitindo colaboração e gerenciamento de ativos ininterruptos entre essas plataformas.

Essa opção de armazenamento também prepara o caminho para futuras integrações de gerenciamento de ativos com outros produtos da Adobe, como o Adobe Creative Cloud.

## Recursos principais

* **Camada de armazenamento unificado**: o armazenamento corporativo da Adobe atua como um back-end de armazenamento compartilhado para Workfront, Frame.io, Document Cloud e Creative Cloud. Isso permite colaboração e gerenciamento de ativos ininterruptos nessas plataformas.

* **Habilitação de supply chain de conteúdo**: o armazenamento corporativo do Adobe é um componente fundamental para a visão de Supply chain de conteúdo da Adobe, permitindo que as equipes gerenciem ativos em andamento sem a necessidade de downloads manuais ou reupload em vários aplicativos da Adobe.

* **Permissões e acesso centralizados**: o armazenamento corporativo da Adobe oferece suporte a controles de acesso de nível empresarial, integrando-se ao Adobe IMS (Identity Management System) para obter permissões de usuário seguras e escalonáveis.

* **Visibilidade completa de ativos**: o Assets armazenado no Adobe Enterprise Storage pode ser exibido e gerenciado diretamente nos aplicativos Workfront, Frame.io e Creative Cloud, fornecendo metadados, controle de versão e trilhas de auditoria consistentes.

* **Integração com fluxos de trabalho de revisão e aprovação**: o armazenamento corporativo da Adobe habilita fluxos de trabalho de revisão e aprovação criativos, servindo como fonte da verdade para todos os ativos, garantindo que os comentários e as aprovações sejam rastreados centralmente.

* **Gerenciamento de cotas e armazenamento escalável**: o armazenamento corporativo da Adobe oferece opções de armazenamento escalável e rastreamento unificado de cotas em todos os produtos da Adobe.

## Integração com workflows de revisão e aprovação

A integração do Workfront com o Frame.io aproveita o armazenamento corporativo da Adobe para fornecer uma experiência unificada de análise e aprovação. Essa integração permite que os coordenadores de projetos gerenciem projetos e planejem o trabalho no Workfront, enquanto os criadores, profissionais de marketing e participantes podem revisar e aprovar ativos no Frame.io. Isso garante que todas as partes interessadas tenham acesso às versões mais recentes dos ativos e que o feedback seja centralizado em um único local.

Para obter mais informações sobre a integração do Workfront e do Frame.io, consulte [Visão geral da integração do Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).

## Diferenças entre o armazenamento corporativo Adobe e o armazenamento Workfront herdado

Os ambientes Workfront existentes têm uma combinação de armazenamento corporativo Adobe e armazenamento Workfront herdado. Qualquer objeto criado antes do lançamento do armazenamento corporativo Adobe usa o armazenamento Workfront herdado.

Depois de habilitar o armazenamento corporativo da Adobe em seu ambiente, você pode criar projetos de armazenamento corporativo da Adobe e projetos de armazenamento herdados da Workfront.

>[!NOTE]
>
>Os novos ambientes de rede têm o armazenamento corporativo Adobe habilitado por padrão e não têm a opção de usar o armazenamento Workfront herdado.


### Documentos

#### Nova área de documentos

A nova área de documentos é uma área de documentos unificada reprojetada para armazenamento corporativo Adobe.

Essa interface atualizada simplifica a navegação, melhora a clareza e facilita o gerenciamento de revisões e aprovações por parte das equipes em um ambiente unificado. Para obter mais informações, consulte a [Visão geral da área Documentos](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Novo modelo de permissão de documento

>[!IMPORTANT]
>
>No Adobe Enterprise Storage, as permissões de documento funcionam de forma diferente do armazenamento Workfront herdado. Os documentos herdam permissões do projeto, tarefa ou problema ao qual estão vinculados.

Os documentos não podem ser compartilhados individualmente. Em vez disso, o sistema gera automaticamente uma pasta para cada tarefa ou problema e herda permissões da tarefa ou problema. Qualquer documento carregado na tarefa ou problema é armazenado nessa pasta gerada.

Para obter mais informações sobre o novo modelo de permissão de documento, consulte [Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento corporativo do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Objetos vinculados em pastas

No nível do projeto, as pastas geradas pelo sistema exibem um objeto vinculado. A pasta é automaticamente nomeada da mesma forma que a tarefa ou problema ao qual pertence. As pastas vinculadas mostram como o sistema sabe em qual tarefa ou problema a pasta deve ser visualizada.

Para obter mais informações, consulte [Como funcionam as permissões de documento](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Objetos do Workfront

A tabela abaixo compara os recursos do armazenamento corporativo Adobe e do armazenamento Workfront herdado para objetos Workfront.

Os objetos do Workfront incluem portfólios, programas, projetos, modelos, tarefas e problemas.

| armazenamento corporativo Adobe | Armazenamento herdado do Workfront |
|---|---|
| <ul><li>Usa o armazenamento corporativo da Adobe</li><li>Integrado ao Frame.io</li><li>Usa a nova experiência Documentos</li><li>Impõe convenções de nomenclatura estritas</li><li>O compartilhamento direto de documentos não está disponível</li><li>Os documentos estão disponíveis em outros produtos da Adobe, como Frame.io e Creative Cloud</li></ul> | <ul><li>Usa o armazenamento do Workfront</li><li>Usa o visualizador de provas</li><li>Oferece suporte ao compartilhamento de documentos individuais</li></ul> |

### Mover, copiar e converter objetos

Você pode mover, copiar e converter objetos Workfront entre modelos de armazenamento semelhantes. Por exemplo, você pode mover uma tarefa de um projeto de armazenamento corporativo da Adobe para outro projeto de armazenamento corporativo da Adobe. Não é possível mover uma tarefa de um projeto Adobe enterprise storage para um projeto Workfront storage herdado.

Essas ações estão disponíveis no menu Mais em uma tarefa ou problema. Cada ação respeita a integridade do documento, a herança de permissões e as regras de armazenamento corporativo da Adobe.

## Habilitar o armazenamento corporativo da Adobe

Os clientes existentes podem habilitar o armazenamento corporativo da Adobe em seu ambiente após a renovação do contrato. Para obter mais informações sobre como habilitar o Adobe Enterprise Storage, consulte [Habilitar o Adobe Enterprise Storage para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Os novos clientes têm o armazenamento corporativo da Adobe habilitado por padrão e não têm a opção de usar o armazenamento Workfront herdado.






