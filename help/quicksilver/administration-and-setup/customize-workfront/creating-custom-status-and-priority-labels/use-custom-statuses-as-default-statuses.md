---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Usar status personalizados como status padrão
description: Quando um status personalizado é definido como um status padrão, o novo status padrão é usado em todo o sistema de várias maneiras. As formas como é usado dependem se é definido como um status padrão de nível de sistema ou um status padrão de nível de grupo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Usar status personalizados como status padrão

Quando um status personalizado é definido como um status padrão, o novo status padrão é usado em todo o sistema de várias maneiras. As formas como é usado dependem se é definido como um status padrão de nível de sistema ou um status padrão de nível de grupo.

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

## Status padrão personalizados no nível do sistema

Quando você define um status personalizado como status padrão do sistema, qualquer novo grupo criado no sistema herda esse status.

Os grupos que já existiam quando você definiu o novo status padrão do sistema não herdam automaticamente.

Por exemplo, suponha que já existam dois grupos criados em seu ambiente Adobe Workfront (Marketing e Vendas). Você cria um novo status personalizado que é igual a Atual e chama o status Em andamento. Agora você cria um novo grupo chamado Engenharia. Neste cenário, o grupo Engenharia herda o novo status padrão; os grupos de Marketing e Vendas não.

## Status personalizados de nível de grupo padrão

Um status personalizado definido como status de grupo padrão é usado nas seguintes circunstâncias:

* **Quando o sistema Workfront escolhe um status automaticamente, o status padrão do grupo é usado:** O status personalizado definido como status de grupo padrão é usado quando o sistema Workfront atribui automaticamente um status a um objeto.

   Por exemplo, uma tarefa pode ser configurada para alterar automaticamente para o status Concluído quando a porcentagem concluída atingir 100%. Se você criar um status personalizado que seja igual a Concluído e definir esse status personalizado como um status padrão, o Workfront alterará o status da tarefa para o novo status padrão.

   Os status personalizados são usados dessa maneira somente com status de grupo associados a uma tarefa ou problema. Os status personalizados não podem ser usados dessa forma para status associados a um projeto.

* O **o status de um projeto é determinado pelo grupo associado ao projeto**: Se o grupo associado a um determinado projeto for alterado, o status do projeto será alterado, dependendo dos status padrão definidos para o grupo. (Um grupo pode ser associado a um projeto por meio do campo Grupos ao editar o projeto.)

   Se esse grupo for alterado, o status do projeto será alterado se o novo grupo tiver um status padrão diferente definido, que seja igual ao status atual do projeto.

   Por exemplo, um projeto pode ser associado ao grupo Marketing e o status do projeto é definido como Planejamento. O projeto é editado para que agora esteja associado ao grupo Vendas. O grupo Vendas tem um status de grupo padrão personalizado chamado Pensamento (e esse status é igual ao Planejamento). Como o Grupo no projeto foi alterado, o status do projeto muda agora para Pensando.

Se você for um administrador de grupo, consulte [Definir um status como status padrão para um grupo](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Status da emissão

Se o status personalizado for um Status de ocorrência, todos os quatro tipos de problema deverão estar ativados para ele (Relatório de erros, Pedido de alteração, Ocorrência e Solicitação). Por exemplo, no status de emissão mostrado abaixo, o status Reaberto não pode ser usado como um status padrão porque o tipo de problema da Ordem de Alteração não está selecionado:

![](assets/all-4-issue-types-enabled.png)

## Definir um status personalizado como status padrão

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, clique em **Preferências do projeto** > **Status**.
1. (Condicional) Se você estiver definindo um status padrão para um grupo, comece a digitar o nome do grupo no menu no canto superior direito e selecione-o quando ele for exibido.
1. Abra o **Projeto**, **Tarefas** ou **Problemas** , dependendo do tipo de status que deseja definir como status padrão.
1. Clique no botão **Definir status padrão** menu suspenso.
1. Na área suspensa que é exibida, ao lado do status em que você deseja definir o status padrão, selecione o status padrão desejado.
1. Clique em **Salvar**.
1. Associe o projeto ao grupo onde está o status.

   >[!NOTE]
   >
   >Se você estiver definindo o status personalizado de um grupo e posteriormente atribuir o projeto a um grupo diferente, o status do projeto será recarregado e poderá ser alterado.

   1. Vá para o projeto onde deseja usar o status personalizado.
   1. Clique no menu Mais ![](assets/more-icon.png), depois clique em **Editar**.
   1. No **Editar projeto** que é exibida na caixa **Grupo** campo sob **Associação de projeto**, selecione o grupo em que o status reside.
   1. Clique em **Salvar alterações**.
