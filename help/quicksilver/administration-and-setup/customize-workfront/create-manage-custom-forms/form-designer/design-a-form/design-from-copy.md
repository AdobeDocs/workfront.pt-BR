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
TQID: https://experienceleague.adobe.com/WaLGsLpGDMXGvNd7W-8JzmgJYiCaxSd-gaMoGy6j-Zc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 3e77f50ee2297a9c552e27bfcdf7f08a6a4c89b5
workflow-type: tm+mt
source-wordcount: 371
ht-degree: 24%

---

# Criar um formulário com base em uma cópia

Você pode criar um novo formulário personalizado com base em um existente. Você pode anexar formulários personalizados a diferentes objetos do Workfront para captar dados sobre esses objetos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

   * [Reutilizar um campo ou widget já usado em outro formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [Adicionar campos de texto](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [Adicionar campos calculados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [Adicionar botões de opção, grupos de caixas de seleção e menus suspensos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [Adicionar campos de data](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-date-fields)
   * [Adicionar imagens, PDFs e vídeos](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Adicionar arquivos do Adobe XD](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
   * [Adicionar campos de conexão do Planning](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)

1. (Opcional) Depois de clicar em **Salvar e Fechar**, anexe o formulário ao objeto no qual você deseja usá-lo, conforme descrito em [Adicionar um formulário personalizado a um objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).
