---
title: Visão Geral dos Tipos de Registro Entre Espaços de Trabalho
description: Os tipos de registro centralizado podem ser adicionados a vários espaços de trabalho a partir de um espaço de trabalho central ou principal no Adobe Workfront Planning.
hidefromtoc: true
hide: true
source-git-commit: ff5bc262a5ed2a22099c058ebdb61bc32485b201
workflow-type: tm+mt
source-wordcount: '1320'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Visão geral dos tipos de registro entre espaços de trabalho

No Adobe Workfront Planning, você pode ativar recursos entre espaços de trabalho para um tipo de registro que permita fazer referência a um tipo de registro em mais de um espaço de trabalho.

A seguir estão os recursos entre espaços de trabalho dos tipos de registro:

* Você pode designar um tipo de registro como centralizado. Os usuários podem adicionar tipos de registro centralizados a outros espaços de trabalho que eles podem gerenciar.
* Você pode designar um tipo de registro como conectável. Os usuários podem se conectar a esse tipo de registro a partir de outros espaços de trabalho.

Este artigo fornece uma visão geral dos tipos de registro entre espaços de trabalho. Para obter informações sobre como definir os recursos entre espaços de trabalho de um tipo de registro, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).


## Visão geral dos tipos de registros centralizados

Os tipos de registro centralizado podem ser adicionados a vários espaços de trabalho a partir de um espaço de trabalho central ou principal no Adobe Workfront Planning.

Ao implementar o Workfront Planning para uma organização de várias equipes com workflows comuns, talvez seja necessário definir uma estrutura coesa e metadados para os principais tipos de registro (como Campanhas ou Materiais de entrega) que podem ser adicionados aos espaços de trabalho de cada equipe para capturar e gerenciar o trabalho.

Além disso, pode ser necessário que o trabalho de cada equipe atinja um nível central.

Nesse fluxo de trabalho, você pode garantir que as equipes capturem seu trabalho de forma consistente ao desbloquear a visibilidade entre equipes, sem a necessidade de adicionar tudo a um espaço de trabalho, ou todos na organização a cada espaço de trabalho. Você pode usar tipos de registro centralizados para fazer isso.

Para usar tipos de registro centralizados, faça o seguinte:

1. Configure um tipo de registro para ser centralizado em um espaço de trabalho específico.

   Um gerenciador de espaço de trabalho pode selecionar usuários com uma licença, equipes, grupos, funções ou empresas do Standard para adicionar um tipo de registro escolhido a um espaço de trabalho gerenciado por eles.

   O tipo de registro original existirá em seu espaço de trabalho original, mas ficará visível de todos os outros espaços de trabalho.

   Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Adicione um tipo de registro a partir de um já existente que foi configurado como um tipo de registro centralizado a um espaço de trabalho secundário.

   O tipo de registro existirá nos seguintes espaços de trabalho:

   * Seu espaço de trabalho original, onde foi designado como um tipo de registro centralizado.
   * Um espaço de trabalho secundário.

   Para obter informações, consulte [Adicionar tipos de registro existentes de outro espaço de trabalho](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   As seções a seguir descrevem considerações sobre os tipos de registros centralizados e como eles funcionam em seus espaços de trabalho originais ou secundários.

### Considerações sobre os tipos de registros centralizados em seu espaço de trabalho original

O tipo de registro configurado para ser centralizado tem as seguintes propriedades:

* Todas as informações só podem ser editadas no espaço de trabalho original.

* Você pode executar as seguintes ações no tipo de registro centralizado a partir do espaço de trabalho original de um tipo de registro centralizado:

   * Editar

     A edição de um tipo de registro centralizado inclui a edição de sua aparência, recursos entre espaços de trabalho e todos os campos criados no espaço de trabalho original.
   * Criar formulários de solicitação
   * Gerenciar formulários de solicitação

* Você só poderá excluir um tipo de registro centralizado se ele não tiver sido adicionado a um espaço de trabalho secundário. Depois que ele for adicionado a outro espaço de trabalho, tentar excluí-lo do espaço de trabalho original gerará um erro.

  Isso é feito para que o tipo de registro centralizado possa permanecer nos espaços de trabalho em que já foi adicionado.
* Os registros adicionados a um tipo de registro centralizado ficam visíveis somente para usuários com permissões de Exibição no espaço de trabalho ao qual foram adicionados.
* Os registros adicionados de um espaço de trabalho secundário são totalizados e exibidos no espaço de trabalho original. Todos os membros do espaço de trabalho original obtêm permissões de Exibição para ele.

* Os tipos de registro conectados de um tipo de registro centralizado se tornarão disponíveis para conexão a partir dos espaços de trabalho em que esse tipo de registro for adicionado.

  Por exemplo, se você tiver um tipo de registro Campanha que tenha uma conexão com o tipo de registro Regiões e adicionar o tipo de registro Campanha a um espaço de trabalho secundário, as Regiões se tornarão conectáveis entre espaços de trabalho para o espaço de trabalho secundário. Os membros do espaço de trabalho secundário agora podem criar campanhas e vinculá-las a regiões.

* Os campos criados para um tipo de registro centralizado do espaço de trabalho original são visíveis em todos os espaços de trabalho em que o tipo de registro é adicionado. Os campos de um espaço de trabalho original são somente leitura nos espaços de trabalho secundários.

### Considerações sobre tipos de registros centralizados depois de adicioná-los a um espaço de trabalho secundário

* Colaboradores secundários de espaço de trabalho obtêm permissão do Contribute para o tipo de registro centralizado no espaço de trabalho de sua equipe. Eles podem adicionar e gerenciar registros nela.

* Os visualizadores secundários do espaço de trabalho obtêm permissão de Visualização para o tipo de registro centralizado no espaço de trabalho de sua equipe. Eles não podem adicionar e gerenciar registros no.

* Os gerentes de espaço de trabalho secundário podem executar as seguintes ações no tipo de registro adicionado de um tipo de registro centralizado em um espaço de trabalho secundário:

   * Excluí-lo.

     A exclusão do tipo de registro de um espaço de trabalho secundário o remove apenas do espaço de trabalho secundário. Os registros adicionados a ele a partir do espaço de trabalho secundário também são excluídos. Isso não exclui o tipo de registro de seu espaço de trabalho original ou de qualquer outro espaço de trabalho secundário ao qual ele tenha sido adicionado.

  <!--These two capabilities will come later:
    * Add new fields
        Fields added to a centralized record from a secondary workspace are visible only from the secondary workspace. 
    * Share it-->

* Não é possível executar as seguintes ações no tipo de registro adicionado de um tipo de registro centralizado em um espaço de trabalho secundário:

   * Editar

     Não é possível editar a aparência, os recursos entre espaços de trabalho ou os campos adicionados a partir do espaço de trabalho original.
   * Criar e gerenciar formulários de solicitação
   * Criar e gerenciar formulários de solicitação

* Os registros adicionados em espaços de trabalho secundários ficam visíveis nos seguintes espaços de trabalho, se você tiver permissões de Exibição ou superiores para esses espaços de trabalho:

   * O espaço de trabalho secundário onde eles são adicionados.
   * O espaço de trabalho original do tipo de registro centralizado.
   * Todos os outros espaços de trabalho onde o espaço de trabalho centralizado é adicionado.

* Os cenários a seguir existem para registros criados nos espaços de trabalho das equipes:

   * Se você tiver permissões Gerenciar no espaço de trabalho original e não tiver permissões em um espaço de trabalho secundário, poderá exibir registros adicionados dos espaços de trabalho secundários no espaço de trabalho original, mas não poderá gerenciá-los no espaço de trabalho original.
   * Se você tiver permissões de Gerenciamento no espaço de trabalho secundário, poderá gerenciar os registros no espaço de trabalho original do tipo de registro centralizado ou no espaço de trabalho onde eles foram adicionados.

     Você pode exibir os registros em espaços de trabalho secundários adicionais onde o tipo de registro centralizado é adicionado somente se tiver permissões de Exibição para esses espaços de trabalho.

### Acesso às conexões de um tipo de registro centralizado

Os tipos de registro conectados ao tipo de registro centralizado no espaço de trabalho original tornam-se visíveis em outros espaços de trabalho onde o tipo de registro centralizado é adicionado.

### Acesso à API de um tipo de registro centralizado

Ao adicionar registros a um tipo de registro centralizado de um espaço de trabalho secundário usando a API do Workfront Planning, o sistema verifica se o usuário tem acesso para criar registros no espaço de trabalho original do tipo de registro centralizado.

Os seguintes casos existem:

* Se o usuário tiver acesso, o registro será criado no espaço de trabalho original dos tipos de registro centralizado.

* Se o usuário não tiver acesso, ele receberá um erro de que não tem acesso ao espaço de trabalho original do tipo de registro centralizado e precisa fornecer a ID do espaço de trabalho onde tem acesso para criar registros.

## Visão geral dos tipos de registro conectáveis

É possível conectar-se a um tipo de registro definido como conectável a partir de qualquer espaço de trabalho gerenciado.

Suas equipes podem precisar de seus registros vinculados a tipos de registros de outros espaços de trabalho ou visualizar informações capturadas em registros que pertencem a registros em outros espaços de trabalho. Você pode obter essa configuração designando um tipo de registro como conectável.

Para usar tipos de registro conectáveis, faça o seguinte:

1. Configure um tipo de registro para ser conectável em um espaço de trabalho específico.

   Um gerenciador de espaço de trabalho pode selecionar a quais espaços de trabalho um tipo de registro designado está disponível para conexão.

   O tipo de registro original existirá em seu espaço de trabalho original e será adicionado como um tipo de registro conectado a outro espaço de trabalho.

   Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Conecte-se a um tipo de registro designado como conectável de outro espaço de trabalho que você gerencia.

   Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

   As seções a seguir descrevem considerações sobre os tipos de registros centralizados e como eles funcionam em seus espaços de trabalho originais ou secundários.