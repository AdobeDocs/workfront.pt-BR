---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configurar preferências de horas e planilha de horas
description: Como um [!DNL Adobe Workfront] administrador, você pode especificar preferências para planilhas de horas e horas em [!DNL Workfront] para definir com quais itens as folhas de horas podem ser preenchidas previamente e quais itens os usuários podem registrar horas.
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 324ad45b52dafa96c2854f1fec1172b88643bdc2
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 1%

---

# Configurar preferências de horas e planilha de horas

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como um [!DNL Adobe Workfront] administrador, você pode especificar preferências para planilhas de horas e horas em [!DNL Workfront] para definir com quais itens as folhas de horas podem ser preenchidas previamente e quais itens os usuários podem registrar horas.

>[!IMPORTANT]
>
>Além dos itens que preenchem uma folha de horas de acordo com as condições descritas neste artigo, os itens a seguir também são exibidos na folha de horas por padrão:
>* Itens para os quais você fez logon durante o período da folha de horas
>* Itens que estão fixados na folha de horas
>* Itens que você pesquisa e adiciona manualmente à folha de horas. Itens adicionados manualmente são fixados por padrão.
>
>Para obter mais informações, consulte [Registrar tempo](../../../timesheets/create-and-manage-timesheets/log-time.md).



Quaisquer alterações feitas nas folhas de horas afetam todas as folhas de horas criadas no futuro.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Definir preferências de horas e planilha de horas

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Horas e Planilha de Horas]** > **[!UICONTROL Preferências]**.

1. Na página que é exibida, na caixa de diálogo **[!UICONTROL Preferências gerais]** , configure uma das seguintes opções:

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
       </ul> <p>Isso é útil quando os usuários planejam ficar longe do escritório e desejam registrar esse tempo antecipadamente.</p> <p><b>Nota</b>:</p> 
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
      <td> <p>Restringir a edição aos proprietários da folha de horas e [!DNL Workfront] administradores. Quando esta opção está desabilitada, as folhas de horas também podem ser editadas por:</p> 
       <ul> 
        <li> <p>Usuários com acesso administrativo a folhas de horas e horas em seu nível de acesso</p> </li> 
        <li> <p>Aprovadores de planilhas de horas se a opção "Pode editar horas" estiver ativada na planilha de horas</p> </li> 
        <li> <p>O gerente do proprietário da planilha de horas</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir edição de horas a proprietários e administradores]</td> 
      <td>Restringir a edição ao usuário que inseriu as horas e [!DNL Workfront] administradores. Esta configuração se aplica à guia [!UICONTROL Horas] em um projeto ou em um relatório de Horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. No **[!UICONTROL Onde os usuários podem registrar horas]** , configure uma das seguintes opções:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Registrar tempo diretamente em projetos]</td>
        <td>Permite que os usuários registrem horas no projeto (tanto na guia [!UICONTROL Atualizações] quanto na folha de horas). Se os usuários não registrarem tempo no nível do projeto, essas opções deverão permanecer desmarcadas.</td>
    </tr>
    <tr>
        <td>Registrar o tempo em projetos concluídos</td>
        <td>Permite que os usuários gravem tempo em um projeto marcado como concluído. Se essa opção estiver desabilitada, os usuários não poderão registrar o tempo referente ao trabalho concluído em projetos no status [!UICONTROL Concluído].</td>
    </tr>
    <tr>
        <td>Registrar o tempo em projetos mortos</td>
        <td>Quando esta opção está habilitada, os usuários podem registrar horas em projetos com status [!UICONTROL Desativado].</td>
    </tr>
   </table>

1. No **[!UICONTROL Preencher folhas de horas previamente]** , configure uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Trabalho dentro de] &lt;number of="" weeks=""&gt; [!UICONTROL do intervalo de trabalho da folha de horas]</td> 
      <td> <p>Define o número de semanas antes e depois do intervalo de datas da folha de horas que contém datas de tarefas e problemas atribuídas ao usuário. A configuração padrão é 1 semana e você pode estender esse intervalo para 4 semanas. Isso significa que a folha de horas é pré-preenchida com tarefas e problemas que têm datas em qualquer lugar entre quatro semanas antes do intervalo de datas da folha de horas até quatro semanas após o intervalo de datas da folha de horas, se você selecionar 4 semanas para o seu intervalo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tarefas e Problemas que foram concluídos]</td> 
      <td>Se vários recursos forem normalmente atribuídos a uma única tarefa, recomendamos essa configuração. Isso significa que quando um recurso registra o tempo na tarefa e o marca como concluído, os outros recursos atribuídos à tarefa ainda podem encontrar a tarefa ou o problema em sua folha de horas, para registrar suas horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tarefas e Problemas que têm Datas Planejadas no intervalo de datas da folha de horas]</td> 
      <td> <p>Quando selecionada, a folha de horas inclui tarefas e problemas que têm uma Data de início planejada ou uma Data de conclusão que está dentro do intervalo de datas da folha de horas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tarefas que têm Datas Projetadas no intervalo de datas da folha de horas]</td> 
      <td> <p>Quando selecionada, a folha de horas inclui tarefas que têm uma Data de Início Projetada ou uma Data de Conclusão dentro do intervalo de tempo do projeto, mesmo se a data planejada da ocorrência ou tarefa estiver fora do intervalo de datas da folha de horas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. No **[!UICONTROL Projetos, tarefas e problemas excluídos]** especifique o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ao excluir projetos]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Manter tempo registrado já adicionado às folhas de horas como tempo geral]</strong>: Se esse projeto for restaurado em um momento posterior, o tempo permanecerá na folha de horas.</li> 
        <li><strong>[!UICONTROL Excluir todo o tempo reportado]</strong>: Se este projeto for restaurado no futuro, o tempo já registrado será restaurado para o projeto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ao excluir tarefas ou problemas]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Mover o tempo reportado para o projeto onde a tarefa ou problema reside]</strong>: se essa tarefa ou esse problema for restaurado posteriormente, o tempo permanecerá no projeto.<br></li> 
        <li> <p><strong>[!UICONTROL Excluir todo o tempo reportado]</strong>: Se essa tarefa ou esse problema for restaurado no futuro, o tempo registrado será restaurado na tarefa ou no problema.</p> <p>Para obter informações mais detalhadas sobre essas opções, consulte <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configurar efeito] nas horas em que um objeto é excluído e restaurado</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

## Desbloquear preferências de horas e planilhas de horas para grupos

Os grupos em sua organização podem precisar de uma preferência de hora ou folha de horas configurada de forma diferente para seus fluxos de trabalho exclusivos. Você pode desbloquear a preferência para todos os grupos em toda a organização para que eles possam configurá-la por conta própria.

Quando uma preferência é desbloqueada e um administrador de grupo a modifica, ela afeta os proprietários da folha de horas se o grupo for o Grupo Inicial.

Para obter informações sobre como um administrador de grupo configura preferências de horas e folhas de horas para um grupo, consulte [Configurar preferências de horas e planilha de horas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Depois de um [!DNL Workfront] administrador desbloqueia uma preferência no nível do sistema, qualquer administrador de grupo pode configurá-la e bloqueá-la para garantir que todos no grupo e nos subgrupos abaixo estejam usando a mesma configuração. Isso é paralelo à capacidade de um [!DNL Workfront] o administrador precisa configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear uma planilha de horas e uma preferência de horas do grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Para desbloquear uma preferência de projeto para que grupos possam configurá-la:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront e clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Horas e planilhas de horas]** e, em seguida, clique em **[!UICONTROL Preferências]**.

1. Siga um destes procedimentos:

   * Se você quiser que os administradores de grupos possam configurar uma preferência para seus grupos, desbloqueie-a ![](assets/unlock-toggle-button.png).
   * Se desejar que todos os grupos usem sua configuração para uma preferência, certifique-se de que ela esteja bloqueada (esse é o padrão).

     >[!IMPORTANT]
     >
     >Recomendamos que você se comunique com os administradores e usuários em grupos em todo o sistema para garantir que todas as necessidades sejam consideradas na maneira como você configura uma preferência bloqueada. Ao bloqueá-lo, sua configuração para ele é herdada por todos os grupos no sistema. E se a preferência tiver sido desbloqueada por qualquer período, sua configuração substituirá aquelas que os administradores de grupo podem ter feito.

1. Clique em **[!UICONTROL Salvar]**.
