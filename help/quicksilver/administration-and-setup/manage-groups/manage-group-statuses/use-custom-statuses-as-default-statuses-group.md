---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Usar um status personalizado como status padrão para um grupo
description: Como administrador de grupo, você pode configurar um status personalizado como status padrão para um grupo ou subgrupo gerenciado.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 1%

---

# Usar um status personalizado como status padrão para um grupo

Como administrador de grupo, você pode configurar um status personalizado como status padrão para um grupo ou subgrupo gerenciado. Isso é útil quando o sistema precisa atribuir automaticamente um status do Workfront a um projeto, tarefa ou problema. Um projeto, tarefa ou problema sempre exibe o status personalizado definido como status padrão, em vez de exibir o status do Workfront igual a.

O status configurado pode ser qualquer status personalizado criado para o grupo, herdado de um grupo acima do grupo ou herdado do nível do sistema.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!INFO]
>
>**Exemplo:** você poderia criar um status personalizado chamado Concluído e defini-lo como um status padrão equivalente ao status Concluído do Workfront.
>
>Em seguida, para tarefas definidas para alteração para o status Concluído quando atingirem 100%, o status é exibido como Concluído em vez de Concluído.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Status de problemas

Se o status personalizado for um status de Problema, todos os quatro tipos de problemas deverão ser habilitados para ele (Relatório de erros, Pedido de alteração, Problema e Solicitação). Por exemplo, no status de ocorrência mostrado abaixo, o status Reaberto não pode ser usado como um status padrão porque o tipo de ocorrência de Pedido de alteração não está selecionado:

![Todos os tipos de problemas habilitados](assets/all-4-issue-types-enabled.png)

## Definir um status personalizado como status padrão para um grupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png) e depois clique no nome do grupo no qual deseja criar ou personalizar os status.
1. No painel esquerdo, clique em **Status** ![Ícone de configurações de engrenagem](assets/gear-icon-settings.png).
1. Abra a guia **Projeto**, **Tarefas** ou **Problemas**, dependendo do tipo de status que você deseja definir como um status padrão.
1. Clique em **Definir status padrão** próximo ao canto superior direito.
1. Na área suspensa que é exibida, ao lado do status em que você deseja definir o status padrão, selecione o status padrão que deseja definir.
1. Clique em **Salvar**.

   O status agora está disponível como um status padrão para uso com projetos associados ao grupo.

1. Associe o status personalizado ao projeto em que deseja usá-lo.

   Associe o status ao projeto associando o grupo em que o status reside ao projeto. Os usuários podem usar o status personalizado somente se o grupo onde o status reside estiver associado ao projeto.

   >[!NOTE]
   >
   >Se você atribuir o projeto a um grupo diferente, o status do projeto será recarregado e poderá ser alterado.

   1. Vá para o projeto em que deseja usar o status personalizado.
   1. Clique no ícone Mais ![Mais](assets/more-icon.png) do menu e em **Editar**.
   1. Na caixa **Editar Projeto** que é exibida, no campo **Grupo** em **Associação de projeto**, selecione o grupo ao qual o status personalizado está associado.

   1. Clique em **Salvar alterações**.

## Os grupos herdam as configurações de status padrão

Depois que um administrador do Workfront configura um status personalizado como status padrão, novos grupos criados herdam essa configuração.

Da mesma forma, depois que um administrador de grupo define um status personalizado como um status padrão, novos subgrupos criados diretamente abaixo do grupo herdam essa configuração.

Para obter mais informações, consulte [Como os grupos herdam os status](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Quando um status padrão está oculto

Se você ocultar um status padrão (ativando a opção Ocultar status para ele), o sistema tentará definir outro status do tipo equivalente como padrão.

Se não houver status disponível do tipo equivalente, o tipo de status será exibido como **Oculto** e não estará disponível para itens de trabalho.

![Nenhum status disponível](assets/when-hide-default-status-no-equivalent.png)
