---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configurar preferências de horas e planilha de horas
description: Como administrador do  [!DNL Adobe Workfront] , você pode especificar preferências para folhas de horas e horas no  [!DNL Workfront]  para definir com quais itens as folhas de horas podem ser preenchidas previamente e quais itens os usuários podem registrar horas.
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 0%

---

# Configurar preferências de folha de horas e horas

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador do [!DNL Adobe Workfront], você pode especificar preferências para folhas de horas e horas em [!DNL Workfront] para definir com quais itens as folhas de horas podem ser preenchidas previamente e quais itens os usuários podem registrar horas.

>[!IMPORTANT]
>
>Além dos itens que preenchem previamente uma folha de horas de acordo com as condições descritas neste artigo, os itens a seguir também são exibidos em folhas de horas, por padrão:
>
>* Itens para os quais você fez logon durante o período da folha de horas
>* Itens que estão fixados na folha de horas
>* Itens que você pesquisa e adiciona manualmente à folha de horas. Por padrão, os itens adicionados manualmente são fixados.
>
>Para obter mais informações, consulte [Tempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md) e [Visão geral da folha de horas](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).

Quaisquer alterações feitas nas folhas de horas afetam todas as folhas de horas criadas no futuro.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Atual:[!UICONTROL Plano]</p>
   Ou
   <p>Novo: Padrão</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
</tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definir preferências de horas e planilha de horas

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Horas]** > **[!UICONTROL Preferências]**.

   A página Preferências de Horas e Folhas de horas é exibida.

1. (Opcional) Na caixa de pesquisa **Preferências de horas e folhas de horas do sistema**, comece digitando o nome de um grupo e, em seguida, selecione-o quando ele for exibido na lista.

   ![Procurar caixa de grupo](assets/search-for-group-box-in-timesheets-preferences-page.png)

   A página Preferências de Horas e Planilha de Horas é atualizada com as preferências do grupo selecionado. As preferências do nível do sistema devem ser desbloqueadas para modificar as preferências do nível do grupo. Para obter mais informações, consulte a seção [Desbloquear preferências de horas e folha de horas para grupos](#unlock-timesheet-and-hour-preferences-for-groups) neste artigo.

1. Na seção **[!UICONTROL Preferências gerais]**, configure uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tempo de log para datas futuras]</td> 
      <td> <p>Permite que os usuários registrem horas para datas futuras em todo o sistema em:</p> 
       <ul> 
        <li>Qualquer projeto, tarefa e problema que tenha acesso ao registro de tempo</li> 
        <li>Suas planilhas de horas como Tempo geral</li> 
       </ul> <p>Isso é útil quando os usuários planejam ficar longe do escritório e desejam registrar esse tempo antecipadamente.</p> <p><b>NOTA</b>:</p> 
       <p>Não é possível impedir que os usuários registrem tempo em tarefas ou problemas que estão fechados ou cancelados. Você só pode impedir que os usuários registrem horas em projetos concluídos ou inativos. Recomendamos que você use filtros em listas de tarefas e problemas para excluir aqueles que foram concluídos ou cancelados de ficarem visíveis para os usuários.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Atribuir funções de trabalho a entradas de hora manualmente]</td> 
      <td> <p>Permite que os usuários selecionem manualmente qualquer Função atribuída em seu perfil de usuário ou atribuída ao objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Se você desabilitar esta configuração depois de atribuir funções de trabalho a entradas de horas, os usuários deverão ajustar as horas registradas em várias funções na guia [!UICONTROL Hours] do projeto, tarefa ou problema.</li> 
         <li>Se o usuário não tiver uma função de trabalho atribuída em seu perfil e houver uma tarefa atribuída como o [!UICONTROL Proprietário da Tarefa] na caixa de diálogo [!UICONTROL Atribuições Avançadas], essa função de trabalho aparecerá quando o usuário registrar o tempo na tarefa.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir edição de planilha de horas a proprietários e administradores]</td> 
      <td> <p>Restringir a edição aos proprietários da folha de horas e aos administradores [!DNL Workfront]. Quando esta opção está desabilitada, as folhas de horas também podem ser editadas por:</p> 
       <ul> 
        <li> <p>Usuários com acesso administrativo a folhas de horas e horas em seu nível de acesso</p> </li> 
        <li> <p>Aprovadores de planilhas de horas se a opção "Pode editar horas" estiver ativada na planilha de horas</p> </li> 
        <li> <p>O gerente do proprietário da planilha de horas</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir edição de horas a proprietários e administradores]</td> 
      <td>Restrinja a edição ao usuário que inseriu as horas e [!DNL Workfront] administradores. Esta configuração se aplica à guia [!UICONTROL Horas] em um projeto ou em um relatório de Horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. Na seção **[!UICONTROL Onde os usuários podem registrar horas]**, configure uma das seguintes opções:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Diretamente nos projetos]</td>
        <td>Permite que os usuários registrem horas no projeto (tanto na guia [!UICONTROL Atualizações] quanto na folha de horas). Se os usuários não registrarem tempo no nível do projeto, essas opções deverão permanecer desmarcadas.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Em projetos concluídos]</td>
        <td>Permite que os usuários gravem tempo em um projeto marcado como concluído. Se essa opção estiver desabilitada, os usuários não poderão registrar o tempo referente ao trabalho concluído em projetos no status [!UICONTROL Concluído].</td>
    </tr>
    <tr>
        <td>[!UICONTROL Em projetos mortos]</td>
        <td>Quando esta opção está habilitada, os usuários podem registrar horas em projetos com status [!UICONTROL Desativado].</td>
    </tr>
   </table>

1. Na seção **[!UICONTROL Preencher folhas de horas previamente]**, configure uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Trabalho dentro de] &lt;número de semanas&gt; [!UICONTROL do intervalo de trabalho da folha de horas]</td> 
      <td> <p>Define o número de semanas antes e depois do intervalo de datas da folha de horas que contém datas de tarefas e problemas atribuídas ao usuário.</p> 
      <p>A configuração padrão é 1 semana e você pode estender esse intervalo para 4 semanas.</p> 
      <p>Isso significa que a folha de horas é pré-preenchida com tarefas e problemas que têm datas em qualquer lugar entre quatro semanas antes do intervalo de datas da folha de horas até quatro semanas após o intervalo de datas da folha de horas, se você selecionar 4 semanas para o seu intervalo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tarefas e problemas que foram concluídos]</td> 
      <td>Se vários recursos forem normalmente atribuídos a uma única tarefa, recomendamos essa configuração. Isso significa que quando um recurso registra o tempo na tarefa e o marca como concluído, os outros recursos atribuídos à tarefa ainda podem encontrar a tarefa ou o problema em sua folha de horas, para registrar suas horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tarefas e problemas que têm Datas Planejadas no intervalo de datas da folha de horas]</td> 
      <td> <p>Quando selecionada, a folha de horas inclui tarefas e problemas que têm uma Data de início planejada ou uma Data de conclusão que está dentro do intervalo de datas da folha de horas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tarefas que têm Datas Projetadas no intervalo de datas da folha de horas]</td> 
      <td> <p>Quando selecionada, a folha de horas inclui tarefas que têm uma Data de Início Projetada ou uma Data de Conclusão dentro do intervalo de tempo do projeto, mesmo se a data planejada da ocorrência ou tarefa estiver fora do intervalo de datas da folha de horas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Na seção **[!UICONTROL Projetos, tarefas e problemas excluídos]**, especifique o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> Ao excluir projetos</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Manter tempo registrado já adicionado às folhas de horas como tempo geral]</strong>: Se este projeto for restaurado mais tarde, o tempo permanecerá na folha de horas.</li> 
        <li><strong>[!UICONTROL Excluir todo o tempo reportado]</strong>: Se este projeto for restaurado no futuro, o tempo reportado será restaurado no projeto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ao excluir tarefas ou problemas</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Mover o tempo registrado para o projeto]</strong> onde a tarefa ou problema reside: se essa tarefa ou problema for restaurado no futuro, o tempo permanecerá no projeto.<br></li> 
        <li> <p><strong>[!UICONTROL Excluir todo o tempo reportado]</strong>: Se esta tarefa ou este problema for restaurado no futuro, o tempo reportado será restaurado na tarefa ou no problema.</p> <p>Para obter informações mais detalhadas sobre essas opções, consulte <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configurar afeto] nas horas em que um objeto é excluído e restaurado</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

## Desbloquear preferências de horas e planilhas de horas para grupos

Os grupos em sua organização podem precisar de folhas de horas ou preferências de hora configuradas de forma diferente para seus fluxos de trabalho exclusivos. Você pode desbloquear as preferências de todos os grupos em toda a organização para que eles possam configurá-las por conta própria.

Quando uma preferência é desbloqueada e um administrador de grupo a modifica, ela afeta os proprietários da folha de horas se o grupo for o Grupo Inicial.

Para obter informações sobre como um administrador de grupo configura preferências de horas e folhas de horas para um grupo, consulte [Configurar preferências de horas e folhas de horas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Depois que um administrador do [!DNL Workfront] desbloqueia uma preferência no nível do sistema, qualquer administrador de grupo pode configurá-la e bloqueá-la para garantir que todos no grupo e nos subgrupos abaixo estejam usando a mesma configuração. Isso é paralelo à capacidade que um administrador do [!DNL Workfront] tem de configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear uma planilha de horas e uma preferência de horas de grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Para desbloquear uma preferência de projeto para que grupos possam configurá-la:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Folhas de horas e Horas]** e em **[!UICONTROL Preferências]**.

1. Siga um destes procedimentos:

   * Se você quiser que os administradores de grupos possam configurar uma preferência para seus grupos, clique no botão de alternância **desbloquear** ![Desbloquear](assets/unlock-toggle-button.png) para desbloqueá-la.
   * Se você quiser que todos os grupos usem sua configuração para uma preferência, verifique se essa é a opção bloqueada ![Alternância de preferência bloqueada](assets/locked-preference-toggle.png) (essa é a opção padrão).

     >[!IMPORTANT]
     >
     >Recomendamos que você se comunique com os administradores e usuários em grupos em todo o sistema para garantir que todas as necessidades sejam consideradas na maneira como você configura uma preferência bloqueada.
     >
     >Ao bloqueá-lo, sua configuração para ele é herdada por todos os grupos no sistema. E se a preferência tiver sido desbloqueada por qualquer período, sua configuração substituirá aquelas que os administradores de grupo podem ter feito.

1. Clique em **[!UICONTROL Salvar]**.
