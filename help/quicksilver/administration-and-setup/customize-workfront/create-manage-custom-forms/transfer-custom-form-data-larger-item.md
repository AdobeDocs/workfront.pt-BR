---
title: Transferir dados de formulário personalizados ao converter um objeto
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Quando o trabalho definido em um item de trabalho se torna muito grande, você pode convertê-lo em um item de trabalho maior.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Transferir dados de formulário personalizados ao converter um objeto

Dependendo das necessidades comerciais de sua organização, o trabalho definido em uma tarefa ou problema pode se tornar muito grande para ser gerenciado dentro da tarefa ou do problema. Nesse caso, você pode convertê-los em um item de trabalho maior:

* É possível converter problemas em tarefas ou em projetos
* É possível converter tarefas em projetos

Para transferir dados de formulários personalizados de um problema para uma tarefa ou um projeto, você deve concluir as duas tarefas neste artigo, na ordem abaixo.

Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) ou [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

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

## Primeiro: adicionar outros objetos ao formulário personalizado

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizado**.
1. Localize o formulário necessário e clique em **Editar**.
1. Na parte superior do formulário, adicione o objeto para o qual você planeja converter a tarefa ou problema.
   >[!INFO]
   >
   >**Exemplo**: se desejar transferir os dados do formulário personalizado para um projeto, selecione Projeto.

1. Clique em **Aplicar** na parte inferior do formulário.

1. Continue em para [Segunda: converter o problema ou a tarefa e transferir os dados do formulário personalizado](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Segunda: converter o problema ou a tarefa e transferir os dados do formulário personalizado {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Adicione mais objetos ao formulário personalizado no problema ou tarefa que você está convertendo, conforme explicado na seção [Primeira: Adicionar outros objetos ao formulário personalizado](#first-add-additonal-objects-to-the-custom-form) neste artigo.
1. Converta o problema ou a tarefa usando o **Forms personalizado** na caixa exibida para selecionar o formulário personalizado necessário. Para obter instruções, consulte os seguintes artigos:

   * [Converter um problema em um projeto no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Converter um problema em uma tarefa no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Converter uma tarefa em um projeto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. No **Converter em (tipo de objeto)** que for exibida, clique na guia **Adicionar o Forms** e selecione o formulário copiado na seção anterior.

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