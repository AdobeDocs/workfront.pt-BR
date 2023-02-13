---
title: Editar as configurações de um grupo na área Configuração
description: Como administrador do Adobe Workfront, você pode editar as configurações de uma equipe na área Configuração. Você pode adicionar usuários a uma equipe, definir um modelo de layout da equipe e definir como o status é registrado quando os itens de trabalho são concluídos por uma equipe.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 3%

---

# Editar as configurações de um grupo na área Configuração

Como administrador do Adobe Workfront, você pode editar as configurações de uma equipe na área Configuração. Você pode adicionar usuários a uma equipe, definir um modelo de layout da equipe e definir como o status é registrado quando os itens de trabalho são concluídos por uma equipe.

Para obter informações sobre as equipes, consulte [Visão geral das equipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Um administrador de grupo pode editar as configurações de uma equipe para um grupo que ele administra. Para obter mais informações, consulte [Criar e modificar as equipes de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Um usuário com uma licença de Plano pode editar as configurações de uma equipe na área Pessoas. Para obter mais informações, consulte [Editar configurações do grupo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
>


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
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Editar as configurações de um grupo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Equipes** no painel esquerdo.
1. Selecione um grupo e clique em **Editar** ![](assets/edit-icon.png).

1. Faça qualquer uma das seguintes alterações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome da equipe</td> 
      <td>Digite um nome para a equipe.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Está ativo </td> 
       <td>Essa opção é ativada por padrão para equipes novas e existentes. Desative-o para desativar a equipe. Para obter mais informações, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Desativar uma equipe</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Grupo</td> 
      <td> <p>Associe a equipe a um grupo. Comece digitando o nome do grupo e selecione o nome quando ele for exibido.</p> <p><b>OBSERVAÇÃO</b>: Quando uma equipe é atribuída a um grupo ou subgrupo, qualquer administrador de grupo desse grupo ou subgrupo pode gerenciar a equipe sem ser membro dele. Os administradores de grupo podem ir para a área Equipes no Menu principal e clicar na seta Alternar equipes <img src="assets/switch-team-icon.png" alt="Ícone Alternar equipe"> para listar todas as equipes atribuídas aos grupos que gerenciam.</p> <p>Você pode associar o grupo certo à equipe, passando o mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Isso exibe uma dica de ferramenta listando informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietário</td> 
      <td>Selecione um proprietário para a equipe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membros da Equipe</td> 
      <td> <p>Adicionar e membros da equipe. Comece a digitar o nome de um usuário e selecione o nome quando ele for exibido. Repita esse processo para adicionar vários usuários à equipe.</p> 
      <p><b>DICA</b>: Você pode adicionar qualquer número de usuários a uma equipe. No entanto, recomendamos que você não adicione um número excessivamente grande em uma equipe, porque a gestão do trabalho da equipe pode se tornar complexa demais.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição para a equipe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modelo de Layout</td> 
      <td> <p>Comece digitando o nome do modelo de layout que deseja que a equipe use e clique nele quando ele for exibido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agile</td> 
      <td>Especifique se esta é uma equipe ágil. Para obter informações sobre equipes ágeis e como gerenciar seu trabalho, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Criar uma equipe ágil</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. Clique em **Salvar alterações**.
