---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Delegar tarefas e problemas
description: Você pode delegar temporariamente o trabalho ao qual está atribuído enquanto está fora do escritório. Este artigo descreve como delegar atribuições de tarefa e emissão.
author: Alina
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 72a2927d33f40c4fe08888712bdf62e9a5db9c40
workflow-type: tm+mt
source-wordcount: '1483'
ht-degree: 1%

---

# Gerenciar delegação de tarefa e emissão

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Você pode delegar temporariamente o trabalho ao qual está atribuído enquanto está fora do escritório.

Você pode delegar tarefas e emitir atribuições ou pode delegar aprovações. Este artigo descreve como delegar atribuições de tarefa e emissão.

Para obter informações gerais sobre delegação de trabalho, consulte [Visão geral do trabalho delegado](../../manage-work/delegate-work/delegate-work-overview.md).

## Requisitos de acesso

>[!IMPORTANT]
>
>* Os usuários selecionados como delegados recebem as mesmas permissões que suas permissões nas tarefas e problemas que você delega a eles.
>* As permissões devem funcionar em seus níveis de acesso e, às vezes, seus níveis de acesso podem ser menores do que os seus.

   >
   >   
   >   Por exemplo, se um usuário tiver somente o acesso à Exibição para tarefas em seu nível de acesso e tiver permissões de Gerenciamento nas tarefas que você delegar a ele, ele receberá permissões de Gerenciamento para as tarefas que você delegar a ele. No entanto, eles não poderão executar as mesmas ações que você nas tarefas delegadas. Eles devem solicitar Editar acesso às Tarefas pelo administrador do sistema para poder atualizar tarefas na sua ausência.
   >
   >   
   >   Para obter informações sobre como um pode modificar seu nível de acesso, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Para itens que são atribuídos depois que a delegação já foi iniciada, pode levar até uma hora depois que o item foi atribuído para [!DNL Workfront] para compartilhar os itens recém-atribuídos com o delegado.



Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>Revisar ou superior</p>

>[!NOTE]
>
>Embora você possa ser atribuído ao trabalho quando tem uma licença de Solicitação, não pode delegar seu trabalho a outras pessoas. [!DNL Workfront] não recomenda atribuir trabalho a Revisar ou Solicitar usuários.

</tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Problemas Se você ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar permissões ou permissões superiores para tarefas ou problemas atribuídos a você</p> 
    <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Pré-requisitos

Antes de executar as atividades descritas neste artigo, você deve garantir o seguinte:

* Seu [!DNL Workfront] ou o administrador de grupo ativou a [!UICONTROL Permitir que usuários excluam tarefas e problemas com horas registradas] na configuração do [!UICONTROL Configuração] área de seu [!DNL Workfront] instância.

   Para obter mais informações, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Delegar tarefas e problemas a outro usuário

Antes de delegar trabalhos a outros, recomendamos que você entre em contato com eles e informe que eles serão designados como delegados em seus itens de trabalho. Peça a aprovação verbal deles antes de delegar o trabalho para garantir que eles tenham o tempo necessário para concluir o trabalho enquanto você estiver fora do escritório.

Para obter informações gerais sobre delegação de tarefas e problemas, consulte [Visão geral de Delegar tarefas e problemas](delegate-work.md).

Para delegar suas tarefas e problemas a outros:

1. Vá para o [!UICONTROL **Início**] e clique em [!UICONTROL **Delegar**] na parte superior do [!UICONTROL **Lista de Trabalho**].

   ![](assets/delegate-button-in-home.png)

1. No [!UICONTROL **Delegar tarefas e problemas**] , atualize o seguinte:

   * [!UICONTROL **Delegar suas tarefas e problemas para**]: Comece digitando o nome de um usuário ao qual você deseja que suas tarefas e problemas sejam delegadas e selecione-o quando for exibido na lista. Você só pode selecionar um usuário.\

      O usuário selecionado como delegado recebe as mesmas permissões que suas permissões nas tarefas e problemas que você delega a ele. Para obter mais informações, consulte [Delegar tarefa e visão geral do problema](delegate-work-overview.md).

   * [!UICONTROL **Data de início**]: Selecione uma data no calendário em que a delegação de seus itens de trabalho deve começar.

      >[!TIP]
      >
      >A data de início não pode estar no passado.

   * [!UICONTROL **Sem data final**]: Selecione essa opção se não quiser especificar a data de término da delegação.

   * [!UICONTROL **Data final**]: Selecione uma data no calendário em que a delegação deve parar.

      >[!TIP]
      >
      >Não selecionar uma Data final ativa a delegação somente para o dia atual.

      ![](assets/delegate-box-expanded-in-home.png)

1. Clique em [!UICONTROL **Salvar**].

   As seguintes coisas acontecem:

   * Seu trabalho é delegado ao usuário especificado. Quaisquer tarefas ou problemas incompletos que tenham datas dentro do período selecionado (incluindo as recentemente atribuídas, após a delegação ter sido ativada) são delegados.
   >[!TIP]
   >
   >   Itens de trabalho concluídos que têm datas dentro do período da delegação não são delegados.


   * Você recebe uma mensagem no canto superior direito da tela para confirmar que você ativou a delegação do seu trabalho para outro usuário. O nome do usuário delegado é exibido na mensagem de confirmação.

   * Uma indicação de que suas tarefas e problemas são delegados a outros usuários é exibida na maioria das áreas em que você pode ver atribuições em [!DNL Workfront]. Para obter mais informações sobre quais áreas não incluem nomes de delegados, consulte [Delegar tarefa e visão geral do problema](delegate-work-overview.md).

   * O [!UICONTROL **Delegar**] no botão [!UICONTROL Início] alterações de área para [!UICONTROL **Editar delegação**] para indicar que existe uma delegação em vigor.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Se as notificações do evento e as notificações pessoais estiverem ativadas, você também receberá uma confirmação por email da delegação.

   * O usuário selecionado como seu delegado recebe um email sobre a delegação, se as notificações de evento estiverem ativadas.

      Para obter informações sobre como ativar notificações por email pessoal, consulte [Ativar ou desativar suas próprias notificações de evento](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).





## Editar ou parar delegação

Você pode permitir que uma delegação expire, se tiver selecionado uma Data final ou pode pará-la manualmente. Você também pode modificar o período de tempo da delegação, se as datas da delegação forem alteradas.

1. Vá para o [!UICONTROL Início] e clique em [!UICONTROL Editar delegação] no canto superior direito da Lista de trabalho.
1. No [!UICONTROL Delegar tarefas e problemas] , siga um destes procedimentos:
   * Modifique o [!UICONTROL **Data de início**] ou [!UICONTROL **Data final**]
   * Clique em [!UICONTROL **Parar delegação**]

   >[!TIP]
   >
   >    Você pode editar somente a Data final de uma delegação se a delegação já tiver iniciado.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Condicional) clique em [!UICONTROL **Salvar**] para salvar as novas datas de delegação

   Ou

   Clique em [!UICONTROL **Parar delegação**] na caixa de confirmação para confirmar a interrupção da delegação.

   A delegação atualizou as datas ou parou e os usuários delegados foram removidos de suas tarefas e problemas. Suas permissões para as tarefas e problemas permanecem em vigor.


## Localizar trabalho delegado e delegar informações

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Quando tarefas e problemas são delegados, há várias áreas em [!DNL Workfront] onde você pode ver o trabalho delegado ou quem são os delegados.

* [Localize delegados na caixa Atribuições](#locate-delegates-in-the-assignments-box)
* [Localizar trabalho delegado no [!UICONTROL Início]](#locate-delegated-work-in-home)


### Localize delegados no [!UICONTROL Atribuições] caixa

Quando o administrador do sistema ou do grupo habilita a delegação de trabalho em seu sistema, a variável [!UICONTROL Atribuições] exibe as seguintes guias em todos os locais que você pode acessá-la:

* [!UICONTROL **Atribuições**]: Os usuários atribuídos à tarefa ou ocorrência são exibidos aqui.
* [!UICONTROL **Delegações**]: Os usuários designados como delegados pelos designados na tarefa ou problema são exibidos aqui.

Você pode acessar o [!UICONTROL Atribuições] nas seguintes áreas:

* O cabeçalho da tarefa ou do problema

   ![](assets/assignments-and-delegates-panel-in-task-header.png)

   O [!UICONTROL Atribuições] no campo da tarefa ou do cabeçalho da emissão muda para [!UICONTROL Atribuições e delegações].

* O [!DNL Workload Balancer] ao atribuir tarefas ou problemas manualmente

   ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Não é possível exibir delegados na [!UICONTROL Atribuições] de uma tarefa ou emitir caixa Editar.

Se uma tarefa ou um problema for delegado e a variável [!UICONTROL Delegações] estiver vazia, uma das seguintes situações pode existir:

* Você não está atribuído à tarefa ou ocorrência.
* As datas de tarefa ou emissão estão fora do período de delegação.

>[!TIP]
>
>As Horas Planejadas ou Reais de tarefas delegadas e os problemas não são considerados nas ferramentas de gerenciamento de recursos, como a [!DNL Workload Balancer] ou [!DNL Resource Planner] para os utilizadores delegados. As horas permanecem associadas somente ao usuário atribuído.

### Localizar trabalho delegado no [!UICONTROL Início]

1. Vá para o [!UICONTROL **Início**] clique no menu suspenso de filtro e selecione uma ou mais das seguintes opções:
   * [!UICONTROL **Delegado**]: para visualizar tarefas e problemas delegados a você ou por você.
   * [!UICONTROL **Delegado para mim**]: para exibir tarefas e problemas delegados a você por outro usuário.
   * [!UICONTROL **Delegado por mim**]: para visualizar tarefas e problemas delegados por você a outros usuários.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Clique no botão [!UICONTROL classificação] menu suspenso para classificar a lista de acordo com os seguintes critérios:
   * [!UICONTROL Conclusão planejada]. Esta é a opção de classificação padrão.
   * [!UICONTROL Início planejado]
   * [!UICONTROL Data de confirmação]
   * [!UICONTROL Projeto]
   * [!UICONTROL Minhas Prioridades]
1. Expanda os agrupamentos na [!UICONTROL **Lista de Trabalho**] para visualizar itens de trabalho delegados. Os seguintes cenários existem:
   * Para itens que você delegou a outros, o nome do delegado é exibido no [!UICONTROL **Lista de Trabalho**] bem como [!UICONTROL **Atribuições e delegações**] à direita.

   * Para itens delegados a você, o nome do destinatário é exibido no [!UICONTROL **Lista de Trabalho**] bem como **[!UICONTROL Atribuições e delegações]** à direita.
   >[!TIP]
   >
   >    Se a delegação estiver definida para iniciar em uma data depois da data de hoje, a data de início da delegação também será exibida no [!UICONTROL Lista de Trabalho]. Os itens delegados são exibidos no agrupamento selecionado para a [!UICONTROL Lista de Trabalho], de acordo com o tipo de agrupamento. Por exemplo, se você agrupar por [!UICONTROL Data de Conclusão Planejada], os itens delegados são exibidos no agrupamento que corresponde às datas de conclusão planejadas.
