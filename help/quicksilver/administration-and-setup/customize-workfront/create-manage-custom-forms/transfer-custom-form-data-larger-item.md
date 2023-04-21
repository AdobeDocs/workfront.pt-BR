---
title: Transferir dados de formulário personalizados ao converter um objeto
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Quando o trabalho definido em um item de trabalho se tornar muito grande, você poderá convertê-lo em um item de trabalho maior.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 7b378fdf3530d5e1c06f09d03c23c31afac6aa47
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Transferir dados de formulário personalizados ao converter um objeto

Dependendo das necessidades comerciais da organização, o trabalho definido em uma tarefa ou problema pode se tornar grande demais para gerenciar dentro da tarefa ou do problema. Nesse caso, é possível convertê-los em um item de trabalho maior:

* Você pode converter problemas em tarefas ou em projetos
* É possível converter tarefas em projetos

Para transferir dados de formulário personalizados de um problema para uma tarefa ou projeto, você deve concluir as duas tarefas neste artigo, na ordem abaixo.

Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) ou [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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

## Primeiro: Adicionar objetos adicionais ao formulário personalizado

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizada**.
1. Encontre o formulário necessário e clique em **Editar**.
1. Na parte superior do formulário, adicione o objeto para o qual você planeja converter a tarefa ou o problema.
   >[!INFO]
   >
   >**Exemplo**: Se desejar transferir os dados do formulário personalizado para um projeto, selecione Projeto.

1. Clique em **Aplicar** na parte inferior do formulário.

1. Continue para [Segundo: Converta o problema ou a tarefa e transfira os dados do formulário personalizado](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Segundo: Converta o problema ou a tarefa e transfira os dados do formulário personalizado {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Adicione objetos adicionais ao formulário personalizado no problema ou na tarefa que você está convertendo, conforme explicado na seção [Primeiro: Adicionar objetos adicionais ao formulário personalizado](#first-add-additonal-objects-to-the-custom-form) neste artigo.
1. Converta o problema ou a tarefa usando o **Forms personalizada** na caixa exibida para selecionar o formulário personalizado necessário. Para obter instruções, consulte os seguintes artigos:

   * [Converter um problema em um projeto no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Converter um problema em uma tarefa no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Converter uma tarefa em um projeto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. No **Converter em (tipo de objeto)** caixa de diálogo exibida, clique no botão **Adicionar Forms** e selecione o formulário copiado na seção anterior.

   As informações capturadas nos campos personalizados do problema agora são transferidas para o formulário personalizado na tarefa.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->