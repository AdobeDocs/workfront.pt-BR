---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Tipos de função de licenciamento do Adobe Workfront versus tipos de função do Adobe Workfront DAM
description: Adobe Systems administradores da Workfront usam níveis de acesso para determinar o que os usuários podem fazer em um aplicativo.
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---

# Adobe Systems tipos de função de licenciamento da Workfront em comparação aos Adobe Systems tipos de DAM função da Workfront

Adobe Systems administradores da Workfront usam níveis de acesso para determinar o que os usuários podem fazer em um aplicativo.

* Na Workfront, o licenciamento determina o nível de acesso do usuário.
* No Workfront DAM, os tipos de função definem o acesso dos usuários aos ativos no DAM.

Como os tipos de licença e os tipos de função não são intercambiáveis, ter um nível de acesso em um aplicativo não implica acesso em outro aplicativo. Por exemplo, um usuário com uma licença de Trabalho no Workfront não recebe automaticamente uma função de Colaborador no Workfront DAM.

## Tipos de licença do Workfront

Como administrador do Workfront, você define o nível de acesso que os usuários têm ao atribuir tipos de licença. Cada licença vem com um conjunto de recursos de acesso padrão que você pode modificar antes de atribuir a licença ao usuário. 

Você usa o licenciamento para determinar o que um usuário pode ver e fazer no Workfront. Há cinco tipos de licenciamento disponíveis no Workfront:

* Plano
* Trabalho
* Revisar
* Solicitar
* Externo

Consulte [Visão geral das licenças herdadas](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) para obter uma descrição dos diferentes tipos de licença no Workfront.

## Tipos de função do Workfront DAM

Como administrador do Workfront DAM Workfront, você atribui tipos de função aos usuários para definir o acesso que eles têm aos ativos. Além disso, os tipos de função especificam as áreas no DAM em que os usuários podem trabalhar.

Os tipos de função funcionam em conjunto com Grupos ao estabelecer direitos de acesso do usuário. Os grupos controlam o acesso que os usuários têm às pastas e aos próprios ativos. Os tipos de função determinam as ações que os usuários podem realizar com os ativos. Todos os usuários do DAM devem estar associados a pelo menos um Grupo. Para saber mais sobre os tipos de função e acessar a configuração, consulte a Ajuda no Workfront DAM.

Existem quatro tipos função distintos disponíveis na Workfront DAM:

### AEM Brand Portal

Os usuários com esse tipo de função têm acesso apenas ao portal Brand Connect no DAM. No portal, os usuários podem visualização e baixar ativos aos quais têm permissões.

Os usuários do Brand Portal podem colaborar com outras pessoas criando e compartilhando lightboxes.

### Usuário Normal

Os usuários com esse tipo de função podem visualizar e baixar ativos do Workfront DAM e do portal Brand Connect.

Usuários Comuns também podem colaborar com outras pessoas criando e compartilhando lightboxes.

### Colaborador

Os usuários com esse tipo de função têm acesso ao Workfront DAM e ao portal Brand Connect.

Os colaboradores podem visualizar, baixar, carregar, editar, mover e excluir ativos e pastas aos quais têm acesso. Além disso, os Colaboradores podem colaborar com outras pessoas criando e compartilhando lightboxes. 

### Administrador

Os administradores da Workfront têm acesso a tudo no portal Brand Connect e no Workfront DAM, incluindo ativos que expiraram ou que têm um status inativo.

No solicitar ter acesso de administrador, os usuários com o Tipo de função do Administrador devem estar no Grupo de administradores.
