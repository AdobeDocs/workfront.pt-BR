---
title: Visão geral do tipo de registro entre espaços de trabalho
description: Você pode ativar os tipos de registro para serem globais ou conectáveis. Os tipos de registro global podem ser adicionados a vários espaços de trabalho a partir de um espaço de trabalho central ou principal no Adobe Workfront Planning, enquanto os tipos de registro conectáveis podem ser conectados a partir de outros espaços de trabalho que não os seus próprios.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 895fcc9e8bfc6ef21e82ae6dab4c370b0e267cad
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 0%

---


# Visão geral do tipo de registro entre espaços de trabalho

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Você pode ativar recursos entre espaços de trabalho para um tipo de registro no Adobe Workfront Planning. Um tipo de registro entre espaços de trabalho pode ser referenciado ou acessado em mais de um espaço de trabalho.

>[!IMPORTANT]
>
>Sua organização deve comprar os seguintes pacotes para habilitar recursos entre espaços de trabalho para tipos de registro:
>
>Para configurar tipos de registro conectáveis:
>
>
>* Qualquer pacote do Workfront e qualquer pacote do Planning
>
>   Ou
>
>* Qualquer fluxo de trabalho e um pacote do Planning Prime ou Ultimate
>
><span class="preview">Para configurar tipos de registros globais:</span>
>
>* <span class="preview">Qualquer pacote do Workfront e um pacote do Planning Plus</span>
>     
>   Ou
>
>* <span class="preview">Qualquer Fluxo de Trabalho e um pacote do Planning Prime ou Ultimate</span>
>
>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront.
>Para obter informações, consulte [Visão geral sobre acesso ao Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).


A seguir estão os recursos entre espaços de trabalho dos tipos de registro:

* <span class="preview">**Tipos de registros globais**: os usuários podem adicionar tipos de registros globais a outros espaços de trabalho que gerenciam.</span>

* **Tipos de registro conectáveis**: os usuários podem se conectar a este tipo de registro de outros espaços de trabalho.

Este artigo fornece uma visão geral dos tipos de registro entre espaços de trabalho. Para obter informações sobre como definir os recursos entre espaços de trabalho de um tipo de registro, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

<div class="preview">

## Visão geral dos tipos de registro global

Os tipos de registro global podem ser adicionados a vários espaços de trabalho a partir de um espaço de trabalho central ou principal no Workfront Planning.

Ao implementar o Workfront Planning para uma organização de várias equipes com workflows comuns, talvez seja necessário definir uma estrutura coesa e metadados para os principais tipos de registro (como Campanhas ou Materiais de entrega) que podem ser adicionados aos espaços de trabalho de cada equipe para capturar e gerenciar o trabalho.

Você também pode precisar do trabalho de cada equipe para acumular-se em um nível central.

Nesse fluxo de trabalho, você pode garantir que as equipes capturem seu trabalho de forma consistente ao desbloquear a visibilidade entre equipes, sem a necessidade de adicionar tudo a um espaço de trabalho, ou todos na organização a cada espaço de trabalho. Você pode usar tipos de registro global para fazer isso.

Para usar tipos de registro global, faça o seguinte:

1. Em um espaço de trabalho gerenciado, configure um tipo de registro para ser global.

   Um gerente de espaço de trabalho pode conceder permissões a usuários com uma licença Standard ou a equipes, grupos, funções e empresas para adicionar um tipo de registro escolhido a um espaço de trabalho gerenciado por eles.

   O tipo de registro original existirá em seu espaço de trabalho original, mas ficará visível em outros espaços de trabalho.

   Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Adicione um tipo de registro a um espaço de trabalho secundário a partir de um existente que foi configurado como um tipo de registro global.

   O tipo de registro existirá nos seguintes espaços de trabalho:

   * Seu espaço de trabalho original, onde foi designado como um tipo de registro global.
   * Um espaço de trabalho secundário.

   Para obter informações, consulte [Adicionar tipos de registro existentes de outro espaço de trabalho](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   As seções a seguir descrevem considerações sobre os tipos de registros globais e como eles funcionam em seus espaços de trabalho originais ou secundários.

### Considerações sobre os tipos de registro global em seu espaço de trabalho original

O tipo de registro configurado para ser global tem as seguintes propriedades:

* Todas as informações (aparência, campos originais) só podem ser editadas no espaço de trabalho original.

* Você pode executar as seguintes ações no tipo de registro global a partir de seu espaço de trabalho original:

   * Editar

     A edição de um tipo de registro global inclui a edição de sua aparência, recursos entre espaços de trabalho e todos os campos criados no espaço de trabalho original.
   * Compartilhá-lo

     O compartilhamento de um tipo de registro adiciona usuários ao espaço de trabalho e também compartilha os registros com esses usuários.
   * Excluí-lo

     Você só poderá deletar um tipo de registro global de seu espaço de trabalho original depois de deletar todas as instâncias de if de todos os espaços de trabalho secundários em que ele foi adicionado.

     Para obter mais informações, consulte [Excluir tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Torná-lo conectável de outros espaços de trabalho
   * Criar e gerenciar formulários de solicitação
   * Criar e gerenciar automações

* Os registros adicionados a um tipo de registro global ficam visíveis somente para usuários com permissões de Exibição no espaço de trabalho ao qual foram adicionados. <!-- this needs to be more specific: what does "o the workspace where they were added" mean? - added in which kind of workspaces? secondary or primary; asking Lilit-->
* Os registros adicionados de um espaço de trabalho secundário são totalizados e exibidos no espaço de trabalho original. Todos os membros do espaço de trabalho original obtêm permissões de Exibição para eles.
* Quando o tipo de registro global original é adicionado a vários espaços de trabalho secundários, os seguintes cenários existem:

   * Os membros do espaço de trabalho original obtêm automaticamente permissões de Exibição para todos os registros adicionados de qualquer espaço de trabalho, mesmo que não sejam membros desses espaços de trabalho.
   * Os membros do espaço de trabalho secundário podem exibir somente registros de espaços de trabalho dos quais são membros. <!--change this to: Secondary workspace members can view only records from the workspace the records were added and where they have at least permissions to view the record workspace and the record type.-->

* Os tipos de registro conectados a um tipo de registro global se tornarão disponíveis para conexão a partir dos espaços de trabalho em que esse tipo de registro for adicionado.

  Por exemplo, se você tiver um tipo de registro global do Campaign que tenha uma conexão com um tipo de registro Regiões e adicionar o tipo de registro Campanha a um espaço de trabalho secundário, as Regiões se tornarão conectáveis entre espaços de trabalho do espaço de trabalho secundário. Os membros do espaço de trabalho secundário agora podem criar campanhas e vinculá-las a regiões.

* Os campos criados para um tipo de registro global do espaço de trabalho original são visíveis em todos os espaços de trabalho em que o tipo de registro é adicionado.

  É possível editar configurações de campo somente no espaço de trabalho original.

  As configurações dos campos criados no espaço de trabalho original são somente leitura nos espaços de trabalho secundários para todos os membros, independentemente de suas permissões no espaço de trabalho secundário.

  Os gerentes de espaço de trabalho secundário não podem modificar as configurações de campo para campos configurados no espaço de trabalho original. Somente os gerentes de espaço de trabalho do espaço de trabalho original podem modificar as configurações de campo no espaço de trabalho original.

### Considerações sobre tipos de registro global em um espaço de trabalho secundário

* Colaboradores secundários de espaço de trabalho obtêm permissão do Contribute para o tipo de registro global no espaço de trabalho de sua equipe. Eles podem adicionar e gerenciar registros nela a partir do espaço de trabalho secundário.

* Os visualizadores secundários do espaço de trabalho obtêm a permissão Exibir para o tipo de registro global no espaço de trabalho de sua equipe. Eles não podem adicionar e gerenciar registros nele.

* Os gerenciadores de espaço de trabalho secundário podem executar as seguintes ações adicionais no tipo de registro adicionado de um tipo de registro global em um espaço de trabalho secundário:

   * Excluí-lo.

     A exclusão do tipo de registro de um espaço de trabalho secundário o remove apenas do espaço de trabalho secundário. Os registros e campos adicionados a ele a partir do espaço de trabalho secundário também são excluídos. Isso não exclui o tipo de registro de seu espaço de trabalho original ou de qualquer outro espaço de trabalho secundário ao qual ele tenha sido adicionado.

     Para obter mais informações, consulte [Excluir tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Compartilhar as exibições dos tipos de registro.

     Não é possível compartilhar uma exibição publicamente de um tipo de registro global em um espaço de trabalho secundário. Você só pode compartilhar exibições internamente de um espaço de trabalho secundário. Você pode compartilhar uma exibição interna e publicamente para um tipo de registro global em seu espaço de trabalho original.

     Para obter informações, consulte [Compartilhar modos de exibição](/help/quicksilver/planning/access/share-views.md).

<!--Uncomment this at prod on Jan 15: * Share it-->

<!--You can share a global record type added to a secondary workspace from the secondary space. By sharing a global record type in a secondary workspace, the following also occur:

    * Users are added to the workspace with View permissions.
    * Users receive the same permissions to all the records of the global record type in the secondary workspace.-->

<!--when they will be able to add fields to the secondary space, this bullet will need this extra information: 
    After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added.-->

<!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
* Add new fields
    Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
* Add request forms to it
* Add automations to it-->

* Nenhum usuário pode executar as seguintes ações em um tipo de registro global em um espaço de trabalho secundário:

   * Editar

     Não é possível editar a aparência, os recursos entre espaços de trabalho ou os campos adicionados a partir do espaço de trabalho original.
   * Compartilhar <!-- remove this at Prod on Jan 15-->
   * Criar e gerenciar formulários de solicitação
   * Criar e gerenciar automações

* Os registros adicionados em um espaço de trabalho secundário ficam visíveis nos seguintes espaços de trabalho, somente se você tiver permissões de Exibição ou superiores para esses espaços de trabalho:

   * O espaço de trabalho secundário onde eles são adicionados.
   * O espaço de trabalho original do tipo de registro global.
   * Todos os outros espaços de trabalho onde o espaço de trabalho global é adicionado.

  <!--replace he above bullet with this: 
        * Records added in a secondary workspace are visible from the following workspaces, only if you have View or higher permissions to these workspaces:
        * The secondary place where they were added
        * The global record type's original workspace
    -->

* Existem os seguintes cenários para registros criados em espaços de trabalho secundários:

   * Se você tiver permissões Gerenciar no espaço de trabalho original e não tiver permissões em um espaço de trabalho secundário, poderá exibir registros adicionados dos espaços de trabalho secundários no espaço de trabalho original, mas não poderá gerenciá-los no espaço de trabalho original.
   * Se você tiver permissões de Gerenciamento no espaço de trabalho secundário, poderá gerenciar os registros do espaço de trabalho original do tipo de registro global e do espaço de trabalho secundário em que eles foram adicionados.
   * Você pode exibir os registros em espaços de trabalho secundários adicionais onde o tipo de registro global é adicionado somente se tiver permissões de Exibição para esses espaços de trabalho. <!-- take this bullet out when we change this functionality on Jan 15-->

### Acesso às conexões de um tipo de registro global

Os tipos de registro conectados ao tipo de registro global no espaço de trabalho original tornam-se visíveis a partir de outros espaços de trabalho em que o tipo de registro global é adicionado e ficam disponíveis para conexões a partir dos espaços de trabalho secundários em que o tipo de registro global é adicionado.

### Acesso à API de um tipo de registro global

Ao adicionar registros a um tipo de registro global de um espaço de trabalho secundário usando a API do Workfront Planning, o sistema verifica se o usuário tem acesso para criar registros no espaço de trabalho original do tipo de registro global.

Os seguintes casos existem:

* Se o usuário tiver acesso, o registro será criado no espaço de trabalho original dos tipos de registro global.

* Se o usuário não tiver acesso, ele receberá um erro de que não tem acesso ao espaço de trabalho original do tipo de registro global e precisa fornecer a ID do espaço de trabalho onde tem acesso para criar registros.

</div>

## Visão geral dos tipos de registro conectáveis

É possível conectar-se a um tipo de registro definido como conectável a partir de qualquer espaço de trabalho gerenciado.

Suas equipes podem precisar de seus registros vinculados a tipos de registros de outros espaços de trabalho ou visualizar informações capturadas em registros que pertencem a registros em outros espaços de trabalho. Você pode obter essa configuração designando um tipo de registro como conectável.

Para usar tipos de registro conectáveis, faça o seguinte:

1. Configure um tipo de registro para ser conectável em um espaço de trabalho específico.

   Um gerenciador de espaço de trabalho pode selecionar a quais espaços de trabalho um tipo de registro designado está disponível para conexão.

   O tipo de registro original existirá em seu espaço de trabalho original e poderá ser acessado para conexão de outro espaço de trabalho.

   Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Conecte-se a um tipo de registro designado como conectável de outro espaço de trabalho que você gerencia.

   Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
