---
title: Transferir dados de formulário personalizados ao converter um objeto
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Quando o trabalho definido em um item de trabalho se torna muito grande, você pode convertê-lo em um item de trabalho maior.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '404'
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

## Primeira: Adicionar outros objetos ao formulário personalizado

{{step-1-to-setup}}

1. Clique em **Forms Personalizado**.
1. Localize o formulário necessário e clique em ![Ícone Editar](assets/edit-icon.png).
1. Na parte superior do formulário, adicione o objeto para o qual você planeja converter a tarefa ou problema.

   >[!INFO]
   >
   >**Exemplo**: se você deseja transferir os dados do formulário personalizado para um projeto, selecione Projeto.

1. Clique em **Aplicar** na parte inferior do formulário.

1. Continuar em para [Segundo: converta o problema ou a tarefa e transfira os dados do formulário personalizado](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Segunda: converter o problema ou a tarefa e transferir os dados do formulário personalizado {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Adicione mais objetos ao formulário personalizado no problema ou tarefa que você está convertendo, como explicado na seção [Primeiro: adicione mais objetos ao formulário personalizado](#first-add-additonal-objects-to-the-custom-form) neste artigo.
1. Converta o problema ou a tarefa usando a opção **Forms personalizado** na caixa que é exibida para selecionar o formulário personalizado necessário. Para obter instruções, consulte os seguintes artigos:

   * [Converter um problema em um projeto no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Converter um problema em uma tarefa no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Converter uma tarefa em um projeto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. Na caixa de diálogo **Converter em (tipo de objeto)** que é exibida, clique no menu suspenso **Adicionar Forms** e selecione o formulário copiado na seção anterior.

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