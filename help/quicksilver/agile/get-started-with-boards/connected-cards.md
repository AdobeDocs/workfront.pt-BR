---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Usar placas conectadas em placas
description: Você pode adicionar um cartão ao seu quadro que esteja conectado às tarefas e problemas existentes no Workfront.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 2a71ffd9180f2fe783675ae005165e1fd078178a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Usar placas conectadas em placas

{{highlighted-preview}}

Você pode adicionar um cartão ao seu quadro que esteja conectado a tarefas e problemas existentes em [!DNL Workfront].

Quando qualquer um dos detalhes a seguir for atualizado para o cartão em um local, ele será atualizado automaticamente no outro local:

* [!UICONTROL Nome]
* [!UICONTROL Descrição]
* [!UICONTROL Atribuídos]
* [!UICONTROL Status]
* [!UICONTROL Data de conclusão planejada]
* [!UICONTROL Estimativa] / [!UICONTROL Pontos da história]

>[!NOTE]
>Uma única tarefa ou problema conectado só pode ser adicionado uma vez por quadro. A mesma tarefa ou problema pode ser conectado a vários quadros.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td>
   <td><p>[!UICONTROL View] ou acesso superior a tarefas e problemas</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>Permissões de objeto</strong></td>
   <td><p>[!UICONTROL View] ou permissões superiores para a tarefa ou problema do Workfront</p></td>
  </tr>
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Adicionar uma placa conectada

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **[!UICONTROL Quadros]**.
1. Acesse um quadro. Para obter mais informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Adicionar cartão] > [!UICONTROL Placa conectada]**.
1. Escolha um projeto e escolha uma tarefa ou problema para adicionar como um cartão no quadro.

   É possível selecionar vários objetos e eles serão adicionados como cartões separados.

   >[!NOTE]
   >
   >* Somente os objetos aos quais você tem permissões estão disponíveis nos resultados da pesquisa. Se um item estiver esmaecido, ele já foi adicionado ao quadro.
   >* Ao filtrar por **[!UICONTROL Projetos que possuo]** ou **[!UICONTROL Projetos em que estou]**, os projetos que equivalem a um status Concluído, Adiado ou Rejeitado não são incluídos. Você ainda pode pesquisar esses projetos com a variável **[!UICONTROL Todos]** filtro.


1. Clique em **[!UICONTROL Adicionar]**.

   ![Procure por tarefa ou problema para se conectar](assets/boards-tasksissues-350x94.png)

   O cartão é adicionado na parte inferior da coluna mais à esquerda. O [!DNL Workfront] e seus destinatários são exibidos no cartão.

   >[!NOTE]
   >
   >Se um destinatário no [!DNL Workfront] tarefa ou problema não é um membro no quadro, eles não são atribuídos ao cartão.

   ![Cartão conectado](assets/boards-connected-card-first-added.png)

1. Clique em ![Abrir tarefa ou problema](assets/boards-launch-icon.png) para abrir o [!DNL Workfront] tarefa ou problema em uma nova guia do navegador.
1. Para editar os detalhes do cartão, clique no cartão (não no nome do cartão).

   Ou

   Clique no botão **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) no cartão e selecione **[!UICONTROL Editar]**.

1. No **[!UICONTROL Detalhes do cartão]** , adicione ou atualize as seguintes informações:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td> <p>Alterar o nome também altera o nome no [!DNL Workfront] objeto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Descrição]</strong></td> 
      <td> <p>Alterar a descrição também altera a descrição no [!DNL Workfront] objeto.</p> </td> 
     </tr> 
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Destinatários]</strong></td>
      <td><p>Para atribuir mais pessoas ou uma equipe ao cartão, comece a digitar um nome no campo de pesquisa e, em seguida, selecione-o quando for exibido na lista. Você pode adicionar indivíduos e equipes. Apenas uma atribuição de equipe é permitida em um cartão conectado.</p>
      <p>Os designados devem ser membros do quadro ou não aparecerão na lista de seleção. Quando uma equipe é membro no quadro, os membros individuais da equipe podem ser atribuídos ao cartão.</p>
      <p>Todos os destinatários selecionados também são atribuídos à tarefa ou ocorrência em [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Coluna]</strong></td>
      <td><p>Selecione a coluna do cartão.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Selecione um status para o cartão. Os padrões são [!UICONTROL Novo], [!UICONTROL Em Andamento] e [!UICONTROL Concluído], mas todos os status personalizados definidos para o item em [!DNL Workfront] também estão disponíveis.</p>
      <p>Se você tiver políticas de coluna ativadas para atualizar valores de campo, alterar o status no cartão move automaticamente o cartão para a coluna correspondente. Para obter mais informações, consulte "Definir configurações e políticas da coluna" no artigo <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Gerenciar colunas do quadro</a>.</p>
      <p>Se você clicar em <strong>[!UICONTROL Marca concluída]</strong> na parte superior do cartão, o status muda automaticamente para Complete (Concluído).</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Conclusão planejada]</strong></td>
      <td><p>Alterar essa data também altera a data de conclusão planejada no [!DNL Workfront] objeto.</p></td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimativa]</strong></td>
      <td><p>O número de horas para a conclusão do cartão.</p><p>Se você usar a opção de aceitação de recursos antecipada para [!DNL Workfront] [!UICONTROL Quadros], alterar a estimativa também altera o valor dos pontos de história no [!DNL Workfront] objeto.</p><p>Se você não estiver optando por recursos iniciais, esse campo será apenas uma entrada manual e o valor não poderá ser maior que 99.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Procure e selecione as tags para o cartão.</p>
      <p>Para obter informações sobre como criar novas tags, consulte <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Adicionar tags</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Itens da lista de verificação]</strong> </td> 
      <td> <p>Clique em <strong>[!UICONTROL Adicionar item da lista de verificação]</strong>. Em seguida, digite o título do item e pressione Enter. Outro item é adicionado automaticamente. Continue inserindo títulos para adicionar mais itens.</p> <p>O contador na parte superior da lista de verificação mostra o número de itens concluídos e o número total de itens.</p> <p>Para obter mais informações sobre itens da lista de verificação, consulte <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Gerenciar itens da lista de verificação em cartões</a>.</p></td>
     </tr>
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Fechar]** para retornar ao quadro.
O objeto conectado, os destinatários, as tags, a data de vencimento, o contador da lista de verificação, as horas estimadas e o status são exibidos no cartão.

   ![Cartão adicionado ao quadro](assets/boards-connected-card-details-110922.png)

## Desconecte uma placa conectada

Você pode desconectar um cartão conectado de seu objeto Workfront e ele permanecerá no quadro como um cartão ad hoc que você pode editar.

Para desconectar no nível da placa:

1. Acesse o quadro.
1. Clique no botão **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) na placa conectada e selecione **[!UICONTROL Desconectar]**.
1. Clique em **[!UICONTROL Desconectar]** na mensagem de confirmação.

Para desconectar no nível da placa:

1. Acesse o quadro e abra a placa conectada.
1. Clique no botão **[!UICONTROL Mais]** menu ![Menu Mais](assets/more-icon-spectrum.png) na área Connection dos detalhes do cartão, e selecione **[!UICONTROL Desconectar]**.
1. Clique em **[!UICONTROL Desconectar]** na mensagem de confirmação.

## Converter um cartão ad hoc em um cartão conectado

Depois de criar um cartão ad hoc, você pode convertê-lo em um cartão conectado. Para obter detalhes sobre cartões ad hoc, consulte [Adicionar um cartão ad hoc a um quadro](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Acesse o quadro e abra o cartão ad hoc.
1. Verifique o nome e a descrição no cartão. Eles serão adicionados à tarefa ou problema que você criar no [!DNL Workfront].
1. No [!UICONTROL Conexão] dos detalhes do cartão, clique em **[!UICONTROL Conectar-se com o Workfront]**.
1. No [!UICONTROL Placa Connect] selecione se você está criando uma tarefa ou um problema.
1. Procure e selecione um projeto para adicionar a tarefa ou problema.

   >[!NOTE]
   >
   >* Somente os objetos aos quais você tem permissões estão disponíveis nos resultados da pesquisa.
   >* Ao filtrar por **[!UICONTROL Projetos que possuo]** ou **[!UICONTROL Projetos em que estou]**, projetos que equivalem a um [!UICONTROL Concluído], [!UICONTROL Morto]ou [!UICONTROL Rejeitada] não estão incluídos. Você ainda pode pesquisar esses projetos com a variável **[!UICONTROL Todos]** filtro.


1. Clique em **[!UICONTROL Connect]**.

   ![Conectar cartão ad hoc ao Workfront](assets/boards-connect-ad-hoc-card.png)

   O nome do projeto é exibido na área Conexão nos detalhes do cartão.

1. Clique em **[!UICONTROL Fechar]** para retornar ao quadro.

<div class="preview">

## Registrar horas em uma placa conectada

>[!NOTE]
>
>Esse recurso está disponível somente por meio da aceitação antecipada de recursos para as placas Workfront.

Você deve ter as permissões corretas para registrar horas na tarefa ou problema conectado.

Os campos de registro de tempo não são exibidos nos cartões conectados por padrão. Você deve ativar [!UICONTROL **Horas**] no [!UICONTROL Configurar] área sob [!UICONTROL Cartões]. Para obter mais informações, consulte [Personalizar quais campos são exibidos em um cartão](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Insira o número de horas para a tarefa ou emissão.
1. Selecione um [!UICONTROL Tipo de hora] no menu suspenso, se for diferente do padrão.
1. Clique em [!UICONTROL **Hora de registro**].

   ![Registrar horas no cartão](assets/log-hours-on-card.png)

   O tempo de logon no cartão também é salvo na tarefa ou problema conectado.

O tempo de logon no cartão é igual ao tempo de registro em uma tarefa ou problema. Para obter mais informações, consulte &quot;Log time on a project, task or issue&quot; (Tempo de logon em um projeto, tarefa ou problema) no artigo [Tempo de registro](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

</div>
