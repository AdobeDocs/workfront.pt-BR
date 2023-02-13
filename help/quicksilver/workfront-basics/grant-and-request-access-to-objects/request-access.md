---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Solicitar acesso a objetos
description: Sua visibilidade para objetos no Adobe Workfront depende do acesso a esse tipo de objeto, bem como das permissões em um objeto individual.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---

# Solicitar acesso a objetos

Sua visibilidade para objetos no Adobe Workfront depende do acesso a esse tipo de objeto, bem como das permissões em um objeto individual.

>[!NOTE]
>
>Este artigo descreve como você pode solicitar permissões para todos os objetos, exceto para planos no Adobe Workfront Scenario Planner. Para obter informações sobre a solicitação de acesso aos planos, consulte [Solicitar acesso a um plano no Planejador de Cenário](../../scenario-planner/request-access-to-plan.md). Isso requer uma licença adicional.

O administrador do Workfront configura o acesso a um tipo de objeto no nível de acesso. Para obter mais informações, consulte [Como os níveis de acesso e as permissões funcionam em conjunto](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Se você precisar de permissões para objetos específicos no Workfront, poderá solicitar acesso a eles. Em vez de enviar emails para o administrador do Workfront ou o proprietário do objeto para explicar suas necessidades, você pode solicitar acesso adicional (ou permissões) no Workfront.

Você pode solicitar acesso inicial a objetos se alguém compartilhar um link para o objeto com você ou você pode solicitar acesso adicional a objetos que você possa, pelo menos, visualizar.

Por exemplo, você pode ter permissões de Exibição para um projeto, mas precisa adicionar tarefas a esse projeto. Nesse caso, você pode solicitar permissões do Contribute para o projeto.

## Requisitos de acesso

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Você deve ter o seguinte para compartilhar objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualize o acesso ou superior aos objetos aos quais você solicita permissões</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Entender as regras de compartilhamento padrão

As regras de compartilhamento padrão a seguir entrarão em vigor automaticamente, pois são configuradas como opções padrão em seu sistema Workfront. 

* Os usuários atribuídos a uma tarefa ou problema têm acesso ao Contribute. 
* Os gerentes de projeto, Portfolio e Programa têm acesso de Gerenciar nos objetos que possuem.
* Os usuários incluídos em uma conversa têm acesso de Exibição no objeto em que a conversa acontece.
* Os usuários atribuídos como aprovadores têm acesso de Exibição no objeto aguardando aprovação.
* Ao compartilhar um painel, todos os relatórios no painel também são compartilhados com o mesmo acesso aos mesmos usuários. 
* Os proprietários de objetos não podem estender o acesso a um objeto além do seu acesso nesse objeto, conforme definido pelo administrador.

## Solicitar acesso

Você pode solicitar acesso inicial a objetos aos quais não tem acesso no momento ou pode solicitar acesso adicional a objetos aos quais você tem acesso limitado.

* [Solicitar acesso inicial](#request-initial-access)
* [Solicitar acesso adicional](#request-additional-access)

### Solicitar acesso inicial  {#request-initial-access}

Se você ainda não tiver acesso a um objeto e navegar até esse objeto a partir de um link, uma tela será exibida informando que você não tem acesso para exibir as informações.  

Para solicitar acesso inicial a um objeto:

1. Clique em **Solicitar acesso**.\
   O **Solicitar acesso** será exibida.

1. (Condicional) Se mais de um usuário tiver o acesso apropriado para conceder a você acesso adicional, uma seta suspensa será exibida ao lado do nome do usuário. 
1. Selecione o usuário na lista suspensa que você deseja que receba sua solicitação de acesso.\
   Somente 10 usuários são exibidos na lista suspensa. A lista é classificada alfabeticamente.\
   Para obter mais informações sobre a ordem dos usuários listados neste menu suspenso, consulte  [Hierarquia dos menus suspensos &quot;Solicitar acesso&quot; e &quot;Solicitar mais acesso&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Na lista suspensa, selecione o tipo de acesso que você está solicitando.
1. (Opcional) Na seção **P.S.** , especifique uma observação para o usuário sobre por que você precisa de acesso adicional.

   ![](assets/request-access-dialog-350x314.png)

Se você não tiver direitos de nível de acesso a um objeto e tentar acessá-lo a partir de um link, uma tela será exibida, informando-o para entrar em contato com o administrador do Workfront. 

Por exemplo, se você não tiver acesso ao portfólio, mas recebeu um link para um portfólio, você verá a seguinte mensagem:\
![](assets/permission-request-initial2-350x96.png)

### Solicitar acesso adicional {#request-additional-access}

Para solicitar acesso adicional a um objeto ao qual você já tem acesso limitado:

1. Vá para o objeto para o qual deseja solicitar acesso adicional.

1. Clique no botão **Mais** menu em linha com o nome do projeto e clique em **Solicitar mais acesso**.\
   ![](assets/request-access-in-project-350x201.png)

1. (Condicional) Se mais de um usuário tiver o acesso apropriado para conceder a você acesso adicional, uma seta suspensa será exibida ao lado do nome do usuário.
1. Selecione o usuário na lista suspensa que você deseja que receba sua solicitação de acesso.\
   Somente 10 usuários são exibidos na lista suspensa. A lista é classificada alfabeticamente.\
   Para obter mais informações sobre a ordem dos usuários listados neste menu suspenso, consulte  [Hierarquia dos menus suspensos &quot;Solicitar acesso&quot; e &quot;Solicitar mais acesso&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Na lista suspensa, selecione o nível de acesso que você está solicitando.
1. (Opcional) Na seção **P.S.** , especifique uma observação sobre por que você precisa de acesso adicional.
1. Clique em **Solicitar acesso**.\
   ![](assets/request-access-dialog-350x314.png)

## Hierarquia dos menus suspensos &quot;Solicitar acesso&quot; e &quot;Solicitar mais acesso&quot; {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Entenda a hierarquia de usuários listados nos menus suspensos Solicitar acesso e Solicitar mais acesso](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Entender o proprietário de um objeto](#understand-the-owner-of-an-object)

### Entenda a hierarquia de usuários listados nos menus suspensos Solicitar acesso e Solicitar mais acesso {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Ao preencher as listas &quot;Solicitar acesso&quot; ou &quot;Solicitar mais acesso&quot; em objetos, o Workfront seleciona uma lista de até dez usuários que atendem a várias funções no compartilhamento do objeto, conforme descrito abaixo. Esses usuários podem conceder acesso ao objeto ao usuário que o solicita.\
A lista resultante é então classificada pelo nome em ordem alfabética crescente.\
O Workfront exibe até 10 usuários nas listas &quot;Solicitar acesso&quot; e &quot;Solicitar mais acesso&quot;. 

A ordem dos usuários nos menus suspensos &quot;Solicitar acesso&quot; ou &quot;Solicitar mais acesso&quot; é ditada pelas seguintes regras: 

* O primeiro usuário na lista é o objeto &quot;proprietário&quot;, conforme descrito em [Entender o proprietário de um objeto](#understand-the-owner-of-an-object). 
* Em seguida, a lista é preenchida com usuários com os quais o objeto é compartilhado individualmente. Eles estão listados em ordem alfabética.
* Em seguida, a lista é preenchida com usuários que obtêm o acesso necessário por meio do compartilhamento com suas equipes, grupos ou empresas. Eles estão listados em ordem alfabética.
* Se a lista estiver vazia, os administradores do Workfront serão adicionados para que sempre haja alguém do qual solicitar acesso. Eles estão listados em ordem alfabética. 
* Cada usuário na lista deve ter o acesso solicitado ao objeto e o acesso para compartilhar o objeto. 

### Entender o proprietário de um objeto {#understand-the-owner-of-an-object}

O proprietário de um objeto é definido da seguinte maneira:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objeto</strong> </th> 
   <th><strong>Definição do Proprietário do Objeto</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projetos</td> 
   <td>O proprietário é o Proprietário do Projeto ou, se estiver ausente ou não tiver o acesso necessário, o proprietário do portfólio pai. <p>Eles podem não ser a mesma pessoa que o criador do projeto. </p></td> 
  </tr> 
  <tr> 
   <td>Tarefas</td> 
   <td>O proprietário é o Destinatário Principal ou, se estiver ausente ou não tiver o acesso necessário, o proprietário do projeto no qual a tarefa reside, conforme definido acima. <p>Eles podem não ser a mesma pessoa que o criador da tarefa. </p></td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td> <p>O proprietário é o Contato Principal da emissão ou, se estiver faltando ou não tiver acesso necessário, o proprietário do projeto em que a emissão reside, conforme definido acima. </p> <p>Eles podem não ser a mesma pessoa que o criador da edição. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfólios</td> 
   <td>O proprietário é o Portfolio Owner. <p>Eles podem não ser a mesma pessoa que o criador do portfólio. </p></td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>O proprietário é o Proprietário do documento (o usuário que fez upload do documento) ou, se estiver ausente ou não tiver o acesso necessário, o proprietário do objeto no qual o documento reside.</td> 
  </tr> 
  <tr> 
   <td>Relatórios e painéis</td> 
   <td>O proprietário é o criador ou o relatório ou o painel. </td> 
  </tr> 
  <tr> 
   <td>Calendários</td> 
   <td>O proprietário é o criador do calendário. Todos os usuários têm um calendário atribuído a eles por padrão. Eles são considerados o proprietário desse calendário. </td> 
  </tr> 
  <tr> 
   <td>Filtros, visualizações e agrupamentos</td> 
   <td>O proprietário de um filtro, visualização ou agrupamento é o criador. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Planos</span> </td> 
   <td> <p><span>O proprietário é o criador do plano.</span> </p> <p>Isso requer uma licença adicional. </p> <p><span>Para obter informações sobre o Planejador de Cenário do Workfront, consulte</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">A visão geral do Planejador de cenário</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Metas</td> 
   <td> <p>O proprietário é o usuário designado como o Proprietário. Eles podem não ser a mesma pessoa que o criador do objetivo. </p> <p>Isso requer uma licença adicional. </p> <p>Para obter informações sobre as Metas da Workfront, consulte <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Visão geral das Metas da Adobe Workfront</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

 
