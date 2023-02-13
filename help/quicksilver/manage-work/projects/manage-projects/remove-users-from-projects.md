---
product-area: projects;user-management
navigation-topic: manage-projects
title: Remover usuários de projetos
description: Você pode remover usuários de um projeto quando eles não estiverem mais envolvidos na conclusão do trabalho no projeto.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 301c86152340a184345bd39cec77fdcf28258196
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Remover usuários de projetos

Você pode remover usuários de um projeto quando eles não estiverem mais envolvidos na conclusão do trabalho no projeto. A remoção de usuários de projetos tem implicações em atribuições de tarefas e de emissão, bem como em funções de projeto. Os usuários removidos param de receber notificações destinadas à Equipe do projeto. Para obter mais informações sobre notificações para as equipes de projeto, consulte [Notificações de evento disponíveis no Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Os usuários associados a um projeto são listados na área Pessoas de um projeto. Eles representam a equipe do projeto. Para obter mais informações sobre a Equipe do projeto, consulte [Visão geral da equipe do projeto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Como a remoção de um usuário afeta tarefas, problemas e projetos existentes

Quando um usuário é removido de um projeto, qualquer tarefa ou problema atribuído a ele pode ser afetado, dependendo se a tarefa ou problema foi concluído quando o usuário foi removido:

* **Se o item não estiver concluído quando o usuário for removido:** O item é re-atribuído a uma função de trabalho se uma função de trabalho já tiver sido atribuída ou se for atribuída à função de trabalho que o usuário estava preenchendo no item. Se o item ou o usuário não tiver uma função de trabalho atribuída, você deverá reatribuir manualmente o item.
* **Se o item for concluído quando o usuário for removido:** O nome do usuário removido permanece no item.
* **Se o usuário removido também for o criador de um projeto:** O projeto não é removido de suas **Projetos em que estou** na área Projetos . O projeto é removido das listas para todos os outros usuários que filtram para esse projeto pelo campo Inserido por .
* **Se o usuário for o Proprietário ou Patrocinador do projeto:** O usuário permanece em suas funções como patrocinador ou proprietário do projeto.

## Remover usuários de um projeto e da Equipe do projeto

Você pode remover usuários de um projeto, removendo-os da Equipe do projeto.

Quando os usuários desempenham funções em um projeto, eles se tornam parte da Equipe do projeto.

Quando você remove os usuários de suas funções no projeto, eles permanecem parte da equipe do projeto.

Para obter informações sobre as funções dos usuários em um projeto, consulte [Gerenciar a equipe do projeto](../planning-a-project/manage-project-team.md).

Para remover usuários da Equipe do projeto:

1. Vá para o projeto onde deseja remover os usuários.

1. Clique em **Pessoas** no painel esquerdo, selecione os usuários que deseja remover. Talvez seja necessário clicar em **Mostrar mais**, em seguida **Pessoas**.

1. Clique no botão **Remover** ícone  ![Remover item](assets/remove-icon---x-in-circle.png) na parte superior da lista de usuários.

1. Clique em **Sim, Remover Usuários Selecionados** para confirmar a remoção.

   Os usuários são removidos da equipe do projeto e de qualquer tarefa ou problema incompleto ao qual possam ser atribuídos. Eles não recebem mais notificações destinadas à Equipe do projeto.
