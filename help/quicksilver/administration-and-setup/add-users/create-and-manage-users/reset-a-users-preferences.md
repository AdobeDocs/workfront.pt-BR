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
source-git-commit: a9d507bfcc0a602e71bcdd3142d63cc40175ebf4
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 2%

---

# Redefinir preferências de um usuário

<!-- Audited: 12/2023 -->

Como administrador do Adobe Workfront, você pode redefinir ou remover as configurações de preferência do usuário para qualquer usuário no sistema do Workfront.

Usuários individuais também podem redefinir suas próprias configurações de preferência do usuário.

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
   <td> <p>Revertido para o padrão do sistema</p> <p>As notificações por email são revertidas para os padrões do sistema. As notificações padrão estão listadas em <a href="/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md">Notificações de eventos disponíveis no Adobe Workfront</a>.</p> </td> 
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

1. Selecione **Fazer Logon Como**.
1. Comece digitando o nome do usuário cujas preferências você deseja redefinir, em seguida, clique no nome quando ele aparecer na lista suspensa.
1. Selecione **Fazer Logon**.
1. Se sua organização não tiver sido integrada à Experiência unificada do Adobe, siga esta etapa:

   * No campo URL na parte superior do navegador da Web, adicione `/resetUser` depois de `workfront.com`.

     >[!NOTE]
     >
     >Isso diferencia maiúsculas e minúsculas. O U deve estar em maiúsculas e os caracteres restantes devem estar em minúsculas. Por exemplo:
     >
     >`https://company_domain.my.workfront.com/resetUser`

1. Se sua organização tiver sido integrada à Experiência unificada do Adobe, siga esta etapa:

   * No campo URL na parte superior do navegador da Web, adicione `/resetUser` depois de `workfront`.

     >[!NOTE]
     >
     >Isso diferencia maiúsculas e minúsculas. O U deve estar em maiúsculas e os caracteres restantes devem estar em minúsculas. Por exemplo:
     >
     >`https://experience.adobe.com/#/@company/so:(domain)-(environment)/workfront/resetUser`

1. Pressione **Enter**.
1. Para redefinir todas as preferências de usuário, selecione **Redefinir**.

   Ou

   Para redefinir apenas guias personalizadas, selecione **Redefinir Guias**.
