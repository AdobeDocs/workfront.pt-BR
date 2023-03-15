---
title: Desativar ou reativar um formulário personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: É possível reativar ou desativar um formulário personalizado. Recomendamos desativar formulários personalizados em vez de excluir formulários que não são mais usados para manter os dados históricos.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: c0082dd73e3db8123f9cc08f1798ef8e70730625
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Desativar ou reativar um formulário personalizado

É possível reativar ou desativar um formulário personalizado. Recomendamos desativar formulários personalizados em vez de excluir formulários que não são mais usados para manter os dados históricos.

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
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com o administrador da Workfront.

## Desativar um formulário personalizado

É possível desativar formulários personalizados que não são mais usados sem perder os dados históricos associados. Os usuários não podem adicionar um formulário personalizado inativo a objetos, mas ainda podem exibir e adicionar dados aos seus campos em objetos onde ele já estava anexado.

Os campos em um formulário personalizado inativo também ainda estão disponíveis para edição em linha em uma Exibição. Se um usuário adicionar um campo de um formulário personalizado inativo durante uma edição em linha, o formulário será anexado automaticamente ao objeto, mesmo que o formulário personalizado esteja desativado.

Para desativar um formulário personalizado:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, escolha **Forms personalizada**.
1. No **Forms** selecione o formulário personalizado que deseja desativar.
1. Na coluna Is Ative , escolha **Falso** e clique para fora da coluna . O formulário não está mais ativo.

## Reativar um formulário personalizado

Se você reativar um formulário personalizado, ele manterá as configurações anteriores e os usuários poderão interagir com ele como se ele nunca tivesse sido desativado.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).
1. No painel esquerdo, escolha **Forms personalizada**.
1. No **Forms** selecione o formulário personalizado que deseja reativar.
1. Na coluna Is Ative , escolha **Verdadeiro** e clique para fora da coluna . O formulário agora está ativo.