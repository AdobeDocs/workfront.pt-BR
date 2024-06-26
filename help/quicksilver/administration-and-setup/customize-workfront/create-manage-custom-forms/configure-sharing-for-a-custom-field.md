---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configurar compartilhamento para campos e widgets personalizados com o construtor de formulários herdado
description: Por padrão, quando você adiciona um novo campo ou widget personalizado a um formulário personalizado, qualquer pessoa no sistema com acesso a formulários personalizados pode editar as propriedades desse item, como rótulo e nome. Você pode alterar isso controlando com quem ele pode ser compartilhado.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Configurar compartilhamento para campos e widgets personalizados com o construtor de formulários herdado

{{form-designer-default}}

Por padrão, quando você adiciona um novo campo ou widget personalizado a um formulário personalizado, qualquer pessoa no sistema com acesso a formulários personalizados pode editar as propriedades desse item, como rótulo e nome. Você pode alterar isso controlando com quem ele pode ser compartilhado.

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Adicionar um campo personalizado a um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Adicionar ou editar um widget de ativo em um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Configurar compartilhamento para um campo ou widget personalizado

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms personalizado**.
1. Se você estiver configurando o compartilhamento para um campo ou widget personalizado na instância do Workfront da sua organização, faça o seguinte:

   1. Clique em **Campos** para abrir a área Campos.
   1. Selecione o item para o qual você deseja configurar o compartilhamento e clique em ![Ícone Compartilhar](assets/share-icon.png).

   Ou, se estiver configurando o compartilhamento de um campo ou widget personalizado em um formulário personalizado existente, faça o seguinte:

   1. Selecione o formulário personalizado e clique em ![Ícone Editar](assets/edit-icon.png).
   1. Na área de edição de formulário à direita, selecione o item para o qual deseja configurar o compartilhamento.
   1. No painel esquerdo, clique em **Compartilhar campo**.

1. No **Acesso ao campo personalizado** que é exibida, especifique com quem você deseja compartilhar o item e como deseja compartilhá-lo:

   1. Próximo ao canto inferior esquerdo do **Acesso ao campo personalizado** caixa, em **Conceder acesso ao campo personalizado a**, comece digitando o nome de um usuário, equipe, função de trabalho, grupo ou empresa com a qual deseja compartilhar o item e clique no nome quando ele for exibido.

      ![](assets/share-field-give-access-to.jpg)

   1. Se quiser ser mais específico sobre como compartilhar o item, clique na lista suspensa à direita do nome e use uma das seguintes opções:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Visualizar o projeto</td> 
         <td> <p>Você pode clicar em <strong>Configurações avançadas</strong> para especificar se você deseja que o usuário ou usuários possam usar seu acesso para adicionar o item a um formulário personalizado ou compartilhá-lo com outros usuários.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Gerenciar o projeto</td> 
         <td> <p>Permite acesso para editar o campo personalizado e vê-lo na Biblioteca de campos e na página onde você cria formulários personalizados.</p> <p>Você pode clicar em <strong>Configurações avançadas</strong> para especificar se você deseja que o usuário ou usuários possam usar seu acesso para excluir o item do sistema ou compartilhá-lo com outros usuários.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Opcional) Repita a etapa anterior para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no canto superior direito, se desejar escolher uma opção de compartilhamento em todo o sistema para o campo.

   Nem todas as opções a seguir são exibidas nesse menu suspenso ao mesmo tempo. Por exemplo, o segundo é exibido somente quando um dos outros dois é selecionado.

   * **Tornar isso editável em todo o sistema para que todos no Workfront possam editá-lo** (a opção padrão)

     Ao adicionar um campo ou widget personalizado e não limitar o compartilhamento, todos os usuários no sistema que têm acesso a formulários personalizados podem visualizá-lo e editar suas propriedades.

   * **Remover o acesso para editar em todo o sistema**

     Limita o acesso somente àqueles que você adicionou à lista.

   * **Tornar isto visível em todo o sistema para que todos no Workfront possam vê-lo**

1. Clique em **Salvar** ou **Salvar + Fechar**.

## Acesso herdado a campos e widgets personalizados quando um formulário personalizado é compartilhado

Quando alguém compartilha um formulário personalizado com um grupo, função de trabalho, equipe ou empresa, os recipients herdam o acesso de Visualização a quaisquer campos e widgets personalizados que estejam no formulário. Esse nível de acesso a esses itens no formulário é sempre retido para que o formulário possa funcionar para os recipients conforme pretendido pela pessoa que o criou. Isso é verdade mesmo para recipients que têm acesso para Editar ao formulário.

Você pode descobrir quem herdou acesso a um campo ou widget personalizado e remover o acesso a ele.

>[!NOTE]
>
>Se um recipient tiver Acesso de gerenciamento a um campo ou widget personalizado no formulário personalizado compartilhado, esse acesso será retido para o recipient.

* [Descubra quem herdou acesso a um campo ou widget personalizado](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Descubra quem herdou acesso a um campo ou widget personalizado {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms personalizado**.
1. Clique em **Campos**, em seguida, selecione o campo, imagem ou widget de acesso.
1. Na caixa exibida, clique em **Permissões herdadas** e visualize os nomes exibidos.
1. Clique em **Cancelar**.

### Remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Se você precisar remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado, será necessário cancelar o compartilhamento do formulário. Para obter instruções, consulte na seção [Remover o acesso a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) no artigo [Compartilhar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
