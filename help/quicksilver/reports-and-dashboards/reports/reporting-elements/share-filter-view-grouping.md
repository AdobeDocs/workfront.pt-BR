---
product-area: reporting
navigation-topic: reporting-elements
title: Compartilhar um filtro, visualização ou agrupamento
description: É possível compartilhar filtros, visualizações e agrupamentos que você pode visualizar com outros usuários.
author: Lisa
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 8ac8981a40f051f11eef231397cd231ae1d8ddff
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 1%

---

# Compartilhar um filtro, visualização ou agrupamento

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar objetos quando eles atribuem níveis de acesso. Para obter mais informações sobre a concessão de acesso a objetos, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Juntamente com o nível de acesso que os usuários recebem, você também pode conceder a eles permissões para visualizar ou editar objetos específicos que você criou ou que tem acesso para compartilhar. Para obter mais informações sobre níveis de acesso e permissões, consulte [Como os níveis de acesso e as permissões funcionam em conjunto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

É possível compartilhar filtros, visualizações e agrupamentos que você pode visualizar com outros usuários.

Quando um filtro, visualização ou agrupamento é compartilhado com você, você pode aplicar esse filtro, visualização ou agrupamento às suas listas. Dependendo do acesso concedido a você, é possível modificá-lo e compartilhá-lo com outros usuários.

Para obter informações sobre como criar um filtro, visualização ou agrupamento, consulte os seguintes artigos:

* [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Visualizar ou obter acesso superior a Filtros, Exibições, Agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Visualizar ou aumentar permissões com acesso para compartilhar em uma exibição, filtro ou agrupamento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Compartilhar um filtro, visualização ou agrupamento

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

É possível compartilhar filtros em listas selecionadas usando as seguintes interfaces:

* Interface padrão
* Interface do criador de beta

O compartilhamento de filtros em listas selecionadas é diferente, dependendo da interface usada para compartilhar o filtro. Para obter informações sobre os tipos de interfaces de criação de filtros, consulte [Criar ou editar filtros no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Você pode compartilhar exibições e agrupamentos somente na interface padrão.

* [Compartilhamento de filtros, visualizações e agrupamentos usando a interface padrão](#share-with-standard-interface)
* [Compartilhamento de filtros usando a interface do construtor beta](#share-with-beta-builder-interface)

### Compartilhamento de filtros, visualizações e agrupamentos usando a interface padrão {#share-with-standard-interface}

O compartilhamento de filtros, visualizações e agrupamentos na interface padrão é idêntico.

1. Vá para uma lista de objetos ou um relatório.
1. (Condicional) Em uma lista, clique no botão **Filtro**, **Exibir** ou **Agrupamento** , depois passe o mouse sobre o filtro, a visualização ou o agrupamento que deseja compartilhar, clique no link **Mais** ícone ![Ícone Mais](assets/more-icon.png), em seguida **Compartilhar**.

   Em um relatório, clique no botão **Filtro**, **Exibir** ou **Agrupamento** selecione o filtro, a visualização ou o agrupamento que deseja compartilhar.

1. (Condicional) Se estiver compartilhando um relatório, clique no botão **Filtro**, **Exibir** ou **Agrupamento** menu suspenso novamente e clique em **Compartilhar filtro**, **Compartilhar Exibição** ou **Agrupamento de compartilhamento**.\
   O **Filtrar acesso**, **Ver Acesso** ou **Agrupar acesso** será exibida.

   ![Compartilhar filtro](assets/share-filter-people-box-nwe-350x458.png)

1. Conclua uma das opções a seguir, dependendo de com quem você deseja compartilhar:

   **Para compartilhar com usuários individuais, equipes, funções, grupos ou empresas:** No campo fornecido, comece a digitar o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar e clique no nome quando ele for exibido na lista suspensa.\
   Repita esse processo para compartilhar o acesso com vários usuários, equipes, funções, grupos ou empresas.

   >[!TIP]
   >
   >O compartilhamento com grupos dá permissões para filtrar, exibir ou agrupar os membros do grupo e de todos os subgrupos.


   **Para compartilhar com todos os usuários no sistema:** Clique no botão **Configurações** ícone e, em seguida, clique em **Tornar esse sistema visível**.\
   O administrador deve selecionar a opção Compartilhar todo o sistema para que essa opção esteja disponível. Para obter mais informações, consulte os artigos [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) e [Compartilhar relatórios, painéis e calendários](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Condicional) Se você estiver compartilhando com usuários individuais, equipes, funções, grupos ou empresas, clique no menu suspenso para definir o nível de acesso que deseja conceder.

   Você pode selecionar entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Visualizar o projeto</strong></td> 
      <td> <p>Selecione essa opção para permitir que os destinatários do compartilhamento usem somente o Filtro, a Exibição ou o Agrupamento compartilhado. Quando essa opção é selecionada, os recipients não podem fazer modificações no item compartilhado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gerenciar o projeto</strong></td> 
      <td> <p>Selecione esta opção para permitir que os destinatários do compartilhamento usem e modifiquem o Filtro, Exibição ou Agrupamento compartilhado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Compartilhar</strong></td> 
      <td> <p>Clique em <strong>Configurações avançadas</strong>, em seguida, selecione ou desmarque a <strong>Compartilhar</strong> , dependendo se deseja que os recipients possam compartilhar com outras pessoas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

   Os usuários com quem você compartilhou o filtro, a visualização ou o agrupamento podem acessá-lo clicando no botão **Filtro**, **Exibir** ou **Agrupamento** menu suspenso ou ícone e rolando para baixo até o **Compartilhado comigo** seção.

### Compartilhamento de filtros usando a interface do construtor beta {#share-with-beta-builder-interface}

Ao compartilhar filtros de listas de projetos, tarefas ou problemas, você pode compartilhá-los usando a interface beta builder em vez da interface padrão.

A interface do construtor beta não está disponível para nenhum outro objeto no Workfront.

Não é possível criar filtros na interface do construtor beta ao criar relatórios.

Compartilhe um filtro usando a interface do construtor beta:

1. Vá para uma lista de projetos, tarefas ou problemas.
1. Clique no botão **Filtro** ícone ![Ícone Filtro](assets/filter-nwepng.png), em seguida, ative a **Configuração beta** ![Configuração beta](assets/beta-toggle-white-on-existing-filters.png) para acessar o criador beta. Está desativado por padrão.

   Em seguida, concorde com o contrato beta, se necessário.

   Isso abre a interface do criador de filtros beta.

   >[!TIP]
   >
   >O cabeçalho da interface do construtor muda para azul quando você ativa o construtor beta. Depois de habilitar a interface do criador beta, a Workfront a mantém habilitada para todas as áreas em que está disponível.

   ![Construtor de filtros beta](assets/new-filters-all-filter-types.png)

1. Revise as seguintes listas de filtros:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Marcado como favorito</strong></td>
   <td>Filtros que você marcou como favoritos. Ao marcar um filtro como favorito, seu local original é mostrado abaixo do nome do filtro e ele fica oculto na lista original, a menos que você o remova como favorito.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Salvos</strong></td>
   <td>Filtros que você criou e salvou.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Padrões do sistema</strong></td>
   <td>Filtros padrão do sistema Workfront, bem como filtros que o administrador do Workfront adicionou à sua lista de filtros, no nível do sistema ou no modelo de layout.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Compartilhado(s) comigo</strong></td>
   <td>Filtros que outras pessoas criaram e compartilharam com você ou que são compartilhados em todo o sistema.</td>
   </tr>
   </tbody>
   </table>

1. Passe o mouse sobre um filtro que você tem acesso para pelo menos visualizar e compartilhar e clique no botão **Mais** menu ![Menu Mais](assets/more-icon-spectrum.png), depois clique em **Compartilhar**.

   ![Mais opções de menu](assets/new-filters-more-menu-options-with-delete.png)

   A caixa Compartilhamento de filtro é exibida.

1. Ative a configuração Exibir no sistema. Isso dá a qualquer pessoa no Workfront permissão para visualizar o filtro.

   >[!IMPORTANT]
   >
   >Use essa configuração com cuidado. Adicionar muitos filtros para todos os usuários desordenará a experiência do filtro e tornará os filtros mais difíceis de localizar.

   Ou comece a digitar os nomes de usuários, equipes, funções, grupos ou empresas com os quais você deseja compartilhar na **Conceder acesso a** campo.

   ![Caixa de compartilhamento de filtro](assets/new-filters-share-filter.png)

1. (Opcional) Clique na seta apontando para a direita ao lado do nome de uma entidade para editar suas permissões para o filtro e, em seguida, habilite a opção **Exibir** ou **Gerenciar** opção. **Exibir** é o padrão.

   ![Compartilhamento de permissões](assets/new-filters-sharing-permissions.png)

1. (Opcional) Ative ou desative as permissões adicionais para uma entidade seguindo um destes procedimentos:

   1. Clique em **Exibir** e desative o **Compartilhar** opção. Está ativada por padrão.
   1. Clique em **Gerenciar** e desative qualquer uma das **Compartilhar** ou **Excluir** opção. Eles são ativados por padrão.

      >[!NOTE]
      >
      >Se você habilitar Gerenciar acesso com a opção Excluir , esses usuários poderão excluir o filtro de todos os usuários, mesmo que não sejam proprietários do filtro.
   >[!TIP]
   >
   >Os usuários não podem receber uma permissão maior do que o nível de acesso. Se não tiverem acesso a Editar filtros em seu nível de acesso, não poderão receber permissões para gerenciar um filtro. O Workfront desativa a opção Gerenciar para esses usuários e a opção está esmaecida.

1. Clique em **Compartilhar**. O filtro é compartilhado com as entidades especificadas.

   >[!TIP]
   >
   >O compartilhamento com grupos dá permissões ao filtro para os membros do grupo e de todos os subgrupos.

   Os filtros compartilhados são exibidos na **Compartilhado comigo** seção do painel de filtro para essas entidades.

   ![Filtros compartilhados comigo](assets/new-filters-shared-with-me.png)

