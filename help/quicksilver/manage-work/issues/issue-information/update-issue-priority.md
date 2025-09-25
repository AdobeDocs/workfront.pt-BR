---
product-area: projects
navigation-topic: issue-information
title: Atualizar prioridade do problema
description: Você pode definir uma prioridade para uma ocorrência para indicar a importância da ocorrência.
author: Alina
feature: Work Management
exl-id: eff5c9e8-1908-4654-9629-e20c0ce2a225
source-git-commit: 7db80f5bacf52b7bbe540f4e38e88853af86a5e2
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 3%

---

# Atualizar prioridade do problema

Você pode definir uma prioridade para uma ocorrência para indicar a importância da ocorrência.

Você deve ter permissões de gerenciamento para o problema para modificar a Prioridade do problema. [Atualize a Prioridade de um problema](#update-the-priority-of-an-issue).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

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
   <td> <p>Editar acesso a ocorrências</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Visão geral das prioridades do problema

Cada rótulo de prioridade tem um número associado que não pode ser modificado.

Os administradores do Adobe Workfront podem modificar os rótulos de prioridade no Workfront ou criar novas prioridades. Como resultado, as opções que você pode ter para o campo Prioridade na instância do Workfront podem ser diferentes das listadas abaixo.

Você deve se familiarizar com a sequência de numeração das prioridades usadas em sua organização.\
Por exemplo, sua organização pode usar o número 1 para se referir a tarefas urgentes, se o rótulo da prioridade tiver sido modificado.

Para obter mais informações sobre como personalizar os nomes das prioridades na sua instância, consulte [Criar e personalizar prioridades](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

Consulte a tabela a seguir para entender cada rótulo de prioridade padrão e seu número correspondente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Rótulo de Prioridade <br>(Pode ser modificado) </th> 
   <th>Número de Prioridade <br> (Não pode ser modificado) </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> Nenhum(a) </td> 
   <td> 0 </td> 
  </tr> 
  <tr> 
   <td> Baixa </td> 
   <td> 1 </td> 
  </tr> 
  <tr> 
   <td> Normal </td> 
   <td> 2 </td> 
  </tr> 
  <tr> 
   <td> Alta </td> 
   <td> 3 </td> 
  </tr> 
  <tr> 
   <td> Urgente </td> 
   <td> 4 </td> 
  </tr> 
 </tbody> 
</table>

## Atualizar a prioridade de um problema {#update-the-priority-of-an-issue}

1. Vá para o problema cuja prioridade você deseja modificar.
1. Clique em **Detalhes do problema** no painel esquerdo.

   A seção **Visão geral** deve ser exibida por padrão.

1. Clique no campo **Prioridade** na área **Informações básicas**.

   ![Prioridade do problema](assets/issue-priority-field.png)

1. Selecione um valor para o campo **Prioridade**.

   Dependendo de como o administrador do Workfront configurou as Prioridades no sistema, as opções podem variar.

1. Clique em **Salvar alterações**.
