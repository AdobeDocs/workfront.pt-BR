---
product-area: projects
navigation-topic: manage-issues
title: Modificar atribuições de usuário para vários problemas em uma lista
description: Modificar atribuições de usuário para vários problemas em uma lista
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 1%

---

# Modificar atribuições de usuário para vários problemas em uma lista

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Você pode modificar simultaneamente as atribuições de usuários para várias questões. Para obter informações sobre como editar problemas ou atribuí-los um de cada vez, consulte também os seguintes artigos:

* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Atribuir problemas](../../../manage-work/issues/manage-issues/assign-issues.md)

Para obter informações gerais sobre atribuição de problemas, consulte [Visão geral da modificação de atribuições de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Você deve ter pelo menos permissões do Contribute para que um problema possa fazer atribuições a ele.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:&nbsp;drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of&nbsp;reasons, including the following:</p>
<ul>
<li>Users join or leave&nbsp;your team</li>
<li>A user takes a vacation that extends beyond the issue&nbsp;due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modificar atribuições para vários problemas

1. Vá para a lista de problemas que contém os problemas cujas atribuições você deseja modificar.
1. (Opcional) Crie um filtro para exibir somente problemas atribuídos ao destinatário que você deseja modificar.

   Por exemplo, você pode criar um filtro para exibir somente problemas com uma função específica como destinatário. Em seguida, você pode substituir a função por um usuário específico. Faça o seguinte:

   1. Clique na lista suspensa **Filtro** e em **Novo Filtro**.

      A caixa de diálogo Novo filtro é exibida.

   1. Clique em **Adicionar uma Regra de Filtro.**
   1. Para filtrar por uma função específica, expanda **Funções de atribuição** e clique em **ID.**

      Ou

      Para filtrar por um usuário específico, expanda **Usuários de Atribuição,** e clique em **ID.**

      >[!TIP]
      >
      >Não use **Atribuído a** porque este campo se refere apenas ao Proprietário do problema e não a todos os atribuídos.

   1. Na lista suspensa, selecione **Igual** como qualificador de filtro.
   1. Comece digitando o nome do usuário ou função que deseja filtrar e clique no nome quando ele aparecer na lista suspensa.
   1. Clique em **Salvar filtro.**

1. Selecione os problemas para os quais deseja modificar atribuições e clique no ícone **Editar** ![](assets/qs-edit-icon.png).

   O **Editar problemas** é exibido. Os itens editados são exibidos no canto superior esquerdo da página.

1. Vá para a seção **Atribuições** e selecione **Atribuído**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Siga um destes procedimentos:

   1. Para adicionar um novo destinatário:

      1. Comece a digitar o nome de um usuário, função ou equipe e selecione-o quando ele for exibido na lista. A atribuição é adicionada e não substitui as atribuições atuais nos problemas selecionados.

         >[!TIP]
         >
         >Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
         >
         >Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
         >
         >* Reatribuir o item de trabalho aos recursos ativos.
         >* Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.

         As informações comuns em todas as ocorrências selecionadas são exibidas. Por exemplo, se o mesmo usuário for atribuído a todos os problemas, ele será exibido na coluna **Destinatário**. Se as informações não forem comuns nos problemas selecionados, nenhuma informação será exibida.

   1. Para remover designados individuais:

      1. Clique no ícone **X** ao lado do nome do destinatário que você deseja remover se ele for exibido na lista Atribuições.

         Ou

         (Condicional) Se o destinatário que você deseja remover não for exibido na seção Atribuições porque o destinatário está atribuído a apenas alguns dos problemas selecionados, clique em **Remover destinatário** e comece a digitar o nome do destinatário que você deseja remover, depois clique no nome quando ele aparecer na lista suspensa.

      1. Clique novamente em **Remover responsável** para adicionar outro responsável a ser removido.

   1. Para remover todos os designados existentes:

      1. Clique em **Remover todos os atribuídos existentes** e em **Sim, Excluir todos os atribuídos**.

         Isso remove não somente os atribuídos comuns (atribuídos exibidos na caixa de diálogo de edição), mas também todos os atribuídos em todas as questões selecionadas.

1. (Opcional) Modifique qualquer uma das seguintes opções para os responsáveis selecionados para associar às ocorrências:

   * **Proprietário da Questão:** Selecione o botão de opção para indicar qual destinatário está designado como o Proprietário da Questão. Se não for selecionada, o Adobe Workfront designará o primeiro destinatário como Proprietário do problema. Isso não está disponível para atribuições de equipe.
   * **Função do destinatário**: selecione uma função na lista suspensa. Se não for selecionada, o Workfront selecionará automaticamente a função principal do usuário.

1. Clique em **Salvar alterações**.
