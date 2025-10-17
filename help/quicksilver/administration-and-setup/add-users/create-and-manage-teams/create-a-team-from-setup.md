---
title: Criar uma equipe da área de configuração
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Como administrador do Adobe Workfront, você pode criar uma equipe na área Configuração.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 4%

---

# Crie uma equipe na área Configuração

Como administrador do Adobe Workfront, você pode criar uma equipe na área Configuração. Para obter informações sobre equipes, consulte [Visão geral das equipes](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* Um administrador de grupo pode criar uma equipe para um grupo que administra na área Configuração. Para obter mais informações, consulte [Criar e modificar as equipes de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* Um usuário com uma licença Padrão ou Plano também pode criar uma equipe na área Equipes. Para obter mais informações, consulte [Criar uma equipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

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

## Criar uma equipe

{{step-1-to-setup}}

1. Clique em **Equipes** e em **Nova Equipe**.

1. Na caixa **Nova Equipe** que é exibida, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome da equipe</td> 
      <td>Digite um nome para o grupo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupo</td> 
      <td> <p>Se quiser associar uma equipe a um grupo, comece digitando o nome do grupo, em seguida, selecione o nome quando ele aparecer.</p> <p>Você pode verificar se está associando o grupo correto à equipe, passando o cursor do mouse sobre ele e clicando no ícone de informações <img src="assets/info-icon.png"> que é exibido ao lado dele. Uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> <p><b>OBSERVAÇÃO</b>: quando uma equipe é atribuída a um grupo ou subgrupo, qualquer administrador desse grupo ou subgrupo pode gerenciar a equipe sem ser membro dele. Os administradores de grupo podem ir para a área Equipes no menu principal e clicar na seta Trocar equipes <img src="assets/switch-team-icon.png" alt="Ícone Trocar equipe"> para listar todas as equipes atribuídas aos grupos que eles gerenciam.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Membros da equipe</td> 
      <td> <p>Comece a digitar o nome de um usuário para fazer parte da equipe e selecione o nome quando o no for exibido na lista suspensa. Repita esse processo para adicionar vários usuários à equipe.</p> <p>Não há limite para quantos usuários você pode adicionar a uma equipe. No entanto, recomendamos não ter um número excessivamente grande de usuários em uma equipe, pois o gerenciamento de trabalho da equipe pode se tornar muito complexo.</p> </td> 
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
      <td role="rowheader">Esta é uma Equipe Ágil</td> 
      <td>Selecione este item se você deseja configurar esta nova equipe para ser uma equipe ágil. Para obter mais informações sobre equipes ágeis, consulte <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Criar uma equipe ágil</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Trabalhar na tarefa</td> 
      <td>Altere o botão Trabalhar na tarefa para um botão Iniciar. Quando um usuário clica em Iniciar, o status do item é atualizado automaticamente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botão Concluído</td> 
      <td>Selecione o status que deseja definir para os itens quando clicar no botão Concluído.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Criar Equipe**.

## Proprietários da equipe

Ao criar uma equipe, você se torna o proprietário da equipe, por padrão.

É possível visualizar os proprietários de todas as equipes ao criar um relatório para equipes e incluir o campo Nome do proprietário no relatório. (Para obter mais informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
