---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configurar o compartilhamento de campos e widgets personalizados com o construtor de formulários herdado
description: Por padrão, ao adicionar um novo campo ou widget personalizado a um formulário personalizado, qualquer pessoa no sistema com acesso a formulários personalizados pode editar as propriedades desse item, como seu rótulo e nome. Você pode alterar isso controlando com quem ele pode ser compartilhado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 2%

---

# Configurar o compartilhamento de campos e widgets personalizados com o construtor de formulários herdado

Por padrão, ao adicionar um novo campo ou widget personalizado a um formulário personalizado, qualquer pessoa no sistema com acesso a formulários personalizados pode editar as propriedades desse item, como seu rótulo e nome. Você pode alterar isso controlando com quem ele pode ser compartilhado.

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Adicionar um campo personalizado a um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Adicionar ou editar um widget de ativo em um formulário personalizado com o construtor de formulário herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Configurar compartilhamento para um campo ou widget personalizado

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms personalizada**.
1. Se você estiver configurando o compartilhamento de um campo ou widget personalizado na instância Workfront de sua organização, faça o seguinte:

   1. Clique no botão **Campos** guia .
   1. Selecione o item para o qual deseja configurar o compartilhamento e clique em **Compartilhar**.

   Ou, se você estiver configurando o compartilhamento de um campo ou widget personalizado em um formulário personalizado existente, faça o seguinte:

   1. Selecione o formulário personalizado e clique em **Editar**.
   1. Na área de edição de formulário à direita, selecione o item para o qual deseja configurar o compartilhamento.
   1. No painel esquerdo, clique em **Campo Compartilhar**.


1. No **Acesso a Campo Personalizado** caixa que é exibida, especifique com quem você deseja compartilhar o item e como deseja compartilhá-lo:

   1. Próximo ao canto inferior esquerdo do **Acesso a Campo Personalizado** caixa , abaixo **Conceder acesso a campo personalizado a**, comece digitando o nome de um usuário, equipe, função de trabalho, grupo ou empresa com o qual deseja compartilhar o item e clique no nome quando ele for exibido.

      ![](assets/share-field-give-access-to.jpg)

   1. Se desejar ser mais específico sobre como deseja compartilhar o item, clique na lista suspensa à direita do nome e use qualquer uma das seguintes opções:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Visualizar o projeto</td> 
         <td> <p>Você pode clicar em <strong>Configurações avançadas</strong> para especificar se deseja que o usuário ou usuários possam usar o acesso para adicionar o item a um formulário personalizado ou compartilhá-lo com outros usuários.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Gerenciar o projeto</td> 
         <td> <p>Permite o acesso para editar o campo personalizado e visualizá-lo na Biblioteca de campos e na página em que você cria formulários personalizados.</p> <p>Você pode clicar em <strong>Configurações avançadas</strong> para especificar se deseja que o usuário ou usuários possam usar seu acesso para excluir o item do sistema ou compartilhá-lo com outros usuários.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Opcional) Repita a etapa anterior para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no canto superior direito, se desejar escolher uma opção de compartilhamento do sistema para o campo .

   Nem todas as opções a seguir são exibidas nesse menu suspenso ao mesmo tempo. Por exemplo, o segundo é exibido somente quando um dos outros dois é selecionado.

   * **Faça isso editável em todo o sistema para que todos no Workfront possam editá-lo** (a opção padrão)

      Ao adicionar um campo ou widget personalizado e não limitar o compartilhamento, todos no sistema que tiverem acesso a formulários personalizados poderão exibi-lo e editar suas propriedades.

   * **Remover o acesso para editar em todo o sistema.**

      Limita o acesso somente àqueles que você adicionou à lista.

   * **Tornar isto visível em todo o sistema para que todos no Workfront possam visualizar**

1. Clique em **Salvar** ou **Salvar + Fechar**.

## Acesso herdado a campos e widgets personalizados quando um formulário personalizado é compartilhado

Quando alguém compartilha um formulário personalizado com um grupo, função de trabalho, equipe ou empresa, os destinatários herdam o acesso de Exibição a quaisquer campos e widgets personalizados que estejam no formulário. Esse nível de acesso a esses itens no formulário é sempre retido para que o formulário possa funcionar para os recipients, conforme pretendido pela pessoa que o criou. Isso é verdade mesmo para recipients que têm acesso Editar ao formulário.

Você pode descobrir quem herdou o acesso a um campo ou widget personalizado e remover o acesso a ele.

>[!NOTE]
>
>Se um recipient tiver acesso de Gerenciar a um campo ou widget personalizado no formulário personalizado compartilhado, esse acesso será retido para o recipient.

* [Descubra quem herdou o acesso a um campo ou widget personalizado](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Descubra quem herdou o acesso a um campo ou widget personalizado {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms personalizada**.
1. Clique no botão **Campos** e, em seguida, selecione o campo, a imagem ou o widget de acesso.
1. Na caixa exibida, clique em **Permissões herdadas** e exibir os nomes exibidos.
1. Clique em **Cancelar**.

### Remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Se for necessário remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado, é necessário cancelar o compartilhamento do formulário. Para obter instruções, consulte a seção . [Remover acesso a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) no artigo [Compartilhar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
