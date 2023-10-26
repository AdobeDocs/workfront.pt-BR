---
product-area: projects;user-management
keywords: editar,formulários,rich,texto,especial,formato,campos,personalizado,informações,personalizar,objetos
navigation-topic: work-with-custom-forms
title: Editar informações em campos de formulário personalizados
description: Você pode editar informações em um formulário personalizado depois que o formulário for anexado a um objeto. Para obter informações sobre como adicionar formulários personalizados a objetos, consulte Adicionar um formulário personalizado a um objeto.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 456310e460bae44183de390efc4be919fda3f36d
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Editar informações em campos de formulário personalizados

Você pode editar informações em um formulário personalizado depois que o formulário for anexado a um objeto. Para obter informações sobre como adicionar formulários personalizados a objetos, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>plano do Adobe Workfront*</p> </td> 
   <td>Equipe ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenças da Adobe Workfront*</p> </td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Editar o acesso ao objeto para o qual deseja editar o formulário personalizado</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Permissões de objeto</p> </td> 
   <td> 
    <ul> 
     <li> <p>Permissões do Contribute ou superior no objeto para o qual você deseja editar o formulário personalizado</p> </li> 
     <li>Visualize as permissões nos campos que deseja editar. Para obter informações sobre compartilhamento de permissões para campos personalizados, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">Configurar compartilhamento para campos e widgets personalizados</a>.</li> 
     <li> <p>Editar permissões para as seções no formulário em que os campos que você deseja editar estão localizados</p> </li> 
    </ul> <p>Para obter informações sobre como solicitar acesso adicional para objetos, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Pré-requisitos

* O administrador do Workfront ou um usuário do plano com acesso administrativo a formulários personalizados deve criar formulários personalizados em seu ambiente. Para obter mais informações, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* Você deve ter formulários personalizados anexados a um objeto.

  Para obter informações sobre como aplicar formulários personalizados a um objeto, consulte [Adicionar um formulário personalizado a um objeto](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Editar informações em um formulário personalizado

A edição de informações em um formulário personalizado anexado a um objeto é idêntica para todos os objetos. Para obter informações sobre quais objetos podem ter um formulário personalizado, consulte [Visão geral de formulários personalizados](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Vá para um objeto para o qual deseja editar informações no formulário personalizado.
1. Clique em **`<Object type>`Detalhes** no painel esquerdo.

   Por exemplo, ao editar informações em um formulário personalizado de projeto, clique em **Detalhes do projeto**.

1. Role até o formulário personalizado. Quando houver um formulário personalizado anexado ao objeto, o nome do formulário será exibido como uma área na seção Detalhes.
1. Se necessário, clique na seta ![](assets/expand-arrow-right.png) à esquerda do nome do formulário personalizado para expandi-lo.
1. Ao lado do canto superior direito da página, clique no ícone Editar ![](assets/edit-icon.png).
1. Comece a inserir informações em qualquer campo ao qual você tenha acesso.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   Ou

   Se nenhuma informação tiver sido inserida ainda no formulário, clique em **Adicionar+** para qualquer campo ao qual você tenha acesso e comece a inserir informações.

   ![](assets/plus-add-to-edit-info-350x180.png)

   Se vários formulários personalizados estiverem anexados ao objeto, você poderá fazer isso para cada formulário.

   Dependendo do tipo de campo em que você está trabalhando, considere o seguinte:

   * É possível selecionar apenas uma opção para campos de botão de opção.
   * É possível selecionar uma ou várias opções em um campo de caixa de seleção, dependendo de como o criador do formulário configurou o campo.
   * É possível selecionar uma ou várias opções em um campo suspenso de seleção múltipla, dependendo de como o criador do formulário configurou o campo.
   * Você pode formatar campos de texto (negrito, itálico ou sublinhado) somente se o usuário que criou o formulário os configurar como um Campo de texto com o tipo de campo Formatação. Campos de Texto de Linha Única e Campos de Texto de Parágrafo não podem ser formatados.
   * Você só poderá atualizar a hora do dia em um tipo de campo Data se o usuário que criou o formulário o tiver incluído ao criar o campo.

   Para obter informações sobre todos os tipos de campo, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Clique em **Salvar alterações**.

   >[!IMPORTANT]
   >
   >É necessário preencher todos os campos obrigatórios no formulário antes de salvá-lo. O nome de um campo obrigatório é seguido por um asterisco.
   >
   >![](assets/nwe-required-custom-field.png)

   Quando alguém altera dados em outro objeto referenciado por campos personalizados calculados em seu objeto, as alterações não são refletidas automaticamente no objeto. Para obter informações sobre a atualização manual de todos os campos personalizados calculados no objeto, consulte [Recalcular todos os campos personalizados calculados para um objeto](#recalculate-all-calculated-custom-fields-for-an-object) neste artigo.

   Quando campos dependentes da página são modificados, os campos calculados no formulário personalizado são recalculados dinamicamente em tempo real. Você pode ver o novo valor do campo calculado sem salvar o formulário, mas ele não é realmente aplicado ao formulário e ao objeto até que você salve as alterações. Isso se aplica aos campos calculados em formulários padrão, bem como formulários personalizados.

   Você também pode atualizar manualmente todos os campos personalizados calculados de um objeto ao editá-lo em massa junto com outros objetos em uma lista. Para obter instruções, consulte [Recalcular todos os campos personalizados calculados para vários objetos em uma lista ao editar os objetos](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) neste artigo.

## Recalcular todos os campos personalizados calculados para um objeto  {#recalculate-all-calculated-custom-fields-for-an-object}

1. Vá para a página principal do objeto cujos campos personalizados você deseja recalcular.
1. Clique em **Mais** menu ![](assets/more-icon.png) à direita do nome do objeto e, em seguida, clique em **Recalcular Expressões**.

   Isso recalcula todos os campos personalizados no formulário do objeto.

## Recalcular todos os campos personalizados calculados para vários objetos em uma lista ao editar os objetos {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

Você pode recalcular manualmente os campos personalizados de vários objetos editando-os em massa a partir de uma lista ou relatório.

1. Ir para uma lista de objetos que contêm formulários personalizados com campos calculados.
1. Selecione os objetos cujos campos personalizados calculados você deseja atualizar.
1. Clique em **Ícone Editar**.
1. Clique em **Forms personalizado** no menu esquerdo, selecione **Recalcular expressões personalizadas**.
1. Clique em **Salvar** **Alterações**.

   O Workfront calcula todos os campos personalizados para todos os objetos selecionados.

>[!TIP]
>
>Dependendo da complexidade de seus projetos, recomendamos não selecionar um grande número de projetos ao recalcular campos personalizados calculados em massa para garantir o desempenho ideal. Alguns itens que podem tornar um projeto muito complexo podem ser várias dependências ou atribuições ou um grande número de campos personalizados.
>
>Para recalcular expressões personalizadas em massa de uma lista de projetos:
>
>1. Vá para uma lista de projetos ou relatório e selecione um ou vários projetos.
>1. Clique em **Mais** menu ![](assets/more-icon.png)e, em seguida, clique em **Recalcular expressões personalizadas**.
>
>![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
>
>O Workfront calcula todos os campos personalizados para todos os projetos selecionados.
