---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Compartilhar um relatório de calendário
description: Você pode compartilhar um calendário com outros usuários e disponibilizá-lo publicamente, permitindo que alguém sem uma licença do  [!DNL Adobe Workfront]  o exiba.
author: Jenny
feature: Reports and Dashboards
exl-id: 77eed0fe-2d47-40c4-a03d-590f7fa17dbe
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 1%

---

# Compartilhar um relatório de calendário


Você pode compartilhar um calendário com outros usuários e disponibilizá-lo publicamente, permitindo que alguém sem uma licença do [!DNL Adobe Workfront] o visualize.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Leve</p>
       <p>Revisar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p> Acesso maior ou igual a relatórios, painéis e calendários</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Exibir permissões ou mais altas para o relatório de calendário, com acesso para compartilhar</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartilhar um calendário com [!DNL Workfront] usuários {#share-a-calendar-with-workfront-users}

O compartilhamento de um calendário é semelhante ao compartilhamento de outros objetos. Para obter mais informações sobre o compartilhamento de objetos em [!DNL Adobe Workfront], consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Os calendários compartilhados com você são exibidos com um asterisco (&#42;) ao lado do nome do calendário.

Para compartilhar um calendário dentro de [!DNL Workfront]:

1. Vá para o calendário que deseja compartilhar.
1. Clique no menu **Mais** ao lado do nome do calendário e clique em **Compartilhamento**.
   ![menu de calendário a mais](assets/more-menu-calendar.png)
1. No campo **[!UICONTROL Conceder acesso ao Calendário]**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa à qual deseja compartilhar o calendário e, em seguida, clique no nome quando ele for exibido na lista suspensa.\
   Para saber mais sobre como configurar permissões, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Opcional) Repita a etapa 3 para cada usuário, equipe, função ou grupo ao qual deseja conceder acesso ao calendário.
1. Especifique as permissões para cada usuário, equipe, função, grupo ou empresa adicionada na Etapa 3 clicando no menu suspenso e selecione o nível de permissão que deseja conceder:

   * **[!UICONTROL Exibir]:** Os usuários podem revisar e compartilhar o calendário.

     ![Compartilhar calendário com acesso de exibição](assets/view-calendar.png)

   * **[!UICONTROL Gerenciar]:** os usuários têm acesso total ao calendário, menos os direitos administrativos, que são concedidos no nível de acesso, mais todas as permissões de Exibição.

     ![Compartilhar calendário com acesso de gerenciamento](assets/manage-calendar.png)

     >[!NOTE]
     >
     >O administrador [!DNL Workfront] e o criador do calendário podem remover permissões dessas entidades.

1. (Opcional) Dependendo da função de um usuário, talvez você possa clicar em **[!UICONTROL Opções Avançadas]** e em **[!UICONTROL Compartilhar]**&#x200B; para permitir que o usuário compartilhe o calendário com outros usuários.

   Para obter mais informações sobre os níveis de permissões, consulte [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. (Opcional) Para disponibilizar o calendário para todos os usuários do [!DNL Workfront], clique no ícone de engrenagem e, no menu suspenso, clique em **[!UICONTROL Tornar isto visível em todo o sistema]** para disponibilizar o objeto para todos os usuários do [!DNL Workfront].\
   Todos os usuários podem ver o objeto com base nas permissões definidas.

1. Clique em **[!UICONTROL Salvar]**.

## Compartilhar um calendário com um link público

Você pode tornar um calendário público e compartilhar um link com pessoas que não têm uma licença do [!DNL Workfront].

1. Vá para o calendário que deseja compartilhar.
1. Clique em **[!UICONTROL Ações de Calendário]** e em **[!UICONTROL Compartilhamento]**.
1. Clique no menu **Mais** ao lado do nome do calendário.
   ![menu de calendário a mais](assets/more-menu-calendar.png)
Clique em **Copiar link público**.
1. Clique em **[!UICONTROL Salvar]**.

## Compartilhar um calendário com um link privado

Você pode compartilhar um link privado de calendário com [!DNL Workfront] usuários. Os usuários precisam fazer logon para exibir o calendário quando usam o link.

1. Vá para o calendário que deseja compartilhar.
1. Clique no menu **Mais** ao lado do nome do calendário e clique em **[!UICONTROL Obter link compartilhável]**.
   ![menu de calendário a mais](assets/more-menu-calendar.png)

   >[!NOTE]
   >
   >[!DNL Workfront] usuários devem ter acesso ao calendário para acessá-lo com o link. Para conceder acesso, consulte [Compartilhar um calendário com [!DNL Workfront] usuários](#share-a-calendar-with-workfront-users).\
   >Se os usuários não tiverem acesso, poderão solicitá-lo depois de colar o link em seus navegadores.
