---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Excluir um campo ou widget personalizado do sistema
description: Para melhorar o desempenho do sistema e facilitar o uso de formulários para os usuários, remova campos e widgets personalizados do seu sistema quando eles não estiverem mais sendo usados.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# Excluir um campo ou widget personalizado do sistema

Para melhorar o desempenho do sistema e facilitar o uso de formulários para os usuários, remova campos e widgets personalizados do seu sistema quando eles não estiverem mais sendo usados.

>[!CAUTION]
>
>A exclusão de um campo personalizado também exclui todos os dados personalizados inseridos pelos usuários no campo ao preencher formulários personalizados anexados a objetos. Esses dados excluídos não podem ser recuperados.
>
>É possível exibir todos os formulários e relatórios personalizados que usam um campo personalizado que você deseja excluir para avaliar quais podem ser as repercussões. Para obter mais informações, consulte [Exibir todos os formulários personalizados que usam um campo ou widget personalizado específico](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) e [Exibir todos os relatórios que usam um campo ou widget personalizado específico](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Ou, para uma solução alternativa que pode ser usada para evitar a perda de dados em campos que não são mais usados, consulte [Remover um campo personalizado sem perder os dados inseridos pelos usuários](#remove-a-custom-field-without-losing-data-that-users-have-entered) neste artigo.

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

## Excluir um campo ou widget personalizado do sistema

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizado.**
1. Clique em **Campos** guia.
1. Selecione o campo ou widget personalizado e clique em **Excluir**.
1. Se tiver certeza de que deseja excluir permanentemente o item e (no caso de um campo personalizado) todos os dados associados nos objetos aos quais ele foi anexado, clique em **Sim, exclua.**.

## Remover um campo personalizado sem perder os dados inseridos pelos usuários {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>A remoção de um campo personalizado de um formulário personalizado com mais de 500 campos e widgets não pode ser desfeita. Se você remover o campo, não poderá adicioná-lo novamente até que o formulário tenha menos de 500 campos e widgets.

1. Determine quais campos personalizados você deseja remover do formulário personalizado original, mas não os remova neste momento.
1. Criar um novo formulário personalizado:

   1. Adicione os campos personalizados ao novo formulário que deseja remover do formulário personalizado original.

      * Se estiver usando o construtor de formulários personalizado, consulte [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
      * Se o designer do formulário for usado, consulte [Adicionar campos novos ou existentes ao formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form).

   1. Salve o novo formulário personalizado.

1. Limite o acesso ao formulário personalizado a usuários com acesso administrativo, conforme descrito em [Compartilhar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. Aplique o novo formulário personalizado aos objetos em que o formulário personalizado original já está aplicado, conforme descrito em [Adicionar um formulário personalizado a um objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Aplicar o novo formulário personalizado a esses objetos garante que os dados históricos de relatórios não sejam afetados.

1. Modifique o formulário personalizado original e remova os campos personalizados adicionados ao novo formulário (na Etapa 2).

   Os campos removidos do formulário personalizado original agora estão disponíveis somente no novo formulário personalizado que você criou. Os usuários podem ver o formulário personalizado no objeto, mas os usuários sem acesso administrativo não podem modificar o formulário personalizado.
