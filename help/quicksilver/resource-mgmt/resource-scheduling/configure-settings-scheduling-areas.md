---
product-area: resource-management;setup
navigation-topic: resource-scheduling
title: Definir configurações nas áreas de Agendamento
description: Você pode definir várias configurações para personalizar como e quais informações são exibidas na linha do tempo do agendamento.
author: Alina
feature: Resource Management
exl-id: d76b59c0-d0fd-4698-8017-fa0778f61dc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2280'
ht-degree: 1%

---

# Definir configurações nas áreas de Agendamento

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.</span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Você pode definir várias configurações para personalizar como e quais informações são exibidas na linha do tempo do agendamento.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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
   <td> <p>Exibir o acesso ou superior a Projetos, Tarefas e Problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões ou mais para projetos, tarefas e problemas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Configurar problemas para exibir na linha do tempo do agendamento

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ALL THE SECTIONS BELOW ARE LINKED TO PRODUCT. DO NOT CHANGE TITLES) </p>
-->

Você pode configurar os problemas a serem exibidos além das tarefas na linha do tempo de agendamento.\
Ao agendar recursos na seção Agendamento de uma equipe , os problemas são exibidos por padrão além das tarefas. Ao agendar recursos para projetos, somente as tarefas são exibidas por padrão.

1. Vá para a linha do tempo de agendamento para vários projetos, para um projeto individual ou para uma equipe:

   * **Para vários projetos**:  Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para um projeto individual**: Vá para um projeto e clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para uma equipe**: Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.

1. Clique no botão **Configurações** na linha do tempo de agendamento.

1. Na caixa de diálogo Configurações de agendamento de recursos , habilite o **Mostrar problemas** opção.\
   ![RS_scheduling_tab_all_settings__1_.png](assets/rs-scheduling-tab-all-settings--1--350x417.png)

1. Clique em **Retornar ao agendamento**. 

## Configurar trabalho concluído para exibir na linha do tempo de agendamento

Você pode configurar a linha do tempo de agendamento para exibir o trabalho que já foi marcado como Concluído. Por padrão, o trabalho concluído não é exibido na linha do tempo de agendamento. 

1. Vá para a linha do tempo de agendamento para vários projetos, para um projeto individual ou para uma equipe:

   * **Para vários projetos**:  Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para um projeto individual**: Vá para um projeto e clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para uma equipe**: Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.

1. Clique no botão **Configurações** na linha do tempo de agendamento.

1. Na caixa de diálogo Configurações de agendamento de recursos , habilite o **Mostrar trabalho concluído** opção.\
   ![RSS_show_completed_work_disabled_1_.png](assets/rss-show-completed-work-disabled--1--350x336.png)

1. Clique em **Retornar ao agendamento**.\
   O trabalho concluído é exibido com uma marca de seleção no canto superior direito do item de trabalho.

## Configurar nomes de projeto para exibir na linha do tempo de agendamento 

Você pode configurar o nome do projeto a ser exibido em cada tarefa e problema na linha do tempo de agendamento. Isso permite que os usuários que visualizam a linha do tempo do agendamento vejam rapidamente o nome do projeto em que a tarefa ou problema reside.

Quando você habilita a exibição de nomes de projeto, cada tarefa e problema consome mais espaço vertical na linha do tempo de agendamento, resultando em menos tarefas e problemas exibidos em uma única visualização.

Por padrão, os nomes de projeto não são exibidos nas tarefas e problemas na linha do tempo de agendamento.

Para exibir nomes de projeto em tarefas e problemas na linha do tempo de agendamento:

1. Vá para a linha do tempo de agendamento para vários projetos ou para uma equipe:

   * **Para vários projetos**:  Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para uma equipe**: Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.

1. Clique no botão **Configurações** na linha do tempo de agendamento.

1. Na caixa de diálogo Configurações de agendamento de recursos , habilite a opção , **Mostrar nomes de projeto**.\
   ![RS_scheduling_tab_all_settings__2_.png](assets/rs-scheduling-tab-all-settings--2--350x348.png)

1. Clique em **Retornar ao agendamento**.\
   Cada tarefa e problema na linha do tempo de agendamento exibe o nome do projeto em que a tarefa ou problema reside.\
   ![resourcescheduling_projectnames.png](assets/resourcescheduling-projectnames-350x200.png)

## Configurar datas projetadas para exibição na linha do tempo do agendamento

Por padrão, as Datas Planejadas são usadas na linha do tempo de programação. Como alternativa, você pode configurar a linha do tempo de agendamento para usar Datas Projetadas.

Considere as seguintes informações sobre as Datas Planejadas e Projetadas:

* As Datas Planejadas para tarefas podem ser definidas manualmente ou podem ser definidas automaticamente, dependendo da restrição de tarefa e do tipo de duração. Para obter mais informações, consulte os artigos [Visão geral da restrição de tarefa](../../manage-work/tasks/task-constraints/task-constraint-overview.md) e  [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md) .

   Datas planejadas para problemas são definidas manualmente para problemas por usuários. No entanto, o administrador do sistema pode impedir que os usuários ajustem as Datas planejadas para problemas.

* As datas projetadas para tarefas e problemas são definidas automaticamente. Para obter mais informações sobre as Datas projetadas, consulte os artigos [Visão geral da data de conclusão projetada para projetos, tarefas e problemas](../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

>[!NOTE]
>
>Ao usar Datas projetadas na linha do tempo do agendamento, as informações de alocação do usuário não podem ser exibidas. Para obter mais informações sobre alocações de usuários, consulte o artigo [Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

Para configurar a linha do tempo de agendamento para exibir tarefas e problemas de acordo com as Datas projetadas: 

1. Vá para a linha do tempo de agendamento para vários projetos, para um projeto individual ou para uma equipe:

   * **Para vários projetos**:  Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para um projeto individual**: Vá para um projeto e clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para uma equipe**: Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.

1. Clique no botão **Configurações** na linha do tempo de agendamento.

1. Na caixa de diálogo Configurações de agendamento de recursos , desative o **Usar datas previstas em vez de datas projetadas** opção.
1. Clique em **Retornar ao agendamento**.

## Configurar como os usuários são exibidos na linha do tempo do agendamento

>[!NOTE]
>
>Esta seção se aplica somente ao agendar recursos para equipes (na seção Agendamento de uma equipe ). Ao programar recursos para vários projetos (na guia Scheduling ) ou para um único projeto (na guia Staffing ), os usuários não podem ser exibidos em ordem alfabética; elas são sempre organizadas por função.

Ao programar recursos para uma equipe, você pode configurar usuários para serem exibidos na linha do tempo de programação alfabética ou por função. Por padrão, os usuários são exibidos em ordem alfabética (as funções não são exibidas).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em Equipes. Um grupo é selecionado por padrão.

1. Clique no botão **Configurações** na linha do tempo de agendamento.

1. Na caixa de diálogo Configurações , selecione se deseja ativar a variável **Grupo por função** opção.\
   Quando essa opção está desativada, os usuários são exibidos em ordem alfabética e as funções não são exibidas na linha do tempo de programação.\
   Quando essa opção é ativada, as funções são exibidas na linha do tempo do agendamento e os usuários são agrupados em suas respectivas funções. Se um determinado usuário tiver várias funções definidas no sistema, ele aparecerá várias vezes na linha do tempo de programação, abaixo de cada função apropriada.\
   ![RS_working_on_time_scheduling_full_settings__1_.png](assets/rs-working-on-team-scheduling-full-settings--1--350x348.png)

1. Clique em **Retornar ao agendamento**.

## Configurar se as tarefas pai são exibidas na linha do tempo de agendamento

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This section is linked to the UI in a tooltip inside the Settings of the scheduler. do not rename/ remove/ edit the tag!! - Resource Scheduling (People> Scheduling>Settings>Show Parent Tasks tooltip)</p>
-->

As Tarefas pai são exibidas de forma diferente, dependendo da linha do tempo de programação que você está acessando. 

* [Exibir tarefas pai para vários projetos](#display-parent-tasks-for-multiple-projects)
* [Exibir tarefas pai para um projeto ou equipe](#display-parent-tasks-for-a-project-or-a-team)

### Exibir tarefas pai para vários projetos {#display-parent-tasks-for-multiple-projects}

Ao agendar recursos para vários projetos na seção Agendamento , se as tarefas pai forem exibidas ou não dependerão das seguintes configurações:

* O modo de conclusão do projeto.
* O modo de conclusão do resumo do projeto.
* A configuração Mostrar tarefas pai na guia Agendamento .

A tabela a seguir descreve quando as tarefas pai são exibidas na guia Agendamento e quando somente as subtarefas são exibidas. 

| **Mostrar configuração de tarefas pai** | **Modo de conclusão do projeto** | **Modo de conclusão do resumo do projeto** | **Tipo de tarefas exibidas na linha do tempo de agendamento** |
|---|---|---|---|
| Desabilitado | Manual | Automático | Somente subtarefas |
| Desabilitado | Manual | Manual | Somente subtarefas |
| Desabilitado | Automático | Automático | Somente subtarefas |
| Desabilitado | Automático | Manual | Somente subtarefas |
| Ativado | Automático | Manual | Subtarefas e tarefas pai |
| Ativado | Automático | Automático | Somente subtarefas |
| Ativado | Manual | Manual | Subtarefas e tarefas pai |
| Ativado | Manual | Automático | Somente subtarefas |

Para obter informações sobre como configurar o **Modo de conclusão** e **Modo de conclusão do resumo** para cada projeto, consulte a seção &quot;Configurações&quot; no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

Você pode configurar manualmente a configuração Mostrar tarefas pai na seção Agendamento para vários projetos. 

Para configurar a configuração Mostrar tarefas pai: 

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
1. Clique no botão **Configurações** na linha do tempo de agendamento.

1. Na caixa de diálogo Configurações de agendamento de recursos , selecione se deseja habilitar a opção , **Mostrar Tarefas Pai.**
Quando essa opção é ativada, as tarefas principais de todos os projetos são exibidas de acordo com o Modo de conclusão de resumo e as configurações do Modo de conclusão dos projetos, conforme descrito na tabela acima. Essa opção é ativada por padrão.
\
   ![RS_scheduling_tab_all_settings__3_.png](assets/rs-scheduling-tab-all-settings--3--350x348.png)

1. Clique em **Retornar ao agendamento** no canto inferior esquerdo.

### Exibir tarefas pai para um projeto ou equipe {#display-parent-tasks-for-a-project-or-a-team}

Ao agendar recursos na seção Pessoal de um projeto ou na seção Agendamento , se as Tarefas pai são exibidas ou não depende das seguintes configurações:

* O modo de conclusão do projeto.
* O modo de conclusão do resumo do projeto.

Para obter informações sobre como configurar o **Modo de conclusão** e **Modo de conclusão do resumo** para cada projeto, consulte a seção &quot;Configurações&quot; no artigo [Editar projetos](../../manage-work/projects/manage-projects/edit-projects.md).

A tabela a seguir descreve quando as Tarefas principais são exibidas na seção Pessoal de um projeto ou na seção Programação e quando somente as subtarefas são exibidas. 

| Modo de conclusão do projeto | Modo de conclusão do resumo do projeto | Tipo de tarefas exibidas na seção Agendamento | Tipo de tarefas exibidas na seção Agendamento de equipes |
|---|---|---|---|
| Manual | Automático | Somente subtarefas | Somente subtarefas |
| Manual | Manual | Subtarefas e tarefas pai | Somente subtarefas |
| Automático | Automático | Somente subtarefas | Somente subtarefas |
| Automático | Manual | Subtarefas e tarefas pai | Somente subtarefas |
| Automático | Manual | Subtarefas e tarefas pai | Somente subtarefas |
| Automático | Automático | Somente subtarefas | Somente subtarefas |
| Manual | Manual | Subtarefas e tarefas pai | Somente subtarefas |
| Manual | Automático | Somente subtarefas | Somente subtarefas |

## Configure se as Horas Planejadas Diárias são exibidas na linha do tempo de programação

Para configurar a linha do tempo de programação para exibir os totais diários das Horas Planejadas para cada usuário: 

1. Vá para a linha do tempo de agendamento para vários projetos, para um projeto individual ou para uma equipe:

   * **Para vários projetos**:  Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, clique em **Recursos > Balanceador de carga de trabalho**, em seguida selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para um projeto individual**: Vá para um projeto e clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.
   * **Para uma equipe**: Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Equipes**, selecione um grupo, clique em **Balanceador de Carga de Trabalho** no painel esquerdo e selecione **Agendamento** no menu suspenso superior esquerdo.

1. Clique no botão **Configurações** na linha do tempo de agendamento.

1. Na caixa de diálogo Configurações , ative as seguintes opções:

   *  **Mostrar totais para horas diárias planejadas**: Mostra o total de Horas Planejadas diárias para cada usuário.
   * **Mostrar realce da alocação de recursos**: Destaca a alocação do usuário para tarefas e problemas, bem como destaca os dias em que os usuários são alocados em excesso.\
      Essas opções são desativadas por padrão.\
      ![RS_all_settings__1_.png](assets/rs-all-settings--1--350x358.png)

1. Clique em **Retornar ao agendamento**.\
   O total de Horas Planejadas alocadas ao usuário para cada dia.\
   As Horas Planejadas dos dias em que o usuário está sobrealocado são destacadas em vermelho.\
   Para obter mais informações sobre alocações de usuários, consulte o artigo [Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

## Configure se todas as tarefas do usuário são exibidas na linha do tempo de agendamento

>[!NOTE]
>
>Essa opção se aplica somente ao agendar recursos para projetos individuais (na seção Agendamento do projeto ). Essa opção não está disponível ao agendar recursos para vários projetos (na seção Agendamento ) ou para equipes (na seção Agendamento de uma equipe ).

Para configurar se todas as tarefas atribuídas a cada usuário (não apenas as tarefas associadas ao projeto que você está visualizando) serão exibidas na linha do tempo de agendamento:

1. Vá para o projeto em que deseja configurar a linha do tempo de agendamento para exibir todas as tarefas atribuídas a cada usuário.
1. Clique no botão **Balanceador de Carga de Trabalho** no painel esquerdo (pode estar localizado em **Mostrar mais**) e, em seguida, selecione **Agendamento** no menu suspenso superior esquerdo.
1. Clique no botão **Configurações** na linha do tempo de agendamento.

1. Na área Configurações , selecione se a opção deve ser ativada, **Mostrar todas as tarefas do usuário**.\
   Quando essa opção é ativada, todas as tarefas atribuídas a cada usuário são exibidas na linha do tempo do agendamento, independentemente do projeto no qual as tarefas estão localizadas.\
   Essa opção é desativada por padrão.\
   ![RS_project_scheduling_area_1_.png](assets/rs-project-scheduling-area--1--350x340.png)

1. Clique em **Retornar ao agendamento**.
