---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: Gerenciar solicitações de trabalho e de equipe na área Página inicial
description: Quando tarefas de trabalho e problemas são atribuídos a você, eles são listados na [!UICONTROL Lista de Trabalho] na área [!UICONTROL Página inicial]. Você pode visualizar, reatribuir, responder, trabalhar ou remover uma solicitação. As solicitações de trabalho na área [!UICONTROL Página inicial] não estão limitadas a problemas associados a filas de solicitações.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Gerenciar solicitações de trabalho e de equipe na área [!UICONTROL Página inicial]

Quando tarefas de trabalho e problemas são atribuídos a você, eles são listados na [!UICONTROL Lista de Trabalho] na área [!UICONTROL Página inicial]. Você pode visualizar, reatribuir, responder, trabalhar ou remover uma solicitação. As solicitações de trabalho na área [!UICONTROL Página inicial] não estão limitadas a problemas associados a filas de solicitações.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Work] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Acesso de [!UICONTROL Editar] a Tarefas e Problemas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>permissões do Contribute ou superior para as tarefas e problemas que você precisa para trabalhar</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Exibir uma solicitação de trabalho

As solicitações de trabalho atribuídas a você são exibidas no painel esquerdo em [!UICONTROL Página inicial]. Você pode configurar quais solicitações serão exibidas na [!UICONTROL Página Inicial] usando o filtro na parte superior da [!UICONTROL Lista de Trabalho].

É possível selecionar filtros que exibem itens prontos para você trabalhar ou itens nos quais você já está trabalhando no momento.

Este artigo descreve como usar os filtros na área [!UICONTROL Página inicial] para exibir os itens nos quais você está trabalhando no momento ou que devem ser considerados para começar a trabalhar. Para obter informações sobre todos os filtros na área [!UICONTROL Página inicial], consulte [Exibir itens na Lista de Trabalho na área [!UICONTROL Página inicial]](../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).

1. Clique no **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito e em **[!UICONTROL Página inicial]**.
1. Clique no menu suspenso **[!UICONTROL Filtro]**.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Clique em uma ou em ambas as opções para tarefas:

   **[!UICONTROL Pronto para Iniciar]:** Exibe somente tarefas e problemas que estão prontos para iniciar. Ambas as declarações a seguir devem ser verdadeiras:

   * As tarefas e seus pais não têm predecessores ou restrições de tarefa que as impeçam de ser trabalhadas.
   * A [!UICONTROL Data de Início Planejada] das tarefas ou problemas está no passado ou em até duas semanas no futuro.

   **[!UICONTROL Não está pronto]**: exibe somente tarefas e problemas que ainda não estão prontos para serem iniciados. Qualquer uma das seguintes declarações deve ser verdadeira:

   * As tarefas e seus pais podem ter predecessores ou restrições de tarefa que impedem seu trabalho.
   * As tarefas ou problemas têm uma [!UICONTROL Data de Início Planejada] que é mais de duas semanas no futuro.


1. Clique em **[!UICONTROL Trabalhando]** em [!UICONTROL Tarefas] ou [!UICONTROL Problemas] para exibir as tarefas e problemas nos quais você está trabalhando no momento.
1. Clique em **[!UICONTROL Solicitado]** em [!UICONTROL Problemas] para exibir problemas que foram solicitados a você (você está atribuído a eles), mas você ainda não aceitou trabalhar neles.

## Acessar uma solicitação de equipe

Você pode acessar uma solicitação atribuída à sua equipe diretamente da área [!UICONTROL Página inicial]. Para obter mais informações sobre solicitações de equipe, consulte [Visão geral das solicitações de equipe](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md).

1. Clique no **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito e em **[!UICONTROL Página inicial]**.
1. Na área **[!UICONTROL Lista de Trabalho]**, clique para expandir o agrupamento **[!UICONTROL Solicitações de Equipe]**.

   Se não houver solicitações atribuídas à sua equipe, o agrupamento não será exibido.

   ![](assets/team-requests-expanded-home-group-by-drop-down-nwe-350x314.png)

1. Clique no nome do grupo.\
   A seção **[!UICONTROL Solicitações da equipe]** exibe e mostra todas as solicitações atribuídas à sua equipe. Para obter mais informações sobre como trabalhar com solicitações de equipe, consulte [Gerenciar solicitações de trabalho e de equipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Reatribuir uma solicitação

1. Clique no **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito e em **[!UICONTROL Página inicial]**.
1. Na área **[!UICONTROL Lista de Trabalho]**, selecione a solicitação que deseja reatribuir.

1. Clique no widget **[!UICONTROL Atribuições]**, remova-se da solicitação e digite o nome do usuário ao qual deseja reatribuir a solicitação.

   >[!TIP]
   >
   >Se a solicitação de trabalho ainda estiver no estado Pronto para Iniciar ou Não Pronto, você poderá usar o botão **[!UICONTROL Reatribuir]** no menu **[!UICONTROL Mais]** da [!UICONTROL Lista de Trabalho].\
   >![Botão Reatribuir](assets/reassign-in-left-panel-350x204.png)

1. Se o status de uma tarefa for alterado para [!UICONTROL Nova] ou [!UICONTROL Em andamento] após sua conclusão, você deverá cancelar a atribuição do usuário, salvar a tarefa e reatribuir o usuário para que a tarefa seja exibida novamente na Lista de trabalho da página inicial.

## Responder a uma requisição

Você pode responder a uma solicitação para esclarecer ainda mais a solicitação ou para propor uma nova data.

1. Clique no **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito e em **[!UICONTROL Página inicial]**.
1. Na área **[!UICONTROL Lista de Trabalho]**, selecione a solicitação à qual deseja responder.
1. Localize a pessoa que atribuiu a solicitação a você.

   Você pode encontrar essas informações na guia [!UICONTROL Atualizações] da tarefa. Verifique se a opção de **[!UICONTROL Mostrar Atualizações do Sistema]** está habilitada.

1. Clique em **[!UICONTROL Iniciar nova atualização]** e comece a digitar sua resposta.
1. Insira o nome do destinatário na caixa **[!UICONTROL Notificar]** e clique em **[!UICONTROL Atualizar]**.

   >[!TIP]
   >
   >Se a solicitação de trabalho ainda estiver no estado Pronto para Iniciar ou [!UICONTROL Não Está Pronto], você poderá usar o botão **[!UICONTROL Responder]** no menu **[!UICONTROL Mais]** da [!UICONTROL Lista de Trabalho].\
   >![[!UICONTROL Botão Responder]](assets/reassign-in-left-panel-350x204.png)   >

## Trabalhar em uma solicitação

Ao clicar no botão [!UICONTROL Trabalhar nisto], você está indicando ao usuário que enviou a solicitação e a qualquer outro usuário que esteja atribuído à solicitação que você vai começar a trabalhar na solicitação. Para obter mais informações sobre como trabalhar em solicitações, consulte [Gerenciar solicitações de trabalho e de equipe](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

1. Clique no **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito e em **[!UICONTROL Página inicial]**.
1. Na área **[!UICONTROL Lista de Trabalho]**, selecione a solicitação na qual deseja trabalhar e clique em **[!UICONTROL Trabalhar Nela]**.\
   As informações sobre o problema são exibidas no painel direito.

## Remover uma solicitação

Se decidir que não deve trabalhar na solicitação, poderá converter a tarefa ou o problema de volta em uma solicitação ou removê-lo da lista.

1. Clique no **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito e em **[!UICONTROL Página inicial]**.
1. Na **[!UICONTROL Lista de Trabalho]**, aponte para o item aguardando para ser trabalhado.
1. Clique no widget **[!UICONTROL Atribuições]** e remova-se. Isso remove o item de trabalho da sua Lista de trabalho. Se a solicitação não for atribuída a outra pessoa, equipe ou função de trabalho, a solicitação será deixada não atribuída.

   Ou

   Clique no ícone de menu **[!UICONTROL Mais]** ![](assets/more-icon.png) à direita do nome da tarefa ou do problema na Lista de [!UICONTROL Trabalho da Página Inicial].

   ![](assets/more-menu-in-home-work-list-convert-to-request-remove-add-to-priority-options-nwe-350x160.png)

1. Selecione entre as seguintes opções:

   * **[!UICONTROL Converter para solicitação de trabalho]:** Selecione esta opção para converter o item de trabalho novamente em uma solicitação de trabalho.\

     O item de trabalho passa por uma solicitação e você permanece atribuído a ela.\
      Você pode aceitar a solicitação mais tarde clicando em **[!UICONTROL Trabalhar nisto]** novamente.

   * **[!UICONTROL Remover]:** Selecione esta opção para remover uma solicitação da sua [!UICONTROL Lista de Trabalho].\

     Você foi desatribuído da solicitação e a solicitação não está mais associada ao seu nome em [!DNL Adobe Workfront].\
      Se a solicitação não for atribuída a outra pessoa, equipe ou função de trabalho, a solicitação será deixada não atribuída.
