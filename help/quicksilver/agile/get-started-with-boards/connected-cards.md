---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Uso de placas conectadas em placas
description: Você pode adicionar um cartão ao seu quadro conectado a tarefas e problemas existentes no Workfront.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: f8feca57e039e34c320f2b967c58c5fc0862f665
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 0%

---

# Usar placas conectadas em placas

<!-- Audited: 2/2024 -->

Você pode adicionar um cartão ao seu quadro que esteja conectado a tarefas e problemas existentes no [!DNL Workfront].

Quando qualquer um dos detalhes a seguir é atualizado para o cartão em um local, ele é atualizado automaticamente no outro local:

* [!UICONTROL Nome]
* [!UICONTROL Descrição]
* [!UICONTROL Responsáveis]
* [!UICONTROL Status]
* [!UICONTROL Data de conclusão planejada]
* [!UICONTROL Estimativa] / [!UICONTROL Pontos da História]
* [!UICONTROL Subtarefas]
* [!UICONTROL Documentos]

Para sincronizar cartões conectados com o Workfront, clique no menu **[!UICONTROL Mais]** ![[!UICONTROL Mais menu]](assets/more-icon-spectrum.png) ao lado do nome do quadro e selecione **[!UICONTROL Sincronizar itens conectados]**. Cartões arquivados não são sincronizados com tarefas e problemas do Workfront. Se você restaurar um cartão, ele será sincronizado novamente.

>[!NOTE]
>
>Uma única tarefa ou problema conectado só pode ser adicionado uma vez por quadro. A mesma tarefa ou problema pode ser conectado a várias placas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>
   <p>Novo: Colaborador ou superior</p>
   <p>Ou</p>
   <p>Atual: solicitação ou superior</p>
 </td> 
  </tr> 
  <tr>
   <td role="rowheader">Configurações de nível de acesso</td>
   <td><p>Visualize ou aumente o acesso a tarefas e problemas</p></td>
  </tr>
  <tr>
   <td role="rowheader">Permissões de objeto</td>
   <td><p>Visualize ou aumente as permissões para a tarefa ou problema do Workfront</p>
   <p><strong>Observação:</strong> usuários com permissões de Exibição para uma tarefa ou problema não podem executar nenhuma ação em cartões conectados a ela, incluindo mover o cartão para outra coluna no quadro. Os usuários da exibição só podem abrir o cartão para ver suas propriedades e abrir a tarefa ou problema conectado. Para solicitar acesso adicional, abra a tarefa ou problema e solicite acesso lá.</td>
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar um cartão conectado

{{step1-to-boards}}

1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Adicionar cartão] > [!UICONTROL Cartão conectado]**.
1. Escolha um projeto e escolha uma tarefa ou problema para adicionar como cartão ao quadro.

   Você pode selecionar vários objetos e todos eles serão adicionados como cartões separados.

   >[!NOTE]
   >
   >* Somente objetos para os quais você tem permissão estarão disponíveis nos resultados da pesquisa. Se um item estiver esmaecido, ele já foi adicionado ao quadro.
   >* Quando você filtra por **[!UICONTROL Projetos dos quais sou proprietário]** ou **[!UICONTROL Projetos dos quais sou proprietário]**, os projetos com status Concluído, Inativo ou Rejeitado não são incluídos. Você ainda pode pesquisar por esses projetos com o filtro **[!UICONTROL Todos]**.

1. Clique em **[!UICONTROL Adicionar]**.

   ![Procurar tarefa ou problema para conectar](assets/boards-tasksissues-350x94.png)

   O cartão é adicionado na parte inferior da coluna mais à esquerda. O objeto conectado [!DNL Workfront] e seus atribuídos são exibidos no cartão.

   ![Cartão conectado](assets/boards-connected-card-first-added.png)

1. Clique em ![Abrir tarefa ou problema](assets/boards-launch-icon.png) para abrir a tarefa ou problema [!DNL Workfront] em uma nova guia do navegador.
1. Para editar os detalhes do cartão, clique nele (não no nome do cartão).

   Ou

   Clique no menu **[!UICONTROL Mais]** ![Mais menus](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Editar]**.

1. Na caixa **[!UICONTROL Detalhes do cartão]**, adicione ou atualize as seguintes informações:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Nome]</strong></td> 
      <td>Alterar o nome também altera o nome no objeto [!DNL Workfront] conectado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong></td> 
      <td>Alterar a descrição também altera a descrição no objeto [!DNL Workfront] conectado. Você pode adicionar URLs na descrição e eles se tornarão links clicáveis quando o cartão for salvo.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Coluna]</strong></td>
      <td>Selecione a coluna do cartão.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Selecione um status para o cartão. Os padrões são [!UICONTROL Novo], [!UICONTROL Em Andamento] e [!UICONTROL Concluído], mas todos os status personalizados definidos para o item em [!DNL Workfront] também estão disponíveis.</p>
      <p>Se você tiver políticas de coluna ativadas para atualizar valores de campo, alterar o status no cartão moverá automaticamente o cartão para a coluna correspondente. Para obter mais informações, consulte "Definir configurações e políticas de coluna" no artigo <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Gerenciar colunas do quadro</a>.</p>
      <p>Se você clicar em <strong>[!UICONTROL Marcar como Concluída]</strong> na parte superior do cartão, o status será alterado automaticamente para Concluída.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Término Planejado]</strong></td>
      <td>Alterar essa data também altera a data de conclusão planejada no objeto [!DNL Workfront] conectado.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimativa]</strong></td>
      <td><p>O número de horas para a conclusão do cartão.</p><p>Alterar a estimativa também altera o valor dos pontos da história no objeto conectado [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Atribuições]</strong></td>
      <td><p>Para atribuir mais pessoas ou uma equipe ao cartão, clique em <strong>[!UICONTROL Adicionar Atribuição]</strong> e comece a digitar um nome no campo de pesquisa. Em seguida, selecione-o quando ele for exibido na lista de resultados. Você pode adicionar indivíduos e equipes. Somente uma atribuição de equipe é permitida em um cartão conectado.</p>
      <p>Todos os atribuídos selecionados também são atribuídos à tarefa ou problema em [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Marcas]</strong></td>
      <td><p>Procure e selecione tags para o cartão.</p>
      <p>Para obter informações sobre como criar novas marcas, consulte <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Adicionar marcas</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Campos personalizados]</strong></td>
      <td><p>Todos os campos personalizados adicionados são exibidos nesta área.</p>
      <p>Para obter mais informações, consulte <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personalizar quais campos são exibidos em um cartão</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtarefa]</strong></td>
      <td><p>Todas as subtarefas existentes para a tarefa aparecem nesta seção. Clique em <strong>[!UICONTROL Adicionar Subtarefa]</strong> para adicionar uma nova subtarefa.</p>
      <p>O contador na parte superior da seção mostra o número de subtarefas concluídas e o número total de subtarefas.</p>
      <p>Para obter mais informações sobre subtarefas, consulte <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Gerenciar subtarefas em quadros</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Lista de Verificação]</strong></td>
      <td><p>Clique em <strong>[!UICONTROL Adicionar item de lista de verificação]</strong>. Em seguida, digite o título do item e pressione Enter. Outro item é adicionado automaticamente. Continue inserindo títulos para adicionar mais itens.</p>
      <p>O contador na parte superior da lista de verificação mostra o número de itens concluídos e o número total de itens.</p> <p>Para obter mais informações sobre itens da lista de verificação, consulte <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Gerenciar itens da lista de verificação em cartões</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Documentos]</strong></td>
      <td>Para um documento existente, passe o mouse sobre a miniatura do documento e clique em <strong>Visualizar</strong> para exibir o arquivo no navegador ou em <strong>Baixar</strong> para baixar o arquivo no computador. Para um novo documento, consulte <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Adicionar documentos em cartões</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Horas]</strong></td>
      <td>Consulte "Registrar horas em uma placa conectada" abaixo.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comentários]</strong></td>
      <td><p>Clique no campo <strong>[!UICONTROL Novo comentário]</strong> e digite seu comentário. Use as ferramentas de formatação para formatar o texto. Para marcar uma pessoa ou equipe, use a caixa de pesquisa na parte inferior da área de comentários. O usuário não precisa ser membro do painel. Os usuários marcados em cartões conectados receberão notificações por email.</p><p>Clique em <strong>[!UICONTROL Enviar]</strong> para adicionar o comentário ao cartão.</p>
      <p>Para obter mais informações sobre comentários, consulte <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Atualizar trabalho</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Atividade do sistema]</strong></td> 
      <td><p>Se você tiver a <strong>Atividade do sistema</strong> habilitada como uma seção de cartão, a atividade será exibida nesta área.</p> <p>Para obter mais informações, consulte <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Personalizar quais campos são exibidos em um cartão</a> e <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Atualizações rastreadas pelo sistema</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Use o painel de navegação esquerdo para se mover entre seções de campos nos detalhes do cartão.

1. Clique em **[!UICONTROL Fechar]** para retornar ao quadro.
O objeto conectado, os atribuídos, as tags, a data de vencimento, o contador da lista de verificação, as horas estimadas e o status são exibidos no cartão.

   ![Cartão adicionado ao quadro](assets/boards-connected-card-details-110922.png)

## Desconecte um cartão conectado

Você pode desconectar um cartão conectado do objeto Workfront dele, e o cartão permanece no quadro como um cartão ad hoc que pode ser editado.

Para desconectar-se no nível do quadro:

1. Acesse o quadro.
1. Clique no menu **[!UICONTROL Mais]** ![Mais menu](assets/more-icon-spectrum.png) no cartão conectado e selecione **[!UICONTROL Desconectar]**.
1. Clique em **[!UICONTROL Desconectar]** na mensagem de confirmação.

Para desconectar no nível da placa:

1. Acesse a placa e abra a placa conectada.
1. Clique no menu **[!UICONTROL Mais]** ![Mais menu](assets/more-icon-spectrum.png) na área Conexão dos detalhes do cartão e selecione **[!UICONTROL Desconectar]**.
1. Clique em **[!UICONTROL Desconectar]** na mensagem de confirmação.

## Converter um cartão ad hoc em um cartão conectado

Depois de criar um cartão ad hoc, você pode convertê-lo em um cartão conectado. Para obter detalhes sobre cartões ad hoc, consulte [Adicionar um cartão ad hoc a um quadro](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Acesse o quadro e abra o cartão ad hoc.
1. Verifique o nome e a descrição na placa. Eles serão adicionados à tarefa ou problema criado em [!DNL Workfront].
1. Na área [!UICONTROL Conexão] dos detalhes do cartão, clique em **[!UICONTROL Conectar-se ao Workfront]**.
1. Na janela [!UICONTROL Conectar Cartão], selecione se você está criando uma tarefa ou um problema.
1. Procure e selecione um projeto ao qual adicionar a tarefa ou problema.

   >[!NOTE]
   >
   >* Somente objetos para os quais você tem permissão estarão disponíveis nos resultados da pesquisa.
   >* Quando você filtra por **[!UICONTROL Projetos dos quais sou proprietário]** ou **[!UICONTROL Projetos dos quais sou proprietário]**, os projetos com o status [!UICONTROL Concluído], [!UICONTROL Desativado] ou [!UICONTROL Rejeitado] não são incluídos. Você ainda pode pesquisar por esses projetos com o filtro **[!UICONTROL Todos]**.

1. Clique em **[!UICONTROL Conectar]**.

   ![Conectar cartão ad hoc à Workfront](assets/boards-connect-ad-hoc-card.png)

   O nome do projeto é exibido na área Conexão nos detalhes do cartão.

1. Clique em **[!UICONTROL Fechar]** para retornar ao quadro.

## Registra horas em um cartão conectado

Você deve ter as permissões corretas para registrar horas na tarefa ou problema conectado.

Por padrão, os campos de registro de tempo não são exibidos em cartões conectados. Você deve habilitar [!UICONTROL **Horas**] na área [!UICONTROL Configurar] em [!UICONTROL Cartões]. Para obter mais informações, consulte [Personalizar quais campos são exibidos em um cartão](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Insira o número de horas da tarefa ou problema.
1. Selecione um [!UICONTROL Tipo de Hora] no menu suspenso, se for diferente do padrão.
1. Clique em [!UICONTROL **Log Time**].

   ![Registrar horas no cartão](assets/log-hours-on-card.png)

   O tempo registrado no cartão também é salvo na tarefa ou problema conectado.

O tempo de registro no cartão é o mesmo que o tempo de registro em uma tarefa ou problema. Para obter mais informações, consulte &quot;Registrar tempo em um projeto, tarefa ou problema&quot; no artigo [Registrar tempo](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

