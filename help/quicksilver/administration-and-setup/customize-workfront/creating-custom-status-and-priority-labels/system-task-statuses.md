---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Status da tarefa do sistema
description: Os três status de tarefa do sistema incorporados no Workfront são necessários, o que significa que você pode desbloqueá-los, renomeá-los e reorganizá-los, mas não pode ocultá-los ou excluí-los. Você também pode adicionar novos status de tarefa do sistema para atender às necessidades em sua organização. Alterar o status de uma tarefa normalmente é um processo manual, mas às vezes o status de uma tarefa é alterado automaticamente, dependendo de outros fatores que estão acontecendo no sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Status da tarefa do sistema

Os três status de tarefa do sistema incorporados no Workfront são necessários, o que significa que você pode desbloqueá-los, renomeá-los e reorganizá-los, mas não pode ocultá-los ou excluí-los.

Você também pode adicionar novos status de tarefa do sistema para atender às necessidades em sua organização.

A alteração do status de uma tarefa geralmente é um processo manual. No entanto, há momentos descritos na lista a seguir quando o status de uma tarefa é alterado automaticamente, dependendo de outros fatores que estão acontecendo no sistema.

Os seguintes status de tarefa são fornecidos com sua instância do Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status da tarefa do sistema</th> 
   <th>Quando este status ocorrer</th> 
   <th>Ações que ocorrem quando uma tarefa está nesse status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Novo (status obrigatório)</td> 
   <td>Este é o status padrão para cada tarefa recém-criada.</td> 
   <td>Se a tarefa estiver em um projeto no status Atual, ela será exibida na guia Solicitações de Trabalho dos usuários atribuídos às tarefas. Os usuários agora podem começar a trabalhar na tarefa.</td> 
  </tr> 
  <tr> 
   <td>Em Andamento (status obrigatório)</td> 
   <td>Você pode colocar uma tarefa nesse status para indicar que o trabalho nessa tarefa foi iniciado.</td> 
   <td> <p>Quando você marca uma tarefa como Em Andamento, ela mostra um valor para a Data de Início Real.</p> <p>O progresso na tarefa não é registrado até que você atualize manualmente o percentual de conclusão da tarefa.</p> </td> 
  </tr> 
  <tr> 
   <td>Concluído (status necessário)</td> 
   <td> <p>Você pode marcar manualmente uma tarefa como concluída quando o trabalho nela for concluído.</p> <p>Quando o Modo de rastreamento de uma tarefa é definido como Preenchimento automático, a tarefa é automaticamente marcada como Concluído quando atinge a Data de conclusão planejada.</p> </td> 
   <td> <p>Quando uma tarefa é concluída, a porcentagem completa da tarefa é marcada como 100%. A tarefa é removida da Lista de Trabalho do destinatário na área Inicial quando é concluída.</p> <p>Quando você marca uma tarefa como Concluída, a tarefa mostra um valor para a Data de Conclusão Real.</p> <p><b>OBSERVAÇÃO</b>: Se a tarefa tiver problemas incompletos e você alterar o status da tarefa para Concluído, o status será alterado automaticamente para Concluído - Problemas pendentes.</p> </td> 
  </tr> 
 </tbody> 
</table>
