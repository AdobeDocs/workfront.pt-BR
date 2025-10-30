---
product-area: projects
navigation-topic: manage-issues
title: Modificar atribuições de usuário para vários problemas em uma lista
description: Modificar atribuições de usuário para vários problemas em uma lista
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: ac5552f1c235f595b1c0d2558fcf88b1e03f5a8e
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 1%

---

# Modificar atribuições de usuário para vários problemas em uma lista

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

Você pode modificar simultaneamente as atribuições de usuários para várias questões. Para obter informações sobre como editar problemas ou atribuí-los um de cada vez, consulte também os seguintes artigos:

* [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md)
* [Atribuir problemas](../../../manage-work/issues/manage-issues/assign-issues.md)

Para obter informações gerais sobre atribuição de problemas, consulte [Visão geral da modificação de atribuições de problemas](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md).

>[!NOTE]
>
>Você deve ter pelo menos permissões do Contribute para que um problema possa fazer atribuições a ele.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Standard</p>
   <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p> <p>Acesso de visualização ou superior aos Projetos e Tarefas para atribuir um problema</p> </td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do problema</p> <p>Ao atribuir vários problemas, contribua com permissões ou mais altas para o projeto ou tarefa em que o problema está localizado.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## Modificar atribuições para vários problemas

1. Vá para a lista de problemas que contém os problemas cujas atribuições você deseja modificar.
1. (Opcional) Crie um filtro para exibir somente problemas atribuídos ao destinatário que você deseja modificar.

   Por exemplo, você pode criar um filtro para exibir somente problemas com uma função específica como destinatário.  Em seguida, você pode substituir a função por um usuário específico. Faça o seguinte:

   1. Clique na lista suspensa **Filtros** e em **Novo filtro**.

   1. No primeiro campo, comece digitando **Funções de atribuição** e escolha **Funções de atribuição: Nome** na lista.
   1. Selecione **É qualquer um de** no menu suspenso do modificador, em seguida, comece a digitar o nome de uma função e selecione-o quando ele for exibido na lista. Você pode digitar várias funções.

      >[!TIP]
      >
      >Não use **Atribuído a** porque este campo se refere apenas ao Proprietário do problema e não a todos os atribuídos.

      A lista de problemas filtra automaticamente os critérios de filtro.
   1. (Opcional) Clique em **Salvar como novo** e depois em **Salvar**.

1. Selecione os problemas para os quais deseja modificar atribuições e clique no **ícone Editar** ![ícone Editar](assets/qs-edit-icon.png).

   O **Editar problemas** é exibido. O número de itens selecionados é exibido no canto superior esquerdo da página.

1. (Condicional) No ambiente de Produção, faça o seguinte:

   1. Vá para a seção **Atribuições** e selecione **Atribuído**.

      ![Área de atribuições](assets/classic-assignmens-area-on-edit-box-350x119.png)

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

            Se o destinatário que você deseja remover não for exibido na seção Atribuições porque o destinatário está atribuído a apenas alguns dos problemas selecionados, clique em **Remover destinatário** e comece a digitar o nome do destinatário que você deseja remover, em seguida, clique no nome quando ele aparecer na lista suspensa.

         1. Clique novamente em **Remover responsável** para adicionar outro responsável a ser removido.

      1. Para remover todos os designados existentes:

         1. Clique em **Remover todos os atribuídos existentes** e em **Sim, Excluir todos os atribuídos**.

            Isso remove não somente os atribuídos comuns (atribuídos exibidos na caixa de diálogo de edição), mas também todos os atribuídos em todas as questões selecionadas.

         1. (Opcional) Modifique qualquer uma das seguintes opções para os responsáveis selecionados para associar às ocorrências:

            * **Proprietário da Questão:** Selecione o botão de opção para indicar qual destinatário está designado como o Proprietário da Questão. Se não for selecionada, o Adobe Workfront designará o primeiro destinatário como Proprietário do problema. Isso não está disponível para atribuições de equipe.
            * **Função do destinatário**: selecione uma função na lista suspensa. Se não for selecionada, o Workfront selecionará automaticamente a função principal do usuário.

      1. Clique em **Salvar alterações**.

1. <span class="preview">No ambiente de Visualização, faça o seguinte:</span>

   1. <span class="preview">Clique em **Atribuições** no painel esquerdo e clique no ícone **x** ao lado do destinatário que você deseja remover. </span>

      >[!TIP]
      >
      ><span class="preview">Somente os atribuídos a todas as questões selecionadas são exibidos na área **Atribuições**. </span>

      ![Área de atribuições em problemas de edição em massa](assets/assignments-area-on-bulk-edit-issues.png)

   1. <span class="preview">Comece digitando o nome de um usuário, função ou equipe para adicionar atribuídos a todas as questões selecionadas. </span>

      >[!TIP]
      >
      >Você pode atribuir vários usuários, funções de trabalho ou equipes. Você pode atribuir somente usuários, funções de trabalho e equipes ativos.
      >
      >Se um usuário, função de trabalho ou equipe foi atribuído antes de ser desativado, ele permanece atribuído ao item de trabalho. Nesse caso, recomendamos o seguinte:
      >
      >* Reatribuir o item de trabalho aos recursos ativos.
      >* Associe os usuários de uma equipe desativada a uma equipe ativa e reatribua o item de trabalho à equipe ativa.

      <span class="preview">Os atribuídos adicionados são adicionados aos existentes. Elas não substituem as existentes para cada problema selecionado. </span>
   1. <span class="preview">(Opcional) Clique em **Atribuir a mim** para atribuir todos os problemas a você mesmo.</span>
   1. <span class="preview">Clique em **Salvar**. </span>




