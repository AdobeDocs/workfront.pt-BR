---
title: Adicionar ou excluir tipos de objeto de um formulário personalizado existente com o designer do formulário
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode adicionar ou remover tipos de objetos de formulários personalizados com o designer de formulários.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: c0082dd73e3db8123f9cc08f1798ef8e70730625
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---


# Adicionar ou excluir tipos de objeto de um formulário personalizado existente com o designer do formulário

{{highlighted-preview-article-level}}

É possível adicionar ou excluir tipos de objetos de um formulário personalizado existente com o designer do formulário.

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
   <td>
   <p>Plano atual: Padrão</p>
   <p>ou</p>
   <p>Plano herdado: plano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td><p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;Para descobrir quais configurações de plano, tipo de licença ou nível de acesso você tem, entre em contato com o administrador do Workfront.

## Adicionar tipos de objeto a um formulário personalizado existente

Você pode adicionar outros tipos de objetos ao formulário para que ele possa ser anexado a vários objetos.

>[!NOTE]
>
>As permissões de quebra de seção podem ser afetadas pelo tipo de objeto. A permissão Edição limitada para quebras de seção de formulário personalizado está disponível somente para os tipos de objeto Projeto, Tarefa, Problema e Usuário.
>
>Para obter mais informações, consulte [Como vários tipos de objeto podem afetar as permissões de quebra de seção](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizado** no painel esquerdo.

   Na exibição exibida, você pode revisar todos os formulários personalizados que foram criados para sua organização. Você também pode ver quem criou cada formulário, com que tipo de objeto ele funciona e se ele está ativo.

1. Selecione o formulário personalizado ao qual você deseja adicionar outros tipos de objeto e clique em **Editar**.

1. Na parte superior do formulário, clique no sinal de mais + depois de **Tipos de objeto** e, em seguida, selecione o tipo desejado no menu exibido. Você pode repetir isso para adicionar quantos tipos de objetos desejar.

   ![](assets/add-new-object.png)

1. Clique em **Salvar e fechar**.

   >[!TIP]
   >
   >Você pode clicar em **Aplicar** a qualquer momento enquanto estiver criando um formulário personalizado para salvar suas alterações e manter o formulário aberto.

## Excluir tipos de objeto em um formulário personalizado

Você pode excluir tipos de objetos de um formulário personalizado existente. Um formulário personalizado deve ter pelo menos um tipo de objeto.

>[!CAUTION]
>
>Se as pessoas já tiverem anexado o formulário personalizado a objetos do tipo que você deseja excluir e adicionado dados a ele, esses dados serão excluídos permanentemente quando você excluir esse tipo de objeto no formulário. Pode incluir informações históricas que os usuários precisarão mais tarde.
>
>Em geral, recomendamos minimizar o número de vezes que você edita um formulário personalizado que já está em uso. Não há um sistema de notificação para alertar as pessoas que usam o formulário personalizado sobre suas alterações.

Para deletar um tipo de objeto:

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizado** no painel esquerdo.
1. Selecione o formulário personalizado que deseja editar e clique em **Editar**.
1. Clique no X em qualquer uma das **Tipos de objeto** que deseja excluir do formulário e, em seguida, clique em **Excluir** na mensagem de aviso que é exibida.

   ![](assets/delete-object-types.png)

1. (Opcional) Repita a etapa anterior para qualquer outro tipo de objeto que você deseja remover do formulário.
1. Clique em **Concluído** e, em seguida, clique em **Fechar e salvar**.
