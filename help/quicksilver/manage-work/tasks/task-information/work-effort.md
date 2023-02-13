---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Visão geral do esforço de trabalho
description: Visão geral do esforço de trabalho
author: Alina
feature: Work Management
exl-id: 70f51e4b-43cc-427a-99e4-ebb056bb1070
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Visão geral do esforço de trabalho

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the UI >> in the Project/ Template edit box > Tasks area> Learn more) </p>
-->

Como gerente de projeto, você pode decidir como deseja estimar a quantidade de trabalho necessária para as tarefas serem concluídas em um projeto. Estime a quantidade de trabalho necessária para concluir tarefas usando um dos seguintes indicadores:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Horas planejadas</td> 
   <td> <p> Uma entrada numérica manual ou um cálculo do Adobe Workfront que exibe o número de horas que seriam necessárias para que os recursos atribuídos a uma tarefa a concluíssem. </p> <p>Considere o seguinte sobre as Horas Planejadas: </p> 
    <ul> 
     <li>Este é o método padrão. </li> 
     <li>Você pode atualizar manualmente as Horas Planejadas somente para tarefas com um Tipo de duração de Atribuição calculada ou Simples. </li> 
    </ul> <p>Para obter informações sobre Horas Planejadas, consulte <a href="../../../manage-work/tasks/task-information/planned-hours.md" class="MCXref xref">Visão geral das Horas Planejadas</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Esforço do trabalho </td> 
   <td> <p>Um rótulo manual que define se é necessário um pequeno, médio ou grande esforço diário para concluir uma tarefa. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The level of effort is estimated to be a percentage of the daily amount of working time. (NOTE: keep this drafted. Vazgen said it's not needed, but waiting for feedback from users)
      </MadCap:conditionalText>
     --> </p> <p>Considere o seguinte sobre o Esforço de Trabalho:</p> 
    <ul> 
     <li>Este campo está disponível somente para tarefas com um Tipo de duração simples. </li> 
     <li>Você pode ativar o uso desse rótulo e definir a porcentagem do tempo de trabalho associado a ele no nível do projeto. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Este artigo descreve o que é Esforço de trabalho e como usá-lo ao estimar a quantidade de trabalho para suas tarefas.

>[!NOTE]
>
>As Horas Planejadas e o Esforço do Trabalho influenciam-se mutuamente. Atualizar as Horas Planejadas pode atualizar o Esforço de Trabalho e atualizar o Esforço de Trabalho pode atualizar as Horas Planejadas da tarefa.

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
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Tarefas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um projeto e suas tarefas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Considerações sobre o uso do esforço de trabalho

* Quando as tarefas do projeto tiverem 0 Horas Planejadas e você ativar a configuração Usar Esforço de Trabalho para calcular automaticamente as Horas Planejadas da tarefa no projeto, o nível padrão de Esforço de Trabalho associado a elas será Médio. As Horas Planejadas são atualizadas automaticamente para tarefas do Tipo de duração simples. Para obter mais informações, consulte a seção  [Níveis de esforço de trabalho](#levels-of-work-effort) neste artigo.
* Quando as tarefas do projeto têm Horas Planejadas superiores a 0 e você ativa a configuração Usar Esforço de Trabalho para calcular automaticamente a tarefa Horas Planejadas no projeto, o nível de Esforço de Trabalho é atualizado de acordo com a quantidade de Horas Planejadas sem alterar a quantidade de Horas Planejadas para tarefas do Tipo de Duração Simples. Para obter mais informações, consulte a seção [Como a Workfront calcula o esforço de trabalho com base nas horas planejadas](#how-workfront-calculates-work-effort-based-on-planned-hours) neste artigo.
* Quando as tarefas do projeto têm 0 Horas Planejadas e você ativa a configuração Usar Esforço de Trabalho para calcular automaticamente a tarefa Horas Planejadas no projeto e, em seguida, atualiza o nível de Esforço de Trabalho de Médio para Pequeno ou Grande, as Horas Planejadas também são atualizadas. Para obter mais informações, consulte a seção [Como o Workfront calcula as Horas Planejadas com base no Esforço do Trabalho](#how-workfront-calculates-planned-hours-based-on-work-effort) neste artigo.
* Ao editar tarefas em linha e modificar os campos Horas Planejadas e Esforço do Trabalho para tarefas ao mesmo tempo, as Horas Planejadas serão atualizadas com o valor especificado, enquanto o valor Esforço do Trabalho é calculado com base nas Horas Planejadas atualizadas.
* Quando você atualiza o valor do Esforço de trabalho de uma tarefa, a Duração não é mais calculada automaticamente com base nas Horas Planejadas. Para obter mais informações sobre como a Duração é calculada para tarefas de Duração simples, consulte [Visão geral do Tipo de duração: Simples](../../../manage-work/tasks/taskdurtn/simple-duration-type.md).
* Quando você altera o Tipo de duração de uma tarefa de Simples para qualquer outro tipo, o campo Esforço do trabalho fica oculto na tarefa. As Horas Planejadas permanecem inalteradas.
* Não é possível atualizar o nível de Esforço de Trabalho em uma tarefa pai. O nível de Esforço de Trabalho para uma tarefa pai é calculado automaticamente com base no número de Horas Planejadas para as tarefas que é um rollup de todas as tarefas filho. Para obter informações sobre tarefas pai, consulte [Criar subtarefas](../../../manage-work/tasks/create-tasks/create-subtasks.md).

## Ativar usando Esforço de Trabalho em vez de Horas Planejadas

1. Vá para um projeto e clique no botão **Mais** menu ![](assets/more-icon.png), depois clique em **Editar**.
1. Clique em **Configurações da tarefa** e selecione a opção **Usar Esforço de Trabalho para calcular automaticamente as horas da tarefa Planejada**. Isso é desmarcado por padrão.

   ![](assets/nwe-work-effort-on-projects-350x182.png)

   Para obter mais informações sobre como habilitar o uso do Esforço de trabalho em um projeto, consulte a seção &quot;Configurações de tarefas&quot; na [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md) artigo 10. o

1. Clique em **Tarefas** no painel esquerdo, em seguida, clique no nome de uma tarefa para acessá-la.
1. Clique no botão **Mais** menu ![](assets/more-icon.png), depois clique em **Editar**. Verifique se a tarefa tem um Tipo de duração simples.

   >[!TIP]
   >
   >Também é possível atualizar o Esforço de trabalho para uma tarefa na seção Detalhes da tarefa.

1. No **Visão geral** , clique no menu suspenso Esforço de trabalho para corrigir a quantidade de esforço necessária para concluir a tarefa.

   ![](assets/work-effort-on-edit-task-page-350x239.png)

   Para obter mais informações sobre como atualizar o campo Esforço de trabalho em uma tarefa, consulte os seguintes artigos:

   * A seção &quot;Visão geral&quot; na [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md) artigo
   * [Gerenciar informações da tarefa na área Visão geral de detalhes da tarefa](../../../manage-work/tasks/manage-tasks/task-information-in-overview.md)

## Níveis de esforço de trabalho {#levels-of-work-effort}

Como gerente de projeto, você pode identificar três níveis de Esforço do Trabalho para seus projetos. Cada nível de esforço equivale a uma porcentagem do tempo diário que os usuários precisam para concluir a tarefa.

Ao configurar o nível de Esforço do Trabalho, você precisa se perguntar: &quot;Quanto tempo um usuário atribuído a esta tarefa deve gastar diariamente para fazê-lo a tempo?&quot; 

A tabela a seguir ilustra os possíveis níveis de Esforço de Trabalho e suas porcentagens correspondentes padrão. Como gerente de projeto, você pode atualizar as porcentagens para atender às necessidades de sua organização. Faça isso ao editar um projeto. Para obter informações sobre edição de projetos, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

Como administrador do Workfront, você define as Horas típicas por dia de trabalho na área Preferências do projeto da Configuração. Este é o tempo diário considerado como tempo de trabalho. Para obter informações sobre como configurar Preferências de projeto para sua instância do Workfront, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

>[!NOTE]
>
>Nos exemplos abaixo, supomos que o administrador do Workfront tenha definido o valor Típico de horas por dia de trabalho como 8 horas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Nível de esforço de trabalho</td> 
   <td>Valores percentuais</td> 
  </tr> 
  <tr> 
   <td>Pequena </td> 
   <td>Um pequeno nível de esforço para concluir uma tarefa é definido como 25% do horário típico por dia de trabalho. Isso significa que uma tarefa atribuída a esse nível de Esforço de Trabalho deve levar até 2 horas por dia para ser concluída em um dia. <code>(0.25*8=2)</code></td> 
  </tr> 
  <tr> 
   <td>Média</td> 
   <td> <p>Um Nível Médio de esforço para concluir uma tarefa é definido como 50% das horas típicas por dia de trabalho. Isso significa que uma tarefa atribuída a esse nível de Esforço de Trabalho deve levar mais de 2 e menos de 6 horas para ser concluída em um dia. <code>(0.50*80=4)</code> </p> <p>Observação: Quando a configuração Usar Esforço de Trabalho para calcular automaticamente a tarefa Horas Planejadas está ativada no projeto, essa é a configuração padrão para uma tarefa, se a tarefa tiver 0 Horas Planejadas antes que essa configuração fosse habilitada. Isso faz com que a tarefa Horas Planejadas seja atualizada para 4 horas. </p> </td> 
  </tr> 
  <tr> 
   <td>Grande</td> 
   <td>Um grande nível de esforço para concluir uma tarefa é definido como 75% das horas típicas por dia de trabalho. Isso significa que uma tarefa atribuída a esse nível de Esforço de Trabalho deve levar 6 horas ou mais para ser concluída em um dia. <code>(0.75*8=6)</code></td> 
  </tr> 
 </tbody> 
</table>

## Como o Workfront calcula as Horas Planejadas com base no Esforço do Trabalho {#how-workfront-calculates-planned-hours-based-on-work-effort}

Ao ativar a configuração Usar Esforço de Trabalho para calcular automaticamente a tarefa Horas Planejadas em um projeto, o Workfront calcula o número de Horas Planejadas para uma tarefa com um Tipo de Duração Simples usando a seguinte fórmula:

```
Task Planned Hours = Number of days in task Duration * Work Effort percentage * Typical hours per work day
```

Por exemplo, uma tarefa com uma Duração de 3 dias e um Esforço de Trabalho Médio tem 12 Horas Planejadas:

```
Planned Hours = 3*4=12
```

em que o valor do horário típico por dia de trabalho é de 8 horas.

>[!TIP]
>
>Quando uma tarefa é atribuída a vários recursos, as Horas Planejadas são distribuídas uniformemente para cada recurso para cada dia da duração da tarefa.

## Como a Workfront calcula o esforço de trabalho com base nas horas planejadas {#how-workfront-calculates-work-effort-based-on-planned-hours}

Quando você ativa a configuração Usar Esforço de Trabalho para calcular automaticamente a tarefa Horas Planejadas em um projeto e já tem Horas Planejadas na tarefa ou edita o número de Horas Planejadas na tarefa, o Workfront atualiza o valor Esforço de Trabalho.

O Workfront usa a seguinte fórmula para atualizar o nível de Esforço de Trabalho de acordo com as Horas Planejadas:

```
Work Effort level = Task Planned Hours / Duration / Typical hours per work day
```

Por exemplo, se você tiver uma tarefa com uma Duração de 2 dias e atualizar as Horas Planejadas de 8 a 20 horas, o Esforço de Trabalho para a tarefa será atualizado de Médio a Grande:

```
Work Effort level = 20 / 2 / 8 = 125 % = Large
```

## Localizar Esforço de Trabalho para tarefas e projetos

* [Esforço de trabalho para projetos](#work-effort-for-projects)
* [Esforço de trabalho para tarefas](#work-effort-for-tasks)

### Esforço de trabalho para projetos {#work-effort-for-projects}

Você pode localizar a seção Esforço de trabalho em um projeto na seguinte área:

* A área Configurações da tarefa na caixa Editar projeto

### Esforço de trabalho para tarefas {#work-effort-for-tasks}

Você pode localizar o campo Esforço de trabalho para uma tarefa nas seguintes áreas:

* A área Visão geral na caixa Editar tarefa
* A área Visão Geral da seção Detalhes da Tarefa, na área Tempo de Trabalho
* Uma lista de tarefas ou relatório
