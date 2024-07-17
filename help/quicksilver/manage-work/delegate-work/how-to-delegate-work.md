---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Delegar tarefas e problemas
description: Você pode delegar temporariamente o trabalho ao qual está atribuído enquanto estiver fora do escritório. Este artigo descreve como delegar atribuições de tarefas e problemas.
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1460'
ht-degree: 0%

---

# Gerenciar delegação de tarefas e problemas

<!-- Audited: 1/2024 -->


<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote this as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Você pode delegar temporariamente o trabalho ao qual está atribuído enquanto estiver fora do escritório.

Você pode delegar atribuições de tarefas e problemas ou pode delegar aprovações. Este artigo descreve como delegar atribuições de tarefas e problemas.

Para obter informações gerais sobre a delegação de trabalho, consulte [Visão geral da delegação de trabalho](../../manage-work/delegate-work/delegate-work-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

>[!IMPORTANT]
>
>* Os usuários selecionados como delegados recebem as mesmas permissões que suas permissões nas tarefas e problemas que você delega a eles.
>* As permissões devem funcionar dentro de seus níveis de acesso e, às vezes, seus níveis de acesso podem ser inferiores aos seus.
>
>   
>   Por exemplo, se um usuário tiver somente o acesso de Visualização às tarefas em seu nível de acesso e você tiver permissões de Gerenciamento nas tarefas que você delegar a ele, ele receberá permissões de Gerenciamento para as tarefas que você delegar a ele. No entanto, eles não poderão executar as mesmas ações que você nas tarefas delegadas. Para poder atualizar tarefas em sua ausência, é necessário solicitar ao administrador do sistema o acesso para Editar tarefas.
>
>   
>   Para obter informações sobre como um administrador do sistema pode modificar seu nível de acesso, consulte [Criar ou modificar níveis de acesso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Para itens atribuídos depois que a delegação já foi iniciada, pode levar até uma hora depois que o item foi atribuído para [!DNL Workfront] compartilhar os itens recentemente atribuídos com o representante.


Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: Colaborador ou superior</p><p>Ou</p><p>Atual: revisão ou superior</p>

>[!NOTE]
>
>Embora você possa ser designado para trabalhar quando tiver uma licença de Solicitação, não poderá delegar seu trabalho a outras pessoas. [!DNL Workfront] não recomenda atribuir trabalho aos usuários de Revisão, Solicitação ou Colaborador.

</tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e problemas 
     </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualize ou aumente as permissões para as tarefas ou problemas aos quais você está atribuído</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Pré-requisitos

Antes de executar as atividades descritas neste artigo, você deve garantir o seguinte:

* O [!DNL Workfront] ou o administrador de grupo habilitou a configuração [!UICONTROL Permitir que usuários excluam tarefas e problemas com horas reportadas] na área [!UICONTROL Configuração] da sua instância [!DNL Workfront].

  Para obter mais informações, consulte [Configurar preferências de tarefas e problemas do sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Delegar tarefas e problemas a outro usuário

Antes de delegar trabalho a outras pessoas, recomendamos que você entre em contato com elas e informe que elas serão designadas como delegados em seus itens de trabalho. Solicite a aprovação verbal deles antes de delegar o trabalho para garantir que eles tenham o tempo necessário para concluir o trabalho enquanto você estiver fora do escritório.

Para obter informações gerais sobre a delegação de tarefas e problemas, consulte [Visão geral de Delegar tarefas e problemas](/help/quicksilver/manage-work/delegate-work/delegate-work-overview.md).

Para delegar tarefas e problemas a outras pessoas:

1. Vá para a área [!UICONTROL **Página Inicial**] e clique em [!UICONTROL **Delegar**] na parte superior da [!UICONTROL **Lista de Trabalho**].

   ![](assets/delegate-button-in-home.png)

1. Na guia [!UICONTROL **Delegar tarefas e problemas**], atualize o seguinte:

   * [!UICONTROL **Delegar tarefas e problemas a**]: comece digitando o nome de um usuário ao qual você deseja que suas tarefas e problemas sejam delegados, em seguida, selecione-o quando ele for exibido na lista. Você só pode selecionar um usuário.

     O usuário selecionado como representante recebe as mesmas permissões que suas permissões nas tarefas e problemas que você delega a ele.

   * [!UICONTROL **Data de início**]: selecione uma data no calendário em que a delegação dos itens de trabalho deve começar.

     >[!TIP]
     >
     >A data de início não pode estar no passado.

   * [!UICONTROL **Sem data de término**]: selecione essa opção se não quiser especificar a data de término da delegação.

   * [!UICONTROL **Data de término**]: selecione uma data no calendário em que a delegação deve parar.

     >[!TIP]
     >
     >Se você deixar o campo Data final vazio e a opção Sem data final não estiver selecionada, a delegação será definida somente para o dia atual.

     ![](assets/delegate-box-expanded-in-home.png)

1. Clique em [!UICONTROL **Salvar**].

   As seguintes coisas acontecem:

   * Seu trabalho é delegado ao usuário especificado. Qualquer tarefa incompleta ou problema que tenha datas dentro do período selecionado (incluindo as recentemente atribuídas, após a delegação ter sido habilitada) é delegado.

     >[!TIP]
     >
     >   Itens de trabalho concluídos que têm datas dentro do período de delegação não são delegados.


   * Você receberá uma mensagem no canto superior direito da tela para confirmar que ativou a delegação do seu trabalho para outro usuário. O nome do usuário delegado é exibido na mensagem de confirmação.

   * Uma indicação de que suas tarefas e problemas estão delegados a outros usuários é exibida na maioria das áreas em que você pode ver as atribuições no [!DNL Workfront]. Para obter mais informações sobre quais áreas não incluem nomes de representantes, consulte [Visão geral do trabalho de delegação](delegate-work-overview.md).

   * O botão [!UICONTROL **Delegar**] na área [!UICONTROL Página inicial] é alterado para [!UICONTROL **Editar delegação**] para indicar que há uma delegação em vigor.
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Se as notificações de eventos e as notificações pessoais estiverem ativadas, você também receberá uma confirmação por email da sua delegação.

   * O usuário selecionado como seu representante receberá um email sobre a delegação, se as notificações de evento estiverem habilitadas.

     Para obter informações sobre como habilitar notificações por email pessoais, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## Editar ou parar delegação

Você pode permitir que uma delegação expire se tiver selecionado uma Data final ou pode interrompê-la manualmente. Também é possível modificar o período da delegação, se as datas da delegação tiverem sido alteradas.

1. Vá para a área [!UICONTROL Página inicial] e clique em [!UICONTROL Editar delegação] no canto superior direito da Lista de trabalho.
1. Na guia [!UICONTROL Delegar tarefas e problemas], siga um destes procedimentos:
   * Modifique a [!UICONTROL **Data inicial**] ou a [!UICONTROL **Data final**]
   * Clique em [!UICONTROL **Parar delegação**]

   >[!TIP]
   >
   >    Você poderá editar somente a Data de término de uma delegação se ela já tiver sido iniciada.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Condicional) clique em [!UICONTROL **Salvar**] para salvar as novas datas de delegação

   Ou

   Clique em [!UICONTROL **Parar delegação**] na caixa de confirmação para confirmar a interrupção da delegação.

   A delegação atualizou as datas ou parou e os usuários delegados foram removidos de suas tarefas e problemas. As permissões para as tarefas e problemas permanecem em vigor.


## Localizar trabalho delegado e informações delegadas

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Quando tarefas e problemas forem delegados, há várias áreas em [!DNL Workfront] onde você pode ver o trabalho delegado ou quem são os delegados.

* [Localizar delegados na caixa Atribuições](#locate-delegates-in-the-assignments-box)
* [Localizar trabalho delegado em [!UICONTROL Residência]](#locate-delegated-work-in-home)


### Localizar delegados na caixa [!UICONTROL Atribuições]

Quando o administrador do sistema ou do grupo habilita a delegação de trabalho no sistema, a caixa [!UICONTROL Atribuições] exibe as seguintes guias em todos os locais que você pode acessá-las:

* [!UICONTROL **Atribuições**]: os usuários atribuídos à tarefa ou problema são exibidos aqui.
* [!UICONTROL **Delegações**]: os usuários designados como delegados pelos atribuídos na tarefa ou problema são exibidos aqui.

Você pode acessar a caixa [!UICONTROL Atribuições] nas seguintes áreas:

* O cabeçalho da tarefa ou do problema

  O campo [!UICONTROL Atribuições] no cabeçalho da tarefa ou problema é alterado para [!UICONTROL Atribuições e delegações].

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

* O [!UICONTROL Balanceador de carga de trabalho] ao atribuir tarefas ou problemas manualmente

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Não é possível exibir representantes na seção [!UICONTROL Atribuições] de uma caixa de edição de tarefas ou problemas.

Se uma tarefa ou um problema for delegado e a subguia [!UICONTROL Delegações] estiver vazia, um dos seguintes cenários pode existir:

* Você não está atribuído à tarefa ou problema.
* As datas da tarefa ou do problema estão fora do período de delegação.

>[!TIP]
>
>As horas planejadas ou reais para tarefas delegadas e problemas não são consideradas nas ferramentas de gerenciamento de recursos, como o [!UICONTROL Balanceador de carga de trabalho] ou o [!DNL Resource Planner] para os usuários delegados. As horas permanecem associadas somente ao usuário atribuído.

### Localizar trabalho delegado em [!UICONTROL Residência]

1. Vá para a área [!UICONTROL **Início**], clique no menu suspenso de filtro e selecione uma ou mais das seguintes opções:
   * [!UICONTROL **Delegado**]: para exibir tarefas e problemas delegados a você ou por você.
   * [!UICONTROL **Delegado a mim**]: para exibir tarefas e problemas delegados a você por outro usuário.
   * [!UICONTROL **Delegado por mim**]: para exibir tarefas e problemas delegados por você a outros usuários.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Clique no menu suspenso [!UICONTROL sorting] para classificar a lista pelos seguintes critérios:
   * [!UICONTROL Conclusão planejada]. Esta é a opção de classificação padrão.
   * [!UICONTROL Início planejado]
   * [!UICONTROL Data de confirmação]
   * [!UICONTROL Projeto]
   * [!UICONTROL Minha Prioridade]
1. Expanda os agrupamentos na [!UICONTROL **Lista de trabalho**] para exibir os itens de trabalho delegados. Existem os seguintes cenários:
   * Para itens que você delegou a outras pessoas, o nome do delegado é exibido na [!UICONTROL **Lista de Trabalho**], bem como no campo [!UICONTROL **Atribuições e delegações**] à direita.

   * Para itens delegados a você, o nome do destinatário é exibido na [!UICONTROL **Lista de trabalho**], bem como no campo **[!UICONTROL Atribuições e delegações]** à direita.

   >[!TIP]
   >
   >    Se a delegação estiver definida para iniciar em uma data posterior à data de hoje, a data de início da delegação também será exibida na [!UICONTROL Lista de Trabalho]. Os itens delegados são exibidos no agrupamento selecionado para a [!UICONTROL Lista de Trabalho], de acordo com o tipo de agrupamento. Por exemplo, se você agrupar por [!UICONTROL Data de conclusão planejada], os itens delegados serão exibidos no agrupamento de acordo com suas datas de conclusão planejadas.
