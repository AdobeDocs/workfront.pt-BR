---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: A área Documentos
description: Na área Documentos, é possível organizar, gerenciar e exibir metadados de documentos carregados no Adobe Workfront. Você também pode ver a decisão da prova.
author: Courtney
feature: Digital Content and Documents
exl-id: 64612345-d1ce-41db-939b-3af30d1c6a51
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: ed7944fe4934ac5ab52b1eed3e144309de9781c4
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 1%

---

# A área Documentos

Na área Documentos, é possível organizar, gerenciar e exibir metadados de documentos carregados no Adobe Workfront. Você também pode ver a decisão da prova.

Atualmente, o Workfront tem duas versões da área Documentos: a área documentos herdados e a nova área documentos. A versão usada por sua organização depende do armazenamento Workfront herdado ou do armazenamento corporativo. Para obter mais informações sobre esses tipos de armazenamento, consulte [visão geral do armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Área de documentos herdados

Há dois tipos de áreas de Documentos. Os recursos e as funcionalidades são os mesmos para:

* **Área de documentos em um programa, portfólio, projeto, tarefa ou problema:** Lista todos os documentos aos quais você tem acesso para um determinado projeto, tarefa ou problema. Para acessar esta área, clique em **Documentos** ![Ícone de documentos](assets/document-icon-12x14.png) no painel esquerdo ao exibir um projeto, tarefa ou problema.

* **Área de Documentos Globais:** Lista todos os documentos aos quais você tem acesso no Workfront. Para acessar esta área, clique em **Documentos** ![Ícone Documentos](assets/document-icon.png) no ![Ícone Menu Principal](assets/main-menu-icon.png) do Menu Principal.

Para obter informações sobre como carregar documentos para o Workfront, consulte [Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).


A área de documentos registra uma contagem dos seguintes itens:

* Pastas do Workfront
* Arquivos carregados do sistema de arquivos
* Arquivos adicionados ao Workfront a partir de integrações
* Experience Manager Assets vinculado

### Painel de resumo

Ao selecionar um documento na área de documentos, você pode usar o Resumo à direita para exibir detalhes do documento, gerenciar atualizações e aprovações de documentos, exibir versões do documento e adicionar e editar Forms Personalizado para o documento.

Se a prova estiver configurada para o documento, a seção Detalhes incluirá informações como a data de vencimento da prova e o andamento da prova atual.

Você pode clicar no cabeçalho Detalhes para ir para a área Detalhes do documento completa quando precisar de todas as informações sobre um documento.

![Área de documentos](assets/documents-area-v2-350x199.png)

Para obter informações sobre o Resumo, consulte [Resumo de documentos](../../documents/managing-documents/summary-for-documents.md).

### Decisão da prova

Depois que uma decisão de prova é tomada, ela aparece na lista Documento.

![Decisão de prova na lista de documentos](assets/proof-decision---doc-list-350x168.png)

### Pastas

Em um projeto, tarefa ou problema em que os documentos são carregados, você pode configurar pastas para organizar os documentos. Para obter mais informações, consulte [Criar pastas de documentos](../../documents/organizing-documents/create-documents-folder.md).

Na área Documentos globais, você pode configurar dois tipos de pastas para organizar os documentos aos quais tem acesso:

* **Pastas Inteligentes:** Mostre apenas os documentos que deseja ver. Para obter mais informações, consulte [Criar e Gerenciar Pastas Inteligentes](../../documents/organizing-documents/create-manage-smart-folders.md).

* **Minhas pastas:** organize os documentos da maneira que você desejar. Para obter mais informações, consulte [Criar pastas de documentos](../../documents/organizing-documents/create-documents-folder.md).

### Detalhes do documento expandido

A página Detalhes do documento fornece uma versão mais em escala completa dos Detalhes do documento no Resumo à direita.

## Nova área de documento

A nova área de documentos só estará disponível para o se sua organização estiver em armazenamento corporativo. Para obter mais informações sobre o armazenamento corporativo, consulte [visão geral sobre o armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Usar o painel de resumo

Ao selecionar um documento na área documentos, você pode usar o painel Resumo à direita para exibir detalhes sobre o documento, adicionar e editar formulários personalizados anexados, criar e gerenciar fluxos de trabalho de aprovação, exibir versões do documento e muito mais.

#### Revisar e aprovar com Frame.io

Você pode revisar e aprovar documentos na área de novos documentos usando o visualizador Frame.io.

Para obter mais informações, consulte [Introdução à revisão e aprovação unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Gerenciar versões

Você pode fazer upload de novas versões de um documento na área novos documentos. Ao fazer upload de uma nova versão, a versão anterior é retida e pode ser acessada no painel Resumo. As versões são nomeadas automaticamente com a data e a hora do upload, mas podem ser renomeadas conforme necessário.

Você também pode iniciar um novo fluxo de trabalho de aprovação para uma versão específica de um documento.

#### Exibir histórico do documento

Você pode visualizar o histórico de um documento na área de novos documentos. O histórico inclui os seguintes tipos de informações:

* Quando o documento foi carregado
* Quando novas versões são carregadas
* Quando os fluxos de trabalho de aprovação foram iniciados para o documento
* E muito mais

### Pastas no nível do sistema para permissões de documento

O Workfront cria automaticamente uma pasta no nível do sistema quando o primeiro documento é carregado para uma tarefa ou problema. Essas pastas herdam permissões da tarefa ou do problema e estão visíveis na área de documentos do nível do projeto. Todos os documentos carregados para essa tarefa ou problema são armazenados nessa pasta e herdam permissões dela. Essa é a forma principal como as permissões são gerenciadas para documentos na nova área de documentos. Para obter mais informações, consulte [Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento corporativo do Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Considerações

* A nova área de documentos é otimizada para telas com 1024 pixels de largura ou maiores. Se você tiver uma tela menor, poderá ter problemas ao acessar o painel Resumo.

* A área de documentos globais não está disponível na nova experiência da área de documentos. Você só pode acessar documentos de programas, portfólios, projetos, tarefas ou problemas.
