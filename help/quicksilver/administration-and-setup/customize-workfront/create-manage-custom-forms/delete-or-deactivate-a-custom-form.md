---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Excluir ou desativar um formulário personalizado
description: É possível excluir ou desativar um formulário personalizado do sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d97badf-b6d0-4e7c-bff8-9ff63e83586b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Excluir ou desativar um formulário personalizado

É possível excluir ou desativar um formulário personalizado do sistema.

>[!CAUTION]
>
>A exclusão de um formulário personalizado também exclui todos os dados personalizados dos objetos associados ao formulário. Os dados excluídos não podem ser recuperados. Considere desativar um formulário personalizado em vez disso — ao desativar um formulário personalizado que não é mais usado, você mantém todos os dados históricos associados.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plano Adobe Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com o administrador da Workfront.

## Excluir um formulário personalizado

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizada.**
1. Selecione o formulário personalizado e clique em **Excluir**.
1. Se tiver certeza de que deseja excluir permanentemente o formulário personalizado e todos os dados associados nos objetos aos quais ele foi anexado, clique em **Sim, Excluir**.

## Desativar um formulário personalizado

É possível desativar formulários personalizados que não são mais usados sem perder os dados históricos associados. Os usuários não podem adicionar um formulário personalizado inativo a objetos, mas ainda podem exibir e adicionar dados aos seus campos em objetos onde ele já estava anexado.

Os campos em um formulário personalizado inativo também ainda estão disponíveis para edição em linha em uma Exibição. Se um usuário adicionar um campo de um formulário personalizado inativo durante uma edição em linha, o formulário será anexado automaticamente ao objeto, mesmo que o formulário personalizado esteja desativado.

Se você reativar um formulário personalizado, ele manterá as configurações anteriores e os usuários poderão interagir com ele como se ele nunca tivesse sido desativado.

Para desativar um formulário personalizado:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique no nome do formulário personalizado que deseja desativar.
1. Clique no botão **Configurações do formulário** guia .
1. Desative o **Está ativo** opção.
1. Clique em **Salvar + Fechar**.
