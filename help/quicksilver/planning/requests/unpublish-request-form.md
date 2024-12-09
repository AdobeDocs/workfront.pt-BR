---
title: Cancelar a Publicação de um Formulário de Solicitação no Adobe Workfront Planning
description: Você pode desfazer a publicação de um formulário de solicitação se ele não for mais necessário ou relevante. Ao desfazer a publicação, você remove as permissões de todos para acessar o formulário.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: b42436ad660642bd23638a8a44d9561513d748ed
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---


# Cancelar a publicação de um formulário de solicitação no Adobe Workfront Planning


<!--take Preview and Production references at Production time-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode desfazer a publicação de um formulário de solicitação se ele não for mais necessário ou relevante. Ao desfazer a publicação, você remove as permissões de todos para acessar o formulário.

Também é possível alterar as entidades com as quais você compartilha um formulário de solicitação, caso deseje mantê-lo disponível para um grupo menor de pessoas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produtos</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td>
   <td>
<p>Qualquer um dos seguintes planos da Workfront:</p>
<ul><li>Selecionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p>
   </td>

<tr>
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td>
   <td>
<p>Qualquer </p>  
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </td>

<tr>
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td>
   <td>
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões de objeto</p></td>
   <td>
   <ul>
   <li><p>Gerenciar permissões em um espaço de trabalho</p></li>
    <li><p>Os administradores do sistema podem gerenciar espaços de trabalho que não criaram. </p></li>
    </ul>
   <p>Para obter informações sobre o compartilhamento de permissões para objetos do Workfront Planning, consulte  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Visão geral das permissões de compartilhamento no Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Alterar o compartilhamento de um formulário de solicitação

Se você compartilhar uma solicitação de publicamente, com todos, incluindo usuários de fora da organização, poderá considerar restringir esse acesso a determinados usuários que visualizam ou gerenciam o espaço de trabalho ao qual o formulário está associado.

Para alterar o compartilhamento de um formulário de solicitação:

{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.

1. Clique no menu **Mais** ![](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho da página e clique em **Atualizar formulário de solicitação**.
1. Clique em **Compartilhar** no canto superior direito da tela e atualize as opções de compartilhamento. Para obter mais informações, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Opcional) Clique em **Copiar link**, se você alterou o compartilhamento do formulário de solicitação e deseja compartilhá-lo com o novo grupo de pessoas com um novo link.

## Cancelar publicação de um formulário de solicitação para um tipo de registro

Quando um formulário de solicitação se torna irrelevante e você não deseja que ninguém o acesse mais, é possível desfazer a publicação.

{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.

1. Clique no menu **Mais** ![](assets/more-menu.png) à direita do nome do tipo de registro no cabeçalho da página e clique em **Atualizar formulário de solicitação**.
1. Clique em **Cancelar publicação** no canto superior direito.

   ![](assets/unpublish-button-highlighted.png)

   Uma confirmação é exibida na parte inferior da tela notificando que a publicação do formulário foi cancelada.

   O botão **Cancelar publicação** é alterado para **Publish**.

1. Clique em **Salvar**.

   O formulário não pode mais ser acessado de um link <!--or from the request queue in the Requests area of Workfront-->.

   Todos os registros adicionados anteriormente usando o formulário de solicitação permanecem na página de tipo de registro.

   <span class="preview">Todas as solicitações adicionadas anteriormente permanecem na área Solicitações do Workfront, na guia Planejamento.</span>