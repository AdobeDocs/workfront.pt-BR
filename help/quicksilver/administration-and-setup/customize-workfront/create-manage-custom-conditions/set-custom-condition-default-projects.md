---
title: Definir uma condição personalizada como padrão para projetos
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Se o Tipo de condição de um projeto estiver definido como Status de progresso em vez de Manual, o Adobe Workfront exibirá automaticamente uma das três condições padrão incorporadas no projeto (No destino, Em risco ou Em problemas) conforme ele progride, conforme explicado em Visão geral da condição do projeto e do Tipo de condição.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 1%

---

# Definir uma condição personalizada como padrão para projetos

Se o Tipo de condição de um projeto estiver definido como Status de progresso em vez de Manual, o Adobe Workfront exibirá automaticamente uma das três condições padrão incorporadas no projeto (No Target, Em risco ou Em problemas) à medida que progride, conforme explicado em [Visão geral da condição do projeto e do tipo de condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![](assets/condition-in-project-header-nwe.png)

Você pode definir suas condições personalizadas como condições padrão em vez de usar essas três condições padrão incorporadas. Por exemplo, você pode alterar a condição padrão No Target para exibir como Tracking well em todos os projetos.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Defina uma condição personalizada como condição padrão para todos os projetos:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Preferências do projeto** > **Condições**.

1. Clique no botão **Projeto** guia .
1. Clique em **Definir condições padrão**.
1. No menu suspenso próximo à condição padrão que você deseja alterar, clique na condição personalizada que deseja usar.
1. Repita a etapa anterior para qualquer outra condição padrão que desejar alterar.
1. Clique em **Salvar**.

Para obter informações sobre como definir uma condição personalizada como condição padrão para tarefas e problemas, consulte [Definir uma condição personalizada como padrão para tarefas e problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Para obter informações sobre como configurar um projeto para que os usuários possam atualizar sua condição manualmente, consulte [Atualizar condição para tarefas e problemas](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

Para obter informações sobre condições personalizadas, consulte [Condições personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
