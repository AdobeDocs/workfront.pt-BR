---
user-type: administrator
product-area: system-administration;user-management
keywords: grupo,preferências,tarefa,grupos,problema,desbloquear
navigation-topic: create-and-manage-groups
title: Configurar as preferências de hora e folha de ponto para um grupo
description: No nível do sistema, um administrador do Adobe Workfront pode desbloquear as seções de folha de ponto e hora de preferência Preferências Gerais e Preencher folhas de ponto com. Isso permite que os administradores de grupo configurem as opções nessas seções de maneira independente para seus próprios grupos.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: 3b0a82381d1c33d897b123a597df21ba54cc2565
workflow-type: tm+mt
source-wordcount: '1368'
ht-degree: 5%

---

# Configurar as preferências de hora e folha de ponto para um grupo

{{highlighted-preview}}

Um administrador do Adobe Workfront pode desbloquear as seguintes seções de folhas de horas e preferências de hora no nível do sistema para que os administradores de grupo possam configurá-las independentemente para seus próprios grupos:

* Preferências gerais
* <span class="preview">Onde os usuários podem registrar o tempo</span>
* Preencher previamente folhas de ponto

Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

As seguintes seções na página Folha de Horas e Preferências de Horas são configuráveis somente no nível do sistema e não podem ser desbloqueadas para grupos:

* Projetos, tarefas e problemas excluídos

Para obter informações sobre como um administrador do Workfront desbloqueia uma folha de ponto e uma preferência de hora, consulte a seção [Desbloquear folha de horas e preferências de hora para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) no artigo [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>A configuração de nível de grupo também é possível para preferências de projeto e para preferências de tarefa e emissão. Para obter mais informações, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) e [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Preferências de hora e hora do grupo

Considere as seguintes informações sobre a configuração de uma folha de ponto desbloqueada ou a preferência de hora para um grupo:

* Se você for um administrador de grupo e configurar uma folha de ponto ou preferência de hora para seu grupo, isso afetará as pessoas que usam o grupo como Grupo doméstico.
* Normalmente, uma preferência desbloqueada permanece desbloqueada indefinidamente. Se o administrador do Workfront rebloquear, a configuração do sistema entrará em vigor novamente e as configurações da preferência feitas pelos administradores do grupo serão perdidas.
* Uma folha de ponto herda as preferências de hora e folha de ponto configuradas para o Grupo Doméstico do proprietário da folha de ponto.

   <!--
  Add example here?
  -->

* Depois que um administrador do Workfront desbloquear uma preferência no nível do sistema e você configurá-la para seu grupo, você poderá bloqueá-la para garantir que todos nos grupos abaixo do seu estejam usando a mesma configuração. Isso é paralelo à capacidade de um administrador do Workfront configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear uma folha de horas e uma preferência de hora do grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Configurar uma folha de ponto ou preferência de hora desbloqueada para um grupo

>[!TIP]
>
>Se você for um administrador do Workfront, é possível ignorar as etapas 1 a 4, acessando Configurar > Folha de Horas e Horas > Preferências e, em seguida, pesquisando o nome do grupo na caixa na parte superior da página.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo cujas preferências de hora ou hora você deseja configurar.
1. No painel esquerdo, clique em **Folhas de Horas e Horas**.

1. Na página que é exibida, no **Preferências gerais** configure qualquer uma das seguintes opções:

   >[!TIP]
   >
   >Se você passar o mouse sobre uma preferência e uma dica de ferramenta for exibida para informá-lo que está bloqueada, você pode solicitar que o administrador do Workfront a desbloqueie para todos os grupos na organização.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Registrar horas para datas futuras</td> 
      <td> <p>Permite aos usuários registrar tempo para datas futuras em todo o sistema em:</p> 
       <ul> 
       <li>Quaisquer projetos, tarefas e problemas em que tenham acesso ao tempo de registro, independentemente do grupo do projeto</li> 
       <li>Suas folhas de ponto como Tempo Geral</li>
       </ul> 
       <p>Isso é útil quando os usuários planejam estar longe do escritório e desejam registrar esse tempo com antecedência.</p> 
       <p><b>OBSERVAÇÃO</b>: Não é possível impedir que os usuários registrem tempo em tarefas ou problemas que estejam fechados ou cancelados. Você só pode impedir que os usuários façam logon em projetos concluídos ou inativos. Recomendamos usar filtros em listas de tarefas e problemas para excluir as que foram concluídas ou canceladas da visibilidade para os usuários.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Adicionar despesas de uma planilha de horas</td> 
      <td> <p>Permite que os usuários registrem tempo e despesas na folha de ponto.</p> 
      <p>Quando essa preferência é ativada para um grupo e o grupo é definido como o grupo inicial para determinados usuários, um ícone de despesa é exibido ao lado de projetos e tarefas nas folhas de ponto desses usuários. Os usuários podem clicar nesse ícone para adicionar ou editar despesas do projeto ou tarefa.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Atribuir Funções de Trabalho a entradas de hora manualmente</td> 
      <td> <p>Permitir que os usuários selecionem manualmente qualquer Função de trabalho atribuída em seu perfil de usuário ou atribuída ao objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Se você desativar essa configuração depois de atribuir funções de trabalho a entradas de hora, os usuários deverão ajustar as horas registradas em várias funções na guia Horas do projeto, tarefa ou problema.</li> 
         <li>Se o usuário não tiver uma função de trabalho atribuída em seu perfil e houver uma tarefa atribuída como o Proprietário da Tarefa na caixa de diálogo Atribuições Avançadas, essa função de trabalho será exibida quando o usuário registrar o tempo na tarefa.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restringir a edição da planilha de horas aos proprietários e administradores</td> 
      <td> <p>Restrinja a edição aos proprietários da folha de ponto, independentemente do grupo do projeto e dos administradores do Workfront. Quando essa opção está desativada, as folhas de horas também podem ser editadas por:</p> 
       <ul> 
        <li> <p>Usuários com acesso administrativo a folhas de ponto e horas em seu nível de acesso</p> </li> 
        <li> <p>Aprovadores da folha de ponto se "Pode editar horas" estiver ativado na folha de ponto</p> </li> 
        <li> <p>O gerente do proprietário da folha de ponto</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Restringir edição de hora a proprietários e administradores</td> 
      <td>Restrinja a edição ao usuário que inseriu as horas e administradores do Workfront. Essa configuração se aplica à guia Horas em um projeto ou em um relatório de Horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. <span class="preview">No **Onde os usuários podem registrar o tempo** configure qualquer uma das seguintes opções:</span>

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><span class="preview">Registrar o tempo diretamente nos projetos</span></td> 
      <td><span class="preview">Permite que os usuários façam logon no projeto (tanto na guia Atualizações quanto na folha de horas). Se quiser restringir o tempo de gravação dos usuários no nível do projeto, deixe essa opção desmarcada.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview">Registrar o tempo em projetos concluídos</span></td>
      <td><span class="preview">Permite que os usuários registrem o tempo em um projeto que foi marcado como concluído. Se essa opção estiver desativada, os usuários não poderão registrar tempo para o trabalho que concluíram nos projetos no status Concluído .</span></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview">Registrar o tempo em projetos mortos</span></td> 
      <td><span class="preview">Quando essa opção é ativada, os usuários podem registrar horas em projetos com um status de Inativo.</span></td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Essa preferência é aplicada com base na configuração das preferências do Grupo doméstico do usuário. Se essas configurações estiverem ativadas nas preferências do Grupo doméstico do usuário, ele poderá registrar o tempo diretamente nos projetos, incluindo projetos concluídos ou inativos, independentemente das preferências de grupo do projeto permitirem ou não.

1. No **Preencher previamente folhas de ponto** configure qualquer uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Trabalho que está dentro &lt;number of="" weeks=""&gt; do intervalo de trabalho da folha de ponto</td> 
      <td> <p>Define o número de semanas antes e depois do intervalo de datas da folha de ponto que contém datas de tarefas e problemas atribuídos ao usuário. A configuração padrão é 1 semana e você pode estender esse intervalo para 4 semanas. Isso significa que a folha de ponto é pré-preenchida com tarefas e problemas que têm datas entre quatro semanas antes do intervalo de datas da folha de ponto até quatro semanas após o intervalo de datas da folha de ponto, se você selecionar 4 semanas para o intervalo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tarefas e problemas que foram concluídos</td> 
      <td>Se vários recursos normalmente forem atribuídos a uma única tarefa, recomendamos essa configuração. Isso significa que, quando um recurso registra o tempo em relação à tarefa e a marca como concluída, os outros recursos atribuídos à tarefa ainda poderão encontrar a tarefa ou o problema em sua folha de ponto, para registrar suas horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tarefas e problemas que têm Datas planejadas no intervalo de datas da folha de horas</td> 
      <td> <p>Quando selecionada, a folha de ponto inclui tarefas e problemas que têm uma Data inicial planejada ou uma Data de conclusão que se enquadram no intervalo de datas da folha de ponto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Tarefas que têm datas projetadas no intervalo de datas da folha de dados</td> 
      <td> <p>Quando selecionada, a folha de ponto inclui tarefas que têm uma Data de Início Projetada ou uma Data de Conclusão que se enquadram no período do projeto, mesmo se a data planejada da emissão ou tarefa estiver fora do intervalo de datas da folha de ponto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
