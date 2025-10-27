---
title: Redefinir preferências de um usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, você pode redefinir ou remover as configurações de preferência do usuário para qualquer usuário no sistema do Workfront. Usuários individuais também podem redefinir suas próprias configurações de preferência do usuário.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: 5706ebd11985b9e67c93686918f8f0327adabdf1
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 3%

---

# Redefinir preferências de um usuário

<!-- Audited: 12/2023 -->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox e está sendo lançado em uma implantação em fases para Produção.</span>

Como administrador do Adobe Workfront, você pode redefinir ou remover as configurações de preferência do usuário para qualquer usuário no sistema do Workfront.

Usuários individuais também podem redefinir suas próprias configurações de preferência do usuário.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Administrador de Sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sobre as configurações afetadas

Ao redefinir as preferências do usuário, algumas preferências são revertidas para o padrão do sistema e outras são apagadas ou removidas:

<!--
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preference</strong> </th> 
   <th><strong>Status after the reset</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Views</td> 
   <td> <p> Reverted to the system default</p> <p>Existing views are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Filters</td> 
   <td> <p>Reverted to the system default</p> <p>Existing filters are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Groupings</td> 
   <td> <p>Reverted to the system default</p> <p>Existing groupings are not deleted. You can select them again.</p> </td> 
  </tr> 
  <tr> 
   <td>Recent Items list</td> 
   <td>Cleared</td> 
  </tr> 
  <tr> 
   <td>Favorites list</td> 
   <td>Unaffected</td> 
  </tr> 
  <tr> 
   <td>User Preferences</td> 
   <td> <p>Reverted to the system default</p> <p>Email notifications revert to the system defaults. The default notifications are listed in <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Event notifications available in Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>User-Defined Custom Tabs</td> 
   <td>Removed</td> 
  </tr> 
  <tr> 
   <td>User-Defined Global Navigation Options</td> 
   <td>Set back to layout template definition, or system default if no layout template is assigned.</td> 
  </tr> 
 </tbody> 
</table>
-->

<!--Display this table and hide the HTML table above, when the unshim is released.-->

<div class="preview">

| Preferência | Status após a redefinição |
| --- | --- |
| Exibições | Revertido para o padrão do sistema <p>As exibições existentes não são excluídas. Você pode selecioná-los novamente.</p> |
| Filtros | Revertido para o padrão do sistema <p>Os filtros existentes não são excluídos. Você pode selecioná-los novamente.</p> |
| Agrupamento | Revertido para o padrão do sistema <p>Os agrupamentos existentes não são excluídos. Você pode selecioná-los novamente.</p> |
| Lista de itens recentes | Limpo |
| Lista Favoritos | Não afetado |
| Preferências do usuário | Revertido para o padrão do sistema <p>As notificações por email são revertidas para os padrões do sistema. As notificações padrão estão listadas em [Notificações de eventos disponíveis no Adobe Workfront](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).</p> |

</div>

## Redefinir preferências do usuário

{{step-1-to-setup}}

1. Selecione **Fazer Logon Como**.
1. Comece digitando o nome do usuário cujas preferências você deseja redefinir, em seguida, clique no nome quando ele aparecer na lista suspensa.
1. Selecione **Fazer Logon**.
1. Se sua organização não tiver sido integrada à Experiência unificada da Adobe, siga esta etapa:

   * No campo URL na parte superior do navegador da Web, adicione `/resetUser` depois de `workfront.com`.

     >[!NOTE]
     >
     >Isso diferencia maiúsculas e minúsculas. O U deve estar em maiúsculas e os caracteres restantes devem estar em minúsculas. Por exemplo:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Se sua organização tiver sido integrada à Experiência unificada da Adobe, siga esta etapa:

   * No campo URL na parte superior do navegador da Web, adicione `/resetUser` depois de `workfront`.

     >[!NOTE]
     >
     >Isso diferencia maiúsculas e minúsculas. O U deve estar em maiúsculas e os caracteres restantes devem estar em minúsculas. Por exemplo:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Pressione **Enter**.

1. <span class="preview">Para redefinir todas as preferências de usuário, clique em **Redefinir**.</span>

   <span class="preview">Ou</span>

   <span class="preview">Para redefinir a navegação à esquerda do usuário para a configuração de modelo de layout original, clique em **Redefinir Navegação à Esquerda**.</span>
