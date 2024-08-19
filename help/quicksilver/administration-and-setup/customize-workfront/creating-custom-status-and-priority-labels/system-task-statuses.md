---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Status de tarefas do sistema
description: Os três status de tarefa do sistema incorporados no Workfront são obrigatórios, o que significa que você pode desbloqueá-los, renomeá-los e reordená-los, mas não pode ocultá-los ou excluí-los. Você também pode adicionar novos status de tarefas do sistema para atender às necessidades em sua organização. A alteração do status de uma tarefa geralmente é um processo manual, mas, às vezes, o status de uma tarefa é alterado automaticamente, dependendo de outros fatores que estão acontecendo no sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Status de tarefas do sistema

Os três status de tarefa do sistema incorporados no Workfront são obrigatórios, o que significa que você pode desbloqueá-los, renomeá-los e reordená-los, mas não pode ocultá-los ou excluí-los.

Você também pode adicionar novos status de tarefas do sistema para atender às necessidades em sua organização.

A alteração do status de uma tarefa geralmente é um processo manual. No entanto, há momentos descritos na lista a seguir quando o status de uma tarefa é alterado automaticamente, dependendo de outros fatores que estão acontecendo no sistema.

Os seguintes status de tarefa são fornecidos com a instância do Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status da tarefa do sistema</th> 
   <th>Quando este status ocorre</th> 
   <th>Ações que ocorrem quando uma tarefa está neste status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Novo (status obrigatório)</td> 
   <td>Esse é o status padrão para cada tarefa recém-criada.</td> 
   <td>Se a tarefa estiver em um projeto com o status Atual, ela será exibida na guia Solicitações de trabalho dos usuários atribuídos às tarefas. Os usuários agora podem começar a trabalhar na tarefa.</td> 
  </tr> 
  <tr> 
   <td>Em andamento (status obrigatório)</td> 
   <td>Você pode colocar uma tarefa neste status para indicar que o trabalho nessa tarefa foi iniciado.</td> 
   <td> <p>Quando você marca uma tarefa como Em Andamento, a tarefa mostra um valor para a Data Inicial Real.</p> <p>O progresso na tarefa não é registrado até que você atualize manualmente o percentual concluído da tarefa.</p> </td> 
  </tr> 
  <tr> 
   <td>Concluído (status obrigatório)</td> 
   <td> <p>Você pode marcar uma tarefa manualmente como concluída quando o trabalho nela for concluído.</p> <p>Quando o Modo de Rastreamento de uma tarefa é definido como Preenchimento Automático, a tarefa é automaticamente marcada como Concluída quando atinge a Data de Conclusão Planejada.</p> </td> 
   <td> <p>Quando uma tarefa é concluída, o percentual concluído da tarefa é marcado como 100%. A tarefa é removida da Lista de trabalho do destinatário na área da Página inicial quando é concluída.</p> <p>Quando você marca uma tarefa como Concluída, ela mostra um valor para a Data de Término Efetivo.</p> <p><b>OBSERVAÇÃO</b>: se a tarefa tiver problemas incompletos e você alterar o status da tarefa para Concluído, o status será alterado automaticamente para Concluído - Problemas Pendentes.</p> </td> 
  </tr> 
 </tbody> 
</table>
