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
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Transferir dados de formulário personalizados ao converter um objeto

Dependendo das necessidades comerciais da organização, o trabalho definido em uma tarefa ou problema pode se tornar grande demais para gerenciá-lo dentro da tarefa ou do problema. Nesse caso, é possível convertê-los em um item de trabalho maior:

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

## Primeiro: Copiar o formulário personalizado {#first-copy-the-custom-form}

Primeiro, é necessário manter os dados personalizados do formulário em uma tarefa ou problema que você deseja converter. Como os dados do formulário personalizado devem ser uma correspondência exata no item convertido, a prática recomendada é duplicar o formulário para que você possa anexá-lo ao novo objeto.

>[!TIP]
>
>Outra maneira de manter os dados de formulários personalizados nessa situação é adicionar o tipo de objeto maior ao formulário personalizado. Para obter instruções, consulte a seção [Comece a editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) no artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizada**.
1. Selecione o formulário personalizado do tipo tarefa ou ocorrência e clique em **Copiar**.
1. No **Formulário personalizado** , especifique um nome para o novo formulário.

1. No **Tipo de formulário** no menu suspenso , selecione o tipo de objeto para o qual deseja criar o novo formulário personalizado

   **Exemplo:** Se desejar transferir os dados do formulário personalizado para um projeto, selecione Projeto.

1. Clique em **Copiar formulário**.

   Esse formulário personalizado copiado agora pode ser anexado a uma tarefa ou projeto.

1. Continue para [Segundo: Converta o problema ou a tarefa e transfira os dados do formulário personalizado](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Segundo: Converta o problema ou a tarefa e transfira os dados do formulário personalizado {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Copie o formulário personalizado no problema ou na tarefa que você está convertendo, conforme explicado na seção [Primeiro: Copiar o formulário personalizado](#first-copy-the-custom-form) neste artigo.
1. Converta o problema ou a tarefa usando o **Forms personalizada** na caixa exibida para selecionar o formulário personalizado copiado. Para obter instruções, consulte os seguintes artigos:

   * [Converter um problema em um projeto no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Converter um problema em uma tarefa no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Converter uma tarefa em um projeto](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. No **Converter em (tipo de objeto)** caixa de diálogo exibida, clique no botão **Adicionar Forms** e selecione o formulário copiado na seção anterior.

   As informações capturadas nos campos personalizados do problema agora são transferidas para o formulário personalizado na tarefa.

