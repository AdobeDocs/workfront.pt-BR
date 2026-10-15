---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Migrar para o Workfront no Adobe Cloud Storage
description: Planeje sua mudança para o Workfront no armazenamento em nuvem da Adobe. Entenda o que acontece quando sua organização está habilitada, o que é diferente em objetos de armazenamento na nuvem do Adobe e como implantá-lo em seu próprio tempo.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---
# Migrar para o Workfront no Adobe Cloud Storage

O Workfront no Adobe Cloud Storage fornece a experiência completa de revisão e aprovação unificada: revisões no visualizador Frame.io, fluxos de trabalho de aprovação avançados, visibilidade entre produtos de ativos e muito mais.

Este artigo é o ponto de partida para administradores do Workfront que migram para o Adobe Cloud Storage. Ele explica o que acontece quando você ativa o armazenamento na nuvem do Adobe, aponta para os detalhes das diferenças e oferece links para os artigos que ajudam a planejar e implantar a alteração.

## Você decide quando o armazenamento em nuvem do Adobe é ativado

Nada será alterado em seu ambiente do Workfront até que um administrador do Workfront habilite o armazenamento na nuvem do Adobe como a opção de armazenamento padrão em **Configuração** > **Sistema** > **Preferências**. Até lá, os projetos existentes e os novos projetos criados permanecerão no armazenamento herdado do Workfront e manterão o serviço de aprovação usado atualmente.

Quando um administrador habilita o armazenamento em nuvem do Adobe como a opção de armazenamento padrão:

* Novos projetos usam o armazenamento em nuvem do Adobe
* Frame.io é o visualizador padrão
* Aprovações unificadas é o serviço de aprovação padrão

Os projetos existentes não são alterados.

Como você controla o tempo, pode testar a experiência, atualizar seus cenários do Workfront Fusion e planejar as alterações de relatório antes que qualquer pessoa trabalhe neles. Para obter instruções passo a passo, consulte [Habilitar o Adobe Cloud Storage para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

## Como as aprovações funcionam no armazenamento em nuvem do Adobe

Os projetos de armazenamento em nuvem do Adobe usam Aprovações unificadas por padrão, com revisão e aprovação no visualizador Frame.io. Os objetos que permanecem no armazenamento herdado do Workfront mantêm qualquer serviço de aprovação que já usem: aprovações de documentos herdadas ou aprovações unificadas.

>[!NOTE]
>
>Definir o Adobe Cloud Storage como padrão não altera o serviço de aprovação que já está em uso nos objetos de armazenamento herdados do Workfront. Aprovações unificadas é o padrão somente para novos objetos criados no armazenamento em nuvem do Adobe.

Antes de implantar o Adobe Cloud Storage, verifique se as pessoas que gerenciam aprovações sabem o que esperar. Para obter mais informações, consulte [Mover de aprovações de documentos herdados para Aprovações unificadas](/help/quicksilver/review-and-approve-work/move-to-unified-approvals.md).

## Planeje sua mudança

Analise esses artigos para preparar:

* [O que há de diferente no armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md): as principais diferenças nos objetos de armazenamento na nuvem do Adobe, desde a nova área Documentos e o visualizador Frame.io até regras de nomenclatura, cota de armazenamento e Fusão.
* [Planeje a implantação do armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md): como escolher uma configuração de implantação, testar com um único grupo e sequenciar o trabalho para que não haja surpresas para seus usuários.
* [Habilitar o armazenamento na nuvem do Adobe para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md): as etapas para definir a opção de armazenamento padrão para toda a organização ou para grupos específicos.
* [Converter objetos herdados para o armazenamento na nuvem do Adobe](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md): os três casos em que você pode converter um objeto herdado para o armazenamento na nuvem do Adobe e o que é movido durante cada conversão.


## Artigos relacionados

* [Visão geral do armazenamento em nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Visão geral unificada de revisão e aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [A área Documentos](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento em nuvem do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)
