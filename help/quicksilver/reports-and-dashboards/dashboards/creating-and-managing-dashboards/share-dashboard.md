---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Compartilhar um painel
description: O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar painéis ao atribuir níveis de acesso. Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir ou Gerenciar painéis específicos que você tenha acesso para compartilhar.
author: Nolan
feature: Reports and Dashboards
exl-id: 21bd531f-8732-4d6c-b91f-990887285447
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Compartilhar um painel

<!-- Audited: 1/2025 -->

O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar painéis ao atribuir níveis de acesso. Para obter mais informações sobre como conceder acesso a problemas, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir ou Gerenciar painéis específicos que você tenha acesso para compartilhar. Para obter mais informações sobre níveis de acesso e permissões, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
    <td> 
   <p>Leve ou superior</p>
   <p>Revisar ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de visualização ou superior a relatórios, painéis, calendários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores ao painel</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

O painel deve ser criado antes que você possa compartilhá-lo.

Para obter informações sobre como criar painéis, consulte [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Considerações sobre o compartilhamento de painéis

Além das considerações abaixo, consulte também [Compartilhar relatórios, painéis e calendários](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Por padrão, o criador de um painel tem Gerenciar permissões para ele.

* Você pode compartilhar painéis que cria com outros indivíduos, equipes, grupos, funções de trabalho ou empresas. Você também pode compartilhar painéis que outras pessoas criaram e que foram compartilhados com você.
* Você também pode compartilhá-los com toda a organização, tornando-a visível em todo o sistema.
* Você pode compartilhar um painel individual ou vários painéis de uma lista.
* Quando você compartilha um painel, os usuários herdam permissões de Exibição para todos os objetos de relatórios no painel, por padrão.

  Para obter mais informações sobre a hierarquia de objetos no Workfront, consulte [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Para obter informações sobre como visualizar permissões herdadas, consulte [Exibir permissões herdadas em objetos](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Compartilhar um painel

O compartilhamento de um ou vários painéis de uma lista é idêntico.

1. Vá para uma lista de painéis, selecione um ou vários painéis e clique em **Compartilhar** ![](assets/share-icon.png).

   Ou

   Clique no nome de um painel e em **Ações do Painel** > **Compartilhamento**.

   ![](assets/unshimmed-share-dashboard.png)

1. No campo **Adicionar pessoas, equipes, funções, grupos ou empresas**, comece digitando o nome do usuário, equipe, função, grupo ou empresa com a qual deseja compartilhar o painel e clique no nome quando ele aparecer na lista suspensa.
1. (Opcional) Para tornar o painel acessível a todos os usuários no sistema, clique no menu suspenso **Somente pessoas convidadas podem acessar** na caixa de diálogo de compartilhamento e selecione **Todos no sistema podem exibir**.

1. Clique em **Salvar**.
