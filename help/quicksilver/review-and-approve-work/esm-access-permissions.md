---
product-area: documents
navigation-topic: approvals
title: Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento em nuvem do Adobe
description: Permissões de armazenamento na nuvem e visão geral de acesso do Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 758d17e6-f31f-42b7-a9e6-6bd1821f5c15
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7fc5fe2f2692841a8663740441f70be0c82c4073
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 1%

---

# Visão geral das permissões de objeto e do nível de acesso para o modelo de armazenamento em nuvem do Adobe

<!--linked in UI -->

O armazenamento em nuvem da Adobe é uma solução de armazenamento baseada em nuvem que serve como repositório de armazenamento central para ativos em produtos corporativos da Adobe. Os ambientes do Workfront que usam o Adobe Cloud Storage têm permissões de objeto e comportamentos de nível de acesso ligeiramente diferentes daqueles que usam o armazenamento de documentos herdado do Workfront.

## Níveis de acesso

Os níveis de acesso do Workfront se aplicam somente no Workfront. As restrições de projeto e documento no Workfront nem sempre se aplicam a outros aplicativos da Adobe.

### Ambientes que usam o armazenamento em nuvem do Adobe e o armazenamento herdado do Workfront

O acesso a documentos se comporta de forma diferente dependendo se o projeto está no Adobe Cloud Storage ou no Workfront Storage herdado:

* **Armazenamento herdado do Workfront**: projetos, programas, portfólios e modelos que usam o armazenamento herdado do Workfront seguem a lógica padrão de nível de acesso do Workfront para acesso a documentos. Quando um nível de acesso tem **Nenhum acesso** selecionado para documentos, eles não podem ver documentos no Workfront ou em outros produtos da Adobe, como Frame.io ou Creative Cloud.
* **Adobe Cloud Storage**: projetos, programas, portfólios e modelos que usam o Adobe Cloud Storage seguem a lógica de nível de acesso do Adobe Cloud Storage para outros produtos da Adobe.


   * **Permissões de objeto de projetos, programas, portfólios e modelos**: quando um nível de acesso tem **Nenhum acesso** selecionado para projetos, programas, portfólios e modelos, mas o objeto é compartilhado com eles, os usuários não podem ver o objeto no Workfront, mas ainda podem exibir o nome do objeto e quaisquer documentos associados em outras ferramentas do Adobe, como Frame.io e Adobe Creative Cloud.
   * **Permissões de documentos**: quando um nível de acesso tem **Nenhum acesso** selecionado para documentos, os usuários não podem ver documentos em projetos no Workfront, mas ainda podem exibir e gerenciar documentos de projetos compartilhados com eles em outras ferramentas do Adobe, como Frame.io e Adobe Creative Cloud. Isso ocorre porque o acesso a documentos é determinado por permissões no nível do projeto no Adobe Cloud Storage, em vez de apenas nos níveis de acesso do Workfront.

Se você tiver o Adobe Cloud Storage habilitado em seu ambiente Workfront, poderá criar projetos Adobe Cloud Storage e projetos Workfront Storage herdados. Os projetos de armazenamento herdados do Workfront mostram um ícone ao lado do nome do projeto em toda a Workfront. Os projetos de armazenamento na nuvem do Adobe não mostram um ícone.

![ícone de armazenamento herdado do workfront ao lado do nome do projeto](assets/legacy-project-icon.png)


### Ambientes que usam somente o armazenamento em nuvem do Adobe

Não é possível modificar permissões de documento no nível de acesso para projetos, programas e portfólios que usam o armazenamento na nuvem do Adobe.

Todos os níveis de acesso têm acesso de edição aos documentos. As permissões no nível do projeto determinam o acesso aos documentos em outras ferramentas do Adobe.

Não é possível restringir o acesso à herança de documentos.


### Ambientes que usam somente o armazenamento Workfront herdado

Nenhuma alteração nos níveis de acesso ou comportamento do documento.

## Permissões de objeto

As permissões de objeto determinam o que você pode ver e fazer com projetos, tarefas, problemas e documentos no Workfront. As permissões são atribuídas quando alguém compartilha um objeto com você.

>[!IMPORTANT]
>
>No Adobe Cloud Storage, as permissões de documento funcionam de forma diferente do armazenamento herdado do Workfront. Os documentos herdam permissões do projeto, tarefa ou problema ao qual estão vinculados.


### Como funcionam as permissões de documento

As permissões de documento são orientadas pelo objeto ao qual o documento está vinculado. Você não pode definir permissões em documentos individuais.

Quando você carrega um documento para uma tarefa ou problema, uma pasta gerada pelo sistema é criada usando o nome da tarefa ou problema. Esta pasta está vinculada à tarefa ou problema e herda suas permissões.

Você pode criar subpastas dentro da pasta gerada pelo sistema para organizar ainda mais os documentos. Todas as subpastas herdam permissões da pasta principal. No nível do projeto, você pode fazer upload de documentos fora de uma pasta, mas somente os usuários com acesso no nível do projeto podem visualizá-los.

No nível do projeto, as pastas geradas pelo sistema exibem um objeto vinculado. Geralmente, esse é o nome da tarefa ou do problema e é como o sistema sabe em qual tarefa ou problema a pasta deve ser visualizada.

### Permissões do projeto

Quando você tem permissões no nível do projeto, pode visualizar e gerenciar documentos desse projeto no Workfront e outros produtos da Adobe, como Frame.io e Adobe Creative Cloud. O nome do projeto também está visível nessas ferramentas. Outros dados do projeto não estão visíveis fora do Workfront.

### Permissões de tarefas e problemas

Tarefas e problemas herdam permissões do projeto. Quando você tem permissões de nível de tarefa ou problema, pode visualizar e gerenciar documentos vinculados a essa tarefa ou problema no Workfront e outros produtos da Adobe, como Frame.io e Adobe Creative Cloud.

**Pastas geradas pelo sistema**

* Remover usuários de uma tarefa ou problema não remove automaticamente o acesso às pastas. Eles ainda podem ter acesso por meio de permissões no nível do projeto.
* As subtarefas não herdam permissões de pastas geradas pelo sistema de tarefas pai. Você deve ser adicionado diretamente a uma subtarefa para acessar sua pasta gerada pelo sistema.
* Adicionar usuários a uma tarefa ou problema compartilha com eles a pasta gerada pelo sistema desse objeto.

**Movendo e renomeando pastas geradas pelo sistema:**

* As pastas geradas pelo sistema podem ser renomeadas e movidas.
* Se uma pasta gerada pelo sistema for movida para outro local, seu objeto vinculado será atualizado para o novo objeto. As permissões são herdadas do novo objeto pai.

As solicitações seguem o mesmo comportamento que tarefas e problemas.

### Aprovações

Quando adicionado a um fluxo de trabalho de aprovação de documento, você pode ver o seguinte, independentemente das permissões do projeto:

* Nome do projeto
* Nome do documento
* Miniatura do documento


## Mapeamento de permissão para Frame.io

Como parte da integração, as permissões do usuário são controladas no Workfront e fluem para o Frame.io. Isso significa que não é possível convidar um usuário para um projeto no Frame.io ou modificar permissões de usuário no Frame.io. Essas ações precisam ser feitas por meio do modal Compartilhamento de projetos no Workfront.

A tabela a seguir mostra como as permissões do Workfront são mapeadas para permissões de Frame.io:

<table>
<tr>
<th>Permissão de usuário do Workfront</th>
<th>Permissão de usuário do Frame.io</th>
</tr>
<tr>
<td>Gerenciar</td>
<td>Editar e compartilhar</td>
</tr>
<tr>
<td>Contribuir</td>
<td>Editar e compartilhar</td>
</tr>
<tr>
<td>Exibir</td>
<td>Somente comentário</td>
</tr>
</table>






