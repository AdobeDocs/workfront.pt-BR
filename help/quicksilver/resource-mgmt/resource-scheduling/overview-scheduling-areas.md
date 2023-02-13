---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Visão geral das áreas de Agendamento
description: As seções a seguir descrevem onde você pode acessar a área de agendamento no Adobe Workfront, bem como a funcionalidade disponível na área de agendamento.
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# Visão geral das áreas de Agendamento

>[!IMPORTANT]
>  
><span class="preview">A funcionalidade de Agendamento descrita neste artigo foi descontinuada e removida do Adobe Workfront a partir da versão 23.1 em janeiro de 2023.   </span>
>  
> <span class="preview"> Este artigo também será removido logo após a versão 23.1, no início de 2023. Nesse momento, recomendamos que você atualize todos os marcadores adequadamente. </span>
> 
><span class="preview"> Agora você pode usar o Balanceador de Carga de Trabalho para agendar o trabalho de seus recursos. </span>
>  
> <span class="preview">Para obter informações sobre como programar recursos usando o Balanceador de Carga de Trabalho, consulte a seção [O Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--  

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->


As seções a seguir descrevem onde você pode acessar a área de agendamento no Adobe Workfront, bem como a funcionalidade disponível na área de agendamento.

## Áreas do Workfront que permitem agendar recursos

Você pode programar recursos nas seguintes áreas no Workfront:

* **Para quaisquer projetos para os quais você é o gerente de recursos** (do **Agendamento** (Área de agendamento no Workfront permite que os gerentes de recursos façam atribuições de recursos em vários projetos.

* **Para um projeto individual quando você é membro da equipe do projeto** (do **Agendamento** área de um projeto):

   A área Agendamento em um projeto permite que os membros da equipe do projeto atribuam trabalhos do projeto aos usuários da equipe do projeto.

* **Para uma equipe individual, você é membro de** (do **Agendar** seção da equipe) A seção Agendamento em uma equipe permite que os membros da equipe atribuam trabalhos já atribuídos à equipe de vários projetos a membros individuais da equipe.

## Funcionalidade disponível na área Agendamento

A área de programação exibe tarefas e problemas e atribuições de recursos atuais.\
![resource_scheduling_overview.png](assets/resource-scheduling-overview-350x237.png)

* [Ferramentas Filtrar e trocar](#filter-and-swap-tools)
* [Seleção de data](#date-selection)
* [Área não atribuída](#unassigned-area)
* [Usuários e funções](#users-and-roles)
* [Programação da linha do tempo](#scheduling-timeline)

### Ferramentas Filtrar e trocar {#filter-and-swap-tools}

* **Ferramenta Filtrar:** Permite filtrar o conteúdo exibido na linha do tempo do agendamento. Para obter mais informações sobre como usar a ferramenta Filtro, consulte [Filtrar informações na área Agendamento](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **Ferramenta Trocar:** (Disponível somente ao agendar recursos para projetos na guia Agendamento ou na guia Pessoal) Permite atribuir, trocar ou cancelar a atribuição de usuários rapidamente a tarefas em vários projetos. Para obter mais informações, consulte [Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Seleção de data {#date-selection}

É possível ajustar o intervalo de datas cujos dados são exibidos na linha do tempo do agendamento. Por padrão, o intervalo de datas é de 2 semanas (14 dias consecutivos, incluindo fins de semana), começando no dia atual.

### Área não atribuída {#unassigned-area}

* [Ao programar recursos como o gerenciador de recursos (para vários projetos na área Agendamento)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Ao programar recursos como membro da equipe do projeto (de um projeto)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Ao programar recursos como membro da equipe (de uma equipe)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Ao programar recursos como o gerenciador de recursos (para vários projetos na área Agendamento) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

O **Não atribuído** na linha do tempo de programação exibe somente as tarefas e os problemas que atendem a todos os seguintes critérios:

* Não atribuído a um usuário.
* Não atribuído a uma equipe.\
   Se a tarefa ou o problema for atribuído a uma equipe, ele ainda será exibido no **Não atribuído** área se a tarefa ou emissão também estiver atribuída a uma função além da atribuição da equipe.\
   Se tarefas ou problemas tiverem atribuições adicionais de função de trabalho que não estão sendo realizadas por um usuário, elas também serão exibidas.\
   Por exemplo, uma tarefa é atribuída a 3 funções de trabalho: Designer, Gerenciador de produtos e Desenvolvedor. Você atribui essa tarefa ao Usuário A, que tem uma função de trabalho no Designer, e ao Usuário B, que tem uma função de trabalho no Gerenciador de Produtos. Nesse cenário, a tarefa ainda está visível na área Não atribuído na linha do tempo de agendamento, pois a função de trabalho do Desenvolvedor não está atribuída a um usuário.

#### Ao programar recursos como membro da equipe do projeto (de um projeto) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

O **Não atribuído** área na parte superior da linha do tempo do agendamento exibe tarefas e problemas que atendem aos seguintes critérios:

* Associado ao projeto, mas não atribuído a nenhum usuário na equipe do projeto.\
   As tarefas que estão associadas ao projeto e são atribuídas a um usuário na equipe do projeto são exibidas na linha do usuário ao qual as tarefas são atribuídas.
* Associado ao projeto, mas atribuído a um membro que não faz parte da equipe do projeto.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **Ao programar recursos como membro da equipe (de uma equipe)** {#when-scheduling-resources-as-a-team-member-from-a-team}

O **Não atribuído** área na parte superior da linha do tempo do agendamento exibe tarefas e problemas que atendem aos seguintes critérios:

* Atribuído à equipe e a nenhum outro usuário da equipe.\
   As tarefas atribuídas à equipe e a um usuário na equipe são exibidas na linha do usuário ao qual as tarefas são atribuídas.
* Atribuído à equipe e a um usuário que não seja membro da equipe.

### Usuários e funções {#users-and-roles}

* [Ao programar recursos como o gerenciador de recursos (para vários projetos na área Agendamento)](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Ao programar recursos como membro da equipe do projeto (de um projeto)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Ao programar recursos como membro da equipe (de uma equipe)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Ao programar recursos como o gerenciador de recursos (para vários projetos na área Agendamento) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

Todos os usuários qualificados para receber uma das tarefas não atribuídas estão localizados abaixo do **Não atribuído** área. Os usuários estão disponíveis na linha do tempo de programação para receber uma tarefa ou problema nas seguintes circunstâncias:

* Por padrão, os usuários são exibidos na linha do tempo de agendamento somente quando têm uma função de trabalho definida no sistema (a função de trabalho primária ou uma função de trabalho secundária) e essa função de trabalho corresponde à função de trabalho atribuída a uma tarefa ou problema que está visível atualmente na **Não atribuído** na linha do tempo de programação. Você pode desativar essa funcionalidade para permitir que tarefas e problemas sejam atribuídos a qualquer usuário, independentemente de esse usuário ter uma função definida em seu perfil de usuário que corresponda à atribuição de função da tarefa ou problema que está sendo atribuído a ele. Para obter mais informações, consulte [Permitir atribuições de usuários independentemente da função e associação de grupo nas áreas de Programação](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   Um usuário e as tarefas atribuídas do usuário podem aparecer várias vezes na linha do tempo de agendamento se o usuário tiver várias funções de trabalho designadas no sistema Workfront.\
   Os usuários permanecem na linha do tempo de agendamento depois de receberem uma tarefa ou um problema, mesmo que não haja tarefas ou problemas restantes que tenham uma atribuição de função correspondente. Isso permite fazer as alterações necessárias após sua atribuição.\
   Se a tarefa não estiver atribuída a uma função de trabalho, todos os usuários que atenderem aos requisitos de filtro serão exibidos. Para obter mais informações sobre o filtro, consulte [Filtrar informações na área Agendamento](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* Foram designados para **Usuários** no campo **Filtro** guia .\
   Para obter mais informações sobre o filtro, consulte [Filtrar informações na área Agendamento](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   Ao programar recursos para uma equipe (na guia Trabalhando em ), a atribuição da equipe também é mostrada.

Quaisquer outras tarefas ou problemas atribuídos a esses usuários também são exibidos na linha do tempo.

Você pode ver o nível em que os usuários são alocados em um determinado dia, conforme descrito em [Gerenciar alocações de usuários nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Tarefas que você não tem pelo menos permissões do Contribute são exibidas como uma barra cinza na linha do tempo de agendamento.

#### Ao programar recursos como membro da equipe do projeto (de um projeto) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

Cada membro da equipe é sempre exibido na linha do tempo de programação, independentemente das atribuições de função de trabalho dos usuários e das atribuições de função das tarefas na área Não Atribuído.

Se um usuário tiver várias funções de trabalho definidas no sistema, ele aparecerá várias vezes na linha do tempo de programação quando um dos seguintes critérios for atendido:

* Há tarefas ou problemas exibidos na **Não atribuído** área atribuída às funções de trabalho associadas ao usuário.
* Há tarefas ou problemas no projeto que atribuíram funções de trabalho, e essas tarefas ou problemas são atribuídos a um usuário que tem essa função de trabalho definida no sistema.

#### Ao programar recursos como membro da equipe (de uma equipe) {#when-scheduling-resources-as-a-team-member-from-a-team-1}

Cada membro da equipe é sempre exibido na linha do tempo de programação, independentemente das atribuições de função de trabalho dos usuários e das atribuições de função das tarefas na área Não Atribuído.

Você pode ver o nível em que os usuários são alocados em um determinado dia, conforme descrito em [Gerenciar alocações de usuários nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Tarefas que você não tem pelo menos permissões do Contribute para exibir como uma barra cinza na linha do tempo de agendamento.

### Programação da linha do tempo {#scheduling-timeline}

* **Conteúdo padrão:** Por padrão, todas as tarefas que atendem aos requisitos definidos na seção [Pré-requisitos de tarefa e emissão](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) no [Introdução ao Agendamento de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) artigo sobre todos os projetos com o status Current são exibidos na linha do tempo de agendamento.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   Para personalizar o que é exibido na linha do tempo do agendamento, incluindo a exibição de problemas e projetos com um status diferente, use o filtro , conforme descrito em [Filtrar informações na área Agendamento](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   Um máximo de 10 tarefas por dia é exibido para um determinado usuário. Você pode expandir a lista para exibir todas as tarefas atribuídas a esse usuário no momento.

* **Tarefas principais:** Se as tarefas pai são exibidas na linha do tempo depende de várias configurações. Para obter mais informações, consulte a seção &quot;Configurar se as tarefas pai são exibidas na linha do tempo de agendamento&quot; no [Definir configurações nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) artigo 10. o

* **Codificação a cores:** As tarefas e os problemas na linha do tempo do agendamento são codificados por cores de acordo com o projeto ao qual pertencem. Não é possível personalizar a cor associada a um projeto específico.

   Ao agendar trabalho para equipes (na guia Pessoal ), as cores são usadas somente se a variável **Mostrar todas as tarefas do usuário** está ativada. Para obter mais informações, consulte a seção &quot;Configurar se as tarefas pai são exibidas na linha do tempo de agendamento&quot; no [Definir configurações nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) artigo 10. o

* **Duração da tarefa:** As durações da tarefa são representadas na linha do tempo de cada tarefa (a tarefa se estende fisicamente pelo número de dias igual à duração). Não é possível ajustar a duração da tarefa a partir da linha do tempo de agendamento.

* **Hora de desligar:** O tempo limite é representado na linha do tempo de programação por um indicador cinza-claro na coluna no dia em que o tempo limite é agendado para um determinado usuário.\
   O tempo limite é configurado para cada usuário com base nas seguintes informações:

   O calendário pessoal do usuário. Para obter mais informações sobre o calendário de tempo de folga pessoal, consulte [Configurar o horário pessoal no Adobe Workfront](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   O agendamento atribuído ao usuário. Pode ser o agendamento padrão ou personalizado. Para obter mais informações sobre programações, consulte [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Fim de semana:** Os finais de semana são representados na linha do tempo do agendamento como sombreamento cinza claro nos sábados e domingos. Os dias da semana definidos como finais de semana na linha do tempo de programação não são configuráveis. Você pode programar usuários para trabalhar nos finais de semana.
