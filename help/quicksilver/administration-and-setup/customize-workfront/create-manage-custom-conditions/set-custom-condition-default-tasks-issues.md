---
title: Definir uma condição personalizada como padrão para tarefas e problemas
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Quando um usuário clica em Trabalhar nela ou adiciona um comentário de atualização a uma nova tarefa à qual foi atribuído (sem definir manualmente uma condição para a tarefa), o Adobe Workfront exibe a condição padrão para tarefas, que é configurada em Configuração. O mesmo se aplica às questões.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 1%

---

# Definir uma condição personalizada como padrão para tarefas e problemas

Quando um usuário clica em Trabalhar nela ou adiciona um comentário de atualização a uma nova tarefa à qual foi atribuído (sem definir manualmente uma condição para a tarefa), o Adobe Workfront exibe a condição padrão para tarefas, que é configurada em Configuração. O mesmo se aplica às questões.

O Workfront usa a condição integrada Indo bem como a condição padrão para tarefas e, separadamente, para problemas. Como administrador do Workfront, você pode alterar a condição padrão para ambos os tipos de objeto para uma condição personalizada criada.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Administrador de Sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Defina uma condição personalizada como uma condição padrão para tarefas ou problemas:

{{step-1-to-setup}}

1. Clique em **Preferências do projeto** > **Condições**.

1. Clique na guia **Tarefas** ou **Problemas**.

1. Clique em **Definir condições padrão**.
1. No menu suspenso, clique na condição personalizada desejada como condição padrão para tarefas (ou problemas).
1. Clique em **Salvar**.

>[!NOTE]
>
>* Um usuário atribuído a uma tarefa ou problema, ou que tenha permissões de Gerenciamento, pode alterar sua condição manualmente. Para obter mais informações, consulte [Atualizar condição para tarefas e problemas](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* As três condições padrão para tarefas e problemas que acompanham o Workfront são Indo bem, Algumas preocupações e Principais bloqueios. Não é possível ocultar ou excluir essas condições, mas você pode alterar seus nomes e cores. Ou você pode criar novos itens para usar, conforme descrito em [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

Para obter informações sobre como configurar uma condição personalizada como uma condição padrão para projetos, consulte [Definir uma condição personalizada como padrão para projetos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).
