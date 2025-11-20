---
title: Compartilhar registros
description: Você pode compartilhar registros usando o botão Compartilhar para aumentar a colaboração no Adobe Workfront Planning.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---


<!--update metadata with real information at release-->

# Compartilhar registros

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Você pode ajustar as permissões das pessoas para registros individuais em um tipo de registro. O

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

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

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

* Você pode compartilhar registros com as seguintes entidades: pessoas, grupos, equipes, empresas ou funções de trabalho.
* Quando você compartilha um espaço de trabalho com usuários, eles também recebem as mesmas permissões para os registros no espaço de trabalho, por padrão.
* Quando você remove uma entidade de um espaço de trabalho, todas as permissões de compartilhamento são removidas dos tipos de registro e de todos os registros nele.
* O acesso de um usuário ao registro é determinado por meio da combinação das três configurações a seguir:

   * Suas permissões herdadas do tipo de registro e do espaço de trabalho
   * Permissões adicionadas individualmente na caixa de diálogo de compartilhamento de registros
   * As seguintes permissões:

      * **Todos no espaço de trabalho podem exibir**: isso torna o registro visível para todos no espaço de trabalho <!-- is this OK to say "workspace? should it be "record"??-->
      * **Somente pessoas convidadas podem acessar**: esta opção é selecionada por padrão e permite restringir o acesso ao registro a pessoas específicas.

* Você pode conceder os seguintes níveis de permissões a um registro:

   * Exibir
   * Gerenciar

* Quando você compartilha um registro com um usuário, ele é adicionado com a mesma permissão que tem no tipo de registro, por padrão.

  Por exemplo:

   * Se tiverem permissões de Exibição para o tipo de registro, eles obterão permissões de Exibição para o registro
   * Se tiverem permissões do Contribute ou do Manage para o tipo de registro, eles obterão permissões do Manage para o registro

* Como gerenciador de espaço de trabalho, você pode compartilhar um registro com um usuário que não faz parte do espaço de trabalho. Nesse caso, há um aviso ao lado da entidade adicionada notificando que ela não tem acesso ao espaço de trabalho. Você pode aceitar adicionar o usuário ao registro e ao espaço de trabalho ou negar sua adição ao espaço de trabalho que também o remove do registro.

* Ao compartilhar um registro com usuários que têm permissões de gerenciamento no espaço de trabalho, eles também obtêm permissões de gerenciamento para o registro por padrão. A permissão Exibir fica esmaecida.

* Se não tiver permissões para adicionar pessoas ao espaço de trabalho, você só verá e adicionará usuários, equipes, grupos, funções e empresas que já foram adicionados ao espaço de trabalho. Não é possível adicionar nenhuma outra entidade que ainda não faça parte do espaço de trabalho.

* Você pode desativar permissões herdadas para um único registro, nesse caso, você pode conceder permissões a eles individualmente ou eles podem obter permissões se pertencerem à opção &quot;Todos no espaço de trabalho&quot;. <!-- is this OK to say "workspace? should it be "record"??-->

* Se várias permissões de compartilhamento se aplicarem ao mesmo usuário, ele receberá a maior permissão dessas permissões.

  Por exemplo, se um registro é compartilhado com um usuário com permissões de Exibição e seu grupo com acesso de Gerenciamento, ele obtém permissões de Gerenciamento para o registro.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Se um campo de fórmula ou um campo de pesquisa de um registro conectado for baseado em um campo em um registro no qual você não tem permissões, você verá o cálculo correto de quais fatores no registro não poderão ser acessados de outra forma.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Compartilhar permissões de registro

