---
title: Configurar compartilhamento para campos e widgets personalizados
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Por padrão, quando você adiciona um novo campo ou widget personalizado a um formulário personalizado, qualquer pessoa no sistema com acesso a formulários personalizados pode editar as propriedades desse item, como rótulo e nome. Você pode alterar isso controlando com quem ele pode ser compartilhado.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
source-git-commit: a8e2558469d3abc355eb58f81658db3d1cfc7315
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 5%

---

# Configurar compartilhamento para campos e widgets personalizados

Por padrão, quando você adiciona um novo campo ou widget personalizado a um formulário personalizado, qualquer pessoa no sistema com acesso a formulários personalizados pode editar as propriedades desse item, como rótulo e nome. Você pode alterar isso controlando com quem ele pode ser compartilhado.

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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

<!--

## Configure sharing a custom field or widget from the list of forms

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Click **Fields** to open the Fields area.
1. Select the item you want to configure sharing for, then click ![Share icon](assets/share-icon.png).
1. In the Custom Field Access box that displays, specify who you want to share the item with and how you want to share it:

   1. Near the lower-left corner of the **Custom Field Access** box, under **Give custom field access to**, start typing the name of a user, team, job role, group, or company you want to share the item with, then click the name when it appears.

      ![Custom Field Access box](assets/share-field-give-access-to.jpg)

   1. If you want to be more specific about how you want to share the item, click the drop-down list to the right of the name, then use any of the following options:

      ![Sharing options](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">View it</td> 
         <td> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to add the item to a custom form or share it with other users.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Manage it</td> 
         <td> <p>Allows access to edit the custom field and to see it in the Field Library and on the page where you build custom forms.</p> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to delete the item from the system or share it with other users.</p> </td> 
        </tr> 
       </tbody> 
      </table>   

1. (Optional) Repeat the previous step to add other names to the list and configure their options.
1. (Optional) Click the gear icon ![Settings icon](assets/gear-icon-settings.png) in the top-right corner if you want to choose a system-wide sharing option for the field.

   Not all of the following options display in this drop-down menu at the same time. For example, the second one displays only when one of the other two are selected.

   * **Make this editable system-wide so that everyone in Workfront can edit it** (the default option)

     When you add a custom field or widget and you don't limit sharing for it, everyone in the system who has access to custom forms can view it and edit its properties.
   
   * **Remove system-wide edit access**

     Limits access to only those whom you added to the list. 
   
   * **Make this visible system-wide so that everyone in Workfront can see it**

1. Click **Save**.

-->

## Configurar o compartilhamento de um campo ou widget personalizado

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Para compartilhar na lista de formulários e campos:

   1. Clique em **Campos** para abrir a área Campos.
   1. Selecione o campo que você deseja compartilhar e clique em ![Ícone Compartilhar](assets/share-icon.png).

1. Para compartilhar no designer do formulário:
   1. Abra um formulário personalizado ou crie um novo formulário personalizado.
   1. No designer do formulário, selecione o campo que deseja compartilhar e clique em **Compartilhar** na área de edição de campos à direita.

1. Na caixa de compartilhamento, em **Conceder acesso ao campo**, comece digitando o nome do usuário, da equipe, da função de trabalho, do grupo, da empresa ou do perfil comercial com o qual deseja compartilhar o item e pressione **Enter** quando o nome for exibido.
1. Se quiser ser mais específico sobre como compartilhar o item, clique no menu suspenso à direita do nome e use uma das seguintes opções:

   * **Exibir**: clique no ícone **Configurações Avançadas** ![ícone Configurações Avançadas](assets/configure-options-icon.png) para especificar se você deseja que os usuários possam adicionar o item a um formulário personalizado ou compartilhá-lo com outros usuários.
   * **Gerenciar**: permite acesso para editar o campo personalizado e visualizá-lo na biblioteca de campos e no designer do formulário. Clique no ícone **Configurações Avançadas** ícone ![Configurações Avançadas](assets/configure-options-icon.png) para especificar se você deseja que os usuários possam excluir o item do sistema ou compartilhá-lo com outros usuários.

1. (Opcional) Repita as etapas 5 a 6 para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Escolha uma opção de compartilhamento em todo o sistema para o campo:

   * **Todos no sistema podem editar** (a opção padrão)

     Ao adicionar um campo ou widget personalizado e não limitar o compartilhamento, todos os usuários no sistema que têm acesso a formulários personalizados podem visualizá-lo e editar suas propriedades.

   * **Todos no sistema podem visualizar**

     Todas as pessoas no sistema que têm acesso a formulários personalizados podem visualizar o campo, mas não editá-lo.

   * **Somente pessoas convidadas podem acessar**

     Limita o acesso somente àqueles que você adicionou à lista.

   ![Opções de compartilhamento](assets/share-field-in-designer.png)

1. Clique em **Salvar**.

## Acesso herdado a campos e widgets personalizados quando um formulário personalizado é compartilhado

Quando alguém compartilha um formulário personalizado com um grupo, função de trabalho, equipe, empresa ou perfil comercial, os destinatários herdam o acesso de Visualização a todos os campos e widgets personalizados que estão no formulário. Esse nível de acesso a esses itens no formulário é sempre retido para que o formulário possa funcionar para os recipients conforme pretendido pela pessoa que o criou. Isso é verdade mesmo para recipients que têm acesso para Editar ao formulário.

Você pode descobrir quem herdou acesso a um campo ou widget personalizado e remover o acesso a ele.

>[!NOTE]
>
>Se um recipient tiver Acesso de gerenciamento a um campo ou widget personalizado no formulário personalizado compartilhado, esse acesso será retido para o recipient.

### Descubra quem herdou acesso a um campo ou widget personalizado {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Clique em **Campos** e selecione o campo, a imagem ou o widget de acesso.
1. Na caixa exibida, clique em **Permissões Herdadas** e exiba os nomes exibidos.
1. Clique em **Cancelar**.

### Remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Se você precisar remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado, será necessário cancelar o compartilhamento do formulário. Para obter instruções, consulte a seção [Remover acesso a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form) no artigo [Compartilhar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).


