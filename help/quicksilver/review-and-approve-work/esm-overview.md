---
product-area: documents
navigation-topic: approvals
title: Visão geral do armazenamento em nuvem do Adobe
description: Visão geral do armazenamento em nuvem do Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# Visão geral do armazenamento em nuvem do Adobe

O Adobe Cloud Storage é uma solução de armazenamento em nuvem que serve como repositório central para ativos em produtos corporativos da Adobe. A integração do Workfront e do Frame.io é criada no armazenamento em nuvem do Adobe, permitindo colaboração e gerenciamento de ativos ininterruptos entre essas plataformas.

Essa opção de armazenamento também prepara o caminho para futuras integrações de gerenciamento de ativos com outros produtos da Adobe, como o Adobe Creative Cloud.

## Recursos principais

* **Camada de armazenamento unificado**: o armazenamento em nuvem do Adobe atua como um back-end de armazenamento compartilhado para Workfront, Frame.io, Document Cloud e Creative Cloud. Isso permite colaboração e gerenciamento de ativos ininterruptos nessas plataformas.

* **Habilitação de supply chain de conteúdo**: o armazenamento em nuvem do Adobe é um componente fundamental para a visão de Supply chain de conteúdo da Adobe, permitindo que as equipes gerenciem ativos em andamento sem a necessidade de downloads manuais ou reupload em vários aplicativos da Adobe.

* **Permissões e acesso centralizados**: o armazenamento em nuvem da Adobe oferece suporte a controles de acesso de nível empresarial, integrando-se ao Adobe IMS (Identity Management System) para obter permissões de usuário seguras e escaláveis.

* **Visibilidade completa de ativos**: o Assets armazenado no armazenamento em nuvem da Adobe pode ser exibido e gerenciado diretamente nos aplicativos Workfront, Frame.io e Creative Cloud, fornecendo metadados consistentes, controle de versão e trilhas de auditoria.

* **Integração com fluxos de trabalho de revisão e aprovação**: o armazenamento na nuvem do Adobe habilita fluxos de trabalho de revisão e aprovação criativos, servindo como fonte da verdade para todos os ativos, garantindo que os comentários e as aprovações sejam rastreados centralmente.

* **Gerenciamento de cotas e armazenamento escalável**: o armazenamento em nuvem da Adobe oferece opções de armazenamento escalável e rastreamento unificado de cotas em todos os produtos da Adobe.

## Integração com workflows de revisão e aprovação

A integração do Workfront e do Frame.io aproveita o armazenamento em nuvem do Adobe para fornecer uma experiência unificada de revisão e aprovação. Essa integração permite que os coordenadores de projetos gerenciem projetos e planejem o trabalho no Workfront, enquanto os criadores, profissionais de marketing e participantes podem revisar e aprovar ativos no Frame.io. Isso garante que todas as partes interessadas tenham acesso às versões mais recentes dos ativos e que o feedback seja centralizado em um único local.

Para obter mais informações sobre a integração do Workfront e do Frame.io, consulte [Visão geral da revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Diferenças entre o armazenamento em nuvem do Adobe e o armazenamento Workfront herdado

Os ambientes Workfront existentes têm uma combinação de armazenamento em nuvem Adobe e armazenamento Workfront herdado. Todos os objetos criados antes do lançamento do Adobe Cloud Storage usam o armazenamento Workfront herdado.

Depois de habilitar o armazenamento em nuvem do Adobe em seu ambiente, você pode criar projetos de armazenamento em nuvem do Adobe e projetos de armazenamento herdados do Workfront.

>[!NOTE]
>
>Os novos ambientes de rede têm o armazenamento em nuvem do Adobe habilitado por padrão e não têm a opção de usar o armazenamento Workfront herdado.


### Documentos

#### Nova área Documentos

A nova área Documentos é uma área de documentos unificada reprojetada para o armazenamento em nuvem do Adobe.

Essa interface atualizada simplifica a navegação, melhora a clareza e facilita o gerenciamento de revisões e aprovações por parte das equipes em um ambiente unificado. Para obter mais informações, consulte a [Visão geral da área Documentos](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Novo modelo de permissão de documento

>[!IMPORTANT]
>
>No Adobe Cloud Storage, as permissões de documento funcionam de forma diferente do armazenamento herdado do Workfront. Os documentos herdam permissões do projeto, tarefa ou problema ao qual estão vinculados.

Os documentos não podem ser compartilhados individualmente. Em vez disso, o sistema gera automaticamente uma pasta para cada tarefa ou problema e herda permissões da tarefa ou problema. Qualquer documento carregado na tarefa ou problema é armazenado nessa pasta gerada.

Para obter mais informações sobre o novo modelo de permissão de documento, consulte [Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Objetos vinculados em pastas

No nível do projeto, as pastas geradas pelo sistema exibem um objeto vinculado. A pasta é automaticamente nomeada da mesma forma que a tarefa ou problema ao qual pertence. As pastas vinculadas mostram como o sistema sabe em qual tarefa ou problema a pasta deve ser visualizada.

Para obter mais informações, consulte [Como funcionam as permissões de documento](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Objetos do Workfront

A tabela abaixo compara os recursos do armazenamento na nuvem do Adobe e do armazenamento herdado do Workfront para objetos do Workfront.

Os objetos do Workfront incluem portfólios, programas, projetos, modelos, tarefas e problemas.

| armazenamento em nuvem Adobe | Armazenamento herdado do Workfront |
|---|---|
| <ul><li>Usa o armazenamento em nuvem do Adobe</li><li>Integrado ao Frame.io</li><li>Usa a nova experiência Documentos</li><li>Impõe convenções de nomenclatura estritas</li><li>O compartilhamento direto de documentos não está disponível</li><li>Os documentos estão disponíveis em outros produtos da Adobe, como Frame.io e Creative Cloud</li></ul> | <ul><li>Usa o armazenamento do Workfront</li><li>Usa o visualizador de provas</li><li>Oferece suporte ao compartilhamento de documentos individuais</li></ul> |

### Mover, copiar e converter objetos

Você pode mover, copiar e converter objetos Workfront entre modelos de armazenamento semelhantes. Por exemplo, você pode mover uma tarefa de um projeto do Adobe Cloud Storage para outro projeto do Adobe Cloud Storage. Não é possível mover uma tarefa de um projeto do Adobe Cloud Storage para um projeto do Workfront Storage herdado.

Essas ações estão disponíveis no menu Mais em uma tarefa ou problema. Cada ação respeita a integridade do documento, a herança de permissões e as regras de armazenamento na nuvem do Adobe.

## Habilitar o armazenamento em nuvem do Adobe

Você deve ter uma versão do Workfront compatível com o armazenamento em nuvem da Adobe. Se sua organização ainda não tiver uma versão compatível, entre em contato com o representante de conta da Adobe.

Para obter informações sobre como habilitar o armazenamento em nuvem do Adobe em seu ambiente, consulte [Habilitar o armazenamento em nuvem do Adobe para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Os novos clientes têm o Adobe Cloud Storage habilitado por padrão e não têm a opção de usar o armazenamento Workfront herdado.



## Armazenamento em nuvem do Adobe em ambientes de sandbox

O armazenamento na nuvem do Adobe está disponível em ambientes de sandbox [!DNL Workfront] para que você possa testá-lo antes de habilitá-lo na produção. No entanto, o visualizador Frame.io não está disponível na sandbox, portanto, a experiência de revisão e aprovação unificada completa deve ser validada na produção.

Se você tiver uma sandbox de atualização personalizada, atualize-a depois de atualizar para uma versão do Workfront compatível com o Adobe Cloud Storage para acessar a funcionalidade de armazenamento em nuvem da Adobe na sandbox. Para obter mais informações, consulte [O [!DNL Adobe Workfront] ambiente de Sandbox de Atualização Personalizada](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

## Considerações

* É possível que o Workfront fique fora de sincronia com o Frame.io ou o Creative Cloud, como um ativo que está sendo excluído no Workfront, mas que ainda aparece no Frame.io, entre em contato com o suporte da Workfront para ressincronizar o ambiente.


