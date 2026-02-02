---
product-area: documents
navigation-topic: approvals
title: Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento corporativo da Adobe
description: Visão geral das permissões e do acesso do armazenamento corporativo da Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento corporativo da Adobe

<!--linked in UI -->

O armazenamento corporativo da Adobe é uma solução de armazenamento baseada em nuvem que serve como repositório de armazenamento central para ativos em produtos corporativos da Adobe. Os ambientes Workfront que usam o armazenamento corporativo Adobe têm permissões de objeto e comportamentos de nível de acesso ligeiramente diferentes daqueles que usam o armazenamento de documentos Workfront herdado.

## Níveis de acesso

Os níveis de acesso do Workfront se aplicam somente no Workfront. As restrições de projeto e documento no Workfront nem sempre se aplicam a outros aplicativos da Adobe.

### Ambientes que usam armazenamento corporativo Adobe e armazenamento Workfront herdado

O acesso a documentos se comporta de forma diferente se o projeto estiver no armazenamento corporativo da Adobe ou no armazenamento Workfront herdado:

* **Armazenamento herdado do Workfront**: projetos, programas, portfólios e modelos que usam o armazenamento herdado do Workfront seguem a lógica padrão de nível de acesso do Workfront para acesso a documentos. Quando um nível de acesso tem **Nenhum acesso** selecionado para documentos, eles não podem ver documentos no Workfront ou em outros produtos da Adobe, como Frame.io ou Creative Cloud.
* **Adobe enterprise storage**: projetos, programas, portfólios e modelos que usam o Adobe enterprise storage seguem a lógica de nível de acesso ao armazenamento corporativo da Adobe para outros produtos Adobe.


   * **Permissões de objeto de projetos, programas, portfólios e modelos**: quando um nível de acesso tem **Nenhum acesso** selecionado para projetos, programas, portfólios e modelos, mas o objeto é compartilhado com eles, os usuários não podem ver o objeto no Workfront, mas ainda podem exibir o nome do objeto e quaisquer documentos associados em outras ferramentas do Adobe, como Frame.io e Adobe Creative Cloud.
   * **Permissões de documentos**: quando um nível de acesso tem **Nenhum acesso** selecionado para documentos, os usuários não podem ver documentos em projetos no Workfront, mas ainda podem exibir e gerenciar documentos de projetos compartilhados com eles em outras ferramentas do Adobe, como Frame.io e Adobe Creative Cloud. Isso ocorre porque o acesso a documentos é determinado por permissões no nível do projeto no armazenamento corporativo da Adobe, em vez de somente pelos níveis de acesso da Workfront.

Se você tiver o armazenamento corporativo da Adobe habilitado em seu ambiente Workfront, poderá criar projetos de armazenamento corporativo da Adobe e projetos de armazenamento herdados da Workfront. Os projetos de armazenamento herdados do Workfront mostram um ícone ao lado do nome do projeto em toda a Workfront. Os projetos de armazenamento corporativo da Adobe não mostram um ícone.

![ícone de armazenamento herdado do workfront ao lado do nome do projeto](assets/legacy-project-icon.png)


### Ambientes que usam somente o armazenamento corporativo Adobe

Não é possível modificar permissões de documentos no nível de acesso para projetos, programas e portfólios que usam o Adobe Enterprise Storage.

Todos os níveis de acesso têm acesso de edição aos documentos. As permissões no nível do projeto determinam o acesso aos documentos em outras ferramentas do Adobe.

Não é possível restringir o acesso à herança de documentos.


### Ambientes que usam somente o armazenamento Workfront herdado

Nenhuma alteração nos níveis de acesso ou comportamento do documento.


## Projetos

Os usuários com permissões no nível do projeto podem visualizar e gerenciar documentos de projetos em outros produtos da Adobe, como Frame.io e Adobe Creative Cloud.

Os nomes dos projetos também são visíveis fora do Workfront para projetos ESM.

Os dados financeiros não estão visíveis fora do Workfront para projetos ESM.

## Tarefas e problemas

Os documentos são armazenados no nível do projeto, mas podem ser compartilhados com tarefas e problemas individuais, conforme necessário. Os usuários com acesso a tarefas e problemas herdam automaticamente o acesso a documentos do projeto. Você não pode modificar o nível de acesso deles. Eles têm acesso de gerenciamento ou nenhum acesso.