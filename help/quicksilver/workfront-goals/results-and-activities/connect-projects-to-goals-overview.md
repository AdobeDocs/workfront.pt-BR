---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adicionar projetos às metas em Metas da Adobe Workfront
description: Você pode conectar projetos a metas para indicar como a meta progride, com base no progresso real do projeto. O projeto se torna um indicador de progresso para a meta.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# Adicionar projetos às metas em Metas da Adobe Workfront

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Você pode conectar projetos a metas para indicar como a meta progride, com base no progresso real do projeto. O projeto se torna um indicador de progresso para a meta.

Ao conectar projetos a metas, você pode vincular o planejamento estratégico (metas) de sua organização ao trabalho real que suas pessoas estão realizando e concluindo todos os dias (projetos).

>[!IMPORTANT]
>
>As metas a nível de projeto criadas na área Caso de negócios de um projeto não estão vinculadas às metas estratégicas criadas na Workfront Metas. Para obter informações sobre as metas do projeto de Caso de Negócios, consulte [Criar metas de caso de negócios](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Requisitos de acesso

<!--drafted for P&P release: replace the table below with this: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
  </tr>
 </tbody>
</table>

-->
Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Visão geral das licenças do Adobe Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td> <p>Você deve comprar uma licença adicional para a funcionalidade Metas da Adobe Workfront para acessar descrita neste artigo. </p> <p>Para obter mais informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as metas do Workfront</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar o acesso às Metas</p> <p><b>Nota</b>

<p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Conceder acesso às Metas da Adobe Workfront</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> 
    <div> 
     <p>Gerenciar permissões para a meta</p> 
     <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta na Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

Para obter informações adicionais sobre o acesso às Metas da Workfront, consulte [Requisitos para usar as metas do Workfront](../goal-management/access-needed-for-wf-goals.md).

## Considerações sobre a conexão de projetos a metas

* Você pode adicionar um projeto que atenda aos seguintes critérios para uma meta:

   * Você deve ter pelo menos permissões para exibi-lo.

      >[!NOTE]
      >
      >Se você perder as permissões para visualizar o projeto depois de anexá-lo à meta, ainda poderá ver as informações do projeto sobre a meta, mas não poderá mais acessá-lo.

   * O projeto não deve estar em um status de inativo.

* Você pode associar vários projetos com uma meta.
* Você pode associar o mesmo projeto a várias metas.
* Não é possível atualizar manualmente o progresso de um projeto a partir da meta à qual o projeto está anexado. Em vez disso, o Workfront calcula a porcentagem completa do projeto e o Workfront Metas calcula o progresso da meta usando essa porcentagem concluída. Isso atualiza a meta em tempo real depois que a porcentagem do projeto é atualizada.
* A duração do projeto pode estar fora do período de uma meta. Se um projeto durar mais do que o prazo final da meta, você ainda poderá fechar sua meta e considerá-la concluída, mas a porcentagem da meta concluída não será de 100%. A porcentagem completa do projeto não é mais atualizada na meta.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Quando você exclui um projeto anexado a uma meta, o projeto também é excluído dessa meta.

   >[!CAUTION]
   >
   >Se a meta estava ativa antes de excluir o projeto e não há outros indicadores de progresso na meta, a meta fica Inativa.


## Adicionar projetos às metas

1. Clique no botão **Menu principal** ![](assets/main-menu-icon.png) (Escreva isso para a Shell: ou clique no botão **Menu principal** ![](assets/three-line-main-menu-icon.png) no canto superior esquerdo, se estiver disponível.) , **Metas**.
1. Na Lista de metas, clique no nome de uma meta para abrir a página de meta.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. No **Novo indicador de progresso** , clique em **Adicionar projeto existente**.

   A caixa Adicionar projetos à meta é exibida.
1. (Opcional) Atualize o **Exibir**, **Filtro** ou **Agrupamento** clicando nos respectivos ícones no canto superior direito da lista para modificar a forma como a lista de projetos é exibida.
1. (Opcional) Clique no botão **Pesquisar** ícone ![](assets/search-icon.png) e comece a digitar o nome de um projeto para encontrá-lo rapidamente na lista.
1. Selecione os projetos que deseja adicionar à meta e clique em **Adicionar**.

   Os projetos selecionados são adicionados à meta e são exibidos na seção Indicadores de progresso da página de meta, em **Projeto** agrupamento.

   Após ativar a meta, o progresso da meta é atualizado automaticamente quando o progresso de um projeto é atualizado. Para obter informações sobre como ativar uma meta, consulte [Ativar metas nas metas da Adobe Workfront](../goal-management/activate-goals.md).

## Localizar informações do projeto sobre metas

<p>
As seguintes informações do projeto estão visíveis no nível da meta na seção Indicadores de progresso da página de uma meta:

</p>

<table>
  <tr>
   <td>Nome do Projeto
   </td>
   <td>Todas as alterações no nome do projeto também refletem no projeto ligado.
   </td>
  </tr>
  <tr>
   <td>Proprietário do projeto
   </td>
   <td>Todas as alterações no proprietário do projeto também refletem no projeto ligado.
   </td>
  </tr>
    <tr>
   <td>Progresso real
   </td>
   <td> <p>A porcentagem completa do projeto. Não é possível atualizar manualmente a porcentagem de projeto concluída a partir da meta. O Workfront automaticamente o calcula com base na porcentagem completa das tarefas. </p>
   </td>
  </tr>
  <tr>
   <td>Progresso
   </td>
   <td>A porcentagem completa do projeto representada por uma barra. Qualquer alteração na porcentagem completa do projeto atualiza automaticamente o progresso da meta, a menos que a meta seja fechada.
   </td>
  </tr>

</table>

## Localizar informações de meta em projetos

As seguintes informações de meta estão visíveis em uma lista de projetos ou relatório:

| Informações sobre a meta | Descrição |
|---|---|
| Metas | Uma lista de todas as metas que têm um projeto associado a elas. |
| Hierarquia de Meta | A hierarquia à qual uma meta pertence. Somente os pais da meta e da meta são exibidos neste campo. As metas secundárias não são exibidas. |
| Número de metas vinculadas | O número de metas vinculadas a um projeto. |
