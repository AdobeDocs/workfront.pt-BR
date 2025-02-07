---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Exibir e Gerenciar Membros do Subgrupo
description: Ao visualizar um grupo gerenciado por você, é possível visualizar e gerenciar todos os usuários nos subgrupos do grupo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Exibir e gerenciar membros do subgrupo

Ao visualizar um grupo gerenciado por você, é possível visualizar e gerenciar todos os usuários nos subgrupos do grupo.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

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
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. </li> 
     <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-settings.png">. </p> <p>Dessas duas opções, se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir e gerenciar membros dos subgrupos de um grupo

{{step-1-to-setup}}

1. Clique em **Grupos**.

   Na lista exibida, você pode ver os grupos que gerencia, juntamente com quaisquer subgrupos que eles tenham. Os administradores do Adobe Workfront podem visualizar todos os grupos.

1. Clique no nome do grupo para o qual deseja exibir ou gerenciar membros do subgrupo.
1. No painel esquerdo, clique em **Membros do Subgrupo**.

   Este item do painel esquerdo está disponível somente se o grupo tiver subgrupos.

1. Siga um destes procedimentos:

   * Selecione um membro na lista e clique em Editar ![ícone Editar](assets/edit-icon.png) para modificar o perfil de usuário dessa pessoa.

     Para obter mais informações, consulte [Editar perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) ou [Editar perfis de usuário em massa](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * Selecione qualquer número de membros na lista e clique em Atualizar ![Ícone de comentário](assets/comment-icon.png) para adicionar um comentário aos seus perfis de usuário.

     O usuário ou usuários recebem uma notificação no aplicativo, bem como uma notificação por email com seu comentário. O comentário é exibido na área Atualizações no perfil do usuário.

   * Selecione qualquer número de membros na lista e clique em Desativar ![Desativar usuário](assets/deactivate-user.png) ou Ativar ![Ativar usuário](assets/activate-user.png).

     Para obter mais informações, consulte [Desativar ou reativar um usuário](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * Exportar ![Exportar](assets/export.png) a lista de membros.
