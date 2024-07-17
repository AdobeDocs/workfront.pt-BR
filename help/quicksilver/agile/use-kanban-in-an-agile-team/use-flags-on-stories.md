---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Usar sinalizadores em matérias no quadro Kanban
description: No quadro  [!DNL Kanban] , os sinalizadores fornecem uma indicação visual de quando uma história está pronta para ser movida para o próximo status. Isso permite que as equipes Kanban usem uma abordagem de "pull" em vez de uma abordagem de "push" ao mover histórias entre status.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Usar sinalizadores em histórias no quadro [!UICONTROL Kanban]

No quadro [!DNL Kanban], os sinalizadores fornecem uma indicação visual de quando uma história está pronta para ser movida para o próximo status. Isso permite que as equipes do [!UICONTROL Kanban] usem uma abordagem de &quot;pull&quot; em vez de uma abordagem de &quot;push&quot; ao mover histórias entre status.

**Exemplo:** Considere o seguinte exemplo de uma equipe usando uma abordagem &quot;pull&quot;: Olivia, a designer gráfica da equipe, conclui seu trabalho e define o sinalizador de história como &quot;[!UICONTROL Pronto para Puxar].&quot; Esta bandeira fornece uma indicação visual para Tony, o redator da equipe, de que a história está pronta para ele passar para o próximo status. Tony então muda a história para o próximo status quando ele está pronto para começar a trabalhar nela.

Considere o seguinte ao usar sinalizadores em matérias:

* Sinalizadores não são um status, mas uma indicação visual de que a história está pronta para ser movida para o próximo status por outro membro da equipe.
* Os sinalizadores não aparecem em nenhum cartão de história que esteja na coluna [!UICONTROL Backlog] ou na coluna [!UICONTROL Concluído] (ou em qualquer coluna em que o status da coluna seja igual a [!UICONTROL Concluído]).

  Para obter mais informações sobre status de matérias, consulte [Usar sinalizadores em matérias no quadro Kanban](#updating-the-status-of-stories-and-subtasks)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Work] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Usar sinalizadores em histórias no quadro [!UICONTROL Kanban]

Para alterar um sinalizador em uma matéria:

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do switch]** ![Ícone da equipe do switch](assets/switch-team-icon.png) e selecione uma nova equipe [!UICONTROL Kanban] no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Vá para o quadro [!UICONTROL Kanban] onde deseja alterar um sinalizador em uma história.
1. Expanda o bloco da história para exibir o sinalizador.\
   O sinalizador é definido como **[!UICONTROL No Rastreamento]** para cada matéria por padrão.\
   ![Cartão Kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Clique no sinalizador atual e selecione uma das seguintes opções de sinalizador:

   * **[!UICONTROL No Rastreamento]:** A história está no status apropriado e nenhuma ação precisa ser tomada neste momento.\

     Esse é o sinalizador padrão para cada matéria no quadro Kanban.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Está Bloqueado]:** A história não pode passar para o próximo status. Quando esse sinalizador é definido em uma matéria, a matéria não conta para o limite do WIP. (Para obter mais informações sobre limites WIP, consulte o artigo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Pronto para puxar]:** A história está pronta para ser movida para o próximo status por outro membro da equipe.\

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
