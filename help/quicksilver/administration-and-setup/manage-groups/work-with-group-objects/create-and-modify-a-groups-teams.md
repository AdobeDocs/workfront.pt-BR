---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Criar e modificar as equipes de um grupo
description: Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com equipes associadas ao grupo e a qualquer um de seus subgrupos.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# Criar e modificar as equipes de um grupo

Ao visualizar um grupo que você gerencia na área Grupos , é possível visualizar e trabalhar com equipes associadas ao grupo e a qualquer um de seus subgrupos.

Se houver algum grupo acima do seu grupo, os administradores também poderão fazer essas tarefas para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

Para obter informações sobre como os usuários com uma licença do Plano podem criar uma equipe, consulte [Criar um grupo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Para obter informações sobre como um administrador do Workfront pode criar uma equipe, consulte [Criar um grupo na área Configuração](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Exibir, trabalhar e criar equipes para seu grupo na área Grupos

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo para o qual você deseja criar ou modificar equipes.
1. No painel esquerdo, clique em **Equipes** ![](assets/teams.png) para listar as equipes associadas ao grupo e com quaisquer subgrupos que ele possa ter.

1. Siga um destes procedimentos:

   * **Adicionar uma equipe**: Clique em **Nova equipe** e use as seguintes opções para configurá-lo:
   <!-- WRITER please check table below. I stripped out wonky conditions-->

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Nome da equipe</td> 
       <td>Digite um nome para a equipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Grupo</td> 
       <td> <p> O sistema preenche o campo Grupo para o novo portfólio com o grupo que você está visualizando. Se quiser associar a equipe a um grupo diferente, comece a digitar o nome do grupo e selecione o nome quando ele for exibido.</p> <p>Você pode associar o grupo certo à equipe, passando o mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Isso exibe uma dica de ferramenta listando informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> <p><b>OBSERVAÇÃO</b>: Quando uma equipe é atribuída a um grupo ou subgrupo, qualquer administrador de grupo desse grupo ou subgrupo pode gerenciar a equipe sem ser membro dele. Os administradores de grupo podem ir para a área Equipes no Menu principal e clicar na seta Alternar equipes <img src="assets/switch-team-icon.png" alt="Ícone Alternar equipe"> para listar todas as equipes atribuídas aos grupos que gerenciam.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membros da Equipe</td> 
       <td> <p>Comece digitando o nome de um usuário que deve estar no grupo e depois selecione o nome quando for exibido na lista suspensa. Repita esse processo para adicionar vários usuários à equipe.</p> <p>Não há limite para quantos usuários você pode adicionar a uma equipe. No entanto, recomendamos não ter um número excessivamente grande de usuários em uma equipe, pois o gerenciamento de trabalho da equipe pode se tornar muito complexo.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descrição</td> 
       <td>Digite uma descrição para a equipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Calendário</td> 
       <td>Escolha qual guia de calendário será exibida para esta equipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Trabalhar na tarefa</td> 
       <td>Altere o botão Trabalhar nele para um botão Iniciar. Quando um usuário clica em Iniciar, o status do item é atualizado automaticamente.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Botão Concluído</td> 
       <td>Selecione o status que deseja definir para os itens quando o botão Concluído for clicado.</td> 
       </tr> 
      </tbody> 
     </table>

   * **Editar equipes**: Selecione pelo menos uma equipe, clique em **o** Ícone Editar ![](assets/edit-icon.png)e use as seguintes opções para configurá-lo:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">Nome da equipe</td> 
       <td>Digite um nome para a equipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Grupo</td> 
       <td> <p>Associe a equipe a um grupo. Comece digitando o nome do grupo e selecione o nome quando ele for exibido.</p> <p>Você pode associar o grupo certo à equipe, passando o mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Isso exibe uma dica de ferramenta listando informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> <p><b>OBSERVAÇÃO</b>: Quando uma equipe é atribuída a um grupo ou subgrupo, qualquer administrador de grupo desse grupo ou subgrupo pode gerenciar a equipe sem ser membro dele. Os administradores de grupo podem ir para a área Equipes no Menu principal e clicar na seta Alternar equipes <img src="assets/switch-team-icon.png" alt="Ícone Alternar equipe"> para listar todas as equipes atribuídas aos grupos que gerenciam.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Proprietário</td> 
       <td>Selecione um proprietário para a equipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Membros da Equipe</td> 
       <td> <p>Adicionar e membros da equipe. Comece a digitar o nome de um usuário e selecione o nome quando ele for exibido. Repita esse processo para adicionar vários usuários à equipe.</p> <p><b>DICA</b>: Não há limite para quantos usuários você pode adicionar a uma equipe. No entanto, recomendamos não ter um número excessivamente grande de usuários em uma equipe, pois o gerenciamento de trabalho da equipe pode se tornar muito complexo.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Descrição</td> 
       <td>Digite uma descrição para a equipe.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Modelo de Layout</td> 
       <td> <p>Comece digitando o nome do modelo de layout que deseja que a equipe use e clique nele quando ele for exibido.</p> <p>Ao designar a equipe com esse modelo de layout como a Equipe inicial dos usuários, todos os usuários dessa equipe visualizarão as personalizações nesse modelo de layout.<br>As configurações individuais do modelo de layout substituirão as configurações do modelo de layout da equipe inicial. </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Agile</td> 
       <td>Especifique se esta é uma equipe ágil. Para obter informações sobre equipes ágeis e como gerenciar seu trabalho, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Criar uma equipe ágil</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">Trabalhar na tarefa</td> 
       <td> <p>Altere o botão Trabalhar nele para um botão Iniciar. Quando um usuário clica em Iniciar, o status do item é atualizado automaticamente.</p> <p>Para obter mais informações sobre como configurar o botão Iniciar, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substitua o botão Trabalho nele por um botão Iniciar</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">Botão Concluído</td> 
       <td> <p>Personalize o botão Concluído . Para obter mais informações, consulte:</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configurar o botão Concluído para tarefas</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configure o botão Concluído para problemas</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **Excluir equipes**: Selecione pelo menos uma equipe e clique no ícone Excluir ![](assets/delete.png).
   * **Exportar a lista de equipes**: Clique em **Exportar** ![](assets/export.png), em seguida, selecione o formato de arquivo que deseja para a lista exportada.
