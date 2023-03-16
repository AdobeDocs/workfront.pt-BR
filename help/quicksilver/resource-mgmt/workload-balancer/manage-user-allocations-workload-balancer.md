---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Gerenciar alocações de usuários no Balanceador de Carga de Trabalho
description: Como Gerenciador de Recursos, você pode atribuir trabalho aos usuários e gerenciar suas alocações diárias, semanais ou mensais do Balanceador de Carga de Trabalho.
author: Alina
feature: Resource Management
exl-id: 9649e482-af24-4516-9a69-ef12b2f1d579
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '2785'
ht-degree: 0%

---

# Gerenciar alocações de usuários no Balanceador de Carga de Trabalho

Como Gerenciador de Recursos, você pode atribuir trabalho aos usuários e gerenciar suas alocações diárias, semanais ou mensais do Balanceador de Carga de Trabalho para garantir que lhes seja alocada uma quantidade de horas que se ajuste às programações disponíveis.

## Requisitos de acesso {#access-requirements}

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Planejar, ao usar o Balanceador de Carga de Trabalho na área Recursos</p>
   <p>Trabalhe, ao usar o Balanceador de Carga de Trabalho de uma equipe ou projeto</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração de nível de acesso*</td> 
   <td> <p>Edite o acesso ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Tarefas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribua com permissões ou superiores que incluem Fazer atribuições nas tarefas e problemas para os quais você deseja gerenciar alocações. </p> <p>Ou </p> <p>Gerencie permissões das tarefas para as quais deseja atualizar as Horas Planejadas, além de atualizar alocações. Para obter informações sobre como atualizar Horas Planejadas no Balanceador de Carga de Trabalho, consulte o <a href="#update-task-planned-hours-when-managing-user-allocations">Atualizar a tarefa Horas Planejadas ao gerenciar alocações de usuários</a> neste artigo. </p> <p>Para obter informações sobre permissões de tarefas, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md">Compartilhar uma tarefa </a><span> e para obter informações sobre permissões de problemas, consulte</span> <span href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md">Compartilhar um problema </a></span>. </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Entender alocações de usuário

As alocações de usuários são quantidades de horas que indicam o tempo que um usuário deve gastar em um determinado dia ou dia da semana, semana ou mês para concluir o item de trabalho. Eles estão incluídos nas Horas Planejadas do item de trabalho.

Este artigo descreve como atualizar alocações diárias, semanais ou mensais para usuários atribuídos a tarefas ou emissões. Para obter informações sobre o gerenciamento de alocações gerais para usuários e funções de jobs para tarefas, consulte [Gerenciar horas de alocação de usuários e funções em tarefas](../../manage-work/tasks/assign-tasks/manage-allocation-hours-on-tasks.md) .

* [Visão geral da alocação de usuários](#user-allocation-overview)
* [Critérios que redefinem alocações de usuários](#criteria-that-reset-user-allocations)

### Visão geral da alocação de usuários {#user-allocation-overview}

Você pode exibir a alocação de usuário como horas ou como um valor percentual no Balanceador de Carga de Trabalho. É possível ajustar horas ou porcentagens.

As alocações de usuários são incluídas no número de Horas Planejadas de um item de trabalho. Para obter informações sobre Horas Planejadas, consulte [Visão geral das Horas Planejadas](../../manage-work/tasks/task-information/planned-hours.md).

A tarefa Horas Planejadas é distribuída igualmente entre todos os dias dentro da Duração da tarefa para o usuário atribuído à tarefa. Por exemplo, se uma tarefa tiver uma Duração de 5 dias e um total de 10 Horas Planejadas, o número de alocações diárias para a tarefa será de 2 horas. A alocação semanal é de 10 horas. Isso significa que um usuário é alocado para trabalhar na tarefa por 2 horas por dia. No entanto, você pode alterar manualmente a alocação diária para o usuário usando o Balanceador de Carga de Trabalho.

>[!CAUTION]
>
>O Balanceador de Carga de Trabalho exibe somente até 1000 Horas Planejadas por item de trabalho e até 1000 dias da duração de um item. As alocações no Balanceador de Carga de Trabalho são exibidas como zero depois que o limite de 1000 horas ou 1000 dias é atingido. Recomendamos dividir tarefas em subtarefas menores para acomodar um número maior de Horas Planejadas ou para Durações superiores a 1000 dias.

Considere o seguinte ao localizar alocações diárias, semanais ou mensais para tarefas ou problemas no Balanceador de Carga de Trabalho:

* Você pode exibir alocações diárias, semanais e mensais dos usuários em seus itens de trabalho. Ative a visualização Semana ou Mês para exibir alocações semanais ou mensais.
* Você pode usar o Balanceador de Carga de Trabalho para modificar a alocação diária, semanal ou mensal dos usuários para as tarefas ou problemas. Para obter informações sobre como ajustar a exibição do Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   >[!NOTE]
   >
   >Recomendamos que você tome uma decisão sobre qual período (diário, semanal ou mensal) deseja sempre usar ao gerenciar alocações de usuários e não alternar entre eles para os mesmos itens de trabalho. A atualização de alocações semanais para o mesmo usuário para o qual você atualizou anteriormente alocações diárias altera a alocação diária para o usuário.

* Você pode atualizar alocações para dias úteis e não úteis.
* Os carimbos de data e hora para as Datas de Início e Conclusão Planejadas dos itens de trabalho, bem como o Agendamento do projeto, são importantes quando o Workfront calcula automaticamente a alocação diária da tarefa.

>[!INFO]
>
> Por exemplo, uma tarefa pode ter uma Duração de 2 dias e 2 horas planejadas e tem uma Hora de início planejada de 12:00 PM no primeiro dia da duração com um usuário e uma Programação de projeto que termina às 17:00 PM. A capacidade do usuário para o primeiro dia é de 5 horas. A capacidade do usuário para o segundo dia é de 8 horas (se a programação começar às 9h).
>
>O Workfront calcula a alocação das 2 horas nos 2 dias da duração usando a seguinte fórmula:
>
>
```
>
>   Daily allocation hours = (Total Planned Hours / Total of available hours) * Daily available hours
>```
>
>  Para nosso exemplo, as horas diárias de alocação para cada dia são:
>   
>  (2 / 13) * 5 = 0,77 horas de alocação para o primeiro dia
>
>  (2 / 13) * 8 = 1,23 horas de alocação para o segundo dia
>
>  Nos cálculos acima, 13 é o total de horas disponíveis para a tarefa: 5 + 8 = 13



* Dois usuários em fusos horários ou programações diferentes dos usuários atribuídos podem fazer com que os valores de alocação sejam exibidos de forma diferente para dois usuários que visualizam os mesmos itens de trabalho.

* Quando um usuário tiver tempo de folga programado, o dia ou a parte do dia será exibida em um plano de fundo cinza. Se o administrador do Workfront ativou a configuração Tempo de desativação do usuário na área Configuração para considerar o tempo de folga do usuário, as horas alocadas são movidas para o dia seguinte disponível na linha do tempo. Se a configuração estiver desativada, as horas alocadas permanecerão no dia marcado para o tempo de folga e o usuário será exibido como sobrealocado. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   >[!TIP]
   >
   >Se o tempo limite tiver sido marcado depois que o usuário foi atribuído a um item de trabalho, você deverá recalcular a linha do tempo do projeto para exibir a alocação movida. Para obter mais informações, consulte [Recalcular linhas do tempo do projeto](../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* Se houver vários usuários atribuídos à tarefa, a quantidade de Horas Planejadas será distribuída uniformemente para cada usuário primeiro e, em seguida, uniformemente para cada dia dentro da Duração da tarefa. Essa distribuição se torna a alocação de cada usuário para a tarefa.

   Por exemplo, os seguintes cenários podem existir:

   * Para uma tarefa com uma Duração de 2 dias e 10 Horas planejadas atribuídas a um usuário, a alocação diária para o usuário é de 5 horas para cada dia, por padrão.
   * Para uma tarefa com uma Duração de 2 dias e 10 Horas Planejadas atribuídas a dois usuários, a alocação diária para cada usuário é de 2,5 horas para cada dia, por padrão.

* Se uma tarefa ou problema for concluído antes da Data de Conclusão Planejada, o número de horas alocadas para os dias restantes será atingido e não contará para a alocação geral do usuário. Isso é exibido somente quando o ícone Mostrar alocações e a configuração Mostrar datas projetadas estão ativadas. Para obter mais informações sobre como ativar configurações no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   ![](assets/allocations-struck-through-highlighted-350x39.png)

* Quando um usuário é alocado em excesso, suas horas alocadas são exibidas com um fundo vermelho no campo do usuário.
* Quando o usuário está sub-alocado ou recebe uma quantidade igual de horas ao seu tempo disponível programado, as horas são exibidas com um plano de fundo azul.
* Você pode exibir a alocação dos usuários em uma exibição de gráfico na linha de usuário. Para obter informações sobre como ativar a exibição de gráfico para alocações de usuários, consulte a seção &quot;Navegar no Balanceador de Carga de Trabalho&quot; no artigo [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

   ![](assets/user-allocation-chart-350x237.png)

### Critérios que redefinem alocações de usuários {#criteria-that-reset-user-allocations}

Nem todas as alterações de tarefa acionam as alocações modificadas para redistribuir. No entanto, há certas ações que podem redefinir as alocações já ajustadas em seus recursos e redistribuí-las uniformemente para todos os dias durante a duração do item de trabalho para cada um dos destinatários.

>[!NOTE]
>
>Se você não tiver modificado a distribuição automática de alocações em itens de trabalho, as horas serão redistribuídas uniformemente entre todos os destinatários quando houver uma alteração no número de destinatários, na Duração de uma tarefa ou na quantidade de Horas Planejadas no item de trabalho.

* [Ações que redefinem alocações ajustadas](#actions-that-reset-adjusted-allocations)
* [Ações que não redefinem alocações ajustadas](#actions-that-do-not-reset-adjusted-allocations)

#### Ações que redefinem alocações ajustadas {#actions-that-reset-adjusted-allocations}

As seguintes ações redefinem ou modificam as alocações diárias, semanais ou mensais para os usuários depois que você as tiver ajustado manualmente conforme descrito na [Modificar alocações de usuário](#modify-user-allocations) neste artigo:

* Quando você reduz o comprimento de um item de trabalho que reduz a quantidade de dias em sua Duração, as horas alocadas ajustadas dos dias perdidos são adicionadas à quantia de alocação do último dia do item de trabalho.
* Quando você altera a quantidade de Horas Planejadas em uma atribuição ou no item de trabalho, o novo número de Horas Planejadas é redistribuído uniformemente para toda a Duração do item de trabalho.
* Quando você adiciona ou remove um destinatário a um item de trabalho e isso faz com que as Horas Planejadas da tarefa sejam alteradas, os valores ajustados são redistribuídos uniformemente.

#### Ações que não redefinem alocações ajustadas {#actions-that-do-not-reset-adjusted-allocations}

As seguintes alterações em um item de trabalho não acionam as alocações ajustadas para redefinir ou modificar:

* Quando você move os dias de um item de trabalho, mas a quantidade de dias na Duração não muda, os valores alocados ajustados permanecem os mesmos e movem-se para as novas datas.
* Quando você aumenta a Duração de um item de trabalho que aumenta o número de dias em sua Duração, as horas alocadas ajustadas permanecem as mesmas para os dias ajustados. Dias adicionais são adicionados ao item de trabalho com 0 horas alocadas.
* Quando você adiciona ou remove um destinatário a um item de trabalho e isso não faz com que as Horas Planejadas do item sejam alteradas, os valores ajustados permanecem os mesmos.

## Localizar Horas Planejadas no Balanceador de Carga de Trabalho

Você pode modificar as alocações de usuários para tarefas ou problemas usando o Balanceador de Carga de Trabalho ao localizar as Horas Planejadas das tarefas ou problemas atribuídos aos usuários.

Considere o seguinte ao exibir as Horas Planejadas no Balanceador de Carga de Trabalho:

* O total de Horas Planejadas para uma tarefa ou um problema é exibido ao lado do Nome da Tarefa ou do Problema à esquerda do Balanceador de Carga de Trabalho.

* O total de Horas Planejadas de um projeto é exibido ao lado do Nome do Projeto, à esquerda do Balanceador de Carga de Trabalho. Representa o total de Horas Planejadas para todas as tarefas e problemas listados no projeto no Balanceador de Carga de Trabalho e não todas as Horas Planejadas do projeto.
* O tempo alocado diário ou semanal para todas as tarefas e para todos os projetos é exibido somente quando você ativa manualmente a configuração Mostrar alocações . Para obter informações sobre como ativar configurações no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Modificar alocações de usuário {#modify-user-allocations}

Como parte da atribuição de trabalho aos usuários, você pode modificar as alocações de usuários no Balanceador de Carga de Trabalho para garantir que eles nunca sejam sobrealocados ou para garantir um equilíbrio preciso de horas entre seus recursos. Para obter informações sobre como identificar se um usuário está sobrealocado, consulte a seção [Visão geral da alocação de usuários](#user-allocation-overview) neste artigo.

1. Assegure-se de ter tarefas e problemas atribuídos aos usuários. Para obter informações sobre como atribuir trabalho a usuários no Balanceador de Carga de Trabalho, consulte [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).
1. Vá para o Balanceador de Carga de Trabalho .
1. (Opcional) Clique em **Semana** ou **Mês** para gerenciar alocações semanais ou mensais para usuários.

   ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

1. No **Trabalho Atribuído** , localize o usuário para o qual deseja modificar manualmente a alocação e clique na seta apontando para a direita à esquerda do nome de usuário para expandir o usuário.

   ![](assets/wb-highlight-on-name-caret-350x106.png)

1. Clique na seta apontando para a direita à esquerda do nome do projeto para expandir o projeto e exibir os itens de trabalho aos quais o usuário está atribuído.

   >[!TIP]
   >
   >Você pode modificar alocações de usuários somente para tarefas e problemas. Não é possível modificar alocações de usuários para projetos.

1. (Opcional) Clique no botão **Ícone Mostrar alocações** ![](assets/show-allocations-icon-small.png) para exibir alocações para todos os itens de trabalho.

   O nome das tarefas e dos projetos é substituído pela alocação do usuário para a tarefa ou projeto.

1. (Opcional) Clique no botão **Configurações** ícone ![](assets/gear-icon-settings.png) e selecione qualquer uma das seguintes opções:

   1. **Incluir horas de problemas**. Isso permite gerenciar alocações de emissão além de alocações de tarefa.
   1. **Mostrar o trabalho concluído** . Isso exibe itens que foram concluídos e programados durante a linha do tempo para a qual você gerencia alocações.
   1. **Mostrar tempo restante** opção. O número total de horas para cada usuário (na linha de usuário) é alterado. Com essa configuração ativada, o Balanceador de Carga de Trabalho exibe as horas que cada usuário tem disponível para trabalhar em vez do número de horas para as quais está alocado.

      >[!TIP]
      >
      >Modificar alocações quando essa configuração está ativada faz com que o número total na linha do usuário diminua.

   1. **Projeto** no **Selecionar tema de cor** seção. Isso exibe cada projeto e seus respectivos itens de trabalho em cores exclusivas e facilita compreender quais itens pertencem a qual projeto.
   1. **Porcentagem** no **Exibir alocação de usuário em** seção. Isso exibe alocações como um valor percentual. A capacidade do usuário de acordo com o cronograma é considerada de 100%. Por exemplo, se um usuário estiver associado a um agendamento de 8 horas por dia, 8 horas serão iguais a 100% da capacidade. Se quiser alocar o usuário para trabalhar 4 horas em um dia, atualize sua alocação para 50%.

      >[!NOTE]
      >
      >O administrador do Workfront decide qual programação usar em seu sistema para calcular a capacidade do usuário na área Gerenciamento de Recursos da Configuração. Para obter mais informações, consulte [Configurar preferências do Gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).


1. Clique no botão **Mais** menu ![](assets/qs-more-menu.png) para um item de trabalho, clique em **Editar alocações**.

![](assets/more-menu-on-task-wb-nwe.png)

Ou

Clique duas vezes no dia, semana ou mês na barra de uma tarefa ou problema.

As caixas de alocação se tornam editáveis.

1. Clique dentro da caixa de cada alocação diária, semanal ou mensal para atualizar manualmente a quantidade de horas ou o valor percentual para o qual você deseja que o usuário seja alocado a cada dia, semana ou mês e clique no botão **Salvar** ícone ![](assets/checkmark-icon.png).

   >[!TIP]
   >
   >Clique no botão **Cancelar** ícone ![](assets/cancel-allocations-wb.png) para remover as alocações que você ajustou.

   ![](assets/wb-contouring-with-check-and-x-boxes-350x63.png)

   As alocações para a atualização do usuário.

   >[!TIP]
   >
   >Se uma tarefa ou problema for concluído antes da Data de Conclusão Planejada, o número de horas alocadas para os dias restantes será atingido e não contará para a alocação geral do usuário. Isso é exibido somente quando o ícone Mostrar alocações e a configuração Mostrar datas projetadas estão ativadas.

   Os seguintes cenários existem:

   * Para tarefas com Tipos de duração que não são Simples ou para problemas, o total das alocações deve corresponder à tarefa Horas planejadas antes de você poder clicar no ícone de marca de seleção.
   * Para tarefas com um Tipo de duração simples, o total de alocações pode ser maior ou menor do que as Horas planejadas e você pode clicar no ícone de marca de seleção mesmo que elas não correspondam. Isso também atualiza a quantidade de Horas Planejadas para a tarefa. Você deve ter as permissões corretas e o acesso para atualizar as Horas Planejadas nas tarefas do Balanceador de Carga de Trabalho.

      >[!TIP]
      >
      >Um ícone de cadeado é exibido à direita do nome da tarefa quando você começa a ajustar suas alocações para indicar que a tarefa tem um Tipo de duração simples.

      ![](assets/lock-icon-on-simple-task-in-the-balancer-350x119.png)
   Para obter mais informações sobre as condições que precisam ser atendidas para atualizar Horas Planejadas no Balanceador de Carga de Trabalho, consulte a seguinte seção neste artigo: [Atualizar a tarefa Horas Planejadas ao gerenciar alocações de usuários](#update-task-planned-hours-when-managing-user-allocations). Para obter informações sobre os Tipos de duração da tarefa, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. (Condicional) Se a tarefa for atribuída a mais de um usuário, repita essas etapas para cada usuário atribuído à tarefa para atualizar as alocações para cada usuário.

   Qualquer pessoa que tenha acesso para visualizar o Balanceador de Carga de Trabalho e visualizar os mesmos usuários e os mesmos projetos que você gerenciou agora visualiza a alocação atualizada para os usuários que você gerenciou.

## Atualizar a tarefa Horas Planejadas ao gerenciar alocações de usuários {#update-task-planned-hours-when-managing-user-allocations}

Você pode atualizar as Horas Planejadas de uma tarefa ao gerenciar alocações de usuários no Balanceador de Carga de Trabalho para a tarefa. Isso acontece quando o total de horas alocadas atualizadas não corresponde ao total original de Horas Planejadas para uma tarefa.

>[!IMPORTANT]
>
>* Atualizar as Horas Planejadas para tarefas pode afetar o progresso do projeto.
>* A atualização manual de Horas planejadas alterando alocações diárias pode ter impacto nas Horas Planejadas ao remover atribuições das tarefas no futuro. Para obter mais informações, consulte [Visão geral das Horas Planejadas](../../manage-work/tasks/task-information/planned-hours.md).
>
>* Não é possível atualizar Horas Planejadas para problemas atualizando alocações no Balanceador de Carga de Trabalho.
>


Isso é possível quando existem as seguintes condições:

* Você tem as permissões corretas e o acesso para gerenciar as Horas Planejadas no Balanceador de Carga de Trabalho. Isso inclui:

   * Gerencie permissões para as tarefas.
   * Atualize as Horas Planejadas no acesso do Balanceador de Carga de Trabalho na área Gerenciamento de Recursos do Nível de Acesso.

   Para obter mais informações sobre o acesso necessário para usar o Balanceador de Carga de Trabalho, consulte a seguinte seção neste artigo: [Requisitos de acesso](#access-requirements) .

* A tarefa tem um Tipo de duração Simples.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the statement above might include other duration types in the future)</p>
  -->
