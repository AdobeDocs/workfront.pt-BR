---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Criar [!DNL Adobe Workfront] tarefas de [!DNL Microsoft] Equipes
description: Você pode criar tarefas pessoais no Adobe [!DNL Workfront] a partir do Microsoft Teams se um proprietário de equipe tiver instalado e configurado [!DNL Workfront] o para o Microsoft Teams para sua equipe e você estiver conectado ao Workfront a partir do Microsoft Teams.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
TQID: https://experienceleague.adobe.com/EGXeEO-HU8813eA-dyVAuKSv6rAQg8tsDiDT5leVee0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: a7ef0b24-c866-4849-a368-53678af2dfe5
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 31%

---

# Criar [!DNL Adobe Workfront] tarefas a partir de [!DNL Microsoft Teams]

>[!IMPORTANT]
>
>Como a [Microsoft faz a transição para o novo cliente Teams](https://learn.microsoft.com/pt-br/microsoftteams/teams-classic-client-end-of-availability), o cliente Classic Teams não estará mais disponível após 1º de julho de 2025. Para continuar usando o Microsoft Teams e aplicativos integrados como o Workfront, os clientes devem fazer a transição para o novo cliente Teams antes dessa data.
>
>A integração atualizada do Workfront já está disponível e é totalmente compatível com a nova experiência do Teams. Na maioria dos casos, o Workfront aparecerá automaticamente assim que os usuários tiverem feito a transição. Caso contrário, a integração pode ser instalada manualmente a partir da App Store do Microsoft Teams. Para instalar ou verificar a integração do Workfront no novo cliente do Teams, consulte [Instalar [!DNL Adobe Workfront] para Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).



## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <td> <p>Padrão</p>
   <p>Trabalho ou maior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você pode criar tarefas pessoais em [!DNL Adobe Workfront] a partir de [!DNL Microsoft Teams] se as seguintes condições forem atendidas:

* Um proprietário de equipe instalou e configurou o [!DNL Workfront for Microsoft Teams] para sua equipe.
* Você está logado em [!DNL Workfront] a partir de [!DNL Microsoft Teams].

>[!NOTE]
>
>[!DNL Microsoft Teams] não dá mais suporte a [!DNL Internet Explorer]. Para usar a integração do [!DNL Adobe Workfront for Microsoft Teams], você deve usar um navegador da Web diferente do [!DNL Internet Explorer].

Para obter informações sobre como instalar o [!DNL Workfront for Microsoft Teams] e fazer logon no [!UICONTROL Workfront] a partir do [!DNL Microsoft Teams], consulte [Instalar [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## Criar tarefas pessoais de [!DNL Microsoft Teams]

1. Faça logon em [!DNL Workfront] a partir de [!DNL Microsoft Teams].

   Para obter informações sobre como fazer logon no [!DNL Workfront], consulte [Instalar [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. Para abrir o cartão **[!UICONTROL Nova tarefa]**:

   * Se você estiver no canal de chat do bot [!DNL Workfront], digite **[!UICONTROL Nova tarefa]** no campo [!UICONTROL conversa] para criar uma nova tarefa.
   * Se você estiver em um canal de chat diferente do canal de chat do bot [!DNL Workfront]:

      * Comece digitando **[!DNL @workfront]** no campo [!UICONTROL conversa] e selecione o canal de bot [!DNL Workfront] desejado.
      * Continue digitando **[!UICONTROL Nova tarefa]** no campo [!UICONTROL conversa] para criar uma nova tarefa.

        O cartão [!UICONTROL Nova tarefa] é exibido no canal de bot [!DNL Workfront].

        ![ms_team_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. No canal de bot [!UICONTROL Workfront], especifique as seguintes informações no cartão [!UICONTROL Nova tarefa]:

   * Nome da tarefa no campo **[!UICONTROL Escrever o título da tarefa]**.
   * Descrição da tarefa no campo **[!UICONTROL Escrever a descrição da tarefa]**.
   * A data até a qual a tarefa deve ser concluída, no campo **[!UICONTROL Data de Conclusão]**.

1. Clique em **[!UICONTROL Salvar].**

   A nova tarefa pessoal foi criada em [!DNL Workfront]. Um [!UICONTROL Número de Referência] está atribuído a ele e visível no cartão [!UICONTROL nova tarefa].

   Para obter informações sobre números de referência, consulte a seção [[!UICONTROL Números de Referência] de objetos](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) no artigo [Entender objetos em [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Opcional) Clique em **[!UICONTROL Editar]** para editar ainda mais as informações da tarefa.
1. (Opcional) Clique em **[!UICONTROL Exibir em[!DNL Workfront]]** para abrir a tarefa em uma nova guia em [!DNL Workfront] e continuar a editar a tarefa, movê-la para um projeto ou atribuí-la a outra pessoa.
