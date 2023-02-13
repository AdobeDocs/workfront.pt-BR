---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Usar um status personalizado como status padrão para um grupo
description: Como administrador de grupo, você pode configurar um status personalizado como status padrão para um grupo ou subgrupo que você gerencia. Isso é útil quando o sistema precisa atribuir automaticamente um status Workfront a um projeto, tarefa ou problema. Um projeto, tarefa ou problema sempre exibe o status personalizado que você definiu como status padrão em vez de exibir o status do Workfront ao qual ele equivale.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Usar um status personalizado como status padrão para um grupo

Como administrador de grupo, você pode configurar um status personalizado como status padrão para um grupo ou subgrupo que você gerencia. Isso é útil quando o sistema precisa atribuir automaticamente um status Workfront a um projeto, tarefa ou problema. Um projeto, tarefa ou problema sempre exibe o status personalizado que você definiu como status padrão em vez de exibir o status do Workfront ao qual ele equivale.

O status que você configurar pode ser qualquer status personalizado criado para o grupo, herdado de um grupo acima do grupo ou herdado do nível do sistema.

Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!INFO]
>
>**Exemplo:** Você poderia criar um status personalizado chamado Finished e defini-lo como um status padrão equacionado com o status Workfront Complete.
>
>Em seguida, para tarefas definidas para serem alteradas para o status Concluído quando atingirem 100%, o status será exibido como Concluído em vez de Concluído.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Status da emissão

Se o status personalizado for um Status de ocorrência, todos os quatro tipos de problema deverão estar ativados para ele (Relatório de erros, Pedido de alteração, Ocorrência e Solicitação). Por exemplo, no status de emissão mostrado abaixo, o status Reaberto não pode ser usado como um status padrão porque o tipo de problema da Ordem de Alteração não está selecionado:

![](assets/all-4-issue-types-enabled.png)

## Definir um status personalizado como status padrão para um grupo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png), em seguida, clique no nome do grupo em que deseja criar ou personalizar os status.
1. No painel esquerdo, clique em **Status** ![](assets/gear-icon-settings.png).
1. Abra o **Projeto**, **Tarefas** ou **Problemas** , dependendo do tipo de status que deseja definir como status padrão.
1. Clique em **Definir status padrão** próximo ao canto superior direito.
1. Na área suspensa que é exibida, ao lado do status em que você deseja definir o status padrão, selecione o status padrão que deseja definir.
1. Clique em **Salvar**.

   O status agora está disponível como um status padrão para uso com projetos associados ao grupo.

1. Associe o status personalizado ao projeto onde deseja usá-lo.

   Você associa o status ao projeto associando o grupo em que o status reside no projeto. Os usuários podem usar o status personalizado somente se o grupo no qual o status reside estiver associado ao projeto.

   >[!NOTE]
   >
   >Se você atribuir o projeto a um grupo diferente, o status do projeto será recarregado e poderá ser alterado.

   1. Vá para o projeto onde deseja usar o status personalizado.
   1. Clique no menu Mais ![](assets/more-icon.png), depois clique em **Editar**.
   1. No **Editar projeto** que é exibida na caixa **Grupo** campo sob **Associação de projeto**, selecione o grupo ao qual o status personalizado está associado.

   1. Clique em **Salvar alterações**.

## Os grupos herdam as configurações de status padrão

Depois que um administrador do Workfront configura um status personalizado como padrão, os novos grupos criados herdam essa configuração.

Da mesma forma, depois que um administrador de grupo define um status personalizado como padrão, novos subgrupos criados diretamente abaixo do grupo herdam essa configuração.

Para obter mais informações, consulte [Como os grupos herdam os status](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Quando um status padrão está oculto

Se você ocultar um status padrão (ativando a opção Ocultar status para ele), o sistema tentará definir outro status do tipo equivalente como padrão.

Se não houver status disponível do tipo equivalente, o tipo de status será exibido como **Oculto** e não está disponível para itens de trabalho.

![](assets/when-hide-default-status-no-equivalent.png)
