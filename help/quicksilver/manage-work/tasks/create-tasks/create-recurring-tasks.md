---
product-area: projects
navigation-topic: create-tasks
title: Criar tarefas recorrentes
description: É possível criar tarefas recorrentes para tarefas que você precisa repetir como parte de um único projeto.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: dbde5419-02ce-456b-a430-b2825d81fb87
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Criar tarefas recorrentes

É possível criar tarefas recorrentes para tarefas que você precisa repetir como parte de um único projeto.

Para obter informações gerais sobre tarefas recorrentes, incluindo o impacto da edição de uma tarefa recorrente existente, consulte [Visão geral das tarefas recorrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre o acesso a tarefas, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Conceder acesso a tarefas</a>. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões para o projeto com a capacidade de adicionar tarefas ou superior</p> <p>Ao criar uma tarefa, você recebe automaticamente permissões Gerenciar para a tarefa</p> <p> Para obter informações sobre permissões de tarefas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Compartilhar uma tarefa </a>. </p> <p>Para obter informações sobre a solicitação de permissões adicionais, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Criar uma tarefa recorrente

>[!NOTE]
>
>Não é possível criar uma tarefa recorrente modificando uma tarefa existente. Você deve criar uma tarefa do zero.

1. Vá para o projeto em que deseja criar uma tarefa recorrente e clique no botão **Tarefas** no painel esquerdo.
1. Clique em **Nova tarefa**.

   A caixa de diálogo Nova Tarefa é exibida.

   ![](assets/nwe-create-task-small-screen-350x272.png)

1. Clique em **Mais opções** em seguida, insira um nome para a tarefa no campo **Nome da tarefa** campo.
1. Continue atualizando a tarefa da mesma forma que faria se adicionasse uma nova tarefa. Para obter mais informações sobre como adicionar uma nova tarefa, consulte [Criar tarefas em um projeto](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

   >[!TIP]
   >
   >   A Duração e as Horas planejadas indicadas para uma nova tarefa recorrente são a Duração e as Horas planejadas de cada ocorrência. A Duração da tarefa pai é o tempo entre a Data de Início Planejada da tarefa mais antiga e a Data de Conclusão Planejada da tarefa mais recente. As Horas Planejadas da tarefa pai é o total de todas as Horas Planejadas de todas as ocorrências.

1. Clique em **Visão geral** no painel esquerdo.
1. Role para baixo até **Agendamento recorrente** e selecione o **Tornar esta uma tarefa recorrente** opção.

   ![](assets/recurrence-schedule-section-new-recurring-tasks-nwe-350x351.png)

1. No **Frequência** selecione o número de unidades de tempo quando você deseja que a tarefa ocorra e o tipo de unidades de tempo. Selecione entre as seguintes opções:

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
      <td> <p>A tarefa é repetida todos os dias, a cada dois dias, a cada três dias e assim por diante, dependendo da cadência selecionada. Você pode configurar tarefas para repetição até o dia 6. A configuração padrão é 1 dia. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dia de Trabalho</strong> </td> 
      <td> <p> A tarefa se repete todos os dias úteis, a cada dois dias úteis, a cada três dias úteis e assim por diante, dependendo da cadência selecionada. Você pode configurar tarefas para repetir até a cada 6° dia útil.</p> <p>Essa opção usa o agendamento padrão definido pelo administrador do sistema, conforme descrito em <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Criar um agendamento</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Semana</strong> </td> 
      <td> <p> A tarefa é repetida a cada semana, a cada 2 semanas, a cada 3 semanas e assim por diante, dependendo da cadência selecionada.</p> <p>No <strong>Repetições</strong> selecione o dia da semana em que deseja que cada tarefa ocorra. Você pode selecionar vários dias. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mês</strong> </td> 
      <td> <p>A tarefa é repetida a cada mês, a cada dois meses, a cada três meses e assim por diante, dependendo da cadência selecionada. Você pode selecionar entre 1 e 12 meses. </p> <p>No <strong>Repetições</strong> selecione entre as seguintes opções quando quiser que a tarefa ocorra:</p> 
       <ul> 
        <li> <p><strong>todos os meses no dia &lt;month date=""&gt;</strong> </p> <p>Você pode selecionar dias de 1 a 30 ou selecionar <strong>último</strong>. Por exemplo, você pode selecionar "todo mês no dia 30". </p> </li> 
        <li> <p><strong>todos os meses no &lt;number&gt; &lt;day of="" the="" week=""&gt;</strong> </p> <p>No primeiro menu suspenso, você pode selecionar um número entre 1 e 4 para o número da semana no mês ou selecionar "último". </p> <p>No segundo menu suspenso, é possível selecionar qualquer dia da semana. </p> <p>Por exemplo, você pode selecionar "todo mês na 2ª terça-feira". </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Se você tiver uma Exceção de Cronograma associada ao cronograma do projeto, as tarefas recorrentes não poderão ser iniciadas durante a exceção. As tarefas recorrentes que ocorrem durante a exceção de programação são programadas para iniciar no primeiro dia útil após a exceção. Para obter mais informações sobre exceções de cronograma, consulte o artigo [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

1. No **Início** selecione a data e a hora em que deseja que as tarefas recorrentes comecem.
1. No **Término** selecione a data e a hora em que deseja que as tarefas recorrentes sejam concluídas

   Ou

   Selecionar **após `<number>` ocorrências** para indicar quantas vezes a tarefa recorrente deve ocorrer. O Workfront cria o mesmo número de recorrências para as tarefas que o número indicado neste campo.

1. Clique em **Criar tarefa.**

   A lista de tarefas é exibida. A tarefa recorrente é criada como um pai e todas as recorrências são seus filhos. O Workfront gerou automaticamente os nomes das tarefas filhas, usando o nome inserido para o pai seguido por um número. Para obter mais informações sobre quais campos são preenchidos automaticamente na tarefa pai recorrente, consulte [Visão geral das tarefas recorrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).

   ![](assets/recurring-tasks-in-task-list-nwe-350x87.png)

1. (Opcional) Modifique cada tarefa recorrente como faria com qualquer outra tarefa no projeto.

   Por exemplo, você pode adicionar atribuições, predecessores, durações e modificar quaisquer outras informações sobre a tarefa, incluindo campos personalizados.

   >[!IMPORTANT]
   >
   >Modificar a recorrência pai depois que os filhos forem modificados individualmente pode causar informações diferentes entre os filhos ou entre os filhos e o pai. Para obter mais informações, consulte [Visão geral das tarefas recorrentes](../../../manage-work/tasks/manage-tasks/recurring-tasks-overview.md).
