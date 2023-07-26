---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Excluir tipos de objeto em um formulário personalizado
description: Em um formulário personalizado existente, você pode excluir os tipos de objeto associados ao formulário. Depois disso, os usuários não poderão mais anexar o formulário a objetos desse tipo.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Excluir tipos de objeto em um formulário personalizado

Em um formulário personalizado existente, você pode excluir os tipos de objeto associados ao formulário. Depois disso, os usuários não poderão mais anexar o formulário a objetos desse tipo.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront*</p> </td> 
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

&#42;Para descobrir quais configurações de plano, tipo de licença ou nível de acesso você tem, entre em contato com o administrador do Workfront.

## Excluir tipos de objeto em um formulário personalizado

Você pode excluir tipos de objetos de um formulário personalizado existente.

Um formulário personalizado deve ter pelo menos um tipo de objeto.

>[!CAUTION]
>
>Se as pessoas já tiverem anexado o formulário personalizado a objetos do tipo que você deseja excluir e adicionado dados a ele, esses dados serão excluídos permanentemente quando você excluir esse tipo de objeto no formulário. Pode incluir informações históricas que os usuários precisarão mais tarde.
>
>Em geral, recomendamos minimizar o número de vezes que você edita um formulário personalizado que já está em uso. Não há um sistema de notificação para alertar as pessoas que usam o formulário personalizado sobre suas alterações.

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizado** no painel esquerdo.
1. Selecione o formulário personalizado que deseja editar e clique em **Editar**.
1. Clique no X em qualquer uma das **Tipos de objeto** que deseja excluir do formulário e, em seguida, clique em **Excluir** na mensagem de aviso que é exibida.

   ![](assets/click-x-object-types.jpg)

1. (Opcional) Repita a etapa anterior para qualquer outro tipo de objeto que você deseja remover do formulário.
1. Clique em **Concluído** e, em seguida, clique em **Fechar e salvar**.
