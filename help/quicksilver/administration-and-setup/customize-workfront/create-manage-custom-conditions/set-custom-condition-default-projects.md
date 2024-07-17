---
title: Definir uma condição personalizada como padrão para projetos
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Se o Tipo de condição de um projeto for definido como Status de progresso em vez de Manual, o Adobe Workfront exibirá automaticamente uma das três condições padrão incorporadas no projeto (No destino, Em risco ou Com problema) à medida que ele avança, conforme explicado em Visão geral da condição do projeto e do tipo de condição.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Definir uma condição personalizada como padrão para projetos

Se o Tipo de Condição de um projeto for definido como Status de Progresso em vez de Manual, o Adobe Workfront exibirá automaticamente uma das três condições padrão internas no projeto (No Destino, Em Risco ou Com Problemas) conforme avança, conforme explicado em [Visão Geral da Condição do Projeto e do Tipo de Condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![](assets/condition-in-project-header-nwe.png)

Você pode definir suas condições personalizadas como condições padrão em vez de usar essas três condições padrão incorporadas. Por exemplo, você pode alterar a condição padrão No destino para exibir Como rastreamento em todos os projetos.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Definir uma condição personalizada como condição padrão para todos os projetos:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Preferências do projeto** > **Condições**.

1. Clique na guia **Projeto**.
1. Clique em **Definir Condições Padrão**.
1. No menu suspenso ao lado da condição padrão que deseja alterar, clique na condição personalizada que deseja usar.
1. Repita a etapa anterior para qualquer outra condição padrão que desejar alterar.
1. Clique em **Salvar**.

Para obter informações sobre como definir uma condição personalizada como uma condição padrão para tarefas e problemas, consulte [Definir uma condição personalizada como padrão para tarefas e problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Para obter informações sobre como configurar um projeto para que os usuários possam atualizar sua condição manualmente, consulte [Atualizar Condição para tarefas e problemas](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).

Para obter informações sobre condições personalizadas, consulte [Condições personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
