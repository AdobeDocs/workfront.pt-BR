---
user-type: administrator
product-area: system-administration
keywords: criar,personalizado,formulário,copiar,base,outro
navigation-topic: create-and-manage-custom-forms
title: Copie um formulário personalizado para criar um novo com o construtor herdado
description: Você pode criar um novo formulário personalizado baseado em um formulário existente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Copie um formulário personalizado para criar um novo com o construtor herdado

Você pode criar um novo formulário personalizado baseado em um formulário existente.

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

## Copiar um formulário personalizado para criar um novo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizada.**
1. Selecione o formulário personalizado que deseja usar como a base para um novo formulário personalizado e clique em **Copiar**.
1. No **Cópia de formulário personalizada** na caixa exibida, digite as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do formulário</td> 
      <td>Digite um nome para o formulário copiado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Tipos de formulário </p> </td> 
      <td> <p>No <b>Tipo de formulário</b> , selecione os tipos de objetos com os quais deseja que o formulário personalizado funcione e clique no X ao lado de qualquer tipo que deseja remover. Os tipos que já estão associados ao formulário são desativados na lista.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>O formulário deve estar associado a pelo menos um tipo de objeto.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Copiar formulário**.

   No formulário original, se campos calculados referenciarem campos que são incompatíveis com um tipo de objeto adicionado ao novo formulário, uma mensagem solicitará que você altere os cálculos nesses campos.

   Da mesma forma, se uma opção de acesso para uma quebra de seção no formulário original não for compatível com um tipo de objeto adicionado ao novo, uma mensagem solicitará que você ajuste a opção.

1. Selecione o formulário que acabou de copiar e clique em **Editar**.
1. Faça qualquer alteração no formulário, conforme explicado nos seguintes artigos:

   * [Copie um formulário personalizado para criar um novo com o construtor de formulários herdado](#Add2)
   * [Adicionar dados calculados a um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Posicione campos e widgets personalizados em um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar ou editar um widget de ativo em um formulário personalizado com o construtor de formulário herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Reutilizar um campo personalizado calculado existente em um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Adicione a lógica de exibição e ignore a lógica em um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Visualizar e preencher um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. (Opcional) Depois de clicar em **Salvar+Fechar**, anexe o formulário ao objeto em que deseja usá-lo, conforme descrito em [Adicionar um formulário personalizado a um objeto](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
