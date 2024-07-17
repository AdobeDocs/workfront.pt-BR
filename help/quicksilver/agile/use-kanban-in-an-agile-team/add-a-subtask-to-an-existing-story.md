---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Adicionar uma subtarefa a uma história existente no quadro Kanban
description: Leia este artigo para saber como criar subtarefas para histórias existentes no quadro Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '366'
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

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Work] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso à [!UICONTROL Contribute] ou [!UICONTROL Manage] para a tarefa em que a subtarefa está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Adicionar uma subtarefa a uma história existente no quadro [!UICONTROL Kanban]

1. Vá para o quadro [!UICONTROL Kanban] que contém a história em que você deseja adicionar uma subtarefa.
1. Clique no nome da tarefa no bloco de história no quadro [!UICONTROL Kanban].
1. Adicione uma subtarefa à tarefa da mesma maneira que você faria em qualquer outra lista de tarefas em [!DNL Workfront], conforme descrito em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md).
