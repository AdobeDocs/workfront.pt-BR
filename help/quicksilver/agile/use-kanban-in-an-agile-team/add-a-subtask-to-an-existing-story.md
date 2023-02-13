---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Adicionar uma subtarefa a uma história existente no quadro Kanban
description: Revise este artigo para saber como criar subtarefas para histórias existentes no quadro Kanban.
author: Lisa
feature: Agile
exl-id: c6610616-80e5-4ded-9d23-63f15536e45c
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 0%

---

# Adicionar uma subtarefa a uma história existente no quadro Kanban

Ao criar subtarefas para histórias existentes, lembre-se do seguinte:

**Quando a variável [!UICONTROL Modo de conclusão do resumo] a configuração do projeto está definida como [!UICONTROL Manual]:**

* Você pode mover uma história pai com subtarefas para [!UICONTROL Concluído], que atualiza a história principal para 100% e a variável [!UICONTROL Status] para [!UICONTROL Concluído]. Subtarefas não são atualizadas.
* Para atualizar o [!UICONTROL Porcentagem concluída] para a história, você deve atualizá-la do [!UICONTROL Histórias] ou da guia [!UICONTROL Detalhes] página do objeto.

**Quando a variável [!UICONTROL Modo de conclusão do resumo] a configuração do projeto está definida como [!UICONTROL Automático]:**

* Você não pode mover a história principal através do quadro. Para atualizar o [!UICONTROL Porcentagem concluída] para a história, você deve atualizar o [!UICONTROL Porcentagem concluída] para quaisquer subtarefas. O [!UICONTROL Porcentagem concluída] para a história é calculada com base na variável [!UICONTROL Porcentagem concluída] de todas as subtarefas.
* Mover uma história pai com subtarefas para [!UICONTROL Concluído] atualiza a história pai para 100% e a variável [!UICONTROL Status] para [!UICONTROL Concluído]. As subtarefas também são atualizadas para 100% e a variável [!UICONTROL Status] é atualizado para [!UICONTROL Concluído].

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso ao [!UICONTROL Contribute] ou [!UICONTROL Gerenciar] para a tarefa na qual a subtarefa está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Adicionar uma subtarefa a uma história existente no [!UICONTROL Kanban] quadro

1. Vá para o [!UICONTROL Kanban] quadro que contém a história na qual você deseja adicionar uma subtarefa.
1. Clique no nome da tarefa no bloco de história na [!UICONTROL Kanban] quadro.
1. Adicione uma subtarefa à tarefa da mesma forma que faria em qualquer outra lista de tarefas dentro [!DNL Workfront], conforme descrito em [Criar subtarefas](../../manage-work/tasks/create-tasks/create-subtasks.md).
