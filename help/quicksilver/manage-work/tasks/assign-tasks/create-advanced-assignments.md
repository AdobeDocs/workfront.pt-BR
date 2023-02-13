---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Criar atribuições avançadas
description: Você pode gerenciar atribuições de tarefa ou emissão usando Atribuições Avançadas.
author: Alina
feature: Work Management
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '1135'
ht-degree: 0%

---

# Criar atribuições avançadas

Você pode gerenciar atribuições de tarefa ou emissão usando Atribuições Avançadas.

Você pode ajustar as seguintes informações de atribuição ao fazer atribuições avançadas:

* Atribua usuários à tarefa ou ao problema (isso pode ser feito fora de uma atribuição avançada).
* Ajustar e redistribuir o número de horas alocadas por cada destinatário.
* Determine qual usuário deve ser designado como proprietário ou destinatário principal da tarefa ou problema.
* Especifique qual função cada usuário está cumprindo ao trabalhar na tarefa ou problema.

>[!NOTE]
>
>Ao atribuir usuários ao trabalho, sua disponibilidade de acordo com suas programações afeta as Datas Planejadas e Projetadas das tarefas e problemas. Para obter informações sobre programações, consulte [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Áreas do Adobe Workfront onde você pode fazer atribuições avançadas

Este artigo descreve como acessar Atribuições avançadas no cabeçalho da tarefa ou ocorrência.

Além disso, você pode fazer atribuições avançadas nas seguintes áreas do Workfront:

* Em listas e relatórios quando o campo Atribuições é exibido na visualização.
* Na seção Atribuições ao editar uma tarefa. Para obter mais informações, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).
* No cabeçalho da tarefa ou do problema, na área Atribuições.
* No Balanceador de Carga de Trabalho. Para obter mais informações, consulte [Atribuir trabalho manualmente usando o Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

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
   <td> <p>Editar acesso a tarefas e problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Contribuir com permissões ou permissões mais altas para uma tarefa ou problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Fazer atribuições avançadas

1. Vá para o projeto onde deseja atribuir uma tarefa ou um problema.
1. Clique em **Tarefas** ou **Problemas** no painel esquerdo, clique no nome de uma tarefa ou problema na lista.

   >[!TIP]
   >
   >Você pode fazer atribuições avançadas diretamente na tarefa ou na lista de problemas se houver duas ou mais pessoas atribuídas. Clique dentro do **Atribuições** na mesma linha da tarefa ou problema, em seguida, clique no botão **Ícone Pessoas** para abrir a janela Atribuições avançadas. Pule para a etapa 5 para continuar criando atribuições avançadas.\
   >![](assets/nwe-advanced-assignments-350x55.png)   >

1. Clique em **Atribuir a** no **Atribuições** no cabeçalho da tarefa ou do problema

   Ou

   Clique no nome das atribuições se a tarefa ou problema já estiver atribuído.

1. Clique em **Avançado**.

   ![](assets/advanced-assignments-link-from-task-header-nwe-350x267.png)

1. No **Pesquisar pessoas, funções e equipes** , comece digitando o nome de um usuário, função ou equipe e clique no nome quando ele for exibido na lista suspensa.

   >[!NOTE]
   >
   >Se o nome do usuário contiver um caractere especial, você deverá incluir o caractere especial no campo de pesquisa.

1. (Opcional) Continue adicionando os destinatários na **Pesquisar pessoas, funções ou equipes** para adicionar vários recursos à tarefa ou ao problema.

   >[!TIP]
   >
   >* Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários ativos, funções de trabalho e equipes.
   >
   >
   >* Ao adicionar uma atribuição de usuário, observe o avatar, a Função primária do usuário ou seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os adiciona.
   >
   >
   >* Se um usuário, uma função de trabalho ou uma equipe tiver sido atribuída antes de ser desativada, ela permanecerá atribuída ao item de trabalho. Nesse caso, recomendamos o seguinte:
      >   
      >   * Atribua novamente o item de trabalho aos recursos ativos.
      >   * Associe os usuários em uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.


1. Para cada usuário na **Destinatário** , especifique as seguintes informações:


   * **Proprietário**: Passe o mouse sobre o nome do destinatário e clique em **Tornar principal** no campo Proprietário se desejar marcar o destinatário como a tarefa ou o proprietário da emissão. Uma caixa de seleção verde indica que o usuário especificado é o Contato Principal da tarefa ou problema. O Adobe Workfront marca o primeiro usuário ou função de trabalho que você atribui a uma tarefa ou problema como Proprietário ou Atribuição Principal. Uma equipe não pode ser designada como o Proprietário Principal de uma tarefa ou problema.

      >[!IMPORTANT]
      >
      >Dependendo de como o administrador do Workfront ou o administrador do grupo configuram as preferências do projeto, o Workfront pode usar o agendamento do proprietário da tarefa para calcular a linha do tempo da tarefa quando você tem vários usuários atribuídos à tarefa. Para obter informações sobre vários destinatários de tarefas, consulte a seção &quot;Atribuir vários usuários a uma tarefa&quot; no artigo [Atribuir tarefas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Alocações** : Quando o Tipo de duração de uma tarefa for Simples, especifique o número de horas que cada usuário ou função de trabalho deve ser atribuída à tarefa. A soma de todas as horas atribuídas para cada usuário é igual ao número na variável **Horas Planejadas** na parte inferior da coluna Alocações. Em todos os outros casos, especifique a porcentagem de tempo (ou alocação) que você deseja que o destinatário gaste resolvendo a tarefa ou o problema.

      <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: make sure this is right in the new UI for both classic and QS???)</p>   
     -->

      >[!TIP]
      >
      >
      >   
      >   
      >   * Após modificar manualmente as alocações de atribuições em tarefas, as Horas Planejadas das tarefas podem ser atualizadas adequadamente. Para obter mais informações, consulte a seção &quot;Atualizar tarefa Horas Planejadas ao gerenciar alocações de usuários&quot; no artigo [Visão geral das Horas Planejadas](../../../manage-work/tasks/task-information/planned-hours.md).
      >   * Não é possível modificar manualmente as alocações de atribuição em problemas.
      >   * Não é possível modificar manualmente as alocações de equipes atribuídas a tarefas.


   * **Função do destinatário:** Selecione a função que o usuário deve usar ao cumprir esta atribuição.  A Função principal do usuário é exibida por padrão. Clique na caixa Função do destinatário para selecionar outra função.  Quando você atribui a tarefa ou o problema a uma função primeiro e, em seguida, adiciona um usuário que possa cumprir essa função como uma segunda atribuição, a lista de usuários sugeridos é filtrada para os usuários que podem atender às funções já atribuídas à tarefa e ao problema.

      ![](assets/advanced-assignments-box-select-a-role-350x243.png)

   * **Tipo de duração**: Isso só está disponível para tarefas. Clique no nome do Tipo de duração e selecione um Tipo de duração no menu suspenso. Para obter informações sobre Tipos de duração, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duração:** Você pode atualizar este campo para uma tarefa quando tiver permissões de Gerenciamento para a tarefa.

      Para obter mais informações, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Ao editar informações de atribuição em massa, uma caixa de diálogo semelhante é exibida para atribuir usuários, horas, alocação e proprietário da tarefa.

   * **Horas Planejadas**: Quando o Tipo de duração for Atribuição calculada ou Simples, atualize o número de Horas planejadas. As porcentagens de alocação ou as horas de cada recurso são distribuídas igualmente como resultado. O Workfront calcula as Horas Planejadas quando o Tipo de Duração é Trabalho Calculado ou Orientado pelo Esforço. Para obter mais informações, consulte [Visão Geral da Duração da Tarefa e do Tipo de Duração](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

      ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

1. Clique em **Salvar**.
