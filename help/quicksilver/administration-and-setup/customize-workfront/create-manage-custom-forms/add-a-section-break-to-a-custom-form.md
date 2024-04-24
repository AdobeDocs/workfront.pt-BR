---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Adicionar uma quebra de seção a um formulário personalizado com o construtor de formulários herdado
description: Você pode agrupar campos e widgets personalizados em um formulário personalizado em seções com cabeçalhos. Isso é útil para apresentar uma experiência organizada a usuários que preencherão o formulário. Além disso, se você precisar limitar o acesso a determinados campos e widgets personalizados a determinados usuários, poderá colocá-los em uma seção e conceder acesso à seção somente a esses usuários.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: 28961cda48ce4eec84ed272e660be6ba938be370
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 0%

---

# Adicionar uma quebra de seção a um formulário personalizado com o construtor de formulários herdado

Você pode agrupar campos e widgets personalizados em um formulário personalizado em seções com cabeçalhos. Isso é útil para apresentar uma experiência organizada a usuários que preencherão o formulário. Além disso, se você precisar limitar o acesso a determinados campos e widgets personalizados a determinados usuários, poderá colocá-los em uma seção e conceder acesso à seção somente a esses usuários.

Por exemplo, se você precisar rastrear informações confidenciais que somente administradores do sistema devem poder exibir ou editar, poderá criar uma quebra de seção com permissões Somente de administrador e colocar os campos confidenciais nessa seção.

As configurações de acesso selecionadas para uma seção são vinculadas diretamente às permissões que os usuários têm no objeto do Workfront ao qual o formulário personalizado está anexado. Você pode ocultar ou mostrar uma seção com base no fato de o usuário ter acesso para exibir, contribuir ou gerenciar esse objeto. Ou você pode definir uma seção como Somente administrador para que somente usuários com um nível de acesso de administrador do sistema possam acessá-la.

Para obter informações sobre permissões em objetos, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

## Requisitos de acesso

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
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p></td> 
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Criar e configurar o acesso para uma seção em um formulário personalizado

1. Comece a criar ou editar um formulário personalizado, conforme descrito em [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Adicione campos e widgets personalizados ao formulário, conforme descrito em [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. Ao criar ou editar o formulário personalizado, no **Adicionar um campo** clique em **Quebra de seção**.

   ![](assets/click-section-break.jpg)

1. No **Configurações do campo** , configure as opções desejadas para a seção:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rótulo</td> 
      <td> <p>(Obrigatório) Digite um rótulo descritivo para exibir acima da seção. Você pode alterar o rótulo a qualquer momento.</p> <p><b>IMPORTANTE</b>: Evite usar caracteres especiais neste rótulo. Eles não são exibidos corretamente nos relatórios.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite texto se quiser explicar aos usuários para que serve a seção. É exibido abaixo do rótulo da seção no formulário personalizado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Adicionar Lógica</p></td> 
      <td><p>Use a lógica de exibição para especificar se a seção deve ser exibida no formulário, com base nas seleções que os usuários fazem em campos personalizados de múltipla escolha quando preenchem o formulário.</p><p><strong>NOTA:</strong> Se todos os campos individuais em uma quebra de seção tiverem lógica de exibição aplicada a eles e todos estiverem ocultos como resultado da lógica, a seção inteira será ocultada no formulário personalizado. Isso ocorrerá mesmo se a lógica de exibição não for aplicada à quebra de seção.</p><p>Para obter mais informações, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Adicionar lógica de exibição e lógica de salto a um formulário personalizado</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Conceder acesso</p> </td> 
      <td> <p> Selecione as permissões que os usuários precisam em um objeto ao qual o formulário personalizado está anexado para exibir esta seção e editar seus valores de campo.
       <p>As seguintes permissões estão disponíveis em <b>Os usuários com esse acesso ao objeto podem visualizar valores de campo</b>:</p> 
         <ul>
          <li><strong>Exibir</strong>: permissões de exibição para o objeto</li>
          <li><p><b>Edição Limitada</b>: (Disponível somente se o objeto for um projeto, tarefa, problema ou usuário):</p> 
          <p>Permite que os usuários contribuam com o objeto se ele for um projeto, tarefa ou problema.</p>
          <p>Permite que os usuários editem o perfil ou sejam proprietários da permissão de perfil para o objeto, se for um usuário.</p></li> 
          <li><b>Editar</b>: Gerenciar permissões para o objeto </li> 
          <li><b>Somente administrador</b>: Nível de acesso do Administrador do sistema</li> 
         </ul> </li> 
        <p>As seguintes permissões estão disponíveis em <b>Os usuários com esse acesso ao objeto podem editar valores de campo</b>: </p> 
         <ul> 
          <li> <p><b>Edição Limitada</b>: (Disponível somente se o objeto for um projeto, tarefa, problema ou usuário):</p> 
           <p>Se o objeto for um projeto, tarefa ou problema, essa permissão permitirá que os usuários contribuam para o objeto</p>
          <p>Se o objeto for um usuário, essa permissão permitirá que os usuários editem o perfil ou sejam proprietários da permissão de perfil para o objeto.</p> 
          <li><b>Editar</b>: Gerenciar permissões para o objeto </li> 
          <li><b>Somente administrador</b>: Nível de acesso do Administrador do sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Para obter informações sobre permissões em objetos, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral das permissões de compartilhamento em objetos</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Os usuários sem as permissões especificadas aqui não podem ver os campos e widgets personalizados na seção. </p> <p>Isso também é verdadeiro se você exibir os valores dos campos nos relatórios ou usá-los em campos calculados nos relatórios do modo de texto.</p> </li>
       <li><p>Para formulários personalizados de solicitação/ocorrência: se o acesso de Exibição for necessário para ver os campos na quebra de seção, mas o acesso de Administrador for necessário para editar os campos, a seção e todos os seus campos não estarão visíveis para não administradores quando eles preencherem o formulário. Depois que a solicitação é criada, os usuários com acesso de Visualização podem exibir os campos na seção.</p></li>
       <li> <p>Associar vários tipos de objeto ao seu formulário pode alterar as permissões de exibição e edição disponíveis nessas etapas. Para obter mais informações, consulte <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Como vários tipos de objeto podem afetar as permissões de quebra de seção em um formulário personalizado</a> neste artigo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Arraste ou adicione pelo menos um campo ou widget personalizado à nova seção.

   Isso é necessário antes de salvar a seção.

1. Clique em **Concluído**.

   >[!TIP]
   >
   >Você pode clicar em **Aplicar** a qualquer momento enquanto estiver criando um formulário personalizado para salvar suas alterações e manter o formulário aberto.

1. Se quiser continuar criando seu formulário personalizado de outras maneiras, continue com um dos seguintes artigos:

   * [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Posicionar campos e widgets personalizados em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar lógica de exibição e lógica de salto a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Pré-visualizar e preencher um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## Como vários tipos de objeto podem afetar as permissões de quebra de seção {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

A permissão Edição limitada para quebras de seção de formulário personalizado está disponível somente para os tipos de objeto Projeto, Tarefa, Problema e Usuário.

Em um formulário personalizado com uma quebra de seção configurada com a permissão Edição limitada, se você adicionar um dos outros tipos de objeto ao formulário (Portfolio, Programa, Documento, Empresa, Registro de faturamento, Iteração, Despesa ou Grupo), será solicitado que você alterne para a permissão Editar, que é compatível tanto com esse tipo de objeto quanto com os tipos de objeto existentes no formulário.

>[!INFO]
>
>**Exemplo:** Em um formulário personalizado associado ao tipo de objeto Projeto, uma quebra de seção é configurada com a permissão Edição limitada.
>
>Você adiciona o tipo de objeto Portfolio ao formulário, o que significa que a opção de permissão Edição limitada não está mais disponível para a quebra de seção no formulário.
>
>Uma mensagem na tela solicita que você alterne para a permissão Editar, que é a opção mais semelhante à Edição limitada, e compatível com o tipo de objeto Projeto e o tipo de objeto Portfolio.

