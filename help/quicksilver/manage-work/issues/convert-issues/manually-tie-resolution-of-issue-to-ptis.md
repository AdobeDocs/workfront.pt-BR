---
product-area: projects
navigation-topic: convert-issues
title: Vincular manualmente a resolução de um problema a outros problemas, tarefas ou projetos
description: Você pode vincular manualmente a resolução de um problema à resolução de um projeto, tarefa ou problema sem converter o problema. O problema se torna um dos Objetos Resolvíveis do projeto, tarefa ou problema selecionado. Quando você faz isso, uma alteração no status do projeto, tarefa ou problema aciona uma alteração no status do problema original.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Vincular manualmente a resolução de um problema a outros problemas, tarefas ou projetos

Você pode vincular manualmente a resolução de um problema à resolução de um projeto, tarefa ou problema sem converter o problema. O problema se torna um dos Objetos Resolvíveis do projeto, tarefa ou problema selecionado. Quando você faz isso, uma alteração no status do projeto, tarefa ou problema aciona uma alteração no status do problema original.

>[!TIP]
>
>Ao vincular a resolução de uma ocorrência à resolução de outro objeto, não é mais possível editar manualmente o status da ocorrência original.

Para obter mais informações sobre resolução e objetos resolvíveis, consulte [Visão Geral de Objetos Resolventes e Resolvíveis](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a problemas, tarefas e projetos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões para o problema que você vincula a outro problema, tarefa ou projeto</p> <p>Visualize ou aumente as permissões para o problema, tarefa ou projeto que você adiciona ao problema existente</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisitos

Antes de começar, você deve:

* Ter um problema cuja resolução você deseja vincular à resolução de outro problema, tarefa ou projeto

* Ter um problema, tarefa ou projeto adicional

## Vincular a resolução de um problema à resolução de outro problema, tarefa ou projeto

1. Navegue até uma ocorrência cuja resolução você deseja vincular à resolução de outra ocorrência ou à resolução de uma tarefa ou projeto.
1. Clique em **Detalhes do problema** no painel esquerdo, expanda a variável **Visão geral** área.

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Clique em **Resolvido por** e selecione entre os seguintes tipos de objetos de resolução:

   * **Projeto**
   * **Tarefa**
   * **Problema**

   Dependendo do objeto selecionado, os seguintes campos serão exibidos:

   * **Resolvendo projeto**
   * **Resolvendo tarefa**
   * **Resolvendo problema**

1. Comece digitando o nome de um projeto, tarefa ou problema específico na **Resolvendo projeto**, **Tarefa** ou **Problema** e, em seguida, clique nele quando ele aparecer na lista.

   >[!NOTE]
   >
   >Não é possível vincular a resolução de um problema à tarefa ou ao projeto em que o problema está localizado. A tarefa ou o projeto do problema não são exibidos nos campos Resolving Task (Tarefa de resolução) ou Resolving Task (Tarefa de resolução).


1. Clique em **Salvar alterações**.

   O problema original torna-se o Objeto resolvível do projeto, tarefa ou problema selecionado nas etapas 4 e 5. Isso significa que o problema original é concluído quando o objeto de resolução (o projeto, a tarefa ou o problema ao qual você o vinculou) é concluído.

   >[!NOTE]
   >
   >Um projeto, tarefa ou problema pode ter vários problemas como Objetos resolvíveis.
