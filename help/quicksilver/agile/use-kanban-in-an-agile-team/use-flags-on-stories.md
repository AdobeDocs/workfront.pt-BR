---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Usar sinalizadores em histórias no quadro Kanban
description: No [!DNL Kanban] quadro, sinalizadores fornecem uma indicação visual de quando uma história está pronta para se mover para o próximo status. Isso permite que as equipes kanban usem uma abordagem de "pull" em vez de uma abordagem de "push" ao mover histórias entre status.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
source-git-commit: 33daf0633701a1c271552e796ffe22a58645c561
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Use sinalizadores em histórias no [!UICONTROL Kanban] quadro

No [!DNL Kanban] quadro, sinalizadores fornecem uma indicação visual de quando uma história está pronta para se mover para o próximo status. Isso habilita [!UICONTROL Kanban] equipes usam uma abordagem &quot;pull&quot; em vez de uma abordagem &quot;push&quot; ao mover histórias entre status.

**Exemplo:** Considere o exemplo a seguir de uma equipe usando uma abordagem &quot;pull&quot;: Olivia, a designer gráfica da equipe, termina seu trabalho e então marca a história como &quot;[!UICONTROL Pronto para extrair].&quot; Essa bandeira dá uma indicação visual a Tony, redator da equipe, de que a história está pronta para ele se mudar para o próximo status. Tony então move a história para o próximo status quando está pronto para começar a trabalhar nela.

Considere o seguinte ao usar sinalizadores em histórias:

* Sinalizadores não são um status, mas uma indicação visual de que a história está pronta para ser movida para o próximo status por outro membro da equipe.
* Os sinalizadores não aparecem em nenhum cartão de história que esteja no [!UICONTROL Backlog] ou na [!UICONTROL Concluído] coluna (ou em qualquer coluna onde o status da coluna é igual a [!UICONTROL Concluído]).

   Para obter mais informações sobre status de histórias, consulte [Usar sinalizadores em histórias no quadro Kanban](#updating-the-status-of-stories-and-subtasks)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Use sinalizadores em histórias no [!UICONTROL Kanban] quadro

Para alterar um sinalizador em uma história:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Equipes]**.

1. (Opcional) Clique no botão **[!UICONTROL Alterar equipe]** ícone ![Ícone Alternar equipe](assets/switch-team-icon.png), em seguida, selecione um novo [!UICONTROL Kanban] no menu suspenso ou pesquise por uma equipe na barra de pesquisa.

1. Vá para o [!UICONTROL Kanban] quadro onde você quer mudar uma bandeira de uma história.
1. Expanda o bloco de história para exibir o sinalizador.\
   O sinalizador está definido como **[!UICONTROL No rastreamento]** para cada história por padrão.\
   ![Cartão kanban](assets/agile-storycard-kanban-2021-350x308.png)

1. Clique no sinalizador atual e selecione uma das seguintes opções de sinalizador:

   * **[!UICONTROL No rastreamento]:** A história está no status apropriado e nenhuma ação precisa ser executada no momento.\

      Este é o sinalizador padrão para cada história no quadro Kanban.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Está Bloqueado]:** A história não pode prosseguir para o status seguinte. Quando esse sinalizador é definido em uma história, a história não conta para o limite WIP. (Para obter mais informações sobre os limites WIP, consulte o artigo [Configurar Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_locked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Pronto para extrair]:** A história está pronta para ser movida para o status seguinte por outro membro da equipe.\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
