---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Adicionar uma subtarefa a uma história existente no Quadro Kanban
description: Leia este artigo para saber como criar subtarefas para histórias existentes no quadro Kanban.
author: Courtney
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Wbiao1UjwOzItIGJkh1E9A81RcUfLDJqgYjRDL46qvQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 305
ht-degree: 14%

---

# Adicionar uma subtarefa a um story no quadro Kanban

Ao criar subtarefas para matérias existentes, lembre-se do seguinte:

**Quando a configuração [!UICONTROL Modo de Conclusão de Resumo] do projeto estiver definida como [!UICONTROL Manual]:**

* Você pode mover uma matéria pai com subtarefas para [!UICONTROL Concluído], o que atualiza a matéria pai para 100% e o [!UICONTROL Status] para [!UICONTROL Concluído]. As subtarefas não são atualizadas.
* Para atualizar o [!UICONTROL Percentual concluído] da matéria, atualize-o na guia [!UICONTROL Histórias] ou na página [!UICONTROL Detalhes] do objeto.

**Quando a configuração [!UICONTROL Modo de Conclusão de Resumo] do projeto estiver definida como [!UICONTROL Automático]:**

* Você não pode mover a história principal pelo tabuleiro. Para atualizar o [!UICONTROL Percentual concluído] da matéria, você deve atualizar o [!UICONTROL Percentual concluído] para qualquer subtarefa. O [!UICONTROL Percentual concluído] da história é calculado com base no [!UICONTROL Percentual concluído] de todas as subtarefas.
* Mover uma matéria pai com subtarefas para [!UICONTROL Concluído] atualiza a matéria pai para 100% e o [!UICONTROL Status] para [!UICONTROL Concluído]. Subtarefas também são atualizadas para 100% e o [!UICONTROL Status] é atualizado para [!UICONTROL Concluído].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <td> <p>Padrão</p> 
   <p>Trabalho ou maior</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Contribuir ou gerenciar o acesso à tarefa da subtarefa</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar uma subtarefa a uma história existente no quadro [!UICONTROL Kanban]

1. Vá para o quadro [!UICONTROL Kanban] que contém a história em que você deseja adicionar uma subtarefa.
1. Clique no nome da tarefa no bloco de história no quadro [!UICONTROL Kanban].
1. Adicione uma subtarefa à tarefa da mesma maneira que você faria em qualquer outra lista de tarefas em [!DNL Workfront], conforme descrito em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md).
