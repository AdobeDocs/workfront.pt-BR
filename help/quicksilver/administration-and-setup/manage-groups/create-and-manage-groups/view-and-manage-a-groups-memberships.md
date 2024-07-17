---
user-type: administrator
product-area: system-administration;user-management
keywords: adicionar,usuários,grupo,adicionar,outro,atribuir,administrador,remover,usuário,exibir,funções,membros,exportação,associação,dados
navigation-topic: create-and-manage-groups
title: Exibir e gerenciar associações de um grupo
description: Como administrador do Adobe Workfront, você pode exibir, adicionar, remover, exportar, ativar e desativar membros de qualquer grupo gerenciado. Você também pode editar os perfis, adicionar Atualizações aos perfis e atribuí-los como administradores de grupo adicionais para o grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 1%

---

# Exibir e gerenciar associações de um grupo

Como administrador do Adobe Workfront, você pode exibir, adicionar, remover, exportar, ativar e desativar membros de qualquer grupo gerenciado. Você também pode editar os perfis, adicionar Atualizações aos perfis e atribuí-los como administradores de grupo adicionais para o grupo.

Se houver algum grupo acima do seu, os administradores também poderão fazer essas coisas pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença, contate o administrador do Workfront.

## Exibir e gerenciar associações de um grupo

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos**.

   Na lista exibida, os administradores do Workfront podem ver todos os grupos e subgrupos. Os administradores de grupo podem visualizar apenas os grupos e subgrupos que administram.

1. Clique no nome do grupo que deseja editar.
1. Na página exibida, com **Membros do Grupo** selecionados no menu à esquerda, siga um destes procedimentos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Adicionar um usuário ao grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Clique em <strong>Adicionar membros</strong> <img src="assets/add-icon-plus-in-circle.png">, comece a digitar o nome do usuário e, em seguida, selecione-o quando ele for exibido.</li> 
        <li value="2"> <p>Repita isso para qualquer outro usuário que desejar adicionar.</p> <p>Você pode clicar no X à direita de um nome se decidir não adicionar esse usuário.</p> </li> 
        <li value="3">Clique em <strong>Concluído</strong> quando terminar.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Remover um usuário do grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecione um ou mais nomes de usuário e clique em <strong>Remover membro</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>Clique em <strong>Remover</strong> na mensagem de aviso exibida.</p> <p>Você pode encontrar um usuário que deseja remover da lista clicando em <strong>Pesquisar pessoas e grupos na lista</strong>, digitando seu nome na caixa e clicando no nome quando ele for exibido.</p> <p><b>NOTA</b>:  
          <ul> 
           <li>Se esse for o Grupo padrão de um usuário que você deseja remover, atribua outro Grupo padrão no perfil do usuário. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">Visão geral de Grupos Domésticos</a> e <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de um usuário</a>.</li> 
           <li>Se o grupo tiver apenas um administrador de grupo e você precisar removê-lo do grupo, será necessário atribuir outro administrador de grupo ao grupo primeiro.</li> 
           <li>Um usuário pode pertencer individualmente a um subgrupo, bem como ao grupo principal. Quando você remove alguém de um subgrupo, ele permanece como parte do grupo principal. Da mesma forma, ao removê-los do grupo principal, eles permanecerão como parte do subgrupo. Se você não quiser que um usuário tenha o acesso permitido para o grupo pai, remova o usuário dos subgrupos, bem como do grupo pai, se eles estiverem listados em ambos os locais individualmente.</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Editar informações de perfil de um usuário</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecione um ou mais nomes de usuário e clique em <strong>Editar</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>Alterar as informações de perfil do usuário.</p> <p>Para obter informações sobre as alterações que você pode fazer, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de um usuário</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportar dados de associação do usuário</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecione um ou mais nomes de usuário e clique em <strong>Exportar</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>Exporte os dados como um arquivo delimitado por PDF, Excel ou tabulação.</p> <p>Para obter mais informações sobre como exportar dados, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar dados</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exibir e editar funções de grupo dos membros</td> 
      <td> <p>A coluna <strong>Função do Grupo</strong> lista a função de cada membro. Como administrador de grupo, você pode clicar duas vezes na função de um membro para alterá-la.</p> <p>Para membros do grupo que não são administradores de grupo, esta coluna não é editável.</p> <p>Os administradores de grupo estão sempre no topo da lista.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Enviar um comentário aos membros do grupo</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">Selecione um ou mais nomes de usuário e clique em <strong>Atualizar</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">Digite o comentário.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ativar um usuário no Workfront</td> 
      <td>Selecione um ou mais usuários inativos e clique em <strong>Ativar usuário</strong> para ativá-los no Workfront. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desativar um usuário no Workfront</td> 
      <td>Selecione um ou mais usuários ativos e clique em <strong>Desativar usuário</strong><img src="assets/deactivate-user.png"> para desativá-los no Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Classificar por coluna</td> 
      <td>Clique no cabeçalho de uma coluna para classificar a lista pelo conteúdo dessa coluna.</td> 
     </tr> 
    </tbody> 
   </table>
