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
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 4%

---

# Atribuir usuários a um modelo de layout

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

É possível atribuir um modelo de layout criado a qualquer usuário, função de trabalho, equipe ou grupo que precise usá-lo.

Para usuários que não têm um modelo de layout atribuído a eles, o layout padrão é usado. Para saber mais sobre o layout padrão, consulte [Sobre o layout padrão do Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Os usuários também podem atribuir um modelo de layout a si mesmos, conforme descrito em Alterar as áreas Meu trabalho e Solicitações de trabalho com modelos de layout.

É possível atribuir vários modelos de layout diferentes para o mesmo nome. Para obter mais informações sobre qual modelo de layout está em vigor para um usuário, função, grupo ou equipe, consulte [Prioridade de atribuição de modelo de layout](#layout-template-assignment-priority), mais adiante neste artigo.

Para obter mais informações sobre modelos de layout, consulte [Modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

<span class="preview">Para obter informações sobre modelos de layout e perfis comerciais, consulte [Visão geral dos perfis comerciais](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/business-profiles.md).</span>

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
1. Na caixa exibida, clique em **Adicionar um usuário, função de trabalho, equipe, grupo, <span class="preview">ou nível de acesso</span>**, comece digitando o nome de um usuário, função de trabalho, equipe, grupo, <span class="preview">ou nível de acesso</span> e, em seguida, clique no nome quando ele aparecer no menu suspenso.

   Os nomes adicionados recentemente são exibidos com um plano de fundo azul. Isso é útil ao editar um modelo de layout existente, pois é possível distinguir os nomes que você acabou de adicionar daqueles que já estavam na lista.

   Um ícone Informações ![ícone Informações](assets/info-icon.png) é exibido à direita do nome de qualquer usuário, função de trabalho, equipe, grupo, <span class="preview">ou nível de acesso</span> que já esteja atribuído a outro modelo de layout. Você pode passar o mouse sobre o ícone para ver o nome desse modelo de layout e decidir se deseja sobrepor a atribuição existente.

1. Repita as duas etapas anteriores para atribuir o modelo de layout a outros usuários, funções de trabalho, equipes, grupo, <span class="preview">ou nível de acesso</span>, conforme necessário.

   É possível atribuir até 100 usuários de cada vez.

1. Clique em **Concluído** e em **Salvar e fechar** no canto inferior esquerdo.

   Esta etapa conclui o processo de criação e atribuição de um modelo de layout.

## Prioridade de atribuição do modelo de layout {#layout-template-assignment-priority}

Você e outros administradores do Workfront podem atribuir vários modelos de layout diferentes para o mesmo usuário destas quatro maneiras diferentes:

* Para o usuário individual
* Para uma função de trabalho específica, o usuário tem
* Para uma determinada equipe da qual o usuário faz parte
* Para um determinado grupo em que o usuário está
* <span class="preview">Para um determinado nível de acesso, o usuário é atribuído</span>

No entanto, somente um modelo de layout fica visível para o usuário em um determinado momento. O modelo visível é determinado pela seguinte hierarquia de prioridade:

* **Usuário individual**: o modelo de layout atribuído à pessoa como um usuário individual substitui todos os outros. Você pode sobrepor uma atribuição anterior feita para um usuário individual fazendo uma nova atribuição; a mais recente tem prioridade.
* **Função de trabalho principal**: se não for atribuído um modelo de layout à pessoa como um único usuário, ela verá o modelo atribuído para sua função de trabalho principal.

  Somente o modelo de layout atribuído à função de trabalho principal de um usuário é visível para o usuário. Os modelos atribuídos a quaisquer funções de trabalho secundárias mantidas pelo usuário não estão visíveis.

* **Equipe da página inicial**: se não for atribuído um modelo de layout à pessoa como usuário individual ou como usuário com uma função de trabalho primária, ela verá o modelo atribuído à sua equipe inicial.

  Somente o modelo atribuído à equipe inicial de um usuário é visível para o usuário. Os modelos atribuídos a outras equipes nas quais o usuário é membro não estão visíveis.

* **Grupo padrão**: se não for atribuído um modelo de layout à pessoa como usuário individual, como usuário com função de trabalho primária ou como membro de uma equipe padrão, ela verá o modelo atribuído ao seu grupo padrão.

  Somente o modelo atribuído ao Grupo inicial de um usuário é visível para o usuário. Os modelos atribuídos a qualquer um de seus outros grupos não estão visíveis.

* <span class="preview"> Nível de acesso: se não for atribuído um modelo de layout à pessoa como usuário individual, como usuário com função de trabalho primária, como membro de uma Equipe da página inicial ou como membro de um Grupo da página inicial, ela verá o modelo atribuído ao seu nível de acesso.</span>

## Grande número de usuários atribuídos a um modelo de layout

<!--
If you edit a layout template which is assigned to more than 2000 users and make changes to it, only the first 2000 users will be retained on the layout template and will see the changes you made. The layout template is removed from all others.
-->
Se você tiver mais de 2000 usuários para atribuir a um modelo de layout, recomendamos executar um dos seguintes procedimentos:

* Organize os usuários em grupos ou equipes e atribua o modelo de layout a esses grupos ou equipes. Para obter mais informações, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Criar e gerenciar equipes](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Atribua funções de trabalho aos usuários e atribua o modelo de layout à sua função de trabalho principal. Para obter mais informações, consulte [Criar e gerenciar funções no trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
