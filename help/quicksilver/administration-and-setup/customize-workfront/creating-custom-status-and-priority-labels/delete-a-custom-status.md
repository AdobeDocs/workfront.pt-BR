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

Se o status está bloqueado ou desbloqueado determina se o status é excluído para todos os grupos no sistema:

* Ao excluir um status de sistema que está bloqueado no momento, o status é removido para todos os grupos no sistema, independentemente de o grupo ter renomeado.
* Por outro lado, ao excluir um status do sistema que está atualmente desbloqueado, o status permanece para todos os grupos no sistema.


>[!NOTE]
>
>Não é possível excluir o seguinte:
>
>* Um status de sistema bloqueado ou desbloqueado usado em um processo de aprovação de sistema que está pendente de aprovação para pelo menos um objeto em seu sistema.
>
>  No entanto, é possível excluir um status de sistema desbloqueado usado em um processo de aprovação de uso único ou de nível de grupo que está pendente de aprovação no momento.
>
>  Você pode executar um relatório para localizar os objetos e resolver as aprovações pendentes e tentar novamente excluir o status. Para obter instruções, consulte [Listar objetos com processos de aprovação pendentes usando um determinado status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Status usados em processos de aprovação que estão pendentes de aprovação para pelo menos um objeto em seu sistema.


Para obter instruções sobre como excluir um status de grupo, consulte [Excluir um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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

## Excluir um status de sistema personalizado

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Preferências do projeto** > **Status**.

1. Para excluir o status em todo o sistema (incluindo para grupos individuais), passe o mouse sobre o status e clique em **Editar**, e **Bloquear para todos os grupos** está selecionada. Clique em **Salvar**.

   Ou

   Para excluir o status do sistema, mas mantê-lo para grupos individuais, passe o mouse sobre o status e clique em **Editar**, e **Bloquear para todos os grupos** está desmarcada. Clique em **Salvar**.

1. Passe o mouse sobre o status que deseja excluir, em seguida, clique em **Excluir**.
1. Na mensagem que aparece, clique em **Excluir status**.
1. No **Excluir status** for exibida, selecione um status no campo rotulado **Definir todos os projetos com este status no momento como**.

   Os projetos que estavam usando o status que você está excluindo são definidos com o status selecionado.

   Os status estão disponíveis na lista suspensa somente se corresponderem ao mesmo status que o status que você está excluindo.

   Por exemplo, se você estiver excluindo um status que é igual a Atual, somente os status que também são iguais a Atual estarão disponíveis para seleção.

1. Clique em **Excluir status**.
