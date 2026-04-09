---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Criar atribuições avançadas
description: Você pode gerenciar atribuições de tarefas ou problemas usando Atribuições Avançadas.
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 676cd1697ae2f379a699075f4e1ab06886c6837a
workflow-type: tm+mt
source-wordcount: '3415'
ht-degree: 1%

---

# Criar atribuições avançadas

{{highlighted-preview}}

<!-- Audited: 11/2025-->

<!--remove the bullet indicated when we get rid of the new/old experience of editing tasks-->


<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

Você pode gerenciar atribuições de tarefas ou problemas usando Atribuições Avançadas.

Você pode ajustar as seguintes informações de atribuição ao fazer atribuições avançadas:

* Atribuir usuários à tarefa ou problema (isso pode ser feito fora de uma atribuição avançada).
* Ajuste e redistribua o número de horas que cada destinatário é alocado.
* Determine qual usuário deve ser designado como o proprietário ou o Principal responsável pela tarefa ou problema.
* Especifique qual função cada usuário está cumprindo ao trabalhar na tarefa ou problema.
* <span class="preview">Adicionar informações de cobrança e de taxa de custo no nível de atribuição.</span>
* <span class="preview">Revise os seguintes detalhes para cada atribuição: horas planejadas, custo total e receita total.</span>

>[!NOTE]
>
>Ao atribuir usuários para trabalhar, sua disponibilidade de acordo com seus agendamentos afeta as Datas Planejadas e Projetadas de tarefas e problemas. Para obter informações sobre agendamentos, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Áreas do Adobe Workfront em que você pode fazer atribuições avançadas

Este artigo descreve como acessar Atribuições avançadas no cabeçalho da tarefa ou do problema.

Além disso, você pode fazer atribuições avançadas nas seguintes áreas do Workfront:

* Em listas e relatórios quando o campo Atribuições é exibido na visualização.
* Na seção Atribuições ao editar uma tarefa. Para obter mais informações, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md). <!--When we remove the old/ new experience: take this bullet out completely; in the new Edit Task experience, this is no longer possible-->
* No cabeçalho da tarefa ou do problema, na área Atribuições.
* No Balanceador de carga de trabalho. Para obter mais informações, consulte [Atribuir trabalho manualmente usando o Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Para adicionar taxas de faturamento e de custo em atribuições de tarefa e usar a pesquisa avançada: Ultimate do Workflow</p> <p>Para criar atribuições avançadas: Qualquer pacote do Workfront ou Workflow</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p>
   <p>Trabalho ou maior</p>
   </td> 
  </tr> 
  <tr> 
   <td role>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e problemas</p>  </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Contribuir com permissões ou permissões superiores para a tarefa ou problema</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<div class="preview">

## Criar atribuições avançadas - Pacote de fluxo de trabalho do Ultimate

Este layout de Atribuições Avançadas se aplica somente a tarefas. Para problemas, consulte [Criar atribuições avançadas - todos os outros pacotes](#create-advanced-assignments--all-other-packages).

1. Vá para o projeto ao qual deseja atribuir uma tarefa.
1. Clique em **Tarefas** ou **Problemas** no painel esquerdo e, em seguida, clique no nome de uma tarefa na lista.

   >[!TIP]
   >
   >Você pode fazer atribuições avançadas diretamente na lista de tarefas. Clique dentro do campo **Atribuições** na mesma linha da tarefa e clique em **Avançadas** na parte inferior da lista ou no **ícone Pessoas** no canto superior direito da caixa de atribuições, para abrir a janela Atribuições Avançadas. Vá para a etapa 5 para continuar criando atribuições avançadas.
   >![Clique no ícone Avançado ou Pessoas](assets/access-aa-from-lists.png)

1. Clique em **Atribuir a** no campo **Atribuições** no cabeçalho da tarefa

   Ou

   Clique em um dos nomes atribuídos se a tarefa já estiver atribuída.

1. Clique em **Avançado**.

   ![Clique em Avançado](assets/assignments-from-task-header-0825.png)

   A janela Atribuições Avançadas é exibida.

   ![Janela Atribuições Avançadas](assets/advanced-assignments-031826.png)

1. Revise as informações de duração da tarefa conforme necessário. Todos esses campos são somente para visualização de Atribuições avançadas e você pode atualizá-los na tarefa.

   Para obter informações sobre a duração da tarefa, os tipos de duração, as unidades de tempo e as horas planejadas, consulte [Visão Geral da Duração e do Tipo de Duração da Tarefa](/help/quicksilver/manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   >[!NOTE]
   >
   >Se uma coluna de dados que você deseja exibir não for exibida, você poderá adicioná-la. Consulte [Adicionar e remover colunas na lista de atribuições avançadas](#add-and-remove-columns-on-the-advanced-assignments-list) abaixo.

1. (Opcional) Selecione **Horas**, **FTE** ou **Percentual** para exibir as alocações.

   Você pode ver quanto um usuário é atribuído em horas planejadas, como uma porcentagem de sua capacidade, ou em FTE (equivalente em tempo integral, escala 0-1). A configuração padrão é Horas.

   Para obter informações sobre FTE, consulte [Configurar preferências de Gerenciamento de Recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

1. Clique em **Nova linha** para adicionar uma atribuição à tarefa.

1. Clique na coluna **Atribuído** para adicionar um usuário ou uma equipe. Comece a digitar o nome do usuário ou da equipe e clique no nome quando ele aparecer na lista suspensa.

   >[!NOTE]
   >
   >Se o nome contiver um caractere especial, você deverá incluí-lo no campo de pesquisa.

   Quando você adiciona um usuário que tem uma função de trabalho primária, a **Função do destinatário** é preenchida.

   Se o usuário tiver atributos atribuídos a seu perfil, os atributos serão preenchidos na atribuição da tarefa.

1. Para adicionar uma função de trabalho quando não souber o usuário que trabalhará na tarefa, clique na coluna **Função do destinatário**. Comece digitando o nome da função de trabalho e clique no nome quando ele aparecer na lista suspensa.

   >[!NOTE]
   >
   >Se o nome contiver um caractere especial, você deverá incluí-lo no campo de pesquisa.

   Se a função de trabalho tiver atributos atribuídos a partir do cartão de taxa de um projeto, os atributos serão preenchidos na atribuição da tarefa.

   Ao atribuir um usuário posteriormente usando o campo Destinatário, a pesquisa básica segue este algoritmo:

   * Correspondência completa: função de trabalho e todos os atributos
   * Correspondência parcial: função de trabalho e alguns atributos
   * Somente correspondência da função de trabalho

   Para obter informações sobre a pesquisa avançada, consulte [Usar a pesquisa avançada](#use-the-advanced-search) neste artigo.

1. (Opcional) Continue adicionando atribuídos em novas linhas para adicionar vários recursos à tarefa.

   >[!TIP]
   >
   >* Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos. É permitido um máximo de 200 atribuídos por tarefa.
   >
   >
   >* Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos.
   >Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
   >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
   >   
   >   * Reatribuir o item de trabalho aos recursos ativos.
   >   * Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.

1. Para marcar um destinatário como proprietário da tarefa, marque a caixa de seleção da linha e clique em **Definir principal** na barra de ações na parte inferior da janela Atribuições Avançadas.

   Por padrão, o Workfront marca o primeiro usuário ou função de trabalho que você atribuir a uma tarefa como o Proprietário ou a Atribuição principal. Uma equipe não pode ser designada como o Proprietário principal de uma tarefa.

   Se o Proprietário Principal da tarefa não for exibido, você poderá adicionar a coluna **É Primário** à tabela.

   >[!IMPORTANT]
   >
   >Dependendo de como o administrador do Workfront ou o administrador de grupo configuram as preferências do projeto, a Workfront pode usar o agendamento do proprietário da tarefa para calcular a linha do tempo da tarefa quando vários usuários estão atribuídos a ela. Para obter informações sobre vários atribuídos de tarefas, consulte a seção [Considerações para várias atribuições a funções de trabalho, equipes e usuários](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) no artigo [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

1. Para cada usuário na coluna **Destinatário**, especifique as seguintes informações:

   * (Opcional) **Função de trabalho para faturamento**: procure e selecione a função de trabalho para faturamento para este destinatário e tarefa específicos.

     A função de trabalho para faturamento é usada apenas nesta atribuição e não é aplicada automaticamente às outras atribuições do usuário. Por exemplo, a função de trabalho principal de um usuário é Designer, mas em uma tarefa ele está agindo como um Designer sênior e a taxa de cobrança deve refletir isso. A função de trabalho para faturamento se aplica somente a usuários e não pode ser usada em outras funções de trabalho.

     Quando uma função de trabalho para faturamento é aplicada na atribuição do usuário, a taxa anexada à função de trabalho para faturamento pode ser usada em vez das taxas do usuário ou da função de trabalho nos cálculos de faturamento e receita.

     Uma função de trabalho no nível do projeto para faturamento também pode ser definida para um usuário, e esse valor é usado em todas as atribuições do usuário nesse projeto.

     Para obter mais informações, consulte [Configurar uma função de trabalho para cobrança](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

   * **Alocação**: quando o Tipo de Duração de uma tarefa é Simples, especifique o número de horas que cada usuário ou função de trabalho deve ser atribuída à tarefa. A soma de todas as horas atribuídas para cada usuário é igual ao número no campo **Horas planejadas**, na parte superior da janela Atribuições avançadas. Em todos os outros casos, especifique a porcentagem de tempo (ou alocação) que você deseja que o destinatário passe resolvendo a tarefa.

     >[!TIP]
     >
     >Depois de modificar manualmente as alocações de atribuição em tarefas, as Horas Planejadas das tarefas podem ser atualizadas de acordo. Observe que não é possível modificar manualmente as alocações de equipes atribuídas a tarefas. Para obter mais informações, consulte a seção [Atualizar horas planejadas da tarefa ao gerenciar alocações de usuário](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) no artigo [visão geral das horas planejadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

   * **Atributos**: todos os atributos disponíveis para o usuário são mostrados nos campos de atributo. O administrador configura os atributos e eles são adicionados ao perfil do usuário ou associados a uma função de trabalho em um cartão de taxa. Para obter mais informações, consulte [Definir atributos de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) e [Editar perfil de usuário](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Atualmente, os atributos são somente leitura nas atribuições do usuário. Eles podem ser editados para funções de trabalho.

   * **Moeda da taxa**: a moeda para as taxas de custo e cobrança é assumida como padrão do projeto, mas você pode alterar a moeda dessa atribuição.

   * (Opcional) **Taxa de cobrança**: a taxa de cobrança pode vir de outras áreas do sistema, como cartões de taxa. Para obter mais informações, consulte [Visão geral da hierarquia de receita e custo](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). Você pode sobrepor manualmente a taxa de faturamento para essa atribuição específica nesse campo e ela sobreporá todas as outras taxas para o usuário nos cálculos de receita.
   * (Opcional) **Taxa de custo**: a taxa de custo pode vir de outras áreas do sistema. Para obter mais informações, consulte [Visão geral da hierarquia de receita e custo](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). Você pode sobrepor manualmente a taxa de custo para essa atribuição específica nesse campo e ela sobreporá todas as outras taxas para o usuário nos cálculos de custo.
   * **É Faturável**: selecione essa opção para incluir a atribuição em cálculos financeiros. Desmarque esta opção para excluir a atribuição dos cálculos financeiros.

     Este campo fica ativado por padrão para todas as atribuições quando a tarefa tem um tipo de receita.

1. (Opcional) Para exibir dados de atribuição por data para um usuário ou função, selecione a linha de tabela e clique em **Exibir por datas** na barra de ações na parte inferior da janela Atribuições Avançadas. Para obter mais informações, consulte [Exibir dados de atribuição por datas](#view-assignment-data-by-dates) neste artigo.
1. (Opcional) Para excluir uma ou mais atribuições da lista, marque a caixa de seleção para cada linha e clique em **Excluir** na barra de ações na parte inferior da janela Atribuições Avançadas.
1. Clique em **Salvar** ou **Salvar e fechar** quando terminar de editar as Atribuições Avançadas.

### Adicionar e remover colunas na lista Atribuições Avançadas

Os campos devem existir para que você possa adicioná-los à lista.

1. Clique em **+** na parte superior direita da lista para abrir o **Gerenciador de colunas**.

   ![Gerenciador de Coluna de Atribuições Avançadas](assets/aa-column-manager.png)

1. Selecione a guia **Propriedades** ou a guia **KPIs** para escolher o tipo de campo que deseja adicionar.

   Propriedades como localização ou centro de custo fornecem informações contextuais. KPIs divididos em fase no tempo, como valores de receita ou divisão de custo em períodos.

1. Procure um campo de objeto existente na seção **Disponível** e clique em **+** à direita do nome do campo para adicioná-lo à coluna **Selecionado**.
1. Clique em **-** à direita de um campo na seção **Selecionado** para removê-lo da lista.
1. Clique em **Salvar**.

   Para obter mais informações sobre o Gerenciador de colunas, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Aplicar uma exibição à lista de Atribuições Avançadas

Uma exibição é um conjunto personalizado de disposições de coluna que você pode aplicar à lista.

1. Clique na lista suspensa **Exibições** e selecione o modo de exibição que deseja aplicar à lista.

   **Exibições do Sistema** são exibições que o administrador do sistema adicionou e não podem ser alteradas. **Minhas Exibições** são exibições criadas por você ou compartilhadas com você.

1. Clique em **Nova exibição** na lista suspensa **Exibições** para criar uma exibição.

   Ao adicionar, remover ou reordenar as colunas, as alterações são salvas na exibição automaticamente. Na próxima vez que você aplicar essa visualização, as colunas permanecerão da maneira como você as define.

   Para obter mais informações sobre exibições, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Usar a Pesquisa avançada

A pesquisa avançada ajuda a localizar o usuário ou função de trabalho corretos para adicionar à atribuição.

1. Para abrir a janela de pesquisa avançada, siga um destes procedimentos:

   * Clique em **Pesquisa avançada** na parte superior direita da janela Atribuições avançadas.
   * Selecione uma linha de atribuição e clique em **Pesquisa avançada** na barra de ações na parte inferior da janela Atribuições avançadas. Isso abre a pesquisa avançada com filtros aplicados automaticamente para essa atribuição específica.

1. Selecione a guia Usuários ou Funções na janela de pesquisa avançada.
1. Aplique filtros conforme necessário:

   1. Clique em **Filtro** acima da lista.
   1. Na caixa Filtro, clique em **Adicionar condição**.
   1. Selecione um campo para filtrar.
   1. Selecione um modificador de filtro, como &quot;Tem qualquer um de&quot;, &quot;Não tem nenhum de&quot;, &quot;É antes&quot; ou &quot;É depois de&quot;. As opções do modificador são diferentes dependendo do tipo de campo pelo qual você está filtrando.
   1. Selecione o valor ou os valores do campo. Dependendo do tipo de campo pelo qual você está filtrando, talvez seja solicitado que você selecione o item em uma lista, pesquise por ele ou use um calendário para selecionar um intervalo de datas.

   O filtro é aplicado automaticamente à lista. Para obter mais informações sobre filtros, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

1. Procure por uma função de trabalho ou usuário.

   Ao procurar um usuário que corresponde a uma atribuição de função de trabalho, somente correspondências completas (função de trabalho e todos os atributos) são exibidas.

1. Clique em **+** para adicionar colunas à tabela. Para obter mais informações, consulte [Adicionar e remover colunas na lista de atribuições avançadas](#add-and-remove-columns-on-the-advanced-assignments-list).
1. Selecione um ou mais usuários ou funções de trabalho e clique em **Adicionar usuários** ou **Adicionar funções** na barra de ações na parte inferior da janela.

   As atribuições são adicionadas na janela Atribuições Avançadas.

### Exibir dados de atribuição por datas

A janela **Exibir por datas** para Atribuições Avançadas mostra todo o histórico de data efetiva da atribuição para um usuário ou função específica. As alterações passadas e futuras são exibidas.

Exemplos de itens de data de efetivação que poderiam afetar o histórico de atribuições são:

* Funções de trabalho principais/outras do usuário
* Função de trabalho no nível do projeto para faturamento
* Taxas de custo/cobrança de perfil de usuário
* Substituir taxas de custo/cobrança de projeto (usuário ou função de trabalho)
* Taxas de cartão de taxa por função/atributos de trabalho
* Atributos de Usuário
* Agendamento do usuário

Observe que essa não é uma lista abrangente e o campo que foi alterado não é necessariamente exibido na tabela de dados de atribuição, mas afeta as taxas de faturamento e de custo ou os atributos do usuário ou da função de trabalho.

Você só pode exibir dados de atribuição por datas para um único usuário ou função.

1. Selecione a linha de tabela de um usuário ou função e clique em **Exibir por datas** na barra de ações, na parte inferior da janela Atribuições avançadas.

   A janela **Exibir por datas** é exibida. Os dados são somente leitura.

   Cada linha na tabela representa uma alteração de data efetiva na atribuição. Se não houver alterações na data de efetivação, a tabela terá uma linha mostrando os dados atuais. Os campos destacados apontam o que mudou e as datas de início e término de cada atualização estão listadas. Por exemplo, se a taxa de faturamento tiver mudado de 202 em 20 de agosto para 205 em 21 de agosto, a taxa será destacada. O texto entre parênteses indica onde a alteração foi feita na taxa, como um projeto.

   ![Exibir por janela de datas](assets/resource-changes-view-by-dates.png)

   Quando terminar de revisar os dados, clique na seta na parte superior esquerda para retornar à janela Atribuições Avançadas.

</div>

## Criar atribuições avançadas - todos os outros pacotes

Esse layout de Atribuições avançadas se aplica a tarefas e problemas.

1. Vá para o projeto ao qual deseja atribuir uma tarefa ou um problema.
1. Clique em **Tarefas** ou **Problemas** no painel esquerdo e, em seguida, clique no nome de uma tarefa ou problema na lista.

   >[!TIP]
   >
   >Você pode fazer atribuições avançadas diretamente na lista de tarefas ou problemas. Clique dentro do campo **Atribuições** na mesma linha da tarefa ou do problema e clique em **Avançadas** na parte inferior da lista ou no **ícone Pessoas** no canto superior direito da caixa de atribuições, para abrir a janela Atribuições Avançadas. Vá para a etapa 5 para continuar criando atribuições avançadas.
   >![Clique no ícone Avançado ou Pessoas](assets/access-aa-from-lists.png)

1. Clique em **Atribuir a** no campo **Atribuições** no cabeçalho da tarefa ou problema

   Ou

   Clique em um dos nomes atribuídos se a tarefa ou problema já tiver sido atribuído.

1. Clique em **Avançado**.

   ![Clique em Avançado](assets/assignments-from-task-header-0825.png)

1. No campo **Pesquisar pessoas, funções e equipes**, comece digitando o nome de um usuário, função ou equipe, em seguida, clique no nome quando ele aparecer na lista suspensa.

   >[!NOTE]
   >
   >Se o nome do usuário contiver um caractere especial, você deverá incluí-lo no campo de pesquisa.

1. (Opcional) Continue adicionando atribuídos na caixa **Pesquisar pessoas, funções e equipes** para adicionar vários recursos à tarefa ou problema.

   >[!TIP]
   >
   >* Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
   >
   >
   >* Ao adicionar uma atribuição de usuário, observe o avatar, a função principal do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos.
   >Os usuários devem ser associados a pelo menos uma função de trabalho para visualizá-la à medida que forem adicionados.
   >Você deve ter a configuração Exibir informações de contato ativada no seu nível de acesso para que os usuários visualizem os emails dos usuários. Para obter informações, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
   >   
   >   * Reatribuir o item de trabalho aos recursos ativos.
   >   * Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.

1. Para cada usuário na coluna **Destinatário**, especifique as seguintes informações:

   * **Proprietário**: passe o mouse sobre o nome do destinatário e clique em **Tornar primário** no campo Proprietário se desejar marcar o destinatário como o proprietário da tarefa ou do problema. Uma caixa de seleção verde indica que o usuário especificado é o contato principal da tarefa ou problema. O Adobe Workfront marca o primeiro usuário ou função de trabalho atribuída a uma tarefa ou problema como Proprietário ou Atribuição principal. Uma equipe não pode ser designada como o Proprietário principal de uma tarefa ou problema.

     >[!IMPORTANT]
     >
     >Dependendo de como o administrador do Workfront ou o administrador de grupo configuram as preferências do projeto, a Workfront pode usar o agendamento do proprietário da tarefa para calcular a linha do tempo da tarefa quando vários usuários estão atribuídos a ela. Para obter informações sobre vários atribuídos de tarefas, consulte a seção [Considerações para várias atribuições a funções de trabalho, equipes e usuários](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) no artigo [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Alocações**: quando o Tipo de Duração de uma tarefa for Simples, especifique o número de horas que cada usuário ou função de trabalho deve ser atribuída à tarefa. A soma de todas as horas atribuídas para cada usuário é igual ao número no campo **Horas planejadas**, na parte inferior da coluna Alocações. Em todos os outros casos, especifique a porcentagem de tempo (ou alocação) que você deseja que o destinatário passe resolvendo a tarefa ou problema.

     >[!TIP]
     >   
     >   * Depois de modificar manualmente as alocações de atribuição em tarefas, as Horas Planejadas das tarefas podem ser atualizadas de acordo. Para obter mais informações, consulte a seção [Atualizar horas planejadas da tarefa ao gerenciar alocações de usuário](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) no artigo [visão geral das horas planejadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).
     >   * Não é possível modificar manualmente as alocações de atribuição em ocorrências.
     >   * Não é possível modificar manualmente as alocações de equipes atribuídas a tarefas.

   * **Função do destinatário:** selecione a função que o usuário deve usar ao realizar esta atribuição.  A Função principal do usuário é exibida por padrão. Clique na caixa **Função do destinatário** para selecionar outra função. Ao atribuir a tarefa ou o problema a uma função primeiro e, em seguida, adicionar um usuário que pode desempenhar essa função como uma segunda atribuição, a lista de usuários sugeridos é filtrada para os usuários que podem desempenhar as funções já atribuídas à tarefa e ao problema.

     ![Função do destinatário](assets/advanced-assignments-select-role.png)

   * **Tipo de Duração**: somente disponível para tarefas. Clique no nome do Tipo de duração e selecione um Tipo de duração no menu suspenso. Para obter informações sobre Tipos de Duração, consulte [Visão Geral da Duração e do Tipo de Duração da Tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duração:** é possível atualizar este campo para uma tarefa quando você tem permissões para Gerenciar a tarefa.

     Para obter mais informações, consulte [Visão geral da duração e do tipo de duração da tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Ao editar informações de atribuição em massa, uma caixa de diálogo semelhante é exibida para atribuir usuários, horas, alocação e proprietário da tarefa.

   * **Horas planejadas**: quando o tipo de duração for Atribuição calculada ou Simples, atualize o número de Horas planejadas. Como resultado, as porcentagens de alocação ou as horas de cada recurso são distribuídas uniformemente. O Workfront calcula as horas planejadas quando o tipo de duração é Trabalho calculado ou orientado pelo esforço. Para obter mais informações, consulte [Visão geral da duração e do tipo de duração da tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. Clique em **Salvar**.


