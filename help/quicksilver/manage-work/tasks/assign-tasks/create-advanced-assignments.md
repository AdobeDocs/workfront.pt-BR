---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Criar atribuições avançadas
description: Você pode gerenciar atribuições de tarefas ou problemas usando as Atribuições Avançadas.
author: Alina
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 830ad0411084844ace1e1e543c3ebefcb558af80
workflow-type: tm+mt
source-wordcount: '1110'
ht-degree: 0%

---

# Criar atribuições avançadas

Você pode gerenciar atribuições de tarefas ou problemas usando as Atribuições Avançadas.

Você pode ajustar as seguintes informações de atribuição ao fazer atribuições avançadas:

* Atribuir usuários à tarefa ou problema (isso pode ser feito fora de uma atribuição avançada).
* Ajuste e redistribua o número de horas que cada destinatário é alocado.
* Determine qual usuário deve ser designado como o proprietário ou o Principal responsável pela tarefa ou problema.
* Especifique qual função cada usuário está cumprindo ao trabalhar na tarefa ou problema.
  <!--* <span class="preview">Override the billing rate for a job role.</span>-->

>[!NOTE]
>
>Ao atribuir usuários para trabalhar, sua disponibilidade de acordo com seus agendamentos afeta as Datas Planejadas e Projetadas de tarefas e problemas. Para obter informações sobre agendamentos, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Áreas do Adobe Workfront em que você pode fazer atribuições avançadas

Este artigo descreve como acessar Atribuições avançadas no cabeçalho da tarefa ou do problema.

Além disso, você pode fazer atribuições avançadas nas seguintes áreas do Workfront:

* Em listas e relatórios quando o campo Atribuições é exibido na visualização.
* Na seção Atribuições ao editar uma tarefa. Para obter mais informações, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* No cabeçalho da tarefa ou do problema, na área Atribuições.
* No Balanceador de carga de trabalho. Para obter mais informações, consulte [Atribuir trabalho manualmente usando o Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Padrão</p>
    <p>Atual: trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e problemas</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões do Contribute ou superiores para uma tarefa ou problema</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Fazer atribuições avançadas

1. Vá para o projeto ao qual deseja atribuir uma tarefa ou um problema.
1. Clique em **Tarefas** ou **Problemas** no painel esquerdo e, em seguida, clique no nome de uma tarefa ou problema na lista.

   >[!TIP]
   >
   >Você pode fazer atribuições avançadas diretamente na lista de tarefas ou problemas se houver duas ou mais pessoas atribuídas. Clique dentro do campo **Atribuições** na mesma linha da tarefa ou problema e clique no **ícone Pessoas** para abrir a janela Atribuições Avançadas. Vá para a etapa 5 para continuar criando atribuições avançadas.\
   >![](assets/nwe-advanced-assignments-350x55.png)
   >

1. Clique em **Atribuir a** no campo **Atribuições** no cabeçalho da tarefa ou problema

   Ou

   Clique no nome das atribuições se a tarefa ou problema já estiver atribuído.

1. Clique em **Avançado**.

   ![Clique em Avançado](assets/assignments-box-in-task-header.png)

1. No campo **Pesquisar pessoas, funções e equipes**, comece digitando o nome de um usuário, função ou equipe e clique no nome quando ele aparecer na lista suspensa.

   >[!NOTE]
   >
   >Se o nome do usuário contiver um caractere especial, você deverá incluí-lo no campo de pesquisa.

1. (Opcional) Continue adicionando atribuídos na caixa **Pesquisar pessoas, funções ou equipes** para adicionar vários recursos à tarefa ou problema.

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
   >

   <!-- SHOULD BE THIRD BULLET POINT IN TIP TABLE WHEN THIS FEATURE IS RELEASED 
    * <span class="preview">When adding a job role assignment, you can search for the job role or location. Select the System/Default Job Role to use the default billing rate for the assignment, or select a Rate Card Job Role to override the rate at the assignment level. For more information on rate cards, see [Manage rate cards](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).</span>
    -->

1. Para cada usuário na coluna **Destinatário**, especifique as seguintes informações:


   * **Proprietário**: passe o mouse sobre o nome do destinatário e clique em **Tornar primário** no campo Proprietário se desejar marcar o destinatário como o proprietário da tarefa ou do problema. Uma caixa de seleção verde indica que o usuário especificado é o contato principal da tarefa ou problema. O Adobe Workfront marca o primeiro usuário ou função de trabalho atribuída a uma tarefa ou problema como Proprietário ou Atribuição principal. Uma equipe não pode ser designada como o Proprietário principal de uma tarefa ou problema.

     >[!IMPORTANT]
     >
     >Dependendo de como o administrador do Workfront ou o administrador de grupo configuram as preferências do projeto, a Workfront pode usar o agendamento do proprietário da tarefa para calcular a linha do tempo da tarefa quando vários usuários estão atribuídos a ela. Para obter informações sobre vários atribuídos de tarefa, consulte a seção &quot;Atribuir vários usuários a uma tarefa&quot; no artigo [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Alocações**: quando o Tipo de Duração de uma tarefa for Simples, especifique o número de horas que cada usuário ou função de trabalho deve ser atribuída à tarefa. A soma de todas as horas atribuídas para cada usuário é igual ao número no campo **Horas planejadas**, na parte inferior da coluna Alocações. Em todos os outros casos, especifique a porcentagem de tempo (ou alocação) que você deseja que o destinatário passe resolvendo a tarefa ou problema.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

     >[!TIP]
     >
     >
     >   
     >   
     >   * Depois de modificar manualmente as alocações de atribuição em tarefas, as Horas Planejadas das tarefas podem ser atualizadas de acordo. Para obter mais informações, consulte a seção &quot;Atualizar horas planejadas da tarefa ao gerenciar alocações de usuário&quot; no artigo [visão geral sobre horas planejadas](../../../manage-work/tasks/task-information/planned-hours.md).
     >   * Não é possível modificar manualmente as alocações de atribuição em ocorrências.
     >   * Não é possível modificar manualmente as alocações de equipes atribuídas a tarefas.
     >   
     >

   * **Função do destinatário:** selecione a função que o usuário deve usar ao realizar esta atribuição.  A Função principal do usuário é exibida por padrão. Clique na caixa Função do responsável para selecionar outra função.  Ao atribuir a tarefa ou o problema a uma função primeiro e, em seguida, adicionar um usuário que pode desempenhar essa função como uma segunda atribuição, a lista de usuários sugeridos é filtrada para os usuários que podem desempenhar as funções já atribuídas à tarefa e ao problema.

     ![Função do destinatário](assets/advanced-assignments-select-role.png)

   <!--<div class="preview">

   * **Location**: The location comes from the rate card, if a rate card attached to the project uses locations with the job roles. The location can't be changed. 

   * **Billing Rates**: The billing rate for a user comes from the system rate for the user or their associated job role. The billing rate for a job role comes from the system rate or from the rate card, if a rate card is attached to the project. Existing billing rates are not displayed in this field. Click in the field to change the billing rate for this specific task assignment.

   </div>-->

   * **Tipo de Duração**: somente disponível para tarefas. Clique no nome do Tipo de duração e selecione um Tipo de duração no menu suspenso. Para obter informações sobre Tipos de Duração, consulte [Visão Geral da Duração e do Tipo de Duração da Tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duração:** é possível atualizar este campo para uma tarefa quando você tem permissões para Gerenciar a tarefa.

     Para obter mais informações, consulte [Visão geral da duração e do tipo de duração da tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Ao editar informações de atribuição em massa, uma caixa de diálogo semelhante é exibida para atribuir usuários, horas, alocação e proprietário da tarefa.

   * **Horas planejadas**: quando o tipo de duração for Atribuição calculada ou Simples, atualize o número de Horas planejadas. Como resultado, as porcentagens de alocação ou as horas de cada recurso são distribuídas uniformemente. O Workfront calcula as horas planejadas quando o tipo de duração é Trabalho calculado ou orientado pelo esforço. Para obter mais informações, consulte [Visão geral da duração e do tipo de duração da tarefa](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).


1. Clique em **Salvar**.
