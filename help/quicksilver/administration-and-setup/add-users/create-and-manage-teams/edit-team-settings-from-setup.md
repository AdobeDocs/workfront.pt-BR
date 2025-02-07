---
title: Editar as configurações de uma equipe na área de configuração
description: Como administrador do Adobe Workfront, você pode editar as configurações de uma equipe na área Configuração. Você pode adicionar usuários a uma equipe, definir um modelo de layout de equipe e definir como o status é registrado quando itens de trabalho são concluídos por uma equipe.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 3%

---

# Editar as configurações de uma equipe na área Configuração

Como administrador do Adobe Workfront, você pode editar as configurações de uma equipe na área Configuração. Você pode adicionar usuários a uma equipe, definir um modelo de layout de equipe e definir como o status é registrado quando itens de trabalho são concluídos por uma equipe.

Para obter informações sobre equipes, consulte [Visão geral das equipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Um administrador de grupo pode editar as configurações de uma equipe para um grupo que ele administra. Para obter mais informações, consulte [Criar e modificar as equipes de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Um usuário com uma licença Padrão ou de Plano pode editar as configurações de uma equipe na área Equipes. Para obter mais informações, consulte [Editar configurações da equipe](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar as configurações de uma equipe

{{step-1-to-setup}}

1. Clique em **Equipes** no painel esquerdo.
1. Selecione uma equipe e clique em **Editar** ![Editar ícone](assets/edit-icon.png).

1. Faça qualquer uma das seguintes alterações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome da equipe</td> 
      <td>Digite um nome para o grupo.</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Está ativo </td> 
       <td>Essa opção é ativada para equipes novas e existentes por padrão. Desative essa opção para desativar o grupo. Para obter mais informações, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">Desativar uma equipe</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Grupo</td> 
      <td> <p>Associar a equipe a um grupo. Comece digitando o nome do grupo e selecione o nome quando ele aparecer.</p> <p><b>OBSERVAÇÃO</b>: quando uma equipe é atribuída a um grupo ou subgrupo, qualquer administrador desse grupo ou subgrupo pode gerenciar a equipe sem ser membro dele. Os administradores de grupo podem ir para a área Equipes no menu principal e clicar na seta Trocar equipes <img src="assets/switch-team-icon.png" alt="Ícone Trocar equipe"> para listar todas as equipes atribuídas aos grupos que eles gerenciam.</p> <p>Você pode verificar se está associando o grupo correto à equipe, passando o cursor do mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proprietário</td> 
      <td>Selecione um proprietário para a equipe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membros da Equipe</td> 
      <td> <p>Adicionar e membros da equipe. Comece a digitar o nome de um usuário e selecione o nome quando ele for exibido. Repita esse processo para adicionar vários usuários à equipe.</p> 
      <p><b>DICA</b>: você pode adicionar qualquer número de usuários a uma equipe. No entanto, recomendamos que você não adicione um número excessivamente grande em uma equipe, pois a gestão de trabalho da equipe pode se tornar muito complexa.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição para a equipe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modelo de Layout</td> 
      <td> <p>Comece a digitar o nome do modelo de layout que você deseja que a equipe use e clique nele quando ele aparecer.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ágil</td> 
      <td>Especificar se é uma Equipe Ágil. Para obter informações sobre equipes ágeis e como gerenciar seu trabalho, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Criar uma equipe ágil</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Trabalhar na tarefa</td> 
      <td> <p>Altere o botão Trabalhar na tarefa para um botão Iniciar. Quando um usuário clica em Iniciar, o status do item é atualizado automaticamente.</p> <p>Para obter mais informações sobre como configurar o botão Iniciar, consulte <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">Substituir o botão Trabalhar na tarefa por um botão Iniciar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botão Concluído</td> 
      <td> <p>Personalize o botão Concluído. Para obter mais informações, consulte:</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">Configurar o botão Concluído para tarefas</a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">Configurar o botão Concluído para problemas</a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar alterações**.
