---
product-area: projects
navigation-topic: use-the-home-area
title: Marcar um item como Concluído na área inicial
description: Você pode marcar uma tarefa ou um problema como Concluído se for o destinatário da tarefa ou do problema. Ao marcar uma tarefa ou problema como Concluído, o status da tarefa ou problema é alterado para Concluído.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# Marcar um item como [!UICONTROL Concluído] no [!UICONTROL Início] area

Você pode marcar uma tarefa ou um problema como Concluído se for o destinatário da tarefa ou do problema. Ao marcar uma tarefa ou problema como [!UICONTROL Concluído], o status da tarefa ou problema é alterado para [!UICONTROL Concluído].

>[!NOTE]
>
>Você não vê o [!UICONTROL Concluído] , a menos que você seja um dos recursos atribuídos à tarefa ou ao problema.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Acesso à [!UICONTROL Editar] para tarefas e problemas</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Contribua com permissões ou mais para as tarefas e problemas necessários para trabalhar</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Marcar uma tarefa ou um problema como [!UICONTROL Concluído]

Somente o usuário atribuído à tarefa ou ocorrência pode marcá-la como [!UICONTROL Concluído].

1. Clique no botão **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **[!UICONTROL Início]**.
1. No **[!UICONTROL Lista de Trabalho]**, localize qualquer um dos itens que estão aguardando trabalho.
1. Siga um destes procedimentos:

* Clique em **[!UICONTROL Concluído]** no item de trabalho.\
   Consulte [Entenda as opções da [!UICONTROL Concluído] botão](#understand-the-options-of-the-done-button) para obter informações mais detalhadas sobre como esse botão pode aparecer.

* Selecione o item que deseja marcar como concluído e, no painel direito, clique em **[!UICONTROL Status da atualização]**, em seguida, altere o status do item para um status que seja igual a [!UICONTROL Concluído] ou [!UICONTROL Fechado].

## Entenda as opções da [!UICONTROL Concluído] botão

Por padrão, ao clicar no botão [!UICONTROL Concluído] em um item de trabalho altera o status desse item para [!UICONTROL Concluído] (para tarefas) ou [!UICONTROL Resolvido] (para questões).

Seu [!DNL Adobe Workfront] o administrador pode personalizar os status associados ao [!UICONTROL Concluído] e aplique essas personalizações à sua Equipe inicial.

Dependendo de quantos status estão associados à variável [!UICONTROL Concluído] ou quantos recursos são atribuídos à tarefa ou ao problema, a aparência da variável [!UICONTROL Concluído] pode ser alterado.

* [[!UICONTROL Concluído] botão associado a um status](#done-button-associated-with-one-status)
* [[!UICONTROL Concluído] botão associado a vários status](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL Concluído] botão para itens atribuídos a vários recursos](#done-button-for-items-assigned-to-multiple-resources)

### [!UICONTROL Concluído] botão associado a um status

Quando a variável [!UICONTROL Concluído] estiver associado a um status e o item de trabalho for atribuído somente a você, o botão lê **[!UICONTROL Concluído]**. Quando você clica nele, o status da tarefa ou do problema é alterado para o status associado à função [!UICONTROL Concluído] botão.

![Botão Concluído](assets/Done.png)

Para entender qual status está associado à variável [!UICONTROL Concluído] marque o botão [!UICONTROL Configurações do grupo] da sua equipe inicial para o [!UICONTROL Botão Concluído] conforme descrito em [Editar configurações do grupo](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

Se você não estiver atribuído a uma Home Team, o status padrão é escolhido ao clicar em [!UICONTROL Concluído], conforme descrito acima em [Entenda as opções da [!UICONTROL Concluído] botão](#understand-the-options-of-the-done-button).

### [!UICONTROL Concluído] botão associado a vários status

Quando a variável [!UICONTROL Concluído] estiver associado a mais de um status, o botão mostrará a palavra **[!UICONTROL Concluído]** que é seguido por um menu suspenso. Nesse cenário, não é possível simplesmente clicar em [!UICONTROL Concluído]. Você deve selecionar um status no menu suspenso. Selecione o status que melhor se ajuste à conclusão do item de trabalho. Ao fazer isso, você está alterando o status do item de trabalho.

Para entender como você pode associar vários status com a variável [!UICONTROL Concluído] botão , consulte [Configure o [!UICONTROL Concluído] botão para tarefas](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) e [Configure o [!UICONTROL Concluído] botão para problemas](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### [!UICONTROL Concluído] botão para itens atribuídos a vários recursos

Quando a tarefa ou o problema é atribuído a mais de um recurso, o botão mostra a palavra **[!UICONTROL Concluído]** que é seguido por um menu suspenso. No menu suspenso , você tem a opção de escolher entre **[!UICONTROL Feito com a minha parte]** (que permite que os membros da equipe saibam que você está completo com sua parte da tarefa) ou o status associado à [!UICONTROL Concluído] botão (que conclui o item). Após selecionar **[!UICONTROL Feito com a minha parte]**, o item de trabalho é removido da Lista de Trabalho, mas permanece na Lista de Trabalho daqueles que ainda estão atribuídos ao item de trabalho.\
Se o botão Concluído estiver associado a vários status, eles serão listados em **Feito com a minha parte**.

>[!NOTE]
>
>Em uma tarefa ou problema com vários destinatários, cada usuário é responsável por indicar que sua própria atribuição na tarefa ou problema foi realmente concluída. Por isso, cada destinatário deve clicar em [!UICONTROL Concluído] para mostrar que concluiu o trabalho atribuído a eles no item.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
