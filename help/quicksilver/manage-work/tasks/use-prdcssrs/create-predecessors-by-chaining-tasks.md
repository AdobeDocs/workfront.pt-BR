---
product-area: projects
navigation-topic: use-predecessors
title: Criar relações de antecessor por tarefas encadeadas
description: Você pode criar relacionamentos predecessores de várias maneiras no Adobe Workfront. Um método é encadeando tarefas.
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 1%

---

# Criar relações de antecessor por tarefas encadeadas

Você pode criar relacionamentos predecessores de várias maneiras no Adobe Workfront. Um método é encadeando tarefas.

Para obter informações sobre tarefas anteriores, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Ao encadear tarefas, você pode permitir que o sistema crie os relacionamentos do antecessor automaticamente em tarefas selecionadas, em vez de criar manualmente um relacionamento em cada tarefa. Tipos de relacionamento entre antecessores diferentes ainda podem ser usados entre tarefas.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Tarefas em cadeia para criar relacionamentos predecessores

1. Vá para o projeto que contém as tarefas que você deseja encadear.
1. Clique em **Tarefas** no painel esquerdo.
1. (Condicional) Selecionar **Salvar automaticamente** no canto superior direito da lista de tarefas, selecione as tarefas que deseja encadear.

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >A vinculação de tarefas em uma lista de tarefas não é possível quando você salva manualmente as alterações nas tarefas ou usa o modo Planejamento de Linha do Tempo para salvar tarefas.

1. Clique com o botão direito do mouse nas tarefas selecionadas e depois clique em **Corrente**.
1. Selecione entre os seguintes tipos de dependência:

   * **Término-Inicio**
   * **Término-Término**
   * **Início-Início**
   * **Início-Término**

   Para obter mais informações sobre tipos de dependência de antecessor, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

1. (Opcional) Clique em **Desencadeamento** se algumas das tarefas foram encadeadas anteriormente.

   >[!CAUTION]
   >
   >Somente os predecessores sequenciais são removidos usando a opção de descorrente ao editar tarefas em massa.

   Suas tarefas selecionadas agora são vinculadas por relações do antecessor.
