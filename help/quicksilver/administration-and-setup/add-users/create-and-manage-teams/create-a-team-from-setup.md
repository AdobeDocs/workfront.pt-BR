---
title: Criar um grupo na área Configuração
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Como administrador do Adobe Workfront, você pode criar uma equipe na área Configuração.
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---

# Criar um grupo na área Configuração

Como administrador do Adobe Workfront, você pode criar uma equipe na área Configuração. Para obter informações sobre as equipes, consulte [Visão geral das equipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Um administrador de grupo pode criar uma equipe para um grupo que ele administra na área Configuração. Para obter mais informações, consulte [Criar e modificar as equipes de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Um usuário com uma licença de Plano também pode criar uma equipe da área Pessoas. Para obter mais informações, consulte [Criar um grupo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
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

## Criar um grupo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Equipes**, depois clique em **Nova equipe**.

1. No **Nova equipe** , especifique as seguintes informações:

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
      <td> <p>Se quiser associar a equipe a um grupo, comece a digitar o nome do grupo e selecione o nome quando ele for exibido.</p> <p>Você pode associar o grupo certo à equipe, passando o mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Isso exibe uma dica de ferramenta listando informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> <p><b>OBSERVAÇÃO</b>: Quando uma equipe é atribuída a um grupo ou subgrupo, qualquer administrador de grupo desse grupo ou subgrupo pode gerenciar a equipe sem ser membro dele. Os administradores de grupo podem ir para a área Equipes no Menu principal e clicar na seta Alternar equipes <img src="assets/switch-team-icon.png" alt="Ícone Alternar equipe"> para listar todas as equipes atribuídas aos grupos que gerenciam.</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Esta é uma Equipe Agile</td> 
      <td>Selecione este item se quiser configurar esta nova equipe como uma equipe ágil. Para obter mais informações sobre equipes ágeis, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Criar uma equipe ágil</a>.</td> 
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

1. Clique em **Criar equipe**.

## Proprietários da equipe

Por padrão, ao criar uma equipe, você se torna o proprietário da equipe.

Você pode exibir os proprietários da equipe de todas as equipes ao criar um relatório para as equipes e incluir o campo Nome do proprietário no relatório. (Para obter mais informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
