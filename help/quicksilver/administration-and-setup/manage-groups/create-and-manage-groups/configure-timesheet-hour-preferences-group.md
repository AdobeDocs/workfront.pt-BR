---
user-type: administrator
product-area: system-administration;user-management
keywords: grupo,preferências,tarefa,grupos,problema,desbloquear
navigation-topic: create-and-manage-groups
title: Configurar preferências de horas e planilha de horas para um grupo
description: No nível do sistema, um administrador do Adobe Workfront pode desbloquear as seções de preferências de folha de horas e hora Preferências gerais e Preencher folhas de horas previamente com. Isso permite que administradores de grupos configurem as opções nessas seções independentemente para seus próprios grupos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1364'
ht-degree: 1%

---

# Configurar preferências de horas e planilha de horas para um grupo

Um administrador do Adobe Workfront pode desbloquear as seguintes seções de preferências de folha de horas e horas no nível do sistema para que os administradores de grupo possam configurá-las independentemente para seus próprios grupos:

* Preferências gerais
* Onde os usuários podem registrar o tempo
* Pré-preencher folhas de horas

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

As seguintes seções na página Preferências de Horas e Planilha de Horas são configuráveis apenas no nível do sistema e não podem ser desbloqueadas para grupos:

* Projetos, tarefas e problemas excluídos

Para obter informações sobre como um administrador do Workfront desbloqueia uma folha de horas e uma preferência de horas, consulte a seção [Desbloquear preferências de folha de horas e horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) no artigo [Configurar preferências de folha de horas e horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>A configuração no nível do grupo também é possível para preferências de projeto e preferências de tarefa e problema. Para obter informações, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença, contate o administrador do Workfront.

+++

## Preferências de Horas e Planilha de Horas do Grupo

Considere as seguintes informações sobre a configuração de uma folha de horas desbloqueada ou preferência de horas para um grupo:

* Se você for um administrador de grupo e configurar uma planilha de horas ou uma preferência de horas para o seu grupo, ela afetará as pessoas que usam o grupo como seu Grupo padrão.
* Normalmente, uma preferência desbloqueada permanece desbloqueada indefinidamente. Se o administrador do Workfront o bloquear novamente, a configuração do sistema será aplicada novamente e as configurações da preferência feita pelos administradores de grupo serão perdidas.
* Uma folha de horas herda as preferências de hora e folha de horas configuradas para o Grupo inicial do proprietário da folha de horas.

  <!--
  Add example here?
  -->

* Depois que um administrador do Workfront desbloquear uma preferência no nível do sistema e configurá-la para o seu grupo, você poderá bloqueá-la para garantir que todos os grupos abaixo do seu usem a mesma configuração. Isso é paralelo à capacidade que um administrador do Workfront tem de configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear uma planilha de horas e uma preferência de horas de grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configurar uma planilha de horas ou uma preferência de horas desbloqueada para um grupo

>[!TIP]
>
>Se você for um administrador do Workfront, ignore as etapas 1 a 4. Para isso, acesse Configurar > Folhas de horas e horas > Preferências e, em seguida, procure o nome do grupo na caixa na parte superior da página.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo cujas preferências de folha de horas ou de horas você deseja configurar.
1. No painel esquerdo, clique em **Folhas de horas e Horas**.

1. Na página exibida, na seção **Preferências gerais**, configure uma das seguintes opções:

   >[!TIP]
   >
   >Se você passar o mouse sobre uma preferência e uma dica de ferramenta for exibida para informá-lo de que ela está bloqueada, peça ao administrador do Workfront para desbloqueá-la para todos os grupos na organização.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Registrar horas para datas futuras</td> 
      <td> <p>Permite que os usuários registrem horas para datas futuras em todo o sistema em:</p> 
       <ul> 
       <li>Qualquer projeto, tarefa e problema que tenha acesso ao registro de hora, independentemente do grupo do projeto</li> 
       <li>Suas planilhas de horas como Tempo geral</li>
       </ul> 
       <p>Isso é útil quando os usuários planejam ficar longe do escritório e desejam registrar esse tempo antecipadamente.</p> 
       <p><b>OBSERVAÇÃO</b>: não é possível impedir que os usuários registrem tempo em tarefas ou problemas que estão fechados ou cancelados. Você só pode impedir que os usuários registrem horas em projetos concluídos ou inativos. Recomendamos que você use filtros em listas de tarefas e problemas para excluir aqueles que foram concluídos ou cancelados de ficarem visíveis para os usuários.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adicionar despesas de uma folha de horas</td> 
      <td> <p>Permite que os usuários registrem horas e despesas na planilha de horas.</p> 
      <p>Quando esta preferência está habilitada para um grupo e o grupo é definido como o grupo inicial para certos usuários, um ícone de despesa é exibido ao lado de projetos e tarefas nas folhas de horas desses usuários. Os usuários podem clicar neste ícone para adicionar ou editar despesas para o projeto ou tarefa.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atribuir funções de trabalho a entradas de hora manualmente</td> 
      <td> <p>Permite que os usuários selecionem manualmente qualquer Função atribuída em seu perfil de usuário ou atribuída ao objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Se você desabilitar essa configuração depois de atribuir funções de trabalho a entradas de horas, os usuários deverão ajustar as horas registradas em várias funções na guia Horas do projeto, tarefa ou problema.</li> 
         <li>Se o usuário não tiver uma função de trabalho atribuída em seu perfil e houver uma tarefa atribuída como Proprietário da Tarefa na caixa de diálogo Atribuições Avançadas, essa função de trabalho aparecerá quando o usuário registrar o tempo na tarefa.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restringir a edição da folha de horas aos proprietários e administradores</td> 
      <td> <p>Restringir a edição aos proprietários da folha de horas, independentemente do grupo do projeto e dos administradores do Workfront. Quando esta opção está desabilitada, as folhas de horas também podem ser editadas por:</p> 
       <ul> 
        <li> <p>Usuários com acesso administrativo a folhas de horas e horas em seu nível de acesso</p> </li> 
        <li> <p>Aprovadores de planilhas de horas se a opção "Pode editar horas" estiver ativada na planilha de horas</p> </li> 
        <li> <p>O gerente do proprietário da planilha de horas</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restringir a edição de horas a proprietários e administradores</td> 
      <td>Restringir a edição ao usuário que insere as horas e aos administradores do Workfront. Essa configuração se aplica à guia Horas em um projeto ou em um relatório de Horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. Na seção **Onde os usuários podem registrar horas**, configure uma das seguintes opções:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Registrar o tempo diretamente nos projetos</td> 
      <td>Permite que os usuários registrem horas no projeto (tanto na guia Atualizações quanto na folha de horas). Se quiser impedir que os usuários gravem horas no nível do projeto, deixe essa opção desmarcada.</td>
     </tr>
     <tr>
      <td role="rowheader">Registrar o tempo em projetos concluídos</td>
      <td>Permite que os usuários gravem tempo em um projeto marcado como concluído. Se essa opção estiver desativada, os usuários não poderão registrar o tempo referente ao trabalho que concluíram nos projetos no status Concluído.</td>
     </tr>
     <tr>
      <td role="rowheader">Registrar o tempo em projetos mortos</td> 
      <td>Quando essa opção está ativada, os usuários podem registrar horas em projetos com status Inativo.</td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Esta preferência é aplicada com base na configuração das preferências do Grupo padrão do usuário. Se essas configurações estiverem ativadas nas preferências do Grupo padrão do usuário, ele poderá registrar o tempo diretamente nos projetos, incluindo projetos concluídos ou inativos, independentemente das preferências do grupo do projeto permitirem ou não.

1. Na seção **Preencher folhas de horas previamente**, configure uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Trabalho que está dentro de &lt;número de semanas&gt; do intervalo de trabalho da folha de horas</td> 
      <td> <p>Define o número de semanas antes e depois do intervalo de datas da folha de horas que contém datas de tarefas e problemas atribuídas ao usuário. A configuração padrão é 1 semana e você pode estender esse intervalo para 4 semanas. Isso significa que a folha de horas é pré-preenchida com tarefas e problemas que têm datas em qualquer lugar entre quatro semanas antes do intervalo de datas da folha de horas até quatro semanas após o intervalo de datas da folha de horas, se você selecionar 4 semanas para o seu intervalo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tarefas e problemas que foram concluídos</td> 
      <td>Se vários recursos forem normalmente atribuídos a uma única tarefa, recomendamos essa configuração. Isso significa que quando um recurso registra o tempo na tarefa e o marca como concluído, os outros recursos atribuídos à tarefa ainda podem encontrar a tarefa ou o problema em sua folha de horas, para registrar suas horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tarefas e problemas que têm Datas planejadas no intervalo de datas da folha de horas</td> 
      <td> <p>Quando selecionada, a folha de horas inclui tarefas e problemas que têm uma Data de início planejada ou uma Data de conclusão que está dentro do intervalo de datas da folha de horas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Tarefas que têm Datas Projetadas no intervalo de datas da folha de horas</td> 
      <td> <p>Quando selecionada, a folha de horas inclui tarefas que têm uma Data de Início Projetada ou uma Data de Conclusão dentro do intervalo de tempo do projeto, mesmo se a data planejada da ocorrência ou tarefa estiver fora do intervalo de datas da folha de horas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
