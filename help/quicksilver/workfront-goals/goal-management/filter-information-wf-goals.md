---
product-previous: workfront-goals
navigation-topic: goal-management
title: Filtrar informações em metas do Adobe Workfront
description: É possível visualizar metas que você ou qualquer outra pessoa adicionou às Metas da Adobe Workfront. Para obter informações sobre como criar metas, consulte Criar metas em Metas da Adobe Workfront. Ao visualizar metas, você pode filtrar informações nas Metas da Workfront para visualizar somente as metas que são importantes para você.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 2%

---

# Filtrar informações em metas do Adobe Workfront

É possível visualizar metas que você ou qualquer outra pessoa adicionou às Metas da Adobe Workfront. Para obter informações sobre como criar metas, consulte [Criar metas nas metas da Adobe Workfront](../../workfront-goals/goal-management/create-goals.md). Ao visualizar metas, você pode filtrar informações nas Metas da Workfront para visualizar somente as metas que são importantes para você.

## Requisitos de acesso

<!--drafted - replace the table below with this one when P&P releases: 

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

Você deve ter o seguinte acesso para executar as ações descritas neste artigo:

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
   <td role="rowheader">Nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso às metas</p> <p><b>Nota</b>

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
     <p>Visualizar ou aumentar permissões em metas</p> 
     <p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta na Workfront</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve ter o seguinte antes de começar:

* Um modelo de layout que inclui a área Metas no Menu principal.

## Visão geral dos filtros nas Metas do Workfront

>[!NOTE]
>
>Para encontrar e se concentrar eficientemente nas metas certas, recomendamos que você use filtros nas Metas do Workfront. Isso permite exibir as informações corretas antes de começar a gerenciar metas importantes para você. Por padrão, as Metas do Workfront exibem todas as metas no sistema.

Localize e filtre as metas nas seguintes seções da área de Metas no Workfront:

* Lista de metas
* Gráficos
* Alinhamento de metas

Para obter informações sobre as seções da área Metas , consulte [Visão geral das seções Metas da Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>Você pode configurar filtros para uma seção e eles permanecem persistentes ao mudar para outra seção das Metas do Workfront.

Considere o seguinte ao trabalhar com filtros nas Metas do Workfront:

* Você pode criar e aplicar um filtro sem salvá-lo ou salvar um filtro para reutilização posteriormente.

   Os seguintes cenários existem:

   * Ao salvar um filtro, ele se torna o filtro padrão para você sempre que fizer logon no Workfront Metas.
   * Ao aplicar um filtro sem salvá-lo, você pode reverter para as listas originais atualizando sua página.

* Você só pode exibir e aplicar os filtros criados. Os filtros criados por outros usuários são exibidos somente para esses usuários.
* Não é possível compartilhar filtros criados com outros usuários.

## Aplicar um filtro rápido nas Metas do Workfront

Você pode usar um filtro rápido em uma lista de metas para ajudar a localizar apenas itens importantes para você. Não é possível salvar filtros rápidos e eles não são persistentes. O Workfront limpa os resultados de um filtro rápido quando você atualiza a página.

Para obter mais informações, consulte [Aplicar o filtro rápido a uma lista](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Criar e aplicar um filtro nas Metas do Workfront

O processo para criar filtros é o mesmo para qualquer seção das Metas do Workfront.

Você pode criar um filtro do zero ou editar um dos filtros incorporados.

1. Acesse as Metas da Workfront.

   Para obter informações sobre como acessar as Metas da Workfront, consulte [Acessar e abrir metas em metas na Adobe Workfront](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   Por padrão, a seção Lista de metas é exibida.

1. Clique em **Filtro** no canto superior direito da lista.

   ![](assets/filter-icon-and-label.png)

   Por padrão, o Workfront aplica a variável **Todos** filtro que exibe todas as metas em seu sistema.

   >[!TIP]
   >
   >Não é possível editar ou excluir o filtro Tudo .

1. Siga um destes procedimentos:

   * Clique em qualquer um dos filtros predefinidos a seguir para exibir metas somente para os seguintes proprietários:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>Todas</td> 
        <td> <p>Todas as metas em seu sistema, independentemente de quem as criou, qual é o período de tempo ou quem é o proprietário. Este é o filtro padrão e não pode editá-lo. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>Pessoal</td> 
        <td>As metas para as quais você é o proprietário.</td> 
       </tr> 
       <tr> 
        <td>Minhas equipes</td> 
        <td> <p>As metas para as quais qualquer uma de suas equipes é selecionada como proprietário. </p> <p><b>DICA</b>

      Nenhuma meta é exibida quando você não está atribuído a nenhuma equipe. </p> </td>
      </tr> 
       <tr> 
        <td>Meus grupos</td> 
        <td>As metas para as quais qualquer um dos seus grupos é selecionado como o proprietário. </td> 
       </tr> 
       <tr> 
        <td>Empresa</td> 
        <td> <p>As metas associadas à sua organização. </p> <p><b>DICA</b>
        <p>Nas Metas da Adobe Workfront, o filtro Empresa exibe as metas para as quais sua organização está selecionada como proprietária. </p> <p>Não é possível pesquisar empresas usando esse campo. Somente sua organização, que é a proprietária da instância do Workfront, é selecionada por padrão. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * Passe o mouse sobre o nome de um filtro, em seguida, clique no botão **Editar** ícone ![](assets/edit-icon.png) ao lado do nome para personalizá-lo e adicionar nomes específicos de usuários, equipes, grupos ou o nome de sua organização, em seguida, selecione-o quando eles forem exibidos na lista.

   * Clique em **Novo filtro** para criar um novo filtro, selecione uma das seguintes opções para personalizar o novo filtro:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Período</td> 
        <td>Selecione um período de tempo no menu suspenso. Você pode selecionar vários períodos. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Status</td> 
        <td> <p>Selecione um status no menu suspenso das seguintes opções:</p> 
         <ul> 
          <li> <p>Ativo</p> </li> 
          <li> <p>Rascunho</p> </li> 
          <li> <p>Inativo</p> </li> 
          <li> <p>Fechado</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Progresso</td> 
        <td> <p>Selecione um progresso no menu suspenso das seguintes opções: </p> 
         <ul> 
          <li> <p>Com problemas</p> </li> 
          <li> <p>Em Risco</p> </li> 
          <li> <p>No Prazo</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Proprietário</td> 
        <td> <p>Comece a digitar o nome de um proprietário e selecione-o quando ele aparecer na lista. </p> <p>Você pode digitar os nomes de usuários, equipes, grupos ou o nome de sua organização, ou pode selecionar a partir de opções predefinidas. </p> <p>As opções de filtro predefinidas a seguir sempre se referem ao usuário que está conectado no momento: </p> 
         <ul> 
          <li> <p><strong>Me</strong>: Exibe metas onde você é o proprietário.</p> </li> 
          <li> <p><strong>Minha Equipe Inicial</strong> e <strong>Todas as Minhas Equipes</strong>: Exibe metas onde sua Equipe inicial ou qualquer uma de suas equipes são designadas como o proprietário. </p> <p>Dica: Nenhuma meta é exibida quando você não está atribuído a nenhuma equipe. </p> </li> 
          <li> <p><strong>Meu Grupo Doméstico</strong> e <strong>Todos os Meus Grupos</strong>: Exibe metas em que seu Grupo doméstico ou qualquer um dos seus grupos são designados como proprietários.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (Opcional) Clique em **Redefinir** no canto inferior direito da caixa de filtro para limpar todos os campos selecionados e começar a criar o filtro do zero.
1. (Opcional) Clique em **Aplicar** para aplicar o filtro sem salvar.

   O filtro é exibido no **Não salvo** área do construtor de filtros como **Novo filtro**.

   Não é possível renomear um filtro não salvo.

   Filtros não salvos serão removidos da área Metas na próxima vez que você sair do Workfront e fazer logon novamente.

   >[!TIP]
   >
   >Você pode ter apenas um Novo Filtro não salvo de uma vez.

1. Clique em **Salvar** para salvar o filtro e usá-lo posteriormente, adicione um nome para o filtro no **Adicionar nome de filtro** e clique em **Concluído**.

   Isso salva o filtro no **Salvo** seção do construtor de filtros. Você pode usar esse filtro no futuro.

   O último filtro salvo e aplicado é exibido por padrão na próxima vez que você fizer logon novamente no Workfront

1. (Opcional) Clique no botão **seta apontando para a esquerda** ao lado de **Novo filtro** para sair do construtor de filtros e retornar à lista de filtros.
1. (Opcional) Passe o mouse sobre o nome de um filtro personalizado, clique no botão **Mais** , em seguida, clique em **Excluir**, em seguida **Excluir**. Isso exclui o filtro e não é possível recuperá-lo.

   >[!TIP]
   >
   >Não é possível excluir nenhum dos filtros predefinidos.

1. Clique no botão **Ícone X** no canto superior direito do construtor de filtros para fechar o construtor de filtros.

   O nome do filtro aplicado no momento é exibido à direita do ícone Filtro , no canto superior direito da lista de metas.

   A lista de metas é filtrada pelos critérios do filtro.

1. (Opcional e condicional) Ao exibir metas na seção Alinhamento da meta , clique em **Mostrar** se quiser exibir as metas filtradas.

   ![](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   O nome do filtro é contornado em amarelo para indicar que está sendo ignorado.

   ![](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (Opcional e condicional) Clique em **Reaplicar filtro** para aplicar o filtro e omitir os itens exibidos na etapa anterior.


