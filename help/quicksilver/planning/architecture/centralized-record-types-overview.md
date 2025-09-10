---
title: Visão Geral de Tipos de Registro Centralizados
description: Os tipos de registro centralizado podem ser adicionados a vários espaços de trabalho a partir de um espaço de trabalho central ou principal no Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Visão geral dos tipos de registro centralizado

Os tipos de registro centralizado podem ser adicionados a vários espaços de trabalho a partir de um espaço de trabalho central ou principal no Adobe Workfront Planning.

## Visão geral dos tipos de registros centralizados

Ao implementar o Workfront Planning para uma organização de várias equipes com workflows comuns, talvez seja necessário definir uma estrutura coesa e metadados para os principais tipos de registro (como Campanhas ou Materiais de entrega) que podem ser adicionados aos espaços de trabalho de cada equipe para capturar e gerenciar o trabalho.

Além disso, pode ser necessário que o trabalho de cada equipe atinja um nível central.

Nesse fluxo de trabalho, você pode garantir que as equipes capturem seu trabalho de forma consistente ao desbloquear a visibilidade entre equipes, sem a necessidade de adicionar tudo a um espaço de trabalho, ou todos na organização a cada espaço de trabalho. Você pode usar tipos de registro centralizados para fazer isso.

Para usar tipos de registro centralizados, faça o seguinte:

1. Configure um tipo de registro para ser centralizado em um espaço de trabalho específico.

   Um gerenciador de espaço de trabalho pode selecionar usuários com uma licença, equipes, grupos, funções ou empresas do Standard para adicionar um tipo de registro escolhido a um espaço de trabalho gerenciado por eles.

   O tipo de registro original existirá em seu espaço de trabalho original, mas ficará visível de todos os outros espaços de trabalho.

   Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Adicionar um tipo de registro existente de um já existente que foi configurado como centralizado para o espaço de trabalho de uma equipe.

   O tipo de registro existirá nos seguintes espaços de trabalho:

   * Seu espaço de trabalho original, onde foi designado como um tipo de registro centralizado.
   * O espaço de trabalho da equipe.

   Para obter informações, consulte [Adicionar tipos de registros existentes](/help/quicksilver/planning/architecture/add-cross-workspace-record-types.md).

   As seções a seguir descrevem considerações sobre os tipos de registros centralizados em seus espaços de trabalho originais ou após serem adicionados aos espaços de trabalho de uma equipe.

## Considerações sobre os tipos de registros centralizados em seu espaço de trabalho original

O tipo de registro configurado para ser centralizado tem as seguintes propriedades:

* Todas as informações só podem ser editadas no espaço de trabalho original.

* Você pode executar as seguintes ações no tipo de registro centralizado a partir do espaço de trabalho original de um tipo de registro centralizado:

   * Editar

     A edição de um tipo de registro centralizado inclui a edição de sua aparência, recursos entre espaços de trabalho e todos os campos criados no espaço de trabalho original.
   * Criar formulários de solicitação
   * Gerenciar formulários de solicitação

* Você só pode excluir um tipo de registro centralizado se ele não tiver sido adicionado a um espaço de trabalho de equipe. Após ser adicionado ao espaço de trabalho de uma equipe, tentar excluí-lo do espaço de trabalho original gerará um erro.

  Isso é feito para que o tipo de registro centralizado possa permanecer nos espaços de trabalho em que já foi adicionado.
* Os registros adicionados a um tipo de registro centralizado ficam visíveis somente para usuários com permissões de Exibição no espaço de trabalho original.
* Os registros adicionados do espaço de trabalho da equipe são acumulados e exibidos no espaço de trabalho original. Todos os membros do espaço de trabalho original obtêm permissões de Exibição para ele.

* Os tipos de registro conectados de um tipo de registro centralizado se tornarão disponíveis para conexão a partir dos espaços de trabalho em que esse tipo de registro for adicionado.

* Os campos criados para um tipo de registro centralizado do espaço de trabalho original são visíveis em todos os espaços de trabalho em que o tipo de registro é adicionado.

## Considerações sobre tipos de registros centralizados depois de adicioná-los ao espaço de trabalho de uma equipe

* Os colaboradores do espaço de trabalho da equipe obtêm permissão do Contribute para o tipo de registro centralizado no espaço de trabalho da equipe. Eles podem adicionar e gerenciar registros nela.

* Os visualizadores do espaço de trabalho da equipe obtêm permissão de Visualização para o tipo de registro centralizado no espaço de trabalho da equipe. Eles não podem adicionar e gerenciar registros no.

* Os gerentes de espaço de trabalho da equipe podem executar as seguintes ações no tipo de registro adicionado de um tipo de registro centralizado no espaço de trabalho de uma equipe:

   * Adicionar novos campos

     Os campos adicionados a um registro centralizado de um espaço de trabalho da equipe ficam visíveis somente no espaço de trabalho da equipe.
   * Compartilhá-lo
   * Excluí-lo.

     Excluir o tipo de registro do espaço de trabalho de uma equipe só o remove do espaço de trabalho da equipe. Os registros adicionados a ele a partir do espaço de trabalho da equipe também são excluídos. Isso não exclui o tipo de registro de seu espaço de trabalho original ou de qualquer outro espaço de trabalho de equipe ao qual tenha sido adicionado.

     Isso é feito para que seja possível manter o tipo de registro centralizado já adicionado nos espaços de trabalho que já o estão usando.

* Não é possível executar as seguintes ações no tipo de registro adicionado de um tipo de registro centralizado no espaço de trabalho de uma equipe:

   * Editar

     Não é possível editar a aparência, os recursos entre espaços de trabalho ou os campos adicionados a partir do espaço de trabalho original.
   * Criar formulários de solicitação
   * Gerenciar formulários de solicitação

* Os registros adicionados aos espaços de trabalho de uma equipe ficam visíveis nos seguintes espaços de trabalho, se você tiver permissões de Exibição ou superiores para esses espaços de trabalho:

   * O espaço de trabalho da equipe onde eles são adicionados.
   * O espaço de trabalho original do tipo de registro centralizado.
   * Todos os outros espaços de trabalho onde o espaço de trabalho centralizado é adicionado.

* Os cenários a seguir existem para registros criados nos espaços de trabalho das equipes:

   * Se você tiver permissões Gerenciar no espaço de trabalho original e não tiver permissões nos espaços de trabalho das equipes, poderá exibir registros adicionados dos espaços de trabalho da equipe no espaço de trabalho original, mas não poderá gerenciá-los no espaço de trabalho original.
   * Se você tiver permissões de Gerenciamento no espaço de trabalho da equipe, poderá gerenciar os registros no espaço de trabalho original do tipo de registro centralizado ou no espaço de trabalho onde eles foram adicionados.

     Você pode exibir os registros em espaços de trabalho de equipe adicionais onde o tipo de registro centralizado é adicionado somente se você tiver permissões de Visualização para esses espaços de trabalho.

## Acesso a conexões

Os tipos de registro conectados ao tipo de registro centralizado no espaço de trabalho original tornam-se visíveis para espaços de trabalho de equipe onde o tipo de registro centralizado é adicionado.

## Comportamento da API

Ao adicionar registros a um tipo de registro centralizado de um espaço de trabalho da equipe usando a API do Workfront Planning, o sistema verifica se o usuário tem acesso para criar registros no espaço de trabalho original do tipo de registro centralizado.

Os seguintes casos existem:

* Se o usuário tiver acesso, o registro será criado no espaço de trabalho original dos tipos de registro centralizado.

* Se o usuário não tiver acesso, ele receberá um erro de que não tem acesso ao espaço de trabalho original do tipo de registro centralizado e precisa fornecer a ID do espaço de trabalho onde tem acesso para criar registros.