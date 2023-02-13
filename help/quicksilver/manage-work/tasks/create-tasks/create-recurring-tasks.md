---
product-area: projects
navigation-topic: create-tasks
title: Criar tarefas recorrentes
description: Você pode criar tarefas recorrentes para tarefas que você precisa repetir como parte de um único projeto.
author: Alina
feature: Work Management
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Criar tarefas recorrentes

Você pode criar tarefas recorrentes para tarefas que você precisa repetir como parte de um único projeto.

Para obter informações gerais sobre tarefas recorrentes, incluindo o impacto da edição de uma tarefa recorrente existente, consulte [Visão geral das tarefas recorrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

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
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a tarefas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Conceder acesso a tarefas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões para o projeto com capacidade de adicionar tarefas ou superior</p> <p>Ao criar uma tarefa, você recebe automaticamente permissões de gerenciamento para a tarefa</p> <p> Para obter informações sobre permissões de tarefa, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartilhar uma tarefa </a>. </p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar uma tarefa recorrente

>[!NOTE]
>
>Não é possível criar uma tarefa recorrente modificando uma tarefa existente. Você deve criar uma tarefa do zero.

1. Vá para o projeto onde deseja criar uma tarefa recorrente e clique no botão **Tarefas** no painel esquerdo.
1. Clique em **Nova tarefa**.

   A caixa de diálogo Nova tarefa é exibida.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Clique em **Mais opções** em seguida, insira um nome para a tarefa no **Nome da tarefa** campo.
1. Continue atualizando a tarefa da mesma forma que faria se adicionasse uma nova tarefa. Para obter mais informações sobre como adicionar uma nova tarefa, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)
1. Clique em **Visão geral** no painel esquerdo.
1. Role para baixo até a **Programação de Periodicidade** e selecione a **Tornar isso uma tarefa recorrente** opção.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. No **Frequência** na lista suspensa, selecione o número de unidades de tempo em que deseja que a tarefa ocorra e o tipo de unidades de tempo. Selecione dentre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Tipo de periodicidade</th> 
      <th>Descrição</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Dia</strong> </td> 
      <td> <p>A tarefa se repete todos os dias, a cada 2 dias, a cada 3 dias e assim por diante, dependendo da cadência selecionada. Você pode configurar tarefas para repetir até cada 6 dias. A configuração padrão é 1 dia. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dia útil</strong> </td> 
      <td> <p> A tarefa se repete a cada dia útil, a cada 2 dias úteis, a cada 3 dias úteis e assim por diante, dependendo da cadência selecionada. Você pode configurar tarefas para repetir até cada 6 dias úteis.</p> <p>Essa opção usa o agendamento padrão definido pelo administrador do sistema, conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Semana</strong> </td> 
      <td> <p> A tarefa se repete a cada semana, a cada 2 semanas, a cada 3 semanas e assim por diante, dependendo da cadência selecionada.</p> <p>No <strong>Repetir</strong> selecione o dia da semana em que deseja que cada tarefa ocorra. Você pode selecionar vários dias. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mês</strong> </td> 
      <td> <p>A tarefa se repete a cada mês, a cada 2 meses, a cada 3 meses e assim por diante, dependendo da cadência selecionada. Você pode selecionar entre 1 e 12 meses. </p> <p>No <strong>Repetir</strong> selecione entre as seguintes opções quando desejar que a tarefa ocorra:</p> 
       <ul> 
        <li> <p><strong>todos os meses no dia &lt;month date=""&gt;</strong> </p> <p>Você pode selecionar dias de 1 a 30 ou pode selecionar <strong>last</strong>. Por exemplo, você pode selecionar "todo mês no dia 30". </p> </li> 
        <li> <p><strong>todos os meses no &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>No primeiro menu suspenso, é possível selecionar um número entre 1 e 4 para o número da semana no mês, ou selecionar "último". </p> <p>No segundo menu suspenso, é possível selecionar qualquer dia da semana. </p> <p>Por exemplo, você pode selecionar "todo mês na segunda terça-feira". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Se você tiver uma Exceção de Programação associada ao agendamento do projeto, as tarefas recorrentes não poderão ser iniciadas durante a exceção. As tarefas recorrentes que ocorrem durante a exceção de programação são programadas para iniciar no primeiro dia útil que segue a exceção. Para obter mais informações sobre exceções de programação, consulte o artigo [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. No **Inícios** selecione a data e a hora em que deseja que as tarefas recorrentes sejam iniciadas.
1. No **Termina** selecione a data e a hora em que deseja que as tarefas recorrentes sejam concluídas

   Ou

   Selecionar **after `<number>` ocorrências** para indicar quantas vezes a tarefa recorrente deve ocorrer. O Workfront cria o mesmo número de recorrências para as tarefas que o número indicado neste campo.

1. Clique em **Criar tarefa.**

   A lista de tarefas é exibida. A tarefa recorrente é criada como pai e todas as recorrentes são seus filhos. O Workfront gerou automaticamente os nomes das tarefas filho, usando o nome inserido para o pai seguido de um número. Para obter mais informações sobre quais campos são preenchidos automaticamente a partir da tarefa pai recorrente, consulte [Visão geral das tarefas recorrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Opcional) Modifique cada tarefa recorrente da mesma forma que faria com qualquer outra tarefa no projeto.

   Por exemplo, você pode adicionar atribuições, antecessores, durações e modificar qualquer outra informação sobre a tarefa, incluindo campos personalizados.

   >[!IMPORTANT]
   >
   >Modificar a recorrência do pai após os filhos terem sido modificados individualmente pode causar informações diferentes entre os filhos ou entre eles e o pai. Para obter mais informações, consulte [Visão geral das tarefas recorrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
