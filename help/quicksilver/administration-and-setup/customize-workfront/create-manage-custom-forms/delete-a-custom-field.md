---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Excluir um campo ou widget personalizado do sistema
description: Para melhorar o desempenho do sistema e facilitar o uso dos formulários para os usuários, você pode remover campos e widgets personalizados do sistema quando eles não estiverem mais sendo usados.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Excluir um campo ou widget personalizado do sistema

Para melhorar o desempenho do sistema e facilitar o uso dos formulários para os usuários, você pode remover campos e widgets personalizados do sistema quando eles não estiverem mais sendo usados.

>[!CAUTION]
>
>A exclusão de um campo personalizado também exclui todos os dados personalizados que os usuários inseriram no campo ao preencher formulários personalizados anexados a objetos. Os dados excluídos não podem ser recuperados.
>
>Você pode exibir todos os formulários personalizados e relatórios que usam um campo personalizado que deseja excluir para avaliar quais repercussões podem ser. Para obter mais informações, consulte [Exibir todos os formulários personalizados que usam um campo ou widget personalizado específico](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) e [Exibir todos os relatórios que usam um campo ou widget personalizado específico](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Ou, para uma solução alternativa, é possível usar para evitar a perda de dados em campos que não são mais usados, consulte [Remover um campo personalizado sem perder dados inseridos pelos usuários](#remove-a-custom-field-without-losing-data-that-users-have-entered) neste artigo.

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

## Excluir um campo ou widget personalizado do sistema

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizada.**
1. Clique no botão **Campos** guia .
1. Selecione o campo ou o widget personalizado e clique em **Excluir**.
1. Se tiver certeza de que deseja excluir permanentemente o item e (no caso de um campo personalizado) todos os dados associados nos objetos em que ele foi anexado, clique em **Sim, Excluir**.

## Remover um campo personalizado sem perder dados inseridos pelos usuários {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>A remoção de um campo personalizado de um formulário personalizado que tenha mais de 500 campos e widgets não pode ser desfeita. Se você remover o campo, não será possível adicioná-lo novamente até que o formulário tenha menos de 500 campos e widgets.

1. Determine quais campos personalizados você deseja remover do formulário personalizado original, mas não remova-os nesse momento.
1. Crie um novo formulário personalizado, conforme descrito em [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. Adicione os campos personalizados ao novo formulário que você deseja remover do formulário personalizado original, conforme descrito em [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
   1. Salve o novo formulário personalizado.

1. Limite o acesso ao formulário personalizado somente para usuários com acesso administrativo, conforme descrito em [Compartilhar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Aplique o novo formulário personalizado aos objetos em que o formulário personalizado original já está aplicado, conforme descrito em [Adicionar um formulário personalizado a um objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   A aplicação do novo formulário personalizado a esses objetos garante que os dados históricos de relatórios não sejam afetados.

1. Modifique o formulário personalizado original e remova os campos personalizados adicionados ao novo formulário (na Etapa 2).

   Os campos que você removeu do formulário personalizado original agora estão disponíveis somente no novo formulário personalizado que você criou. Os usuários podem ver o formulário personalizado no objeto, mas os usuários sem acesso administrativo não podem modificar o formulário personalizado.
