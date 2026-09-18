---
title: Compartilhar campos do Workfront Planning
description: Você pode compartilhar o campo de um registro do Workfront Planning com outras pessoas para garantir a colaboração ao usar o Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ac94936cc4dc9dc4f2d56b3f1221f71a405c5c65
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 2%
---

# Compartilhar campos do Workfront Planning

{{planning-important-intro}}

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Após o lançamento para Pré-visualização, os mesmos recursos também estarão disponíveis mensalmente no ambiente de Produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Você pode compartilhar o campo de um registro do Workfront Planning com outras pessoas para garantir a colaboração ao usar o Adobe Workfront Planning.

O compartilhamento de campo permite que os administradores de espaço de trabalho controlem o acesso a um campo individual. Cada campo em um tipo de registro tem seu próprio diálogo de compartilhamento, em que o acesso pode ser definido como Sem acesso, Exibir valores de campo ou Gerenciar valores de campo.

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
<p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p> 
Ou
<p>Qualquer pacote de produto do Workfront Planning como independente</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Qualquer</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Qualquer</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Você deve adicionar um Workflow e um tipo de licença do Planning ao nível de acesso quando tiver um Workflow e um pacote do Planning</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td><p>Gerenciar permissões em um campo para alterar valores do campo</p>  
   <p>Contribuir com ou mais permissões para um tipo de registro para herdar Gerenciar permissões para o campo</p>  
   </td> 
  </tr>
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre o compartilhamento de campos

* Você pode compartilhar campos com usuários, funções de trabalho, grupos, equipes ou empresas.
* Você só pode compartilhar campos da exibição de tabela de um tipo de registro.
* Não é possível compartilhar os seguintes tipos de campos:

  * Campos do sistema (por exemplo, Criado por, ID de registro)
  * Campos primários
  * Campos de pesquisa. Eles sempre herdam as permissões de seus campos de objeto de origem.
* O acesso a um campo vem da combinação das seguintes configurações:

  * **Permissões herdadas**: por padrão, um campo herda o mesmo acesso que alguém tem no tipo de registro. Você pode desativar as Permissões herdadas e conceder aos usuários um acesso ao campo menor do que eles têm para o tipo de registro.
  * O **Todos com acesso ao tipo de registro podem exibir** ou **Somente pessoas convidadas podem acessar a seleção**. Você pode permitir que qualquer pessoa com permissões para o espaço de trabalho exiba o campo ou conceder permissões somente a entidades individuais.

  Se várias regras se aplicarem à mesma pessoa, ela receberá a permissão mais alta disponível de uma das regras.

* Para tornar um campo somente para visualização para todos em um espaço de trabalho, verifique se a seguinte configuração existe:

  * Desativar permissões herdadas
  * Manter a configuração **Todos com acesso ao tipo de registro podem exibir**
  * Não adicione entidades individuais.

* Dependendo das permissões de tipo de registro, os usuários podem receber as seguintes permissões de campo:

  * Exibir permissões de tipo de registro dão a um usuário permissões para exibir valores de campo
  * As permissões de tipo de registro do Contribute ou do Manage fornecem ao usuário permissões para gerenciar valores de campo

* Somente proprietários e gerentes de espaços de trabalho podem ajustar as permissões de campo. Os gerentes do Workspace sempre mantêm o acesso Gerenciar a todos os campos e isso não pode ser reduzido.
* O compartilhamento de campos controla o acesso a valores, não a configurações de campo. Somente gerentes de espaço de trabalho podem alterar a configuração de um campo.
* Adicionar alguém a uma lista de compartilhamento de campo não concede a ele acesso de espaço de trabalho ou tipo de registro. Se não tiverem esse acesso, um ícone de aviso indicará que a permissão só terá efeito depois que forem adicionadas ao tipo de registro.
* Campos com permissões restritas são aplicados em todos os locais em que o campo é exibido. Isso inclui todas as exibições, páginas de detalhes de registro, formulários de solicitação, conexões e campos de pesquisa, painéis do Canvas, a API e ferramentas do MCP.
* As visualizações públicas permanecem totalmente visíveis e somente leitura para qualquer pessoa que possa acessá-las.
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* As alterações de valor de campo restrito não são registradas no Histórico de um registro.
* As alterações de permissão para campos não acionam notificações.
* Para tipos de registros globais, as permissões de campo se aplicam a todos os espaços de trabalho secundários e não podem ser ajustadas localmente.

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## Compartilhar campos

Como um gerenciador de espaço de trabalho, você pode ajustar permissões para campos individuais.

{{step1-to-planning}}

1. Abra o espaço de trabalho e o tipo de registro cujos campos você deseja compartilhar.

1. Na exibição de tabela, passe o mouse sobre o nome do cabeçalho de uma coluna do campo, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Compartilhar campo**.

   A caixa **Compartilhar** é aberta.

1. (Opcional) Na área **Conceder acesso**, a opção **Todos com acesso ao tipo de registro pode visualizar** é selecionada por padrão. Todos os usuários com permissões de **Exibição** ou superior para o espaço de trabalho e o tipo de registro têm as mesmas permissões para o campo.

1. (Opcional) Clique nos avatares dos usuários na opção **Permissões herdadas de** para exibir usuários, equipes, grupos, empresas ou funções de trabalho que herdam permissões do espaço de trabalho.

   As permissões do usuário para o tipo de registro são exibidas ao expandir as permissões herdadas.

   >[!TIP]
   >
   >Não é possível remover entidades individuais da lista de permissões herdadas. Os usuários de equipes, grupos, empresas ou funções de trabalho são listados em vez das entidades às quais estavam associados quando o espaço de trabalho e o tipo de registro foram compartilhados com eles.

1. (Opcional e condicional) Se quiser compartilhar o campo com entidades específicas e conceder a elas um acesso ao campo diferente do que elas já têm para o tipo de registro, faça o seguinte:

   1. Desmarque a opção **Ativado** de **Permissões herdadas**. Ela é selecionada por padrão.

      A opção muda para **Desativada**.

      >[!TIP]
      >
      >Os gerentes do Workspace continuam a ter permissões de gerenciamento para o tipo de registro e o campo.

   1. (Opcional) Clique no menu suspenso **Todos com acesso ao tipo de registro podem exibir** e selecione **Somente pessoas convidadas podem acessar**.

      >[!IMPORTANT]
      >
      >Essa alteração, juntamente com a desativação de **Permissões herdadas**, remove o acesso de todas as pessoas que podem exibir o tipo de registro e conceder acesso somente a pessoas designadas. Os gerentes e administradores do Workspace sempre terão acesso a todos os campos.


   1. Na caixa **Conceder acesso**, adicione os usuários, equipes, grupos, empresas ou funções de trabalho aos quais você deseja conceder um nível de permissão diferente daquele que eles têm para o espaço de trabalho ou tipo de registro.

      Quando você compartilha um campo com um usuário, a função de trabalho principal dele e o email também são exibidos no campo. Você deve ter a configuração Exibir informações de contato ativada para que o objeto Usuários em seu nível de acesso possa exibir o email do usuário.

   1. Escolha um dos seguintes níveis de permissão:

      * Exibir valores de campo
      * Gerenciar valores de campo

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* Você não pode conceder aos usuários uma permissão menor para o campo se eles tiverem o Contribute ou superior para o tipo de registro.
      >
      >* Não é possível conceder permissões a usuários que não estão no espaço de trabalho. Os usuários que não têm permissões para o espaço de trabalho e o tipo de registro não podem acessar nenhum dos campos. Eles poderão acessar os campos quando obtiverem permissões para o espaço de trabalho e tipos de registro.

1. Clique em **Salvar**.

   O campo agora é compartilhado com outros usuários.

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## Remover permissões para um campo

É possível remover permissões de usuários de um campo. No entanto, eles manterão pelo menos permissões de Exibição para o espaço de trabalho e o tipo de registro que também oferece pelo menos permissões de Exibição para o campo.

Você deve remover o acesso deles do espaço de trabalho se quiser que eles não tenham permissões para os tipos de registros ou campos no espaço de trabalho.

Não é possível remover um usuário de permissões herdadas.

{{step1-to-planning}}

1. Abra o espaço de trabalho cujos campos deseja interromper o compartilhamento e clique em um cartão de tipo de registro. Isso abre a página do tipo de registro.
1. Na exibição de tabela, passe o mouse sobre o nome do cabeçalho de uma coluna do campo, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Compartilhar campo**.

   A caixa **Compartilhar** é aberta.
1. Localize o usuário, grupo, equipe, empresa ou função de trabalho cujas permissões você deseja remover, expanda o menu suspenso de permissões à direita de seu nome e clique em **Remover**.

1. Clique em **Salvar**.

   As pessoas não têm mais as permissões indicadas para o campo. No entanto, eles ainda têm permissões para o tipo de registro e o espaço de trabalho, a menos que você também as remova dessas permissões.

   Não há notificação para os usuários que foram removidos do acesso ao campo de que eles não têm mais essas permissões.
