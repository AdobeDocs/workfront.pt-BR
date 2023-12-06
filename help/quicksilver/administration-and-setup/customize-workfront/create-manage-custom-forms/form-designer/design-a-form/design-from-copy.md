---
title: Criar um formulário a partir de uma cópia com o designer do formulário
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode criar um formulário personalizado a partir de uma cópia com o designer do formulário.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Criar um formulário a partir de uma cópia com o designer do formulário

Você pode criar um novo formulário personalizado com base em um existente. Você pode anexar formulários personalizados a diferentes objetos do Workfront para capturar dados sobre esses objetos.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>
   <p>Novo plano: Padrão</p>
   <p>ou</p>
   <p>Plano atual: Plano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para descobrir quais configurações de plano, tipo de licença ou nível de acesso você tem, entre em contato com o administrador do Workfront.

## Copiar um formulário personalizado para criar um novo

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizado.**
1. Selecione o formulário personalizado que deseja usar como base para um novo formulário personalizado e clique em **Copiar**.
1. No **Personalizar cópia do formulário** que for exibida, digite as seguintes informações:

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
      <td> <p>No <b>Tipo de formulário</b> , selecione os tipos de objeto com os quais você deseja que o formulário personalizado funcione e clique no X ao lado de qualquer tipo que você deseja remover. Os tipos que já estão associados ao formulário estão desabilitados na lista.</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>O formulário deve estar associado a pelo menos um tipo de objeto.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Copiar formulário**.

   No formulário original, se os campos calculados referenciarem campos incompatíveis com um tipo de objeto adicionado ao novo formulário, uma mensagem solicitará que você altere os cálculos nesses campos.

   Da mesma forma, se uma opção de acesso para uma quebra de seção no formulário original não for compatível com um tipo de objeto adicionado ao novo, uma mensagem solicitará que você ajuste a opção.

1. Selecione o formulário que acabou de copiar e clique em **Editar**.
1. Faça alterações no formulário, conforme explicado nas seções a seguir do [Criar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) artigo:

* [Reutilizar um campo ou widget existente já usado em outro formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Adicionar campos de texto](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [Adicionar campos calculados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [Adicionar botões de opção, grupo de caixas de seleção e menus suspensos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [Adicionar campos de digitação antecipada e data](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [Adicionar imagens, PDF e vídeos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Adicionar arquivos do Adobe XD](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. (Opcional) Depois de clicar em **Salvar+Fechar**, anexe o formulário ao objeto no qual você deseja usá-lo, conforme descrito em [Adicionar um formulário personalizado a um objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
