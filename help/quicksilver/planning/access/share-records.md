---
title: Compartilhar registros
description: Você pode compartilhar registros usando o botão Compartilhar para aumentar a colaboração no Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 66dd7354f3723e266b77cb2f367b09c022e8c95e
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# Compartilhar registros

<!--this will NOT be available in Preview ever - find a way to add this in this article that is prominent-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Você pode ajustar as permissões das pessoas para registros individuais em um tipo de registro.

Você pode compartilhar um registro do Adobe Workfront Planning das seguintes maneiras:

* Compartilhar um link para o registro.

  Para obter mais informações, consulte [Compartilhar registros usando um link](/help/quicksilver/planning/records/share-records.md).

* Compartilhe todos os registros em um espaço de trabalho com outros usuários compartilhando o espaço de trabalho e o tipo de registro.

  Para obter mais informações, consulte os seguintes artigos:

   * [Compartilhar um espaço de trabalho](/help/quicksilver/planning/access/share-workspaces.md)

   * [Compartilhar um tipo de registro](/help/quicksilver/planning/access/share-record-types.md)

* Compartilhar um registro usando a opção **Compartilhar**.

  Este artigo descreve como compartilhar um registro com outras pessoas usando a opção **Compartilhar**.

>[!IMPORTANT]
>
>Os usuários com acesso a um espaço de trabalho obtêm automaticamente pelo menos permissões de Exibição para todos os registros no espaço de trabalho.
>O compartilhamento de exibições não concede aos usuários permissões para registros. Somente espaços de trabalho de compartilhamento podem conceder aos usuários permissões para tipos de registro e registros.
>
>Para obter informações gerais sobre o compartilhamento de objetos no Workfront Planning, consulte também [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
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

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações ao compartilhar registros

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* Você pode compartilhar registros com as seguintes entidades: pessoas, grupos, equipes, empresas ou funções de trabalho.
* Quando você compartilha um registro, os usuários têm o mesmo acesso em qualquer lugar onde esse registro aparece no sistema.
* Se você restringir permissões a um registro, os usuários não visualizarão mais esse registro e os valores de seus campos de pesquisa em nenhum lugar no sistema em que esse registro for adicionado.
* O Workfront verifica as permissões de registro em conexões de até 5 registros de profundidade, garantindo que os usuários vejam apenas os registros compartilhados com eles.
* Você pode conceder os seguintes níveis de permissões a um registro:

   * Exibir
   * Gerenciar
* Quando você compartilha um espaço de trabalho e um tipo de registro com usuários, eles também recebem as mesmas permissões para os registros no espaço de trabalho, por padrão.
Quando os usuários têm permissões do Contribute para um espaço de trabalho ou tipo de registro, eles recebem permissões de gerenciamento para os registros desse tipo de registro.
* Quando você remove uma entidade de um espaço de trabalho, todas as permissões de compartilhamento são removidas dos tipos de registro e de todos os registros nele.
* O acesso de um usuário ao registro é determinado por meio da combinação das três configurações a seguir:

   * Suas permissões herdadas do tipo de registro e do espaço de trabalho
   * Permissões adicionadas individualmente na caixa de diálogo de compartilhamento de registros
   * As seguintes permissões:

      * **Todos no espaço de trabalho podem exibir**: isso torna o registro visível para todos no espaço de trabalho <!-- is this OK to say "workspace? should it be "record"??-->
      * **Somente pessoas convidadas podem acessar**: esta opção é selecionada por padrão e permite restringir o acesso ao registro a pessoas específicas.

     >[!NOTE]
     >
     >Se você optar por conceder a **Todos no espaço de trabalho podem exibir a permissão** para um tipo de registro ou um registro, todos os usuários listados na lista de compartilhamento das permissões do espaço de trabalho terão as mesmas permissões no tipo de registro e no registro, mesmo quando as permissões herdadas estiverem desabilitadas.


* Quando você compartilha um registro com um usuário, ele é adicionado com a mesma permissão que tem no tipo de registro, por padrão.

  Por exemplo:

   * Se tiverem permissões de Exibição para o tipo de registro, eles obterão permissões de Exibição para o registro
   * Se tiverem permissões do Contribute ou do Manage para o tipo de registro, eles obterão permissões do Manage para o registro

* Como gerenciador de espaço de trabalho, você pode compartilhar um registro com um usuário que não tem permissões para o tipo de registro ou o espaço de trabalho. Nesse caso, há um aviso ao lado da entidade adicionada notificando que ela não tem acesso ao espaço de trabalho ou ao tipo de registro. <!--ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too--> Você pode continuar adicionando o usuário ao registro, o que também o adicionará ao tipo de registro e espaço de trabalho, ou cancelar o compartilhamento.

* Quando um usuário tem permissões de Gerenciar ou Contribuir para o espaço de trabalho e o tipo de registro e você os adiciona às permissões de registro, as permissões de Exibição ficam esmaecidas. Eles retêm as mesmas permissões para o registro que têm para o tipo de registro e não é possível conceder a eles permissões mais baixas para o registro. <!--Lilit is checking on this, it is not working correctly-->

  Quando eles têm permissões de Exibição para o espaço de trabalho ou o tipo de registro, eles retêm permissões de Exibição para os registros. Você pode conceder a eles permissões Gerenciar para o registro ao desabilitar Permissões herdadas e selecionar a configuração Somente pessoas convidadas podem acessar. <!-- I think this is right, but because of the above not working, I can't test-->

<!-- not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.-->

* Você pode desabilitar permissões herdadas para um único registro. Nesse caso, você pode conceder a eles permissões para registros individuais ou eles podem obter permissões se pertencerem à opção **Todos no espaço de trabalho podem exibir**.

* Se várias permissões de compartilhamento se aplicarem ao mesmo usuário, ele receberá a maior permissão dessas permissões.

  Por exemplo, se um registro é compartilhado com um usuário com permissões de Exibição e seu grupo com acesso de Gerenciamento, ele obtém permissões de Gerenciamento para o registro.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Se um campo de fórmula ou um campo de pesquisa de um registro conectado for baseado em um campo em um registro no qual você não tem permissões, você verá o cálculo correto de quais fatores no registro não poderão ser acessados de outra forma.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Compartilhar permissões de registro

Como gerenciador de espaço de trabalho, você pode ajustar permissões para registros individuais.

{{step1-to-planning}}

1. Abra o espaço de trabalho cujos registros você deseja compartilhar.
1. Clique no tipo cujos registros você deseja compartilhar.

1. Siga um destes procedimentos:

   * Na exibição de tabela, passe o mouse sobre o nome de um registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Compartilhar**.
   * Na exibição de tabela, selecione um registro e clique em **Compartilhar** na barra de ferramentas azul na parte inferior da lista.
   * Em qualquer exibição, clique no nome de um registro e em **Compartilhar** no canto superior direito da página de detalhes do registro.

   A caixa **Compartilhar** é aberta.

   ![Permissões para registros com permissões herdadas em](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Opcional) Na área **Quem tem acesso**, a opção **Todos os usuários do espaço de trabalho podem visualizar** é selecionada por padrão.  Todos os usuários com permissões de **Exibição** ou superior para o espaço de trabalho e o tipo de registro têm as mesmas permissões para o registro.

1. (Opcional) Clique no número de usuários na opção **Permissões herdadas** para exibir usuários, equipes, grupos, empresas ou funções de trabalho que herdam permissões do espaço de trabalho.

   >[!TIP]
   >
   >Não é possível remover entidades individuais da lista de permissões herdadas.

1. (Opcional e condicional) Se quiser compartilhar o registro com entidades específicas e conceder a elas um acesso diferente ao tipo de registro do que já têm para o espaço de trabalho, faça o seguinte:

   1. Selecione **Desabilitar** no menu suspenso **Permissões herdadas**.

   >[!TIP]
   >
   >Os gerentes do Workspace continuam a ter permissões de gerenciamento para o tipo de registro e o registro.

   1. (Opcional) Selecione **Somente pessoas convidadas podem acessar** da área **Quem tem acesso**.

   1. No campo **Conceder acesso a este tipo de registro**, adicione os usuários, equipes, grupos, empresas ou funções de trabalho aos quais você deseja conceder um nível de permissão diferente daquele que eles têm para o espaço de trabalho ou tipo de registro.
   1. Escolha um dos seguintes níveis de permissão:

      * Exibir
      * Gerenciar

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* Além de equipes, grupos, empresas e funções de trabalho, você pode compartilhar somente com usuários que foram adicionados à Adobe Admin Console. Não é possível adicionar usuários somente do Workfront. Para obter informações, consulte [Gerenciar usuários na Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >* Se os usuários tiverem permissões do Contribute ou do Manage para o espaço de trabalho e o tipo de registro, eles manterão permissões do Manage para o registro. A permissão Exibir fica esmaecida. <!--this is not dimmed at this time, Lilit to check-->
   >* Você não pode conceder aos usuários uma permissão menor para o registro se eles tiverem o Contribute ou superior ao tipo de registro.
   > Para obter mais informações, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Para conceder aos usuários que não têm permissões para o espaço de trabalho acesso para exibir um registro, no campo **Conceder acesso a este modo de exibição**, comece digitando o nome de um usuário, grupo, equipe, empresa ou função de trabalho e, em seguida, clique nele quando ele for exibido na lista.

   A entidade selecionada é adicionada ao registro e também ao tipo de registro e ao espaço de trabalho com permissões de **Exibição**.

   Os administradores do sistema sempre recebem permissões de gerenciamento para registros compartilhados com eles, e há uma indicação de que um usuário é um administrador do sistema.

1. (Opcional) Clique em **Copiar link** para copiar um link para o registro na área de transferência e compartilhá-lo com outras pessoas. O link abrirá a página de detalhes do registro.
1. Clique em **Salvar**.

   O registro agora é compartilhado com outros usuários.

   Os usuários com os quais você compartilhou o registro recebem uma notificação no aplicativo e por email sobre a concessão de permissões para as seguintes entidades:

   * O registro
   * O tipo de registro, se eles nunca tiveram permissões antes
   * O espaço de trabalho, se eles não tiverem tido permissões para o espaço de trabalho antes do registro ser compartilhado com eles.

   Para obter informações, consulte [Notificações do Adobe Workfront Planning: índice do artigo](/help/quicksilver/planning/notifications/notifications-information.md).

1. Compartilhar o link copiado com outras pessoas. Os usuários que recebem o link devem ser usuários ativos e fazer logon no Workfront para acessar a página de tipo de registro e exibi-la na exibição selecionada. Eles devem ter permissões no tipo de registro para poder visualizá-lo. Para obter mais informações, consulte também [Compartilhar registros usando um link](/help/quicksilver/planning/records/share-records.md).

## Remover permissões para um registro

É possível remover permissões de usuários de um registro. No entanto, eles manterão pelo menos permissões de Exibição no espaço de trabalho, o que também lhes dará pelo menos permissões de Exibição para o tipo de registro. Você deve remover o acesso deles do espaço de trabalho se quiser que eles não tenham permissões para os tipos de registros ou registros no espaço de trabalho.

{{step1-to-planning}}

1. Abra o espaço de trabalho cujos registros deseja interromper o compartilhamento e clique em um cartão de tipo de registro. Isso abre a página do tipo de registro.
1. Siga um destes procedimentos:

   * Na exibição de tabela, passe o mouse sobre o nome de um registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Compartilhar**.
   * Na exibição de tabela, selecione um registro e clique em **Compartilhar** na barra de ferramentas azul na parte inferior da lista.
   * Em qualquer exibição, clique no nome de um registro e em **Compartilhar** no canto superior direito da página de detalhes do registro.

   A caixa **Compartilhar** é aberta.
1. Localize o usuário, grupo, equipe, empresa ou função de trabalho cujas permissões você deseja remover, expanda o menu suspenso de permissões à direita de seu nome e clique em **Remover**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Remover permissões no registro](assets/remove-option-on-record-sharing-drop-down.png)

1. Clique em **Salvar**.

   As pessoas não têm mais as permissões indicadas para o registro. No entanto, eles ainda têm permissões para o tipo de registro e o espaço de trabalho, a menos que você também os remova dessas permissões.

   Não há notificação para os usuários que foram removidos do acesso ao registro de que eles não têm mais essas permissões.
