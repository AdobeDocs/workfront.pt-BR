---
title: Redefinir preferências de um usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, você pode redefinir ou remover as configurações de preferência do usuário para qualquer usuário no sistema do Workfront. Usuários individuais também podem redefinir suas próprias configurações de preferência do usuário.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: abe026d0-3584-49f3-a6db-ef88b3aab186
source-git-commit: ae063189eebb17a3341aabb978ee0f0e03d1e299
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# Redefinir preferências de um usuário

<!-- Audited: 12/2023 -->

Como administrador do Adobe Workfront, você pode redefinir ou remover as configurações de preferência do usuário para qualquer usuário no sistema do Workfront.

Usuários individuais também podem redefinir suas próprias configurações de preferência do usuário.

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
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sobre as configurações afetadas

Ao redefinir as preferências do usuário, algumas preferências são revertidas para o padrão do sistema e outras são apagadas ou removidas:

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
   <td> <p> Revertido para o padrão do sistema</p> <p>As exibições existentes não são excluídas. Você pode selecioná-los novamente.</p> </td> 
  </tr> 
  <tr> 
   <td>Filtros</td> 
   <td> <p>Revertido para o padrão do sistema</p> <p>Os filtros existentes não são excluídos. Você pode selecioná-los novamente.</p> </td> 
  </tr> 
  <tr> 
   <td>Agrupamento</td> 
   <td> <p>Revertido para o padrão do sistema</p> <p>Os agrupamentos existentes não são excluídos. Você pode selecioná-los novamente.</p> </td> 
  </tr> 
  <tr> 
   <td>Lista de Itens Recentes</td> 
   <td>Limpo</td> 
  </tr> 
  <tr> 
   <td>Lista Favoritos</td> 
   <td>Não afetado</td> 
  </tr> 
  <tr> 
   <td>Preferências do usuário</td> 
   <td> <p>Revertido para o padrão do sistema</p> <p>As notificações por email são revertidas para os padrões do sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Guias Personalizadas Definidas pelo Usuário</td> 
   <td>Removido</td> 
  </tr> 
  <tr> 
   <td>Opções de Navegação Global Definidas pelo Usuário</td> 
   <td>Retorne à definição do modelo de layout ou ao padrão do sistema se nenhum modelo de layout for atribuído.</td> 
  </tr> 
 </tbody> 
</table>

## Redefinir preferências do usuário

{{step-1-to-setup}}

1. Selecionar **Fazer logon como**.
1. Comece digitando o nome do usuário cujas preferências você deseja redefinir, em seguida, clique no nome quando ele aparecer na lista suspensa.
1. Selecionar  **Fazer logon**.
1. No campo URL na parte superior do navegador da Web, adicione `/resetUser` após `workfront.com`.

   >[!NOTE]
   >
   >Isso diferencia maiúsculas e minúsculas. O U deve estar em maiúsculas e os caracteres restantes devem estar em minúsculas. Por exemplo:
   >
   >`https://company_domain.my.workfront.com/resetUser`

1. Pressione **Enter**.
1. Para redefinir todas as preferências do usuário, selecione **Redefinir**.

   Ou

   Para redefinir somente guias personalizadas, selecione **Reinicializa Guias**.
