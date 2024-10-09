---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Solicitar Acesso a Objetos
description: A visibilidade dos objetos no Adobe Workfront depende do seu acesso a esse tipo de objeto, bem como das suas permissões em um objeto individual.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 968f17721477a4a4c545a553d24de1855388d585
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 0%

---

# Solicitar acesso a objetos

A visibilidade dos objetos no Adobe Workfront depende do seu acesso a esse tipo de objeto, bem como das suas permissões em um objeto individual.

>[!NOTE]
>
>Este artigo descreve como você pode solicitar permissões para todos os objetos, exceto para o seguinte:
>
>* O Planejador de cenários planeja no Planejador de cenários do Adobe Workfront. Para obter mais informações, consulte [Solicitar acesso a um plano no Planejador de cenários](../../scenario-planner/request-access-to-plan.md). Isso requer uma licença adicional.
>
>* Exibições e espaços de trabalho no Workfront Planning. Para obter mais informações, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). Isso requer uma licença adicional.


O administrador do Workfront configura o acesso a um tipo de objeto no seu nível de acesso. Para obter mais informações, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Se você precisar de permissões para objetos específicos no Workfront, poderá solicitar acesso a eles. Em vez de enviar um email ao administrador ou proprietário do objeto do Workfront para explicar suas necessidades, você pode solicitar acesso adicional (ou permissões) no Workfront.

Você pode solicitar acesso inicial a objetos se alguém compartilhar um link para o objeto com você ou pode solicitar acesso adicional a objetos que você possa, pelo menos, visualizar.

Por exemplo, você pode ter permissões de Visualização para um projeto, mas precisa adicionar tarefas a esse projeto. Nesse caso, você pode solicitar permissões do Contribute para o projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para compartilhar objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Novo: Padrão</p> 
   <p>Atual: trabalho ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualize o acesso ou superior aos objetos para os quais você solicita permissões</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entenda as regras de compartilhamento padrão

As seguintes regras de compartilhamento padrão entram em vigor automaticamente, pois são configuradas como opções padrão no sistema do Workfront.

* Os usuários atribuídos a uma tarefa ou um problema têm acesso ao Contribute a ela.
* Os gerentes de projeto, Portfolio e programa têm acesso de gerenciamento nos objetos que possuem.
* Os usuários incluídos em uma conversa têm acesso de Visualização no objeto em que a conversa acontece.
* Os usuários atribuídos como aprovadores têm acesso de Visualização no objeto aguardando aprovação.
* Ao compartilhar um painel, todos os relatórios no painel também são compartilhados com o mesmo acesso para os mesmos usuários.
* Os proprietários de objetos não podem estender o acesso a um objeto além de seu acesso a esse objeto, conforme definido pelo administrador.

## Solicitar acesso

Você pode solicitar acesso inicial a objetos aos quais não tem acesso no momento ou pode solicitar acesso adicional a objetos aos quais você tem acesso limitado.

* [Solicitar acesso inicial](#request-initial-access)
* [Solicitar acesso adicional](#request-additional-access)

### Solicitar acesso inicial  {#request-initial-access}

Se você ainda não tiver acesso a um objeto e navegar até ele a partir de um link, uma tela será exibida informando que você não tem acesso para exibir as informações.

Para solicitar acesso inicial a um objeto:

1. Clique em **Solicitar Acesso**.\
   A caixa de diálogo **Solicitar Acesso** é exibida.

1. (Condicional) Se mais de um usuário tiver o acesso apropriado para conceder a você acesso adicional, uma seta suspensa será exibida ao lado do nome do usuário.
1. Selecione na lista suspensa o usuário que receberá sua solicitação de acesso.\
   Somente 10 usuários são exibidos na lista suspensa. A lista é classificada em ordem alfabética.\
   Para obter mais informações sobre a ordem dos usuários listados nesse menu suspenso, consulte [Hierarquia dos menus suspensos &quot;Solicitar Acesso&quot; e &quot;Solicitar Mais Acesso&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Na lista suspensa, selecione o tipo de acesso que você está solicitando.
1. (Opcional) No campo **P.S.**, especifique uma observação para o usuário sobre por que você precisa de acesso adicional.

   ![](assets/request-access-dialog-350x314.png)

Se você não tiver direitos de nível de acesso a um objeto e tentar acessá-lo por meio de um link, uma tela será exibida informando para entrar em contato com o administrador do Workfront.

Por exemplo, se você não tiver acesso ao portfólio, mas receber um link para um portfólio, verá a seguinte mensagem:\
![](assets/permission-request-initial2-350x96.png)

### Solicitar acesso adicional {#request-additional-access}

Para solicitar acesso adicional a um objeto ao qual você já tem acesso limitado:

1. Vá para o objeto para o qual deseja solicitar acesso adicional.

1. Clique no menu **Mais** à direita do nome do projeto e em **Solicitar Mais Acesso**.

   ![](assets/request-access-in-project-350x201.png)

1. (Condicional) Se mais de um usuário tiver o acesso apropriado para conceder a você acesso adicional, uma seta suspensa será exibida ao lado do nome do usuário.
1. Selecione na lista suspensa o usuário que receberá sua solicitação de acesso.\
   Somente 10 usuários são exibidos na lista suspensa. A lista é classificada em ordem alfabética.\
   Para obter mais informações sobre a ordem dos usuários listados nesse menu suspenso, consulte [Hierarquia dos menus suspensos &quot;Solicitar Acesso&quot; e &quot;Solicitar Mais Acesso&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Na lista suspensa, selecione o nível de acesso que você está solicitando.
1. (Opcional) No campo **PS.**, especifique uma observação sobre por que você precisa de acesso adicional.
1. Clique em **Solicitar Acesso**.\
   ![](assets/request-access-dialog-350x314.png)

## Hierarquia dos menus suspensos &quot;Solicitar acesso&quot; e &quot;Solicitar mais acesso&quot; {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Entenda a hierarquia de usuários listados nos menus suspensos Solicitar Acesso e Solicitar Mais Acesso](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Entender o proprietário de um objeto](#understand-the-owner-of-an-object)

### Entenda a hierarquia de usuários listados nos menus suspensos Solicitar Acesso e Solicitar Mais Acesso {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Ao preencher as listas &quot;Solicitar acesso&quot; ou &quot;Solicitar mais acesso&quot; em objetos, o Workfront seleciona uma lista de até dez usuários que atendem a várias funções no compartilhamento do objeto, conforme descrito abaixo. Esses usuários podem conceder acesso ao objeto ao usuário que o solicita.\
A lista resultante é então classificada pelo seu nome em ordem alfabética crescente.\
O Workfront exibe até 10 usuários nas listas &quot;Solicitar acesso&quot; e &quot;Solicitar mais acesso&quot;.

A ordem dos usuários nos menus suspensos &quot;Solicitar acesso&quot; ou &quot;Solicitar mais acesso&quot; é ditada pelas seguintes regras:

* O primeiro usuário na lista é o objeto &quot;proprietário&quot;, conforme descrito em [Entender o proprietário de um objeto](#understand-the-owner-of-an-object).
* Em seguida, a lista é preenchida com usuários com os quais o objeto é compartilhado individualmente. Eles são listados em ordem alfabética.
* Em seguida, a lista é preenchida ainda mais com usuários que obtêm o acesso necessário por meio do compartilhamento com suas equipes, grupos ou empresas. Eles são listados em ordem alfabética.
* Se a lista estiver vazia, os administradores do Workfront são adicionados para que sempre haja alguém do qual solicitar acesso. Eles são listados em ordem alfabética.
* Cada um dos usuários na lista deve ter o acesso solicitado ao objeto e o acesso para compartilhar o objeto.

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
   <td>O proprietário é o Proprietário do projeto ou, se estiver ausente ou não tiver o acesso necessário, o proprietário do portfólio principal. <p>Eles podem não ser a mesma pessoa que o criador do projeto. </p></td> 
  </tr> 
  <tr> 
   <td>Tarefas</td> 
   <td>O proprietário é o Destinatário principal ou, se estiver ausente ou se não tiver o acesso necessário, o proprietário do projeto no qual a tarefa reside, conforme definido acima. <p>Eles podem não ser a mesma pessoa que o criador da tarefa. </p></td> 
  </tr> 
  <tr> 
   <td>Problemas</td> 
   <td> <p>O proprietário é o contato principal da ocorrência ou, se estiver faltando ou não tiver acesso necessário, o proprietário do projeto no qual a ocorrência reside, conforme definido acima. </p> <p>Eles podem não ser a mesma pessoa que o criador da ocorrência. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfólios</td> 
   <td>O proprietário é o Proprietário do Portfolio. <p>Eles podem não ser a mesma pessoa que o criador do portfólio. </p></td> 
  </tr> 
  <tr> 
   <td>Documentos</td> 
   <td>O proprietário é o Proprietário do documento (o usuário que carregou o documento) ou, se ele estiver ausente ou não tiver acesso necessário, o proprietário do objeto no qual o documento reside.</td> 
  </tr> 
  <tr> 
   <td>Relatórios e painéis</td> 
   <td>O proprietário é o criador, o relatório ou o painel. </td> 
  </tr> 
  <tr> 
   <td>Calendários</td> 
   <td>O proprietário é o criador do calendário. Todos os usuários têm um calendário atribuído a eles por padrão. Eles são considerados o proprietário desse calendário. </td> 
  </tr> 
  <tr> 
   <td>Filtros, visualizações e agrupamentos</td> 
   <td>O proprietário de um filtro, exibição ou agrupamento é o criador. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Planos</span> </td> 
   <td> <p><span>O proprietário é o criador do plano.</span> </p> <p>Isso requer uma licença adicional. </p> <p><span>Para obter informações sobre o Planejador de cenários do Workfront, consulte</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">A visão geral do Planejador de cenários</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Metas</td> 
   <td> <p>O proprietário é o usuário designado como o Proprietário. Eles podem não ser a mesma pessoa que o criador da meta. </p> <p>Isso requer uma licença adicional. </p> <p>Para obter informações sobre as Metas do Workfront, consulte <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Visão geral das Metas do Adobe Workfront</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


