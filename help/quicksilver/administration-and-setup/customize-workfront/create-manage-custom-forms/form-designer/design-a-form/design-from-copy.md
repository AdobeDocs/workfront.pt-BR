---
title: Criar um formulário a partir de uma cópia
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: É possível criar um formulário personalizado a partir de uma cópia com o designer do formulário.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: e9d1e35a9c94143a84eb2007985a42f0960a09f7
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Criar um formulário a partir de uma cópia

<!--add preview tags and see below in comment out-->

Você pode criar um novo formulário personalizado com base em um existente. Você pode anexar formulários personalizados a diferentes objetos do Workfront para capturar dados sobre esses objetos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Copiar um formulário personalizado para criar um novo

{{step-1-to-setup}}

1. Clique em **Forms Personalizado.**
1. Selecione o formulário personalizado que deseja usar como base para um novo formulário personalizado e clique em ![Ícone Copiar](assets/copy-icon.png).
1. Na caixa **Cópia de Formulário Personalizada** exibida, digite as seguintes informações:

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
      <td> <p>Na caixa <b>Tipo de Formulário</b>, selecione os tipos de objeto com os quais deseja que o formulário personalizado funcione e clique no X ao lado de todos os tipos que deseja remover. Os tipos que já estão associados ao formulário estão desabilitados na lista.</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>O formulário deve estar associado a pelo menos um tipo de objeto.</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Copiar**.

   No formulário original, se os campos calculados referenciarem campos incompatíveis com um tipo de objeto adicionado ao novo formulário, uma mensagem solicitará que você altere os cálculos nesses campos.

   Da mesma forma, se uma opção de acesso para uma quebra de seção no formulário original não for compatível com um tipo de objeto adicionado ao novo, uma mensagem solicitará que você ajuste a opção.

1. Selecione o formulário que você acabou de copiar e clique em ![Ícone Editar](assets/edit-icon.png).
1. Faça alterações no formulário, conforme explicado nas seções a seguir do artigo [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md):

   * [Reutilizar um campo ou widget existente já usado em outro formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Adicionar campos de texto](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [Adicionar campos calculados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [Adicionar botões de opção, grupos de caixas de seleção e menus suspensos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [Adicionar campos de digitação antecipada e data](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [Adicionar imagens, PDF e vídeos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Adicionar arquivos do Adobe XD](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
     <!--* [Add Planning connection fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)-->

1. (Opcional) Depois de clicar em **Salvar e Fechar**, anexe o formulário ao objeto no qual você deseja usá-lo, conforme descrito em [Adicionar um formulário personalizado a um objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
