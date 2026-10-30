---
title: Atribuir usuários a um modelo de layout
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront, você pode atribuir um modelo de layout criado a qualquer usuário, função de trabalho, equipe ou grupo que precise usá-lo.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/hCzefaueJPFQ1jTzePSOC9FIR1SRYTrC3NIKmtIOpp4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: c549503a-6440-4802-9525-ceb73a00feff
    internal-label: Create and manage teams
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: d4a62afa30eb4727619e64ea2a98e639891a29af
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 3%
---
# Atribuir usuários a um modelo de layout

É possível atribuir um modelo de layout criado a qualquer usuário, função de trabalho, equipe ou grupo que precise usá-lo.

Para usuários que não têm um modelo de layout atribuído a eles, o layout padrão é usado. Para saber mais sobre o layout padrão, consulte [Sobre o layout padrão do Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Os usuários também podem atribuir um modelo de layout a si mesmos, conforme descrito em Alterar as áreas Meu trabalho e Solicitações de trabalho com modelos de layout.

É possível atribuir vários modelos de layout diferentes para o mesmo nome. Para obter mais informações sobre qual modelo de layout está em vigor para um usuário, função, grupo ou equipe, consulte [Prioridade de atribuição de modelo de layout](#layout-template-assignment-priority), mais adiante neste artigo.

Para obter mais informações sobre modelos de layout, consulte [Modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Para obter informações sobre modelos de layout e perfis comerciais, consulte [Visão geral dos perfis comerciais](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/business-profiles.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.</p>
        <p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Atribuir um modelo de layout aos usuários

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Quando estiver satisfeito com seu modelo de layout, recomendamos testá-lo, conforme descrito em [Testar um novo modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Clique em **Atribuir a item a** na seção superior da página.
1. Na caixa exibida, clique em **Adicionar usuário, função de trabalho, equipe, grupo ou nível de acesso**, comece a digitar o nome de um usuário, função de trabalho, equipe, grupo ou nível de acesso e, em seguida, clique no nome quando ele aparecer no menu suspenso.

   Os nomes adicionados recentemente são exibidos com um plano de fundo azul. Isso é útil ao editar um modelo de layout existente, pois é possível distinguir os nomes que você acabou de adicionar daqueles que já estavam na lista.

   Um ícone Informações ![ícone Informações](assets/info-icon.png) é exibido à direita do nome de qualquer usuário, função de trabalho, equipe, grupo ou nível de acesso que já esteja atribuído a outro modelo de layout. Você pode passar o mouse sobre o ícone para ver o nome desse modelo de layout e decidir se deseja sobrepor a atribuição existente.

1. Repita as duas etapas anteriores para atribuir o modelo de layout a outros usuários, funções de trabalho, equipes, grupo ou nível de acesso, conforme necessário.

   É possível atribuir até 100 usuários de cada vez.

1. Clique em **Concluído** e em **Salvar e fechar** no canto inferior esquerdo.

   Esta etapa conclui o processo de criação e atribuição de um modelo de layout.

## Prioridade de atribuição do modelo de layout {#layout-template-assignment-priority}

Você e outros administradores do Workfront podem atribuir vários modelos de layout diferentes para o mesmo usuário das seguintes maneiras:

* Para o usuário individual
* Para uma função de trabalho específica, o usuário tem
* Para uma determinada equipe da qual o usuário faz parte
* Para um determinado grupo em que o usuário está
* Para um determinado nível de acesso ao qual o usuário está atribuído
* Para um perfil de negócios atribuído ao usuário

No entanto, somente um modelo de layout fica visível para o usuário em um determinado momento. O modelo visível é determinado pela seguinte hierarquia de prioridade:

* **Perfil comercial**: os perfis comerciais representam o nível mais alto de prioridade para um modelo de layout. Se o usuário tiver um perfil de negócios com modelos de layout atribuídos aos níveis de acesso e estiver em uma página específica do grupo (como um projeto associado a um grupo), todos os modelos de layout de perfil de negócios para esse grupo serão combinados com o modelo de layout atribuído pelo usuário. Quando o usuário não está em uma página específica do grupo, todos os modelos de layout de perfil de negócios são combinados com o modelo de layout atribuído pelo usuário.

  Quando modelos de layout para vários perfis comerciais e níveis de acesso são combinados, todos os elementos de layout disponíveis são exibidos. Se um item de menu for exibido em um modelo, mas oculto em outro, ele será exibido. Somente os itens ocultos em todos os modelos para o perfil comercial ficam ocultos.

  >[!NOTE]
  >
  >Os perfis empresariais estão disponíveis somente para organizações que têm um pacote Ultimate de fluxo de trabalho.

  Para obter mais informações, consulte [Visão geral dos perfis empresariais](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/business-profiles.md)

* **Usuário individual**: o modelo de layout atribuído à pessoa como usuário individual substitui todos os outros, exceto os modelos de layout provenientes de um perfil comercial. Você pode sobrepor uma atribuição anterior feita a um usuário individual fazendo uma nova atribuição; a mais recente tem prioridade.
* **Função de trabalho principal**: se não for atribuído um modelo de layout à pessoa como um único usuário, ela verá o modelo atribuído para sua função de trabalho principal.

  Somente o modelo de layout atribuído à função de trabalho principal de um usuário é visível para o usuário. Os modelos atribuídos a quaisquer funções de trabalho secundárias mantidas pelo usuário não estão visíveis.

* **Equipe da página inicial**: se não for atribuído um modelo de layout à pessoa como usuário individual ou como usuário com uma função de trabalho primária, ela verá o modelo atribuído à sua equipe inicial.

  Somente o modelo atribuído à equipe inicial de um usuário é visível para o usuário. Os modelos atribuídos a outras equipes nas quais o usuário é membro não estão visíveis.

* **Grupo padrão**: se não for atribuído um modelo de layout à pessoa como usuário individual, como usuário com função de trabalho primária ou como membro de uma equipe padrão, ela verá o modelo atribuído ao seu grupo padrão.

  Somente o modelo atribuído ao Grupo inicial de um usuário é visível para o usuário. Os modelos atribuídos a qualquer um de seus outros grupos não estão visíveis.

* **Nível de acesso**: se não for atribuído um modelo de layout à pessoa como usuário individual, como usuário com função de trabalho primária, como membro de uma Equipe da página inicial ou como membro de um Grupo da página inicial, ela verá o modelo atribuído ao seu nível de acesso.

## Grande número de usuários atribuídos a um modelo de layout

<!--
If you edit a layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.
-->
Se você tiver mais de 2000 usuários para atribuir a um modelo de layout, recomendamos executar um dos seguintes procedimentos:

* Organize os usuários em grupos ou equipes e atribua o modelo de layout a esses grupos ou equipes. Para obter mais informações, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Criar e gerenciar equipes](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Atribua funções de trabalho aos usuários e atribua o modelo de layout à sua função de trabalho principal. Para obter mais informações, consulte [Criar e gerenciar funções no trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
