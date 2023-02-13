---
title: Exibir o número de licenças alocadas e usadas em um grupo
description: Como administrador do Adobe Workfront, você pode visualizar as contagens dos tipos individuais de licenças usadas atualmente no seu grupo e em seus subgrupos. Isso é útil quando você precisa avaliar se deseja redistribuir licenças.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Exibir o número de licenças alocadas e usadas em um grupo

Como administrador do Adobe Workfront, você pode visualizar as contagens dos tipos individuais de licenças usadas atualmente no seu grupo e em seus subgrupos. Isso é útil quando você precisa avaliar se deseja redistribuir licenças.

Se houver algum grupo acima do grupo que você gerencia, os administradores também poderão fazer isso para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!IMPORTANT]
>
>A licença de um usuário é contada em um grupo específico somente se o grupo for o Grupo doméstico do usuário.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Plano Workfront</a>*</td> 
   <td> <p>Equipe ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Licença Adobe Workfront</a>*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Exibir o número de licenças usadas em um grupo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo.
1. Na página que é exibida, na área de cabeçalho próxima ao canto superior direito, visualize o **Licenças em uso** para ver o número de **Plano** e **Trabalho** licenças em uso.

   Se você estiver visualizando um grupo de nível superior e o administrador do Workfront tiver definido um número máximo de cada tipo de licença para o grupo, esses números também serão exibidos. Por exemplo, no grupo abaixo, um máximo de 10 usuários pode ter uma licença de Plano e um 15 pode ter uma licença de Trabalho:

   ![](assets/licenses-used-allocated.png)

   Para obter informações sobre como um administrador do Workfront define um número máximo de licenças alocadas para um grupo, consulte a seção [Definir a contagem máxima de licenças para um Grupo Doméstico](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) no artigo [Gerencie as licenças disponíveis em seu sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Se o grupo que você está visualizando for um subgrupo, você poderá exibir apenas os números de licenças usadas, não o número máximo de licenças alocadas para o grupo. Isso ocorre porque os administradores do Workfront não definem uma contagem máxima de licenças para um subgrupo.
   >
   >![](assets/subgroup-used-licenses-only.png)

1. Para contagens separadas de cada tipo de licença usada atualmente no grupo (incluindo Revisar e Solicitar), clique na área de texto logo abaixo **Licenças em uso:**

   ![](assets/click-text-to-see-more.png)

   A caixa que é exibida fornece as mesmas informações para todos os quatro tipos de licença do Workfront: Planejar, trabalhar, revisar e solicitar. Na parte inferior da caixa, é possível ver o número total de licenças usadas por membros desse grupo ou por um de seus subgrupos:

   ![](assets/more-license-info.png)

   Para licenças de Revisão e Solicitação, a coluna Máx sempre exibe Ilimitado.
