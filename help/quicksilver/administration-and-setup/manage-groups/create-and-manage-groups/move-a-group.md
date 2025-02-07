---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Mover um grupo
description: Você pode mover um grupo para outro grupo gerenciado.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Mover um grupo

Você pode mover um grupo para outro grupo gerenciado.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Mover um grupo para outro grupo

>[!NOTE]
>
>Se os status do grupo movido estiverem bloqueados, ele herdará os status do novo grupo pai.
>
>Se os status do grupo movido forem desbloqueados, ele não herdará os status de seu novo grupo pai, nem o novo grupo pai assumirá seus status.
>
>Para obter mais informações sobre status de grupo, consulte [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) e [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

1. Selecione o grupo de destino para o qual deseja mover o grupo e clique no ícone Editar ![ícone Editar](assets/edit-icon.png).
1. Na caixa **Editar Grupo** que aparece, em **Membros do Grupo e Administradores do Grupo**, comece digitando o nome do grupo que deseja mover e, em seguida, clique nele quando ele aparecer.
1. Clique em **Salvar**.

>[!TIP]
>
>Você também pode tornar um subgrupo um grupo de nível superior. Para obter instruções, consulte a seção [Remover um subgrupo de seu grupo pai e torná-lo um grupo de nível superior](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) no artigo [Gerenciar um subgrupo](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
