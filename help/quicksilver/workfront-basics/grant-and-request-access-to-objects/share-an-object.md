---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Compartilhar um objeto
description: O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar objetos ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a objetos, consulte Criar ou modificar níveis de acesso personalizados.
author: Alina, Nolan
feature: Get Started with Workfront
exl-id: 27a1beb9-e83a-4ef6-bf5f-ad52575a993c
source-git-commit: 8b524f7cd7e1bfedbaa1e993cbf4b3b805344b7c
workflow-type: tm+mt
source-wordcount: '1909'
ht-degree: 0%

---

# Compartilhar um objeto

<!--Audited: 01/2024-->

O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar objetos ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a objetos, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Juntamente com o nível de acesso que os usuários recebem, você também pode conceder a eles permissões para exibir ou editar objetos específicos que você criou ou ter acesso para compartilhar. Para obter mais informações sobre níveis de acesso e permissões, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.

Para obter informações sobre o compartilhamento de permissões em objetos, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

Este artigo descreve como compartilhar os seguintes objetos:

* Projetos, tarefas, problemas
* Portfólios, programas
* Documentos

Para obter informações sobre como compartilhar todos os outros objetos no Workfront, consulte também os seguintes artigos:

* Para modelos, consulte [Compartilhar modelos de projeto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Para obter provas, consulte [Compartilhar uma Prova no Workfront Proof](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).
* Para relatórios, painéis e calendários, consulte os seguintes artigos:

   * [Compartilhar um relatório no Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Compartilhar um painel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Compartilhar um relatório de calendário](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

  Além disso, consulte [Compartilhar relatórios, painéis e calendários](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) para obter informações gerais sobre como compartilhar relatórios, painéis e calendários.

* Para filtros, visualizações e agrupamentos, consulte [Compartilhar um filtro, visualização ou agrupamento](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* Para pastas de documentos, consulte [Compartilhar uma pasta de documentos](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).
* Para planos, consulte [Compartilhar um plano no Planejador de Cenários](../../scenario-planner/share-a-plan.md).

  O Planejador de cenários do Workfront pode exigir uma licença adicional.

* Para metas, consulte [Compartilhar uma meta no Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  O Workfront Goals pode exigir uma licença adicional.

* Para objetos do Workfront Planning, consulte os seguintes artigos:

   * [Compartilhar exibições](/help/quicksilver/planning/access/share-views.md)
   * [Compartilhar espaços de trabalho](/help/quicksilver/planning/access/share-workspaces.md)

  O acesso ao Workfront Planning exige uma licença adicional.

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
   <td> <p>Nova licença: Standard</p> 
   Ou
   <p>Licença atual: Comercial ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir o acesso ou superior aos objetos que você deseja compartilhar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores aos objetos que você deseja compartilhar</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartilhar um projeto, tarefa ou problema da página

1. Vá para a página do projeto, tarefa ou problema que deseja compartilhar.

   Para obter informações sobre quais objetos podem ser compartilhados, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Clique no botão **Compartilhar** ao lado do nome do objeto.

   ![](assets/new-share-button.png)

1. Na caixa **Conceder acesso a**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar o objeto e, em seguida, clique no nome quando ele aparecer na lista suspensa.

   ![](assets/new-share-button-add-people.png){width="350"}

   >[!TIP]
   >
   >Você pode compartilhar um objeto somente com usuários, equipes, funções ou empresas ativos.

   >[!TIP]
   >
   >Se você tiver várias entidades nomeadas de forma semelhante, todas serão listadas em seu tipo. Os nomes das entidades aparecem em ordem alfabética. No entanto, a ordem em que os tipos de entidade aparecem é aleatória.
   >

1. (Opcional) Repita a etapa 3 para cada usuário, equipe, função ou grupo ao qual deseja conceder acesso ao objeto.

1. Especifique as permissões para cada usuário, equipe, função, grupo ou empresa adicionada na Etapa 3 clicando no menu suspenso à direita do nome e selecionando o nível de permissão que deseja conceder.

   ![](assets/new-share-permissions-dropdown.png)

   Para remover permissões de um objeto, consulte [Remover permissões de objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   As seguintes opções estão disponíveis:

   * **Exibir:** usuários podem revisar e compartilhar o item.
   * **Contribute**: os usuários podem fazer atualizações, registrar informações, fazer pequenas edições e compartilhar, além de todas as permissões de exibição.
   * **Gerenciar:** usuários têm acesso total ao objeto sem direitos administrativos (que são concedidos no nível de acesso). Além disso, eles também têm todas as permissões de Exibição e Contribute.

     >[!NOTE]
     >
     >O administrador do Workfront ou o criador do objeto tem a capacidade de remover permissões dessas entidades.

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas no objeto.

   ![](assets/new-share-advanced-permissions-dropdown.png)

   Exibir, Gerenciar e Contribute têm opções avançadas diferentes, dependendo do objeto selecionado.

   Para obter mais informações sobre níveis de permissão, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Opcional) Para disponibilizar este objeto para todos os usuários no sistema, clique no menu suspenso em **Quem tem acesso** e, no menu suspenso, clique em **Todos no sistema podem visualizar**.

   ![](assets/new-share-everyone-access.png)

   Todos os usuários podem ver o objeto com base nas permissões definidas.

1. (Opcional e condicional) Ao compartilhar um projeto, clique no ícone **Engrenagem** ![](assets/gear-icon-settings.png) e marque a caixa ao lado de **Definir como meu modelo de acesso ao projeto** para definir as permissões como um modelo.

   Depois de definir as permissões em um projeto, essas mesmas permissões são aplicadas automaticamente na próxima vez que você criar um projeto do zero.

   >[!NOTE]
   >
   >O modelo de acesso ao projeto substitui os padrões de compartilhamento concedidos a você pelo administrador do Workfront em seu Nível de acesso.\
   >Para obter mais informações sobre como especificar padrões de compartilhamento para projetos no Nível de Acesso, consulte [Conceder acesso aos projetos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->

   Você pode especificar permissões nos projetos que serão criados a partir de um modelo quando você compartilhar o modelo. Para obter mais informações, consulte [Compartilhar modelos de projeto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. (Condicional) Para compartilhar rapidamente o objeto com usuários que têm acesso, clique em **Copiar link**.

1. Clique em **Salvar**.

## Compartilhar um documento, portfólio ou programa na página

1. Vá para o documento, portfólio ou página do programa que deseja compartilhar.

   Para obter informações sobre quais objetos podem ser compartilhados, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Para portfólios e programas:

   Clique no botão **Compartilhar** ao lado do nome do objeto.

   ![](assets/new-share-button-on-portfolio.png)

   Ou

   Para documentos:

   Clique no ícone **Mais** ![](assets/more-icon.png) ao lado do nome do objeto e clique em **Compartilhar**.

   ![](assets/share-a-document-350x160.png)

1. No campo **Conceda acesso ao [Nome do Objeto] a**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar o objeto e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >* Se você tiver várias entidades nomeadas de forma semelhante, todas serão listadas em seu tipo. Os nomes das entidades aparecem em ordem alfabética. No entanto, a ordem em que os tipos de entidade aparecem é aleatória.
   >
   >* Você pode compartilhar um objeto somente com usuários, equipes, funções ou empresas ativos.

1. (Opcional) Repita a etapa 3 para cada usuário, equipe, função ou grupo ao qual deseja conceder acesso ao objeto.

1. Especifique as permissões para cada usuário, equipe, função, grupo ou empresa adicionada na Etapa 3.

   Para remover permissões de um objeto, consulte [Remover permissões de objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

   As seguintes opções estão disponíveis:

   * **Exibir:** usuários podem revisar e compartilhar o item.
   * **Gerenciar:** usuários têm acesso total ao objeto sem direitos administrativos (que são concedidos no nível de acesso). Além disso, eles também têm todas as permissões de Exibição e Contribute.

     >[!NOTE]
     >
     >O administrador do Workfront ou o criador do objeto tem a capacidade de remover permissões dessas entidades.

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas no objeto.

   ![](assets/new-share-advanced-permissions-dropdown.png)

   As permissões Exibir e Gerenciar têm opções avançadas diferentes, dependendo do objeto selecionado.\
   Para obter mais informações sobre os níveis de permissões, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Opcional) Para disponibilizar este objeto para todos os usuários no sistema, clique em **Quem tem acesso** no menu suspenso e selecione **Todos no sistema podem visualizar**.

   Todos os usuários podem ver o objeto com base nas permissões definidas.

1. (Opcional) Para tornar o objeto público, clique na moeda de engrenagem e habilite **Tornar público para usuários externos**.

   >[!TIP]
   >
   >Esta opção não está disponível para todos os objetos.

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png)

1. (Condicional) Se você tornou o objeto público para usuários externos, clique em **copiar link** e distribua o link para usuários externos.

   Qualquer usuário com o link pode visualizar o objeto.

   >[!CAUTION]
   >
   >Recomendamos que você tenha cuidado ao compartilhar com usuários externos um objeto que contém informações confidenciais. Isso permite que eles visualizem informações sem ser um usuário da Workfront ou parte da organização.

1. Clique em **Salvar**.

## Compartilhar objetos únicos ou em massa de uma lista

1. Vá para a lista que contém os objetos que você deseja compartilhar.

   Para obter informações sobre quais objetos podem ser compartilhados, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Clique na caixa de seleção ao lado do(s) objeto(s) que você deseja compartilhar e clique no **ícone Compartilhar** ![](assets/share-icon.png) na parte superior da página.

   A caixa **&lt; Objeto > Acesso** é aberta.

   ![](assets/list-share-object-select.png){width="350"}

1. No acesso **Editar &lt; Nome do Objeto > para**, comece digitando o nome do usuário, equipe, função, grupo ou empresa com quem deseja compartilhar os objetos e, em seguida, clique no nome quando ele aparecer na lista suspensa.


   >[!TIP]
   >
   >* Você pode compartilhar um objeto somente com usuários, equipes, funções ou empresas ativos.
   >
   >
   >* Se você tiver várias entidades nomeadas de forma semelhante, todas serão listadas em seu tipo. Os nomes das entidades aparecem em ordem alfabética. No entanto, a ordem em que os tipos de entidade aparecem é aleatória.
   >

1. (Opcional) Repita a etapa 3 para cada usuário, equipe, função ou grupo ao qual deseja conceder acesso ao(s) objeto(s).

1. Especifique as permissões para cada usuário, equipe, função, grupo ou empresa que você adicionou na etapa.

   Para remover permissões de um objeto, consulte [Remover permissões de objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).


   As seguintes opções estão disponíveis:

   * **Exibir:** usuários podem revisar e compartilhar o item.
   * **Contribute**: os usuários podem fazer atualizações, registrar informações, fazer pequenas edições e compartilhar, além de todas as permissões de exibição.

     >[!TIP]
     >
     >Você pode conceder permissões do Contribute somente para os seguintes objetos:
     >
     >* Projetos
     >* Tarefas
     >* Problemas
     >

   * **Gerenciar:** usuários têm acesso total ao objeto sem direitos administrativos (que são concedidos no nível de acesso). Além disso, eles também têm todas as permissões de Exibição e Contribute.

     >[!NOTE]
     >
     >O administrador do Workfront ou o criador do objeto tem a capacidade de remover permissões dessas entidades.

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas no objeto.

   ![](assets/new-share-advanced-permissions-dropdown.png)

   Exibir, Gerenciar e Contribute têm opções avançadas diferentes, dependendo do objeto selecionado.\
   Para obter mais informações sobre os níveis de permissões, consulte [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Opcional) Para disponibilizar este objeto para todos os usuários no sistema, clique no ícone **Engrenagem** ![](assets/gear-icon-settings-with-dn-arrow.jpg) e, no menu suspenso, clique em **Tornar isto visível para todo o sistema**.

   Todos os usuários podem ver os objetos com base nas permissões definidas.

1. (Opcional e condicional) Ao compartilhar um projeto, clique no ícone **Engrenagem** ![](assets/gear-icon-settings-with-dn-arrow.jpg) e, no menu suspenso, clique em **Definir como meu modelo de acesso ao projeto** para definir as permissões como um modelo.

   Depois de definir as permissões em um projeto, essas mesmas permissões são aplicadas automaticamente na próxima vez que você criar um projeto do zero.

   >[!NOTE]
   >
   >O modelo de acesso ao projeto substitui os padrões de compartilhamento concedidos a você pelo administrador do Workfront em seu Nível de acesso.\
   >Para obter mais informações sobre como especificar padrões de compartilhamento para projetos no Nível de Acesso, consulte [Conceder acesso aos projetos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->

   Você pode especificar permissões nos projetos que serão criados a partir de um modelo quando você compartilhar o modelo. Para obter mais informações, consulte [Compartilhar modelos de projeto](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. (Opcional) Para tornar o(s) objeto(s) público(s), clique em **Tornar público para usuários externos**.

   >[!TIP]
   >
   >Esta opção não está disponível para todos os objetos.

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png){width="350"}

1. (Condicional) Se você tornou o(s) objeto(s) público(s) para usuários externos, clique em **copiar link** e distribua o link para usuários externos.

   Qualquer usuário com o link pode visualizar o objeto.

   >[!CAUTION]
   >
   >Recomendamos que você tenha cuidado ao compartilhar com usuários externos um objeto que contém informações confidenciais. Isso permite que eles visualizem informações sem ser um usuário da Workfront ou parte da organização.

1. Clique em **Salvar**.
