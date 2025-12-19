---
title: Cancelar a Publicação de um Formulário de Solicitação no Adobe Workfront Planning
description: Você pode desfazer a publicação de um formulário de solicitação se ele não for mais necessário ou relevante. Ao desfazer a publicação, você remove as permissões de todos para acessar o formulário.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: 66d59467e7e9857ca5573b819d51da839ddbd4f7
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 5%

---

# Cancelar a publicação de um formulário de solicitação no Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Você pode desfazer a publicação de um formulário de solicitação se ele não for mais necessário ou relevante. Ao desfazer a publicação, você remove as permissões de todos para acessar o formulário.

Também é possível alterar as entidades com as quais você compartilha um formulário de solicitação, caso deseje mantê-lo disponível para um grupo menor de pessoas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e qualquer pacote do Planning</p>
Ou
<p>Qualquer pacote de fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e tipo de registro</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Alterar o compartilhamento de um formulário de solicitação

Se você compartilhar uma solicitação de publicamente, com todos, incluindo usuários de fora da organização, poderá considerar restringir esse acesso a determinados usuários que visualizam ou gerenciam o espaço de trabalho ao qual o formulário está associado.

Para alterar o compartilhamento de um formulário de solicitação:

{{step1-to-planning}}

1. Clique no espaço de trabalho onde deseja compartilhar um formulário.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.

1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho da página e clique em **Gerenciar formulários de solicitação**.

   Todos os formulários de solicitação associados ao tipo de registro são exibidos em uma exibição de tabela.
1. Passe o cursor do mouse sobre o nome de um formulário de solicitação e clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome e clique em **Compartilhar**.
1. Atualize as opções de compartilhamento selecionando uma das opções a seguir:

   * Qualquer pessoa com acesso de exibição ou superior ao espaço de trabalho
   * Qualquer pessoa com acesso de contribuição ou superior ao espaço de trabalho
   * Qualquer pessoa com o link

   Para obter mais informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Opcional) Clique em **Copiar link**, se você alterou o compartilhamento do formulário de solicitação e deseja compartilhá-lo com o novo grupo de pessoas com um novo link.

## Cancelar publicação de um formulário de solicitação para um tipo de registro

Quando um formulário de solicitação se torna irrelevante e você não deseja que ninguém o acesse mais, é possível desfazer a publicação.

{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.

1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho da página e clique em **Gerenciar formulários de solicitação**.

   Todos os formulários de solicitação associados ao tipo de registro são exibidos em uma exibição de tabela.
1. Passe o cursor do mouse sobre o nome de um formulário de solicitação e clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome e clique em **Cancelar publicação**

Ou

Clique no nome do formulário de solicitação para abri-lo e em **Desfazer publicação** no canto superior direito do formulário de solicitação.

![Botão Cancelar publicação realçado](assets/unpublish-button-highlighted.png)

Uma confirmação é exibida na parte inferior da tela notificando que a publicação do formulário foi cancelada.

O link ou botão **Cancelar publicação** é alterado para **Publicar**.

1. (Condicional) Clique em **Salvar**, se você desfez a publicação do formulário depois de abri-lo.

   Os usuários não podem mais acessar o formulário de solicitação de um link ou da fila de solicitações na área Solicitações do Workfront.

   Todos os registros adicionados anteriormente usando o formulário de solicitação permanecem na página de tipo de registro.

   Todas as solicitações adicionadas anteriormente permanecem na área Solicitações do Workfront.
