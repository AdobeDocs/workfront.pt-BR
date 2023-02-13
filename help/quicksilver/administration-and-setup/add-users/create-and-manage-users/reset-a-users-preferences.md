---
title: Redefinir as preferências de um usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, você pode redefinir ou remover as configurações de preferência do usuário para qualquer usuário no sistema Workfront. Usuários individuais também podem redefinir suas próprias configurações de preferência de usuário.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# Redefinir as preferências de um usuário

Como administrador do Adobe Workfront, você pode redefinir ou remover as configurações de preferência do usuário para qualquer usuário no sistema Workfront.

Usuários individuais também podem redefinir suas próprias configurações de preferência de usuário.

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

## Sobre as configurações afetadas

Quando você redefine as preferências do usuário, algumas preferências são revertidas para o padrão do sistema e outras são apagadas ou removidas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Preferência</strong> </th> 
   <th><strong>Status após a redefinição</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Visualizações</td> 
   <td> <p> Revertido para o padrão do sistema</p> <p>As Exibições existentes não são excluídas. Você pode selecioná-los novamente.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtros</td> 
   <td> <p>Revertido para o padrão do sistema</p> <p>Os Filtros existentes não são excluídos. Você pode selecioná-los novamente.</p> </td> 
  </tr> 
  <tr> 
   <td>Agrupamento</td> 
   <td> <p>Revertido para o padrão do sistema</p> <p>Os agrupamentos existentes não são excluídos. Você pode selecioná-los novamente.</p> </td> 
  </tr> 
  <tr> 
   <td>Lista de itens recentes</td> 
   <td>Limpo</td> 
  </tr> 
  <tr> 
   <td>Lista de favoritos</td> 
   <td>Não afetado</td> 
  </tr> 
  <tr> 
   <td>Preferências do usuário</td> 
   <td> <p>Revertido para o padrão do sistema</p> <p>As notificações por email revertem para os padrões do sistema</p> </td> 
  </tr> 
  <tr> 
   <td>Guias personalizadas definidas pelo usuário</td> 
   <td>Removido</td> 
  </tr> 
  <tr> 
   <td>Opções de navegação global definidas pelo usuário</td> 
   <td>Defina novamente para a definição do modelo de layout ou o padrão do sistema se nenhum modelo de layout for atribuído.</td> 
  </tr> 
 </tbody> 
</table>

## Redefinir preferências do usuário

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Selecionar **Fazer logon como**.
1. Comece digitando o nome do usuário cujas preferências você deseja redefinir e clique no nome quando ele for exibido na lista suspensa.
1. Selecionar  **Fazer logon**.
1. No campo URL na parte superior do navegador da Web, adicione `/resetUser` after `workfront.com`.

   >[!NOTE]
   >
   >Isso diferencia maiúsculas de minúsculas. O U deve estar em maiúsculas e os caracteres restantes devem estar em minúsculas. Por exemplo:
   >
   >
   ```
   >https://company_domain.my.workfront.com/resetUser
   >```

1. Press **Enter**.
1. Para redefinir todas as preferências do usuário, selecione **Redefinir**.

   Ou

   Para redefinir somente guias personalizadas, selecione **Redefinir guias**.
