---
title: Adicionar lógica de exibição e ignorar lógica a um formulário personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode decidir quais seções de um formulário personalizado devem ser exibidas ou ignoradas com base nas opções que um usuário faz ao preenchê-las.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 59e3b958dd81f2f068bc06c3fe439de0084f9ce4
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Adicionar lógica de exibição e ignorar lógica a um formulário personalizado

Você pode decidir quais seções de um formulário personalizado devem ser exibidas ou ignoradas com base nas opções que um usuário faz ao preenchê-las.

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

## Considerações para usar a lógica de exibição e ignorar a lógica

* Para adicionar lógica de exibição em um campo personalizado, widget ou quebra de seção, pelo menos um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção) deve ser posicionado antes dele no formulário.

   Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Não é possível adicionar lógica de omissão a um widget ou uma quebra de seção. Você pode adicioná-lo somente a um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção).

* Você pode adicionar lógica de exibição e lógica de omissão a um campo personalizado. O seguinte é verdadeiro sobre o campo personalizado:

   * É um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção)
   * É precedido por um campo de escolha múltipla
   * É seguido por outro campo personalizado

* Ao copiar formulários com lógica de exibição ou lógica de omissão, a lógica é copiada para o novo formulário personalizado.
* Lembre-se do seguinte ao criar uma regra de lógica de exibição para um formulário personalizado

   * Campos personalizados não incluídos em uma instrução de lógica de exibição são exibidos em um formulário personalizado, por padrão.
   * Você pode criar instruções de lógica de exibição de vários campos.

* Ao editar objetos em massa, todos os campos personalizados são exibidos na caixa Editar objetos , incluindo os campos que são ignorados ou ocultos.

## Crie um formulário personalizado de amostra que tenha a lógica de exibição e omissão

A melhor maneira de aprender a adicionar a lógica de exibição e de omissão a um formulário personalizado é através do exemplo prático explicado nas duas seções a seguir:

* [Exibir lógica](#display-logic)
* [Ignorar lógica](#skip-logic)

### Exibir lógica {#display-logic}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms personalizada** ![](assets/custom-forms-icon.png).

1. Crie o formulário personalizado de amostra:

   1. Clique em **Novo formulário personalizado**, depois clique em **Projeto** na lista suspensa.

   1. No **Título do formulário** caixa, tipo **Exemplo de formulário personalizado - Saiba mais sobre a lógica de exibição e ignore a lógica**.

   1. Clique em **Adicionar um campo** no canto superior esquerdo.
   1. Adicionar um campo suspenso chamado *Campo de ocorrência* clicando em **Lista suspensa**, em seguida, digitar **Campo de emissão** no **Rótulo** caixa.

   1. Em **Opções**, adicione as seguintes opções nas caixas de texto:

      Necessidade de investigação

      Não mais pesquisa

   1. Clique em **Salvar + Fechar** no canto inferior esquerdo.

1. Selecione o novo **Exemplo de formulário personalizado - Saiba mais sobre a lógica de exibição e ignore a lógica** formulário personalizado e clique em **Editar**.

1. Adicionar um novo campo de texto de linha única chamado *Outras pesquisas* clicando em **Campo de texto de linha única**, em seguida, digitar **Outras pesquisas** no **Rótulo** caixa.

1. Clique em **Adicionar lógica** próximo do lado inferior esquerdo da **Editar formulário personalizado** tela.

1. Na caixa exibida, com a variável **Exibir lógica** da guia aberta, configure a lógica de quando a variável **Outras pesquisas** O campo aparecerá no formulário clicando em **Campo de emissão** na primeira lista suspensa, **Pesquisa necessária** na segunda lista suspensa, e **Selecionado** na terceira lista suspensa.
1. Clique em **Salvar** para fechar o **Lógica do campo** e clique em **Concluído** no **Configurações de campo** área.

   Agora, quando alguém seleciona **Pesquisa necessária** no **Campo de emissão** , o **Outras pesquisas** será exibido.

1. Clique em **Visualizar** para garantir que a lógica seja exibida da maneira desejada no formulário.
1. Clique em **Visualização final** quando você descobrir que a lógica funciona conforme o esperado.
1. Clique em **Salvar + Fechar** no **Editar formulário personalizado** para salvar o formulário, continue em [Ignorar lógica](#skip-logic) abaixo.

### Ignorar lógica {#skip-logic}

Ignorar a lógica funciona de forma semelhante à lógica de exibição, mas atua como o inverso: em vez de fazer com que campos de escolha múltipla personalizados específicos apareçam com base em seleções específicas, você determinará quais deles devem ser ignorados, com base nas seleções dos usuários.

Para saber mais sobre isso, continue trabalhando no formulário personalizado de amostra criado na seção [Exibir lógica](#display-logic) neste artigo:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Forms personalizada**.
1. Selecione o formulário **Exemplo de formulário personalizado - Saiba mais sobre a lógica de exibição e ignore a lógica** que você criou nas etapas acima, em seguida, clique em **Editar**.

1. Selecione o campo suspenso que você criou com o nome *Campo de emissão*.
1. Clique no botão **Adicionar lógica** no botão **Configurações de campo** barra lateral.

1. No **Lógica do campo** verifique se a **Ignorar lógica** é selecionada.

1. Defina o primeiro menu suspenso como **Não mais pesquisa** e o segundo menu suspenso para **Selecionado**.

1. No **Em Seguida, Ignorar Para** , selecione **Fim do formulário.**

   Agora, quando alguém seleciona **Não mais pesquisa** no **Campo de emissão** no campo suspenso , o formulário ignorará diretamente o final do formulário sem exibir o **Outras pesquisas** campo.

1. Clique em **Salvar**.
1. Clique em **Visualizar**  para ter certeza de que a lógica se aplica da maneira que você quer.
1. Clique em **Concluído** no lado inferior esquerdo do formulário.
