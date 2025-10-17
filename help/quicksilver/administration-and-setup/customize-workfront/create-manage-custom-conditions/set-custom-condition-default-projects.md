---
title: Definir uma condição personalizada como padrão para projetos
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Se o Tipo de condição de um projeto for definido como Status de progresso em vez de Manual, o Adobe Workfront exibirá automaticamente uma das três condições padrão incorporadas no projeto (No destino, Em risco ou Com problema) à medida que ele avança, conforme explicado em Visão geral da condição do projeto e do tipo de condição.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: dba052ed-83a2-44d2-b025-d970783c4151
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 2%

---

# Definir uma condição personalizada como padrão para projetos

Se o Tipo de Condição de um projeto for definido como Status de Progresso em vez de Manual, o Adobe Workfront exibirá automaticamente uma das três condições padrão internas no projeto (No Destino, Em Risco ou Com Problemas) conforme avança, conforme explicado em [Visão Geral da Condição do Projeto e do Tipo de Condição](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

![Condição no cabeçalho e detalhes do projeto](assets/condition-of-project-0825.png)

Você pode definir suas condições personalizadas como condições padrão em vez de usar essas três condições padrão incorporadas. Por exemplo, você pode alterar a condição padrão No destino para exibir Como rastreamento em todos os projetos.

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

## Definir uma condição personalizada como condição padrão para todos os projetos:

{{step-1-to-setup}}

1. Clique em **Preferências do projeto** > **Condições**.

1. Clique na guia **Projetos**.
1. Clique em **Definir condições padrão**.
1. No menu suspenso da condição padrão que deseja alterar, clique na condição personalizada que deseja usar.
1. Repita a etapa anterior para qualquer outra condição padrão que desejar alterar.
1. Clique em **Salvar**.

Para obter informações sobre como definir uma condição personalizada como uma condição padrão para tarefas e problemas, consulte [Definir uma condição personalizada como padrão para tarefas e problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Para obter informações sobre como configurar um projeto para que os usuários possam atualizar sua condição manualmente, consulte [Atualizar Condição para tarefas e problemas](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
