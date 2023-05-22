---
title: Exibir o número de licenças alocadas e usadas em um grupo
description: Como administrador do Adobe Workfront, você pode exibir contagens dos tipos individuais de licenças usados atualmente no seu grupo e seus subgrupos. Isso é útil quando você precisa avaliar se redistribui licenças.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: 0e8f8973ad4c1310b973bae4e6fe3578c05db204
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Exibir o número de licenças alocadas e usadas em um grupo

Como administrador do Adobe Workfront, você pode exibir contagens dos tipos individuais de licenças usados atualmente no seu grupo e seus subgrupos. Isso é útil quando você precisa avaliar se redistribui licenças.

Se houver algum grupo acima do grupo gerenciado por você, os administradores também poderão fazer isso pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!IMPORTANT]
>
>Uma licença de usuário é contada em um grupo específico somente se o grupo for o Grupo inicial do usuário.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir o tipo de plano ou licença que possui, entre em contato com o administrador do Workfront.

## Exibir o número de licenças usadas em um grupo

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo.
1. Na página exibida, na área de cabeçalho próxima ao canto superior direito, visualize o **Licenças em uso** área para ver o número de **Plano** e **Trabalho** licenças em uso no momento.

   Se você estiver visualizando um grupo de nível superior e o administrador do Workfront tiver definido um número máximo de cada tipo de licença para o grupo, esses números também serão exibidos. Por exemplo, no grupo abaixo, um máximo de 10 usuários pode ter uma licença de Plano e um máximo de 15 usuários pode ter uma licença de Trabalho:

   ![](assets/licenses-used-allocated.png)

   Para obter informações sobre como um administrador do Workfront define um número máximo de licenças alocadas para um grupo, consulte a seção [Definir a contagem máxima de licenças para um Grupo padrão](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set) no artigo [Gerenciar licenças disponíveis em seu sistema](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

   >[!NOTE]
   >
   >Se o grupo que você está observando for um subgrupo, você poderá ver somente os números de licenças que estão sendo usadas, não o número máximo de licenças alocadas para o grupo. Isso ocorre porque os administradores do Workfront não definem uma contagem máxima de licenças para um subgrupo.
   >
   >![](assets/subgroup-used-licenses-only.png)

1. Para contagens separadas de cada tipo de licença usada atualmente no grupo (incluindo Revisão e Solicitação), clique na área de texto diretamente abaixo **Licenças em uso:**

   ![](assets/click-text-to-see-more.png)

   A caixa que é exibida fornece as mesmas informações para todos os quatro tipos de licença do Workfront: Plano, Trabalho, Revisão e Solicitação. Na parte inferior da caixa, é possível ver o número total de licenças que estão sendo usadas pelos membros deste grupo ou de um de seus subgrupos:

   ![](assets/more-license-info.png)

   Para licenças de Revisão e Solicitação, a coluna Máximo sempre exibe Ilimitado.
