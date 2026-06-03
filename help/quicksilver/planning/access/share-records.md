---
title: Compartilhar registros
description: Você pode compartilhar registros usando o botão Compartilhar para aumentar a colaboração no Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 9ffad1aa-3c96-40fa-9c62-7a3e00699f18
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/NTytTWD-zq3PVhXn4n-GHinvQxna1wfnAXjaeYBgTEY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c33c023ab33a3b0c8369e6fae091d0ec877aa4e2
workflow-type: tm+mt
source-wordcount: 1720
ht-degree: 2%

---

<!--update metadata with real information at release-->

# Compartilhar registros

<!--
this will NOT be available in Preview ever - find a way to add this in this article that is prominent
-->

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>\
<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Você pode ajustar as permissões das pessoas para registros individuais em um tipo de registro no Adobe Workfront Planning.

Você pode compartilhar um registro do Adobe Workfront Planning das seguintes maneiras:

* Compartilhar um link para o registro.

  Para obter mais informações, consulte [Compartilhar registros usando um link](/help/quicksilver/planning/records/share-records.md).

* Compartilhe todos os registros em um espaço de trabalho com outros usuários compartilhando o espaço de trabalho e o tipo de registro.

  Para obter mais informações, consulte os seguintes artigos:

   * [Compartilhar um espaço de trabalho](/help/quicksilver/planning/access/share-workspaces.md)

   * [Compartilhar um tipo de registro](/help/quicksilver/planning/access/share-record-types.md)

* Compartilhe um registro individual ou compartilhe vários registros em massa usando a opção **Compartilhar**.

  Este artigo descreve como compartilhar registros com outras pessoas usando a opção **Compartilhar**.

>[!IMPORTANT]
>
>* Os usuários com acesso a um espaço de trabalho obtêm automaticamente pelo menos permissões de Exibição para todos os registros no espaço de trabalho.
>* O compartilhamento de exibições não concede aos usuários permissões para registros. Somente espaços de trabalho de compartilhamento podem conceder aos usuários permissões para tipos de registro e registros.
>
>Para obter informações gerais sobre o compartilhamento de objetos no Workfront Planning, consulte também [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e do Planning</p> 
Ou
<p>Qualquer pacote de Fluxo de Trabalho e Planejamento</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Qualquer</p> 
   <p><b>Nota</b></p>
   <p>Somente pessoas com uma licença Standard podem receber permissões de Gerenciamento para registros. Todas as outras licenças só podem ter permissões de Exibição e a opção Gerenciar está esmaecida para elas.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>  <p>Gerenciar permissões para um espaço de trabalho, um tipo de registro e o registro</p>  
   <p><b>IMPORTANTE</b></p>
   <p>Somente usuários com permissões para Gerenciar um espaço de trabalho podem compartilhar um registro</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> Os usuários com uma licença Light ou Contributor devem receber um modelo de layout que inclua o Planning.
   <p>Usuários padrão e Administradores do sistema têm as áreas do Planning habilitadas por padrão.</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações ao compartilhar registros

<!--
maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information
-->

<!--checking on the below with Lilit-->

* Você pode compartilhar registros com as seguintes entidades: pessoas, grupos, equipes, empresas ou funções de trabalho.
* Se você restringir permissões a um registro, os usuários não visualizarão mais esse registro e os valores de seus campos de pesquisa em nenhum lugar no sistema em que esse registro for exibido.
* O Workfront verifica as permissões de registro em conexões de até 5 registros de profundidade, garantindo que os usuários vejam apenas os registros compartilhados com eles.
* Você pode conceder os seguintes níveis de permissões a um registro:

   * Exibir
   * Gerenciar
* Quando você compartilha um espaço de trabalho e um tipo de registro com usuários, eles também recebem as mesmas permissões para os registros no espaço de trabalho, por padrão.
Quando os usuários têm permissões do Contribute para um espaço de trabalho ou tipo de registro, eles recebem permissões de gerenciamento para os registros desse tipo de registro.
* Quando você remove uma entidade de um espaço de trabalho, todas as permissões de compartilhamento são removidas dos tipos de registro e de todos os registros nele.
* Não é possível compartilhar um registro com um usuário que não tem permissões para o espaço de trabalho ou o tipo de registro.

  Se você compartilhar um registro com alguém que não esteja no espaço de trabalho, ele será adicionado automaticamente ao espaço de trabalho.
* O acesso de um usuário ao registro é determinado por meio da combinação das três configurações a seguir:

   * Suas permissões herdadas do tipo de registro e do espaço de trabalho
   * Permissões adicionadas individualmente na caixa de compartilhamento de registros
   * A configuração **Todos no espaço de trabalho podem exibir**.

     Isso torna o registro visível para todos no espaço de trabalho

     <!--
      Cannot do this on a record: 
      * **Only invited people can access**: This is selected by default and allows restricting access to the record to specific people. 
      -->

* Quando você compartilha um registro com um usuário, ele é adicionado com a mesma permissão que tem no tipo de registro, por padrão.

  Por exemplo:

   * Se tiverem permissões de Exibição para o tipo de registro, eles obterão permissões de Exibição para o registro
   * Se tiverem permissões do Contribute ou do Manage para o tipo de registro, eles obterão permissões do Manage para o registro

* Quando um usuário tem permissões de Gerenciar ou Contribuir para o espaço de trabalho e o tipo de registro e você os adiciona às permissões de registro, as permissões de Exibição ficam esmaecidas. Eles retêm as mesmas permissões para o registro que têm para o tipo de registro e não é possível conceder a eles permissões mais baixas para o registro.

* Você pode desabilitar permissões herdadas para um único registro, nesse caso, você pode conceder permissões a usuários selecionados para registros individuais, ou eles podem obter permissões se pertencerem ao espaço de trabalho, devido à opção **Todos no espaço de trabalho podem exibir**.

* Se várias permissões de compartilhamento se aplicarem ao mesmo usuário, ele receberá o nível mais alto dessas permissões.

  Por exemplo, se um registro for compartilhado com um usuário com permissões de Exibição e seu grupo com acesso de Gerenciamento, ele receberá permissões de Gerenciamento para o registro.

* Se um campo de fórmula ou um campo de pesquisa de um registro conectado for baseado em um campo em um registro no qual você não tem permissões, você verá o cálculo correto de quais fatores no registro não poderão ser acessados de outra forma.

  <!--
   Not possible: 
   * As a workspace manager, you can share a record with a user that does not have permissions to the record type or the workspace. In this case, there is a warning next to the added entity notifying you that they don't have access to the workspace or the record type.  You can continue adding the user to the record which will also add them to the record type and workspace, or cancel the sharing.
   -->

  <!--
   ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too
   -->

<!--
Lilit is checking on this, it is not working correctly
-->

<!--
   check on this: I cannot disable inherited permissions when this setting is ON and this documented in a TIP below: When they have View permissions to the workspace or the record type, they retain View permissions to the records. You can grant them Manage permissions to the record by disabling Inherited permissions and selecting the Only invited people can access setting.
   -->

<!-- 
   not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.
   -->

<!--
   Too granular??
   If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 
   If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions 
   -->

<!--
   not sure if any of the Share record types points might match here - ask Lilit??
   -->

## Compartilhar registros

Como gerenciador de espaço de trabalho, você pode ajustar permissões para registros individuais.

{{step1-to-planning}}

1. Abra o espaço de trabalho e o tipo de registro cujos registros você deseja compartilhar.

1. Siga um destes procedimentos:

   * Na exibição de tabela, passe o mouse sobre o nome de um registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Compartilhar**.
   * Na exibição de tabela, selecione um ou vários registros e clique em **Compartilhar** na barra de ferramentas azul na parte inferior da lista.
   * Em qualquer exibição, clique no nome de um registro e em **Compartilhar** no canto superior direito da página de detalhes do registro.

   A caixa **Compartilhar** é aberta.

   ![Permissões para registros com permissões herdadas em](assets/permissions-for-records-with-inherited-permissions-on.png)

   >[!WARNING]
   >
   >Não é possível compartilhar permissões para registros adicionados em espaços de trabalho diferentes. Quando você compartilha registros em massa, todos os registros devem ser criados no mesmo espaço de trabalho.

1. (Opcional) Na área **Quem tem acesso**, a opção **Todos os usuários do espaço de trabalho podem visualizar** é selecionada por padrão.  Todos os usuários com permissões de **Exibição** ou superior para o espaço de trabalho e o tipo de registro têm as mesmas permissões para o registro.

1. (Opcional) Clique nos avatares dos usuários na opção **Permissões herdadas de** para exibir usuários, equipes, grupos, empresas ou funções de trabalho que herdam permissões do espaço de trabalho. <!--logged bug to move "Permissions" to lowercase-->

   As permissões do usuário para o tipo de registro são exibidas ao expandir as permissões herdadas.

   >[!TIP]
   >
   >Não é possível remover entidades individuais da lista de permissões herdadas. Os usuários de equipes, grupos, empresas ou funções de trabalho são listados em vez das entidades às quais estavam associados quando o espaço de trabalho e o tipo de registro foram compartilhados com eles.

1. (Opcional e condicional) Se quiser compartilhar o registro com entidades específicas e conceder a elas um acesso diferente ao tipo de registro do que já têm para o espaço de trabalho, faça o seguinte:

   1. Desmarque a opção **Ativado** de **Permissões herdadas**. Ela é selecionada por padrão.

      A opção muda para **Desativada**.

      >[!TIP]
      >
      >Os gerentes e criadores de registros do Workspace continuam a ter permissões de gerenciamento para o tipo de registro e o registro.

      <!-- 
      This is no longer possible for a record: 
      (Optional) Select **Only invited people can access** from the **Who has access** area. You must indicate individual users, groups, teams, or companies to share the records with. 
      >[!TIP]
      >
      >You cannot disable or enable Inherited permissions when this setting is selected.
      -->

   1. No campo **Conceder acesso a este registro**, adicione os usuários, equipes, grupos, empresas ou funções de trabalho aos quais você deseja conceder um nível de permissão diferente daquele que eles têm para o espaço de trabalho ou tipo de registro.

      Quando você compartilha um registro com um usuário, sua função de trabalho principal e seu email também são exibidos no campo. Você deve ter a configuração Exibir informações de contato ativada para que o objeto Usuários em seu nível de acesso possa exibir o email do usuário.

   1. Escolha um dos seguintes níveis de permissão:

      * Exibir
      * Gerenciar

      >[!IMPORTANT]
      >
      >* Se os usuários tiverem permissões do Contribute ou do Manage para o espaço de trabalho e o tipo de registro, você poderá conceder a eles permissões de Manage para o registro. A permissão Exibir fica esmaecida.
      >* Você não pode conceder aos usuários uma permissão menor para o registro se eles tiverem o Contribute ou superior ao tipo de registro.
      >Para obter mais informações, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
      >* Não é possível conceder permissões a usuários que não estão no espaço de trabalho. Os usuários que não têm permissões para o espaço de trabalho e o tipo de registro não podem acessar nenhum dos registros.

   <!--   
   Not possible:
   1. To give users who do not have permissions to the workspace access to view a record, in the **Grant access to this view** field, start typing the name of a user, a group, team, company, or job role, then click it when it displays in the list. 
      The entity you selected is added to the record and also to the record type and the workspace with **View** permissions. 
      System administrators always receive Manage permissions to records shared with them, and there is an indication that a user is a System administrator.
   -->

1. (Opcional) Clique em **Copiar link** para copiar um link para o registro na área de transferência e compartilhá-lo com outras pessoas. O link abrirá a página de detalhes do registro.
1. Clique em **Salvar**.

   O registro agora é compartilhado com outros usuários.

   Os usuários com os quais você compartilhou o registro recebem uma notificação no aplicativo e por email sobre a obtenção de permissões para o registro.

   <!--
   not possible anymore: 
   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them.
   -->

   Para obter informações, consulte [Notificações do Adobe Workfront Planning: índice do artigo](/help/quicksilver/planning/notifications/notifications-information.md).


1. (Opcional) Compartilhe o link copiado com outras pessoas.

   Os usuários que recebem o link devem ser usuários ativos e fazer logon no Workfront para acessar a página de tipo de registro e exibi-la na exibição selecionada.

   Eles devem ter permissões no tipo de registro para poder visualizá-lo.

   Para obter mais informações, consulte também [Compartilhar registros usando um link](/help/quicksilver/planning/records/share-records.md).


## Remover permissões para um registro

É possível remover permissões de usuários de um registro. No entanto, eles manterão pelo menos permissões de Exibição no espaço de trabalho, o que também lhes dará pelo menos permissões de Exibição para o tipo de registro.

Você deve remover o acesso deles do espaço de trabalho se quiser que eles não tenham permissões para os tipos de registros ou registros no espaço de trabalho.

Não é possível remover um usuário de permissões herdadas.

{{step1-to-planning}}

1. Abra o espaço de trabalho cujos registros deseja interromper o compartilhamento e clique em um cartão de tipo de registro. Isso abre a página do tipo de registro.
1. Siga um destes procedimentos:

   * Na exibição de tabela, passe o mouse sobre o nome de um registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Compartilhar**.
   * Na exibição de tabela, selecione um ou vários registros e clique em **Compartilhar** na barra de ferramentas azul na parte inferior da lista.

     Você deve selecionar registros criados no mesmo espaço de trabalho.
   * Em qualquer exibição, clique no nome de um registro e em **Compartilhar** no canto superior direito da página de detalhes do registro.

   A caixa **Compartilhar** é aberta.
1. Localize o usuário, grupo, equipe, empresa ou função de trabalho cujas permissões você deseja remover, expanda o menu suspenso de permissões à direita de seu nome e clique em **Remover**.

   ![Remover permissões no registro](assets/remove-option-on-record-sharing-drop-down.png)

1. Clique em **Salvar**.

   As pessoas não têm mais as permissões indicadas para o registro. No entanto, eles ainda têm permissões para o tipo de registro e o espaço de trabalho, a menos que você também os remova dessas permissões.

   Não há notificação para os usuários que foram removidos do acesso ao registro de que eles não têm mais essas permissões.
