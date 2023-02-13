---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Gerenciar a equipe do projeto
description: A Equipe do projeto consiste em usuários associados ao projeto. Os membros da Equipe do projeto são exibidos na seção Pessoas do projeto.
author: Alina
feature: Work Management
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Gerenciar a equipe do projeto

A Equipe do projeto consiste em usuários associados ao projeto. Os membros da Equipe do projeto são exibidos na seção Pessoas do projeto.

## Requisitos de acesso

<!--drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>Editar acesso a Projetos</p> <p>Visualizar ou acessar mais alto os usuários</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou permissões mais altas para o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Adicionar usuários a uma equipe de projeto

Quando você adiciona usuários à equipe do projeto, eles recebem permissões de Exibição no projeto e nas tarefas, problemas e documentos do projeto. Para obter mais informações, consulte o artigo [Visão geral da equipe do projeto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Os usuários na Equipe do projeto não são adicionados automaticamente às ferramentas de gerenciamento de recursos do projeto.

Você pode adicionar usuários à equipe do projeto das seguintes maneiras:

* [Adicionar automaticamente usuários a uma equipe de projeto](#automatically-add-users-to-a-project-team)
* [Adicionar usuários manualmente a uma equipe de projeto](#manually-add-users-to-a-project-team)

### Adicionar automaticamente usuários a uma equipe de projeto {#automatically-add-users-to-a-project-team}

Os usuários que atendem às seguintes funções no projeto são automaticamente adicionados à equipe do projeto e aparecem na seção Pessoas quando o projeto é criado:

* O criador do projeto
* O proprietário do projeto
* O patrocinador do projeto

Os usuários também são adicionados automaticamente à equipe do projeto quando são atribuídos ao seguinte:

* Tarefas
* Problemas

### Adicionar usuários manualmente a uma equipe de projeto {#manually-add-users-to-a-project-team}

Se os usuários que não cumprirem nenhuma função no projeto quiserem ser notificados sobre determinadas atualizações ou alterações durante a vida útil do projeto, você poderá adicioná-las manualmente à equipe do projeto.

Para obter mais informações sobre quais notificações podem ser ativadas para usuários na equipe do projeto, consulte [Notificações de evento disponíveis no Adobe Workfront](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. Vá para o projeto ao qual deseja adicionar usuários.

1. Clique em **Pessoas** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais** primeiro.

1. Clique em **Adicionar usuários**.

   A caixa de diálogo Adicionar usuários à equipe do projeto é exibida.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. No **Adicionar usuários** , comece digitando o nome de um usuário ativo do Workfront que deseja adicionar à equipe do projeto e clique no nome quando ele for exibido na lista suspensa.

   Repita essa etapa para adicionar vários usuários à equipe do projeto. Os usuários devem pertencer ao grupo associado ao projeto.

   >[!TIP]
   >
   >* Não é possível adicionar usuários adicionando suas equipes, grupos, empresas ou funções de trabalho.
   >* À medida que você adiciona os usuários, observe o avatar, a função principal do usuário e seu endereço de email para distinguir entre usuários com nomes idênticos. Os usuários devem estar associados a pelo menos uma função de trabalho para exibi-la à medida que você os adiciona.



1. Clique em **Adicionar**.

   Os usuários recebem permissões de Visualização do projeto e recebem notificações sobre ele como parte da equipe do projeto.

## Remover usuários de uma equipe de projeto

Quando você remove os usuários de suas funções no projeto, eles permanecem parte da equipe do projeto.

Se você remover um usuário da equipe do projeto e ele for atribuído a tarefas ou problemas no projeto, ele não será atribuído das tarefas e problemas que não estiverem concluídos. Nesse caso, as tarefas e os problemas retornam à área de Trabalho Não Atribuído no Balanceador de Carga de Trabalho.

Os usuários atribuídos a tarefas concluídas e problemas permanecem atribuídos mesmo depois que você os remove da equipe do projeto.

Para obter mais informações sobre como remover usuários da equipe do projeto, consulte [Remover usuários de projetos](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
