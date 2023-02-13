---
product-area: projects
navigation-topic: manage-issues
title: Modificar atribuições de usuários para vários problemas em uma lista
description: Modificar atribuições de usuários para vários problemas em uma lista
author: Alina
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 7e77223595d3c9cf0d6592a09e893142439adb2c
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# Modificar atribuições de usuários para vários problemas em uma lista

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Você pode modificar simultaneamente as atribuições de usuários para vários problemas. Para obter informações sobre como editar problemas ou atribuí-los um de cada vez, consulte também os seguintes artigos:

* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Atribuir problemas](../../../manage-work/issues/manage-issues/assign-issues.md)

Para obter informações gerais sobre atribuição de problemas, consulte [Modificar visão geral de atribuições de emissão](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Você deve ter pelo menos permissões do Contribute para um problema e poder fazer atribuições no problema.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para o problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

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
1. (Opcional) Crie um filtro para exibir somente os problemas atribuídos ao destinatário que você deseja modificar.

   Por exemplo, você pode criar um filtro para exibir apenas problemas com uma função específica como o destinatário. Em seguida, é possível substituir a função por um usuário específico. Faça o seguinte:

   1. Clique no botão **Filtro** lista suspensa e clique em **Novo filtro**.

      A caixa de diálogo Novo filtro é exibida.

   1. Clique em **Adicionar uma regra de filtro.**
   1. Para filtrar uma função específica, expanda **Funções de Atribuição,** em seguida, clique em **ID.**

      Ou

      Para filtrar um usuário específico, expanda **Usuários da Atribuição,** em seguida, clique em **ID.**

      >[!TIP]
      >
      >Não utilizar **Atribuído a** porque este campo se refere somente ao Proprietário da ocorrência e não a todos os destinatários.

   1. Na lista suspensa, selecione **Igual** como qualificador de filtro.
   1. Comece digitando o nome do usuário ou função para a qual deseja filtrar e clique no nome quando ele aparecer na lista suspensa.
   1. Clique em **Salvar filtro.**

1. Selecione os problemas para os quais deseja modificar atribuições e clique no botão **Editar** ícone ![](assets/qs-edit-icon.png).

   O **Editar problemas** será exibido. Os itens editados são exibidos no canto superior esquerdo da página.

1. Vá para o **Atribuições** e selecione **Destinatário**.

   ![](assets/classic-assignmens-area-on-edit-box-350x119.png)

1. Siga um destes procedimentos:

   1. Para adicionar um novo destinatário:

      1. Comece a digitar o nome de um usuário, função ou equipe e selecione-o quando for exibido na lista. A atribuição é adicionada e não substitui as atribuições atuais nos problemas selecionados.

         >[!TIP]
         Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários ativos, funções de trabalho e equipes.
         Se um usuário, uma função de trabalho ou uma equipe tiver sido atribuída antes de ser desativada, ela permanecerá atribuída ao item de trabalho. Nesse caso, recomendamos o seguinte:
         * Atribua novamente o item de trabalho aos recursos ativos.
         * Associe os usuários em uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.


         As informações comuns em todos os problemas selecionados são exibidas. Por exemplo, se o mesmo usuário for atribuído a todos os problemas, esse usuário será exibido no **Destinatário** coluna. Se as informações não forem comuns nos problemas selecionados, nenhuma informação será exibida.
   1. Para remover destinatários individuais:

      1. Clique no botão **Ícone X** ao lado do nome do destinatário que você deseja remover se o destinatário for exibido na lista Atribuições.

         Ou

         (Condicional) Se o destinatário que você deseja remover não for exibido na seção Atribuições porque ele foi atribuído a apenas alguns dos problemas que você selecionou, clique em **Remover Destinatário** e comece a digitar o nome do destinatário que deseja remover, em seguida, clique no nome quando ele for exibido na lista suspensa.

      1. Clique em **Remover Destinatário** novamente para adicionar outro destinatário a ser removido.
   1. Para remover todos os destinatários existentes:

      1. Clique em **Remover todos os destinatários existentes**, depois clique em **Sim, Excluir Todos os Atributos**.

         Isso remove não apenas os destinatários comuns (destinatários que são exibidos na caixa de diálogo de edição), mas também todos os destinatários sobre todos os problemas selecionados.



1. (Opcional) Modifique qualquer uma das seguintes opções para os destinatários selecionados para associar aos problemas:

   * **Proprietário da ocorrência:** Selecione o botão de opção para indicar qual destinatário é designado como o Proprietário dos problemas. Se não for selecionada, a Adobe Workfront designará o primeiro destinatário como o Proprietário da ocorrência. Isso não está disponível para atribuições de equipe.
   * **Função do destinatário**: Selecione uma função na lista suspensa. Se não for selecionada, o Workfront selecionará automaticamente a Função primária do usuário.

1. Clique em **Salvar alterações**.
