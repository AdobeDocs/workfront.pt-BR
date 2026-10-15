---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Converter objetos herdados para o armazenamento em nuvem do Adobe
description: Saiba mais sobre os três casos em que você pode converter um objeto de armazenamento herdado do Workfront para o Adobe Cloud Storage e entender o que se move e o que permanece durante cada conversão.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---
# Converter objetos herdados para o armazenamento em nuvem do Adobe

Na maioria dos cenários, você pode mover, copiar e converter objetos Workfront somente entre modelos de armazenamento semelhantes. Por exemplo, você pode mover uma tarefa de um projeto de armazenamento em nuvem do Adobe para outro projeto de armazenamento em nuvem do Adobe. Em três casos específicos, você pode converter um objeto de armazenamento herdado do Workfront no armazenamento em nuvem do Adobe:

* Converter uma tarefa herdada do Workfront Storage em um projeto do Adobe Cloud Storage
* Converter um portfólio de armazenamento herdado do Workfront em um portfólio de armazenamento em nuvem do Adobe
* Criar um projeto do Adobe Cloud Storage a partir de um modelo herdado do Workfront Storage

Para obter uma orientação sobre a movimentação e as diferenças no armazenamento em nuvem do Adobe, consulte [Mover para o Workfront no armazenamento em nuvem do Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## Converter uma tarefa herdada em um projeto de armazenamento na nuvem do Adobe

Para converter uma tarefa herdada de armazenamento do Workfront em um projeto de armazenamento na nuvem do Adobe, use o fluxo de conversão para projeto existente na tarefa. Durante a conversão:

* Subtarefas e problemas são movidos para o novo projeto.
* Os documentos anexados à tarefa e seus fluxos de trabalho de aprovação permanecem no projeto original.
* As aprovações de trabalho e a resolução de links de objetos são removidas.
* A tarefa original é excluída.

## Converter um portfólio herdado em um portfólio de armazenamento em nuvem da Adobe

Um administrador do Workfront pode converter um portfólio de armazenamento herdado do Workfront em um portfólio de armazenamento em nuvem do Adobe na área Configuração. Após a conversão:

* Não é mais possível mover projetos de armazenamento herdados do Workfront para o portfólio.
* Todos os novos projetos criados no portfólio usam o Adobe Cloud Storage.
* O Frame.io é o visualizador de documentos nos projetos de armazenamento em nuvem do Adobe do portfólio.
* Os projetos secundários que usam o armazenamento Workfront herdado permanecem no armazenamento herdado.
* Os programas secundários permanecem no armazenamento herdado.

>[!NOTE]
>
>Um programa herdado secundário converte automaticamente para o Adobe Cloud Storage somente quando alguém adiciona manualmente um projeto do Adobe Cloud Storage a ele.

Para obter mais informações, consulte [Converter portfólios herdados para o armazenamento na nuvem da Adobe](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md).

## Criar um projeto do Adobe Cloud Storage a partir de um modelo herdado

Ao criar um projeto a partir de um modelo de armazenamento herdado do Workfront, a caixa de seleção **Criar este projeto no Adobe Cloud Storage** da caixa de diálogo de criação do projeto determina o tipo de armazenamento do novo projeto. O comportamento da caixa de seleção depende de onde você cria o projeto:

* **Fora de um portfólio**: a caixa de seleção está disponível e desmarcada por padrão. Selecione-a para criar o novo projeto no Adobe Cloud Storage.
* **Em um portfólio de armazenamento na nuvem da Adobe**: a caixa de seleção está marcada e bloqueada. O novo projeto deve corresponder ao tipo de armazenamento do portfólio.
* **Em um portfólio de armazenamento herdado do Workfront**: a caixa de seleção não está disponível. O novo projeto usa o armazenamento Workfront herdado.

Para obter mais informações, consulte [Criar projetos](/help/quicksilver/manage-work/projects/create-projects/create-project.md).
