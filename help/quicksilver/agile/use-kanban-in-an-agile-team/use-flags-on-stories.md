---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Usar sinalizadores em histórias no Quadro Kanban
description: No quadro  [!DNL Kanban] , os sinalizadores fornecem uma indicação visual de quando uma história está pronta para ser movida para o próximo status. Isso permite que as equipes Kanban usem uma abordagem de "pull" em vez de uma abordagem de "push" ao mover histórias entre status.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '476'
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
   <td> <p>Standard</p> 
   <p>Trabalhar ou superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Usar sinalizadores em histórias no quadro [!UICONTROL Kanban]

Para alterar um sinalizador em uma matéria:

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do switch]** ![Ícone da equipe do switch](assets/switch-team-icon.png) e selecione uma nova equipe [!UICONTROL Kanban] no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Vá para o quadro [!UICONTROL Kanban] onde deseja alterar um sinalizador em uma história.
1. Expanda o bloco da história para exibir o sinalizador.
O sinalizador é definido como **[!UICONTROL No Rastreamento]** para cada matéria por padrão.
   ![Cartão Kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Clique no sinalizador atual e selecione uma das seguintes opções de sinalizador:

   * **[!UICONTROL No Rastreamento]:** A história está no status apropriado e nenhuma ação precisa ser tomada neste momento.

     Esse é o sinalizador padrão para cada matéria no quadro Kanban.
     ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Está Bloqueado]:** A história não pode passar para o próximo status. Quando esse sinalizador é definido em uma matéria, a matéria não conta para o limite do WIP. (Para obter mais informações sobre limites WIP, consulte o artigo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).)

     ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Pronto para puxar]:** A história está pronta para ser movida para o próximo status por outro membro da equipe.

     ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
