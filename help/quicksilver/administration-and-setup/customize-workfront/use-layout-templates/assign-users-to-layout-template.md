---
title: Atribuir usuários a um modelo de layout
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront, você pode atribuir um modelo de layout criado a qualquer usuário, função de trabalho, equipe ou grupo que precise usá-lo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a2915f3a-071f-4e9f-88c9-338bf765f418
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Atribuir usuários a um modelo de layout

Você pode atribuir um modelo de layout criado para qualquer usuário, função de trabalho, equipe ou grupo que precise usá-lo.

Para usuários que não têm um modelo de layout atribuído a eles, o layout padrão é usado. Para saber mais sobre o layout padrão, consulte [Sobre o layout padrão do Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Os usuários também podem atribuir um modelo de layout a eles mesmos, conforme descrito em Alterar as áreas de Meu trabalho e Solicitações de trabalho com modelos de layout.

É possível atribuir vários modelos de layout diferentes ao mesmo nome. Para obter mais informações sobre qual modelo de layout está em vigor para um usuário, função, grupo ou equipe, consulte [Prioridade de atribuição do modelo de layout](#layout-template-assignment-priority) mais tarde neste artigo.

Para obter mais informações sobre modelos de layout, consulte [Modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, é necessário o nível de acesso Administrador do sistema.
Para executá-los para um grupo, você deve ser um gerente desse grupo.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Atribuir um modelo de layout aos usuários

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

   >[!TIP]
   >
   >Quando estiver satisfeito com seu modelo de layout, recomendamos que você o teste, conforme descrito em [Teste de um novo modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md).

1. Clique em **Atribua isso a** na seção superior da página.
1. Na caixa exibida, clique em **Adicionar um usuário, função de trabalho, equipe ou grupo**, comece digitando o nome de um usuário, função de trabalho, equipe ou grupo e clique no nome quando ele for exibido no menu suspenso.

   Os nomes adicionados recentemente são exibidos com um plano de fundo azul. Isso é útil ao editar um modelo de layout existente, pois é possível distinguir os nomes que você acabou de adicionar daqueles que já estavam na lista.

   Um ícone Informações ![](assets/info-icon.png) é exibido à direita do nome de qualquer usuário, função de trabalho, equipe ou grupo já atribuído a outro modelo de layout. Você pode passar o mouse sobre o ícone para ver o nome desse modelo de layout e decidir se deseja substituir a atribuição existente.

1. Repita as duas etapas anteriores para atribuir o modelo de layout a outros usuários, funções de trabalho, equipes ou grupos, conforme necessário.

   Você pode atribuir até 100 usuários por vez.

1. Clique em **Concluído**, depois clique em **Salvar** no canto inferior esquerdo.

   Essa etapa conclui o processo de criação e atribuição de um template de layout.

## Prioridade de atribuição do modelo de layout {#layout-template-assignment-priority}

Você e outros administradores do Workfront podem atribuir vários modelos de layout diferentes ao mesmo usuário de quatro maneiras diferentes:

* Para o usuário individual
* Para uma função de trabalho específica que o usuário tem
* Para um determinado grupo, o usuário está
* Para um determinado grupo, o usuário está em

No entanto, somente um modelo de layout é visível para o usuário em qualquer momento. O modelo visível é determinado pela seguinte hierarquia de prioridade:

* **Usuário individual**: O modelo de layout atribuído à pessoa como um usuário individual substitui todos os outros. Você pode substituir uma atribuição anterior feita de forma que um usuário individual, fazendo uma nova atribuição; a mais recente tem precedência.
* **Função de trabalho principal**: Se a pessoa não receber um modelo de layout como um único usuário, ela verá o modelo atribuído para sua função de trabalho principal.

   Somente o modelo de layout atribuído à função de trabalho principal de um usuário é visível para ele. Os modelos atribuídos a quaisquer funções de trabalho secundárias detidas pelo usuário não são visíveis.

* **Equipe inicial**: Se a pessoa não receber um modelo de layout como um usuário individual, ou como um usuário com uma função de trabalho primária, ela verá o modelo atribuído à equipe inicial.

   Somente o modelo atribuído à equipe inicial de um usuário é visível para ele. Modelos atribuídos a outras equipes em que um usuário é membro não estão visíveis.

* **Grupo doméstico**: Se a pessoa não receber um modelo de layout como um usuário individual, nem como um usuário com uma função de trabalho primária, nem como membro de uma equipe do Início, ela verá o modelo atribuído ao seu grupo do Início.

   Somente o modelo atribuído ao grupo Início de um usuário é visível para o usuário. Os modelos atribuídos a qualquer um de seus outros grupos não estão visíveis.

## Grande número de usuários atribuídos a um modelo de layout

Se você editar um modelo de layout atribuído a mais de 2000 usuários e fizer alterações nele, somente os primeiros 2000 usuários serão retidos no modelo de layout e verão as alterações feitas. O modelo de layout é removido de todos os outros.

Se você tiver mais de 2000 usuários para atribuir a um modelo de layout, recomendamos que execute um dos seguintes procedimentos:

* Organize os usuários em grupos ou equipes e atribua o modelo de layout a esses grupos ou equipes. Para obter mais informações, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Criar e gerenciar equipes](../../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

* Atribua funções de trabalho aos usuários e atribua o modelo de layout à função de trabalho principal. Para obter mais informações, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
