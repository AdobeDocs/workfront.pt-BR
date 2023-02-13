---
product-area: resource-management;user-management
navigation-topic: resource-scheduling
title: Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento
description: Usando a linha do tempo de agendamento, você pode gerenciar atribuições de usuários, além de especificar quanto tempo cada usuário está alocado para um item de trabalho.
author: Alina
feature: Resource Management
exl-id: 627e4442-767a-41a2-9700-76f2ad2dc9cf
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Usando a linha do tempo de agendamento, você pode gerenciar atribuições de usuários, além de especificar quanto tempo cada usuário está alocado para um item de trabalho.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso a Projetos, Tarefas e Problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões para projetos, tarefas e problemas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos antes de atribuir tarefas e problemas na linha do tempo de Agendamento

Antes de começar a gerenciar atribuições de usuários, conforme descrito nesta seção, familiarize-se com o funcionamento do agendamento de recursos no Workfront, conforme descrito em [Introdução ao Agendamento de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Para gerenciar com êxito as atribuições de usuários, conforme descrito nesta seção, você deve primeiro garantir que você, seus projetos e suas tarefas e problemas atendam aos pré-requisitos descritos na seção [Pré-requisitos para usar as ferramentas de agendamento no Workfront](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#prerequisites) no artigo [Introdução ao Agendamento de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

As seções a seguir descrevem como modificar atribuições de usuários manualmente, automaticamente ou trocando atribuições por usuário ou função.

## Atribuir manualmente tarefas ou problemas não atribuídos a usuários

A linha do tempo de agendamento fornece a visibilidade necessária em que os usuários são capazes de concluir a tarefa ou o problema.\
Para obter mais informações sobre a linha do tempo de agendamento, consulte [Introdução ao Agendamento de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Você pode atribuir tarefas e problemas individuais aos usuários na linha do tempo de agendamento nas seguintes áreas do Workfront:

* A seção Agendamento em Recursos (ao agendar recursos para vários projetos).
* A seção Agendamento em um projeto (ao agendar recursos para um único projeto).
* A seção Programação em uma equipe (ao agendar recursos para uma equipe).

As informações exibidas na área Não atribuído na parte superior da linha do tempo de programação diferem dependendo da área do Workfront em que você está usando o agendamento de recursos (na seção Agendamento de recursos para vários projetos), na seção Agendamento (ao agendar recursos para um único projeto) ou na seção Programação (ao agendar recursos para uma equipe). Para obter mais informações, consulte a seção [Funcionalidade disponível na área Agendamento](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md#functionality-available-in-the-scheduling-area) no artigo [Visão geral das áreas de Agendamento](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Dependendo da área do Workfront em que você está visualizando a linha do tempo de agendamento, somente alguns usuários podem receber trabalho atribuído. Para obter mais informações, consulte [Visão geral das áreas de Agendamento](../../resource-mgmt/resource-scheduling/overview-scheduling-areas.md).

Para atribuir tarefas ou problemas não atribuídos a usuários na linha do tempo de agendamento:

1. Vá para a linha do tempo de agendamento para vários projetos, para um projeto individual ou para uma equipe:

   * **Para vários projetos**:  Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para um projeto individual**: Vá para um projeto e clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para uma equipe**: Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.

   ![scheduling_contours.png](assets/scheduling-contours-350x139.png)

1. (Opcional) Crie um filtro para personalizar o conteúdo exibido na linha do tempo do agendamento, conforme descrito em [Filtrar informações na área Agendamento](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) . [Filtrar informações na área Agendamento](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md). Por exemplo, para que os problemas sejam exibidos na linha do tempo do agendamento, você deve criar um filtro.

1. (Opcional) Modifique o intervalo de datas exibido na linha do tempo do agendamento, conforme descrito em [Ajuste o intervalo de datas das áreas de Agendamento](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) em [Introdução ao Agendamento de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

1. Faça o seguinte para atribuir uma tarefa ou problema não atribuído:

   * Arraste a tarefa ou o problema para a linha do usuário que deseja atribuir.\
      Um máximo de 10 tarefas por dia é exibido para um determinado usuário. Você pode expandir a lista para exibir todas as tarefas atribuídas a esse usuário no momento. (Após fazer atribuições na linha do tempo de programação, mais de 10 tarefas podem ser exibidas temporariamente.)\
      À medida que você arrasta um item, as seguintes informações são exibidas antes de liberar a tarefa ou o problema e concluir a atribuição:

   * Se as alocações de usuário estiverem ativadas na linha do tempo de programação, os indicadores de sobrealocação vermelhos serão exibidos se a conclusão da atribuição resultar em sobrealocação do usuário.\
      Para obter mais informações sobre indicadores de atribuição excessiva, consulte a seção [Indicadores de atribuição](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators) no artigo [Gerenciar alocações de usuários nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md).

      Se a variável **Limitar atribuições a usuários com uma função correspondente** estiver ativada na área Configurações , os usuários que não estão qualificados para receber a atribuição serão esmaecidos. Se essa opção estiver desativada, todos os usuários estarão disponíveis para receber a atribuição. A opção é ativada por padrão.\
      Para obter mais informações sobre essa opção, consulte [](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md#allowing-assignmennts-to-users-regardless-of-role) em [Permitir atribuições de usuários independentemente da função e associação de grupo nas áreas de Programação](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md)

      Um indicador de queda é exibido na linha do usuário. Isso permite ver onde um item está sendo atribuído antes de fazer a atribuição.

      Expanda a tarefa ou problema que deseja atribuir, clique na seta suspensa na **Atribuições** , comece a digitar o nome do usuário que deseja atribuir e clique no nome do usuário na lista suspensa.\
      ![schedule_task_expand.png](assets/schedule-task-expanded-350x170.png)

1. (Condicional) Depois de atribuir uma tarefa ou emissão não atribuída a um usuário, você pode ajustar as atribuições existentes para tarefas e problemas entre os usuários na linha do tempo de agendamento. Ao agendar recursos para projetos (na guia Agendamento ou na guia Pessoal ), somente os usuários que têm a mesma função de trabalho podem receber a atribuição.\
   Para atribuir novamente uma tarefa ou problema a outro usuário, arraste a tarefa da linha de um usuário para a linha de outro usuário.
1. (Opcional) Configure o número de horas que cada usuário atribuído é alocado para a tarefa ou problema, conforme descrito em [Gerenciar alocações de usuários nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md) .
