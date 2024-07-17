---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: "Aprimoramentos no gerenciamento de recursos 2020.2: o balanceador de carga de trabalho"
description: Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 2020.2 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 0%

---

# Melhorias no gerenciamento de recursos 2020.2: o balanceador de carga de trabalho

Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 2020.2 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de maio de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 2020.2, consulte a [visão geral da versão 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

As pessoas são um ativo de Nível 1. Com o Balanceador de carga de trabalho, você pode protegê-los contra esgotamento e capacitá-los a fazer o melhor trabalho, alinhando-os às principais estratégias da empresa. Apresentando uma experiência de agendamento reimaginada que permite visualizar e gerenciar as cargas de trabalho e a demanda das pessoas na mesma visualização. A interface do usuário fornece mapeamento visual claro de superutilização e subutilização e é transparente para todas as partes interessadas. Os gerentes de pessoas podem usar essas informações como uma entrada e, na mesma tela, reequilibrar o esforço por meio da linha do tempo, que é refletida no restante da plataforma do Workfront.

>[!NOTE]
>
>O Balanceador de carga de trabalho começou a ser lançado como um beta com a versão 2019.4. Todos os aprimoramentos do Balanceador de carga de trabalho estão disponíveis para o público geral com a versão 2020.2. As melhorias descritas nesta página foram adicionadas com a versão 2020.2. Para obter uma visão geral do Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Ajustar a alocação diária e semanal no Balanceador de carga de trabalho

Para evitar o esgotamento de seus recursos, agora é possível ajustar a alocação diária e semanal de seus usuários para trabalhar usando o Balanceador de carga de trabalho.

Antes desse aprimoramento, isso só era possível usando as ferramentas de Agendamento de recursos.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Filtros do Balanceador de carga de trabalho

Para tornar as informações no Balanceador de carga de trabalho relevantes para você, agora é possível criar filtros para as áreas Trabalho não atribuído e Trabalho atribuído do Balanceador de carga de trabalho e salvá-los para uso futuro. Em seguida, você pode editar a versão salva para fazer pequenas alterações nela, em vez de começar do zero com um novo filtro.

Para obter informações sobre a filtragem no Balanceador de carga de trabalho, consulte [Gerenciar filtros no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Mostrar horas restantes no Balanceador de carga de trabalho

Para ajudá-lo a tomar decisões corretas de atribuição, uma nova configuração agora permite visualizar a diferença de horas entre as horas que um usuário está disponível para trabalhar de acordo com sua programação e as horas que já foram alocadas para o trabalho (as horas restantes). A nova configuração agora está disponível no Balanceador de carga de trabalho.

Para obter informações sobre como visualizar informações no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou se você estiver usando o Adobe Workfront Classic, consulte [Navegar pelo Balanceador de carga de trabalho](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).)

**Disponível nestes ambientes:**

* A nova experiência do Adobe Workfront

## Mostra Horas planejadas diárias para tarefas e projetos na área Trabalho não atribuído do Balanceador de carga de trabalho

Para ajudá-lo a entender como as tarefas afetarão a carga de trabalho dos usuários antes de atribuí-las, a configuração &quot;Mostrar alocações&quot; agora gerencia quais informações são exibidas na área Trabalho não atribuído do Balanceador de carga de trabalho. Quando essa configuração está ativada, as Horas planejadas para tarefas e projetos são exibidas na área Trabalho não atribuído do Balanceador de carga de trabalho.

Antes dessa alteração, essa configuração atualizava somente as informações na área Trabalho atribuído do Balanceador.

Para obter informações sobre como navegar no Balanceador de carga de trabalho, consulte [Navegar no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Navegar no Balanceador de carga de trabalho](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).)

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront (anteriormente disponível apenas para tarefas)

## Nova caixa Configurações para o Balanceador de carga de trabalho

Para simplificar sua experiência, uma caixa Configurações agora está disponível e exibe ferramentas adicionais para atualizar a exibição no Balanceador de carga de trabalho. Esta caixa inclui as seguintes configurações:

* Agrupar por Projeto
* Exiba as Horas alocadas ou as Horas restantes para suas tarefas e projetos.

Para obter informações sobre como visualizar informações no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou se você estiver usando o Adobe Workfront Classic, consulte [Navegar pelo Balanceador de carga de trabalho](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648).)

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Compartilhar o Balanceador de carga de trabalho com um link

Agora você pode compartilhar a carga de trabalho de seus funcionários com os executivos para que eles possam ter contexto sobre suas necessidades de pessoal. Para isso, agora você pode compartilhar o Balanceador de carga de trabalho compartilhando um URL exclusivo para o Balanceador de carga de trabalho com qualquer outra pessoa.

Para obter informações sobre como navegar no Balanceador de carga de trabalho, consulte [Navegar no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Navegar no Balanceador de carga de trabalho](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648)).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Alterar o intervalo de datas no Balanceador de carga de trabalho

Para ajudar você a personalizar a duração da linha do tempo do Balanceador de carga de trabalho para atender às suas necessidades, agora é possível selecionar um período personalizado de 2, 4 ou 6 semanas para exibir de uma só vez.

Antes desse aprimoramento, o Balanceador de carga de trabalho sempre exibia informações que começam com a semana atual.

Para obter informações sobre como navegar no Balanceador de carga de trabalho, consulte [Navegar no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Navegar no Balanceador de carga de trabalho](https://one.workfront.com/s/article/Navigate-the-Workload-Balancer-1841453648)).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront (disponível anteriormente)

## Mover e copiar tarefas para outro projeto mantém a restrição da tarefa quando as tarefas podem se ajustar à linha do tempo do projeto

Melhoramos a maneira como o Workfront lida com a Restrição de tarefa específica por data de uma tarefa quando você copia a tarefa ou a move para outro projeto. Exemplos de Restrições de Tarefas específicas por data são: Deve começar em, Deve terminar em, Datas fixas, Não iniciar depois de e assim por diante.

Por exemplo, quando você move ou copia uma tarefa com uma restrição Deve Iniciar Em para outro projeto cuja Data Inicial Planejada é anterior à Data Inicial da tarefa, a tarefa mantém a restrição após ser copiada ou movida. Quando você move ou copia uma tarefa com uma restrição Deve Iniciar Em para um projeto cuja Data Inicial Planejada é posterior à Data Inicial da tarefa, a Restrição da Tarefa muda para O Mais Breve Possível.

Antes dessa alteração, a Restrição da tarefa sempre muda para O mais rápido possível.

Para obter informações sobre como mover tarefas, consulte [Mover tarefas](../../../manage-work/tasks/manage-tasks/move-tasks.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Movendo Tarefas](https://one.workfront.com/s/article/Moving-Tasks-2081996259)).

Para obter informações sobre como copiar tarefas, consulte [Copiar e duplicar tarefas](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Copiar e Duplicar Tarefas](https://one.workfront.com/s/article/Copy-and-Duplicate-Tasks-218695605)).

Para obter uma visão geral de todas as Restrições de Tarefa, consulte [Visão geral da Restrição de Tarefa](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (ou se estiver usando o Adobe Workfront Classic, consulte [Visão Geral da Restrição de Tarefa](https://one.workfront.com/s/article/Task-Constraint-Overview-453396848)).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Como evitar a perda de dados enquanto faz alterações na guia Detalhes ou em uma lista de tarefas

Para evitar a perda de dados ao atualizar informações na página Detalhes de um objeto ou de tarefas em uma lista de tarefas no nível do projeto ao salvar as alterações manualmente, uma mensagem de aviso agora é exibida para notificá-lo de que você tem alterações não salvas antes de tentar editar informações no cabeçalho. As únicas ações permitidas antes de salvar suas alterações são a assinatura ou a adição do objeto aos favoritos.

Para obter informações sobre como editar tarefas em uma lista, consulte [Editar tarefas em uma lista](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**Disponível nestes ambientes:**

* A nova experiência do Adobe Workfront

## Criar processos de aprovação para grupos que usam status personalizados

Para facilitar o gerenciamento de fluxos de trabalho exclusivos por parte dos grupos, agora é possível usar status personalizados específicos dos grupos nos processos de aprovação.

Anteriormente, um grupo não podia usar seus próprios status personalizados com seus processos de aprovação específicos do grupo. Somente os status de todo o sistema estavam disponíveis e nem sempre se encaixavam nos processos de aprovação de grupo.

Os status personalizados agora podem ser usados em processos de aprovação de uso único e de todo o sistema:

* Crie um processo de aprovação de uso único para um objeto (projeto, tarefa ou problema) e baseie-o nos status associados ao grupo que está trabalhando nesse objeto. Isso inclui todos os status personalizados associados ao grupo.
* Crie um processo de aprovação global e o disponibilize somente para o grupo ou para todos no sistema.

Para usuários com acesso administrativo a processos de aprovação, as informações sobre como configurar processos de aprovação estão disponíveis em [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) (ou se você estiver usando o Adobe Workfront Classic, consulte [Criação de Processos de Aprovação](https://one.workfront.com/s/article/Creating-Approval-Processes-1001577410)).

Para usuários, as informações sobre como associar processos de aprovação a itens de trabalho estão disponíveis em [Associar um processo de aprovação novo ou existente ao trabalho](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) (ou se você estiver usando o Adobe Workfront Classic, consulte [Associando um Processo de Aprovação Novo ou Existente ao Trabalho](https://one.workfront.com/s/article/Associating-a-New-or-Existing-Approval-Process-with-Work-708455630)).

**Disponível nestes ambientes:**

* Adobe Workfront Classic
* A nova experiência do Adobe Workfront

## Uma maneira mais conveniente de atualizar alocações no Balanceador de carga de trabalho

Para facilitar o gerenciamento das alocações de um usuário para um item de trabalho no Balanceador de carga de trabalho, clique duas vezes no item de trabalho. Você também pode usar a opção existente do menu Editar alocações. Além disso, não é mais necessário ativar a exibição de alocações para poder atualizá-las.

Para obter informações sobre como gerenciar alocações no Balanceador de carga de trabalho, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Atualizar horas planejadas da tarefa no Balanceador de carga de trabalho

>[!NOTE]
>
>Esse aprimoramento estará disponível na Produção logo após a versão 2020.2.

Uma nova opção na área Gerenciamento de recursos do nível de acesso agora permite que os usuários com esse acesso editem Horas planejadas no Balanceador de carga de trabalho. Quando você ajusta alocações no Balanceador de carga de trabalho, o total de alocações diárias não precisa corresponder ao número de Horas planejadas das tarefas. Depois que você salvar as alocações, o total de horas de alocação se tornará as Horas planejadas da tarefa. Isso só é possível para tarefas que tenham um Tipo de duração simples.

Para obter informações sobre como gerenciar alocações no Balanceador de carga de trabalho, consulte [Gerenciar alocações de usuário no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Para obter informações sobre como conceder acesso ao Gerenciamento de Recursos, consulte [Conceder acesso ao Gerenciamento de Recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Remoção do rótulo &quot;beta&quot; do Balanceador de carga de trabalho

Com a versão 2020.2, o Balanceador de carga de trabalho não estará mais em um estado beta e você poderá usar o Balanceador de recursos para revisar e gerenciar suas atribuições e alocações de recursos. O rótulo &quot;beta&quot; foi removido no ambiente de Pré-visualização. Essa mesma alteração será feita na versão de produção 20.2. Para obter informações sobre o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
