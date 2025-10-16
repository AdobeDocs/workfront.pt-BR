---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Adicionar uma subtarefa a uma história existente no Quadro Kanban
description: Leia este artigo para saber como criar subtarefas para histórias existentes no quadro Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%

---

# Adicionar uma subtarefa a uma história existente no quadro Kanban

Ao criar subtarefas para matérias existentes, lembre-se do seguinte:

**Quando a configuração [!UICONTROL Modo de Conclusão de Resumo] do projeto estiver definida como [!UICONTROL Manual]:**

* Você pode mover uma matéria pai com subtarefas para [!UICONTROL Concluído], o que atualiza a matéria pai para 100% e o [!UICONTROL Status] para [!UICONTROL Concluído]. As subtarefas não são atualizadas.
* Para atualizar o [!UICONTROL Percentual concluído] da matéria, atualize-o na guia [!UICONTROL Histórias] ou na página [!UICONTROL Detalhes] do objeto.

**Quando a configuração [!UICONTROL Modo de Conclusão de Resumo] do projeto estiver definida como [!UICONTROL Automático]:**

* Você não pode mover a história principal pelo tabuleiro. Para atualizar o [!UICONTROL Percentual concluído] da matéria, você deve atualizar o [!UICONTROL Percentual concluído] para qualquer subtarefa. O [!UICONTROL Percentual concluído] da história é calculado com base no [!UICONTROL Percentual concluído] de todas as subtarefas.
* Mover uma matéria pai com subtarefas para [!UICONTROL Concluído] atualiza a matéria pai para 100% e o [!UICONTROL Status] para [!UICONTROL Concluído]. Subtarefas também são atualizadas para 100% e o [!UICONTROL Status] é atualizado para [!UICONTROL Concluído].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p> 
   <p>Trabalhar ou superior</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Contribuir ou gerenciar o acesso à tarefa da subtarefa</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar uma subtarefa a uma história existente no quadro [!UICONTROL Kanban]

1. Vá para o quadro [!UICONTROL Kanban] que contém a história em que você deseja adicionar uma subtarefa.
1. Clique no nome da tarefa no bloco de história no quadro [!UICONTROL Kanban].
1. Adicione uma subtarefa à tarefa da mesma maneira que você faria em qualquer outra lista de tarefas em [!DNL Workfront], conforme descrito em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md).
