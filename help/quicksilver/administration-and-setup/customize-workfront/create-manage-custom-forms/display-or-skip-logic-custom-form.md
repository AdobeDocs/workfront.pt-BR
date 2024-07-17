---
title: Adicionar lógica de exibição e lógica de salto a um formulário personalizado com o construtor de formulários herdado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode decidir quais seções de um formulário personalizado devem ser exibidas ou ignoradas com base nas escolhas que um usuário faz ao preenchê-lo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 0%

---

# Adicionar lógica de exibição e lógica de salto a um formulário personalizado com o construtor de formulários herdado

{{form-designer-default}}

Você pode decidir quais seções de um formulário personalizado devem ser exibidas ou ignoradas com base nas escolhas que um usuário faz ao preenchê-lo.

>[!NOTE]
>
>A lógica se aplica somente a um formulário e não pode ser baseada em seleções de um formulário diferente.

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
   <td>Plano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber quais configurações de plano, tipo de licença ou nível de acesso você tem, contate o administrador do Workfront.

## Considerações sobre o uso da lógica de exibição e da lógica de salto

* Para adicionar lógica de exibição em um campo personalizado, widget ou quebra de seção, pelo menos um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção) deve ser posicionado antes dele no formulário.

  Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Adicionar um campo personalizado a um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Adicionar ou editar um widget de ativo em um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Não é possível adicionar lógica de salto a um widget ou quebra de seção. Você pode adicioná-lo somente a um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção).

* Você pode adicionar a lógica de exibição e a lógica de salto a um campo personalizado se todos os itens a seguir forem verdadeiros sobre o campo personalizado:

   * É um campo de múltipla escolha (botões de opção, lista suspensa ou caixas de seleção)
   * É precedido por um campo de múltipla escolha
   * Ele é seguido por outro campo personalizado

* Ao copiar formulários com lógica de exibição ou lógica de salto, a lógica é copiada para o novo formulário personalizado.
* Ao editar objetos em massa, todos os campos personalizados são exibidos na caixa Editar objetos, incluindo os campos que são ignorados ou ocultos.
* Lembre-se do seguinte ao criar uma regra de lógica de exibição para um formulário personalizado:

   * Campos personalizados não incluídos em uma instrução lógica de exibição são exibidos em um formulário personalizado por padrão.
   * Você pode criar instruções lógicas de exibição de vários campos.
   * Se todos os campos em uma quebra de seção tiverem lógica de exibição aplicada a eles e todos estiverem ocultos como resultado da lógica, a seção inteira será ocultada no formulário personalizado.

## Criar um formulário personalizado de amostra com lógica de exibição e salto

A melhor maneira de aprender a adicionar lógica de exibição e salto a um formulário personalizado é por meio do exemplo prático explicado nas duas seções a seguir:

### Lógica de exibição {#display-logic}

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms Personalizado**.

1. Crie o exemplo de formulário personalizado:

   1. Clique em **Novo formulário personalizado** e em **Projeto** na lista suspensa.

   1. Na caixa **Título do formulário**, digite **Exemplo de formulário personalizado - Lógica de exibição de aprendizado e lógica de salto**.

   1. Clique em **Adicionar um campo** no canto superior esquerdo.
   1. Adicione um campo suspenso chamado *Campo de problema* clicando em **Suspenso** e digitando **Campo de problema** na caixa **Rótulo**.

   1. Em **Opções**, adicione as seguintes opções nas caixas de texto:

      Investigação necessária

      Sem mais pesquisas

   1. Clique em **Salvar + Fechar** no canto inferior esquerdo.

1. Selecione o novo formulário personalizado de **Amostra - Lógica de exibição de aprendizado e lógica de salto** formulário personalizado e clique em **Editar**.

1. Adicione um novo campo de texto de linha única chamado *Outra Pesquisa* clicando em **Campo de Texto de Linha Única** e digitando **Outra Pesquisa** na caixa **Rótulo**.

1. Clique em **Adicionar Lógica** próximo ao lado inferior esquerdo da tela **Editar formulário personalizado**.

1. Na caixa exibida, com a guia **Lógica de Exibição** aberta, configure a lógica de quando o campo **Outra Pesquisa** aparecerá no formulário clicando em **Campo de problema** na primeira lista suspensa, **Pesquisa Necessária** na segunda lista suspensa e **Selecionada** na terceira lista suspensa.
1. Clique em **Salvar** para fechar a janela **Lógica de Campo** e em **Concluído** na área **Configurações de Campo**.

   Agora, quando alguém selecionar **Pesquisa necessária** no menu suspenso **Campo de problema**, o campo **Outra pesquisa** será exibido.

1. Clique em **Visualizar** para verificar se a lógica aparece da maneira que você deseja no formulário.
1. Clique em **Finalizar visualização** quando descobrir que a lógica funciona conforme o esperado.
1. Clique em **Salvar + Fechar** na janela **Editar Formulário Personalizado** para salvar o formulário e continue com a [Lógica de ramificação](#skip-logic) abaixo.

### Lógica de salto {#skip-logic}

Ignorar funções lógicas de forma semelhante à lógica de exibição, mas age como o inverso: em vez de fazer com que campos específicos personalizados de múltipla escolha apareçam com base em seleções específicas, você determina quais deles devem ser ignorados, com base nas seleções dos usuários.

Para saber mais sobre isso, continue trabalhando no exemplo de formulário personalizado que você criou na seção [Lógica de exibição](#display-logic) neste artigo:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Forms Personalizado**.
1. Selecione o formulário **Exemplo de formulário personalizado - Lógica de exibição de aprendizado e lógica de salto** que você criou nas etapas acima, depois clique em **Editar**.

1. Selecione o campo suspenso criado chamado *Campo de problema*.
1. Clique no botão **Adicionar Lógica** na barra lateral **Configurações de Campo**.

1. Na caixa **Lógica de Campo**, verifique se a guia **Lógica de Ignorar** está selecionada.

1. Defina a primeira lista suspensa como **Sem mais pesquisas** e a segunda lista suspensa como **Selecionado**.

1. No menu suspenso **Pular para**, selecione **Fim do formulário.**

   Agora, quando alguém selecionar **Nenhuma pesquisa adicional** no campo suspenso **Campo de problema**, o formulário pulará diretamente para o final do formulário sem exibir o campo **Outra Pesquisa**.

1. Clique em **Salvar**.
1. Clique em **Visualizar** para verificar se a lógica se aplica da maneira que você deseja.
1. Clique em **Concluído** no lado inferior esquerdo do formulário.
