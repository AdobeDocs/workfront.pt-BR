---
title: Criar ou editar um formulário personalizado com o construtor de formulários herdado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode criar ou editar um novo formulário personalizado.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 8af1890b2e2ae613279b5191cf8f2190364fb524
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Criar ou editar um formulário personalizado com o construtor de formulários herdado

<!--Audited: 01/2024-->

Você pode criar ou editar um novo formulário personalizado. Ambas as tarefas são explicadas neste artigo.

Para obter informações sobre como criar um novo formulário personalizado a partir de um existente, consulte [Copie um formulário personalizado para criar um novo com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

Este artigo descreve como criar um formulário personalizado usando o construtor de formulários herdado. Para obter informações sobre como criar um formulário personalizado usando o designer de formulário, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para descobrir quais configurações de plano, tipo de licença ou nível de acesso você tem, entre em contato com o administrador do Workfront. Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Comece a criar um formulário personalizado

{{step-1-to-setup}}

1. Clique em **Forms personalizado** no painel esquerdo.

   Formulários personalizados são exibidos em uma lista. Você pode revisar todos os formulários e campos personalizados que foram criados para sua organização. Você também pode ver quem criou cada formulário, os objetos associados a ele e se ele está ativo.

1. Clique em **Novo formulário personalizado.**
1. Selecione pelo menos um tipo de objeto que deseja associar ao formulário personalizado e clique em **Continuar**.

   ![](assets/choose-object-type.jpg)

1. No **Configurações de formulário** que for aberta, digite uma **Título do formulário** e um opcional **Descrição** para o formulário personalizado.

1. (Opcional) Se quiser adicionar mais tipos de objeto ao formulário para que ele possa ser anexado a mais objetos, clique no link **mais** assinar depois **Tipos de objeto** e, em seguida, selecione o tipo de objeto desejado no menu exibido.

   Você pode repetir isso para adicionar quantos tipos de objetos desejar.

1. (Opcional) Clique no link **X** em um tipo de objeto para excluí-lo do formulário.

   Para obter informações sobre como excluir tipos de objetos de um formulário personalizado que você já salvou, consulte [Excluir tipos de objeto em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Clique em **Concluído** no canto inferior esquerdo da tela.

   >[!TIP]
   >
   >Você pode clicar em **Aplicar** a qualquer momento enquanto estiver criando um formulário personalizado para salvar suas alterações e manter o formulário aberto.

1. Se quiser adicionar um novo campo personalizado ao formulário, continue em [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) ou [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Ou

   Se quiser continuar criando seu formulário personalizado de outras maneiras, continue com um dos seguintes artigos:

   * [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Posicionar campos e widgets personalizados em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar uma quebra de seção a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Reutilizar um campo personalizado calculado existente em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Adicionar lógica de exibição e lógica de salto a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## Começar a editar um formulário personalizado

É possível editar um formulário personalizado a qualquer momento após sua criação.

>[!CAUTION]
>
>Para obter informações sobre como remover campos de um formulário personalizado sem perder dados inseridos pelos usuários nesses campos, consulte a seção [Remover um campo personalizado sem perder os dados inseridos pelos usuários](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) no artigo [Excluir um campo ou widget personalizado do sistema](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>Em geral, recomendamos minimizar o número de vezes que você edita um formulário personalizado que já está em uso. Não há um sistema de notificação para alertar as pessoas que usam o formulário personalizado sobre suas alterações.

{{step-1-to-setup}}

1. Clique em **Forms personalizado** no painel esquerdo.

   Formulários personalizados são exibidos em uma lista. Você pode revisar todos os formulários e campos personalizados que foram criados para sua organização. Você também pode ver quem criou cada formulário, os objetos associados a ele e se ele está ativo.

1. Selecione o formulário personalizado que deseja editar e clique em **Editar**.
1. (Opcional) Para alterar o título e a descrição do formulário personalizado, clique no **Configurações do formulário** e digite um **Título do formulário** e **Descrição**.

1. (Opcional) Se quiser adicionar mais tipos de objetos ao formulário para que ele possa ser anexado a mais objetos, clique no sinal de mais + depois de **Tipos de objeto** e, em seguida, selecione o tipo desejado no menu exibido.

   ![](assets/add-object-type-existing-form.png)

   Você pode repetir isso para adicionar quantos tipos de objetos desejar.

   Você também pode clicar no X em um tipo de objeto para excluí-lo do formulário. Isso deve ser feito com cuidado quando você quiser excluir um tipo de objeto de um formulário personalizado que já foi salvo. Para obter mais informações, consulte [Excluir tipos de objeto em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. Clique em **Concluído**.

   >[!TIP]
   >
   >Você pode clicar em **Aplicar** a qualquer momento enquanto estiver criando um formulário personalizado para salvar suas alterações e manter o formulário aberto.

1. Se quiser adicionar um novo campo personalizado ao formulário, continue em [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) ou [Reutilizar um campo ou widget personalizado em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   Ou

   Se quiser continuar criando seu formulário personalizado de outras maneiras, continue com um dos seguintes artigos:

   * [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Posicionar campos e widgets personalizados em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Adicionar uma quebra de seção a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Reutilizar um campo personalizado calculado existente em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Adicionar lógica de exibição e lógica de salto a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
