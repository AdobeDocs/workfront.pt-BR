---
product-area: projects;user-management
navigation-topic: manage-projects
title: Remover usuários dos projetos
description: Você pode remover usuários de um projeto quando eles não estiverem mais envolvidos na conclusão do trabalho no projeto.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Remover usuários dos projetos

Você pode remover usuários de um projeto quando eles não estiverem mais envolvidos na conclusão do trabalho no projeto. Remover usuários dos projetos tem implicações nas atribuições de tarefas e problemas, bem como nas funções do projeto. Usuários removidos param de receber notificações destinadas à Equipe do Projeto. Para obter mais informações sobre notificações para as equipes de projeto, consulte [Tipos de notificação de evento](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Os usuários associados a um projeto são listados na área Pessoas de um projeto. Eles representam a Equipe do Projeto. Para obter mais informações sobre a Equipe do Projeto, consulte [Visão geral da Equipe do Projeto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões no projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Como a remoção de um usuário afeta tarefas, problemas e projetos existentes

Quando um usuário é removido de um projeto, qualquer tarefa ou problema atribuído a ele pode ser afetado, dependendo se a tarefa ou problema foi concluído quando o usuário foi removido:

* **Se o item não estiver concluído quando o usuário for removido:** O item será reatribuído a uma função de trabalho se uma função de trabalho já tiver sido atribuída ou se estiver atribuída à função de trabalho que o usuário estava desempenhando no item. Se o item ou o usuário não tiver uma função de trabalho atribuída, será necessário reatribuir o item manualmente.
* **Se o item for concluído quando o usuário for removido:** O nome do usuário removido permanece no item.
* **Se o usuário removido também for o criador de um projeto:** O projeto não será removido da lista **Projetos em que estou** na área Projetos. O projeto é removido das listas de todos os outros usuários que filtram esse projeto pelo campo Informado por.
* **Se o usuário for o Proprietário ou Patrocinador do projeto:** o usuário permanecerá em suas funções como patrocinador ou proprietário do projeto.

## Remover usuários de um projeto e de uma equipe do projeto

Você pode remover usuários de um projeto removendo-os da Equipe do Projeto.

Quando os usuários desempenham funções em um projeto, eles se tornam parte da Equipe do projeto.

Quando você remove usuários de suas funções no projeto, eles permanecem como parte da equipe do projeto.

Para obter informações sobre as funções dos usuários em um projeto, consulte [Gerenciar a Equipe do Projeto](../planning-a-project/manage-project-team.md).

Para remover usuários da equipe do projeto:

1. Vá para o projeto em que deseja remover os usuários.

1. Clique em **Pessoas** no painel esquerdo e selecione os usuários que deseja remover.

1. Clique no ícone **Remover** ![Remover item](assets/remove-icon---x-in-circle.png) na parte superior da lista de usuários.

1. Clique em **Sim, remover usuários selecionados** para confirmar a remoção.

   Os usuários são removidos da equipe do projeto e de qualquer tarefa incompleta ou problema ao qual possam estar atribuídos. Eles não recebem mais notificações destinadas à Equipe do projeto.
