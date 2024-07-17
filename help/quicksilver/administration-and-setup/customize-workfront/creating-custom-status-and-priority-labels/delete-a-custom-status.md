---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Excluir um status personalizado
description: Você pode excluir um status de sistema personalizado se ele não for mais útil para sua organização.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Excluir um status personalizado

Você pode excluir um status de sistema personalizado se ele não for mais útil para sua organização.

Se o status é bloqueado ou desbloqueado determina se o status é excluído para todos os grupos no sistema:

* Quando você exclui um status do sistema que está bloqueado no momento, o status é removido para todos os grupos no sistema, independentemente do grupo o ter renomeado.
* Por outro lado, ao excluir um status do sistema que está desbloqueado no momento, o status permanece para todos os grupos no sistema.


>[!NOTE]
>
>Não é possível excluir o seguinte:
>
>* Um status de sistema bloqueado ou desbloqueado usado em um processo de aprovação do sistema que está atualmente pendente de aprovação para, pelo menos, um objeto no sistema.
>
>  No entanto, é possível excluir um status de sistema desbloqueado usado em um processo de aprovação de uso único ou de nível de grupo que esteja atualmente pendente de aprovação.
>
>  Você pode executar um relatório para encontrar os objetos e resolver as aprovações pendentes e, em seguida, tentar novamente excluir o status. Para obter instruções, consulte [Listar objetos com processos de aprovação pendentes usando um determinado status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Status usados em processos de aprovação que atualmente estão pendentes de aprovação para pelo menos um objeto no sistema.

Para obter instruções sobre como excluir um status de grupo, consulte [Excluir um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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

## Excluir um status de sistema personalizado

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Preferências do projeto** > **Status**.

1. Para excluir o status em todo o sistema (incluindo grupos individuais), passe o mouse sobre o status, clique em **Editar** e verifique se **Bloquear para todos os grupos** está selecionado. Clique em **Salvar**.

   Ou

   Para excluir o status do sistema, mas mantê-lo para grupos individuais, passe o mouse sobre o status, clique em **Editar** e certifique-se de que **Bloquear para todos os grupos** não esteja selecionado. Clique em **Salvar**.

1. Passe o cursor do mouse sobre o status que deseja excluir e clique em **Excluir**.
1. Na mensagem exibida, clique em **Excluir Status**.
1. Na caixa **Excluir Status** que é exibida, selecione um status no campo rotulado **Definir todos os projetos com este status no momento como**.

   Os projetos que estavam usando o status que você está excluindo são definidos com o status selecionado.

   Os status estão disponíveis na lista suspensa somente se forem iguais ao status que você está excluindo.

   Por exemplo, se você estiver excluindo um status que equivale a Atual, apenas os status que também equivalem a Atual estarão disponíveis para seleção.

1. Clique em **Excluir status**.
