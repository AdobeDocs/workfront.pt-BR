---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configurar preferências de hora e folha de ponto
description: Como um [!DNL Adobe Workfront] administrador, você pode especificar preferências para folhas de horas e horas em [!DNL Workfront] para definir com quais itens as folhas de horas podem ser preenchidas previamente e para quais itens os usuários podem registrar o tempo.
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 3b0a82381d1c33d897b123a597df21ba54cc2565
workflow-type: tm+mt
source-wordcount: '1310'
ht-degree: 1%

---

# Configurar preferências de hora e folha de ponto

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como um [!DNL Adobe Workfront] administrador, você pode especificar preferências para folhas de horas e horas em [!DNL Workfront] para definir com quais itens as folhas de horas podem ser preenchidas previamente e para quais itens os usuários podem registrar o tempo.

Quaisquer alterações feitas nas folhas de horas afetam todas as folhas de horas criadas no futuro.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>Nota</b>

Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Definir preferências de hora e folha de horas

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Folha de Horas e Horas]** > **[!UICONTROL Preferências]**.

1. Na página que é exibida, no **[!UICONTROL Preferências gerais]** configure qualquer uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tempo do log para datas futuras]</td> 
      <td> <p>Permite aos usuários registrar tempo para datas futuras em todo o sistema em:</p> 
       <ul> 
        <li>Quaisquer projetos, tarefas e problemas em que tenham acesso ao tempo de registro</li> 
        <li>Suas folhas de ponto como Tempo Geral</li> 
       </ul> <p>Isso é útil quando os usuários planejam estar longe do escritório e desejam registrar esse tempo com antecedência.</p> <p><b>OBSERVAÇÃO</b>: Não é possível impedir que os usuários registrem tempo em tarefas ou problemas que estejam fechados ou cancelados. Você só pode impedir que os usuários façam logon em projetos concluídos ou inativos. Recomendamos usar filtros em listas de tarefas e problemas para excluir as que foram concluídas ou canceladas da visibilidade para os usuários.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Atribuir funções de trabalho a entradas de hora manualmente]</td> 
      <td> <p>Permitir que os usuários selecionem manualmente qualquer Função de trabalho atribuída em seu perfil de usuário ou atribuída ao objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Se você desativar esta configuração após atribuir funções de trabalho a entradas de hora, os usuários deverão ajustar as horas registradas em várias funções na guia [!UICONTROL Hours] do projeto, tarefa ou problema.</li> 
         <li>Se o usuário não tiver uma função de trabalho atribuída em seu perfil e houver uma tarefa atribuída como [!UICONTROL Task Owner] na caixa de diálogo [!UICONTROL Advanced Assignments], essa função de trabalho aparecerá quando o usuário fizer logon na tarefa.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir a edição da folha de ponto a proprietários e administradores]</td> 
      <td> <p>Restringir edição a proprietários de folha de ponto e [!DNL Workfront] administradores. Quando essa opção está desativada, as folhas de horas também podem ser editadas por:</p> 
       <ul> 
        <li> <p>Usuários com acesso administrativo a folhas de ponto e horas em seu nível de acesso</p> </li> 
        <li> <p>Aprovadores da folha de ponto se "Pode editar horas" estiver ativado na folha de ponto</p> </li> 
        <li> <p>O gerente do proprietário da folha de ponto</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir edição de hora a proprietários e administradores]</td> 
      <td>Restringir edição ao usuário que inseriu as horas e [!DNL Workfront] administradores. Essa configuração se aplica à guia [!UICONTROL Horas] em um projeto ou em um relatório de Horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. No **[!UICONTROL Onde os usuários podem registrar o tempo]** configure qualquer uma das seguintes opções:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Tempo do log diretamente nos projetos]</td>
        <td>Permite que os usuários façam logon no projeto (tanto na guia [!UICONTROL Atualizações] quanto na folha de ponto). Se os usuários não registrarem tempo no nível do projeto, essas opções deverão permanecer desmarcadas.</td>
    </tr>
    <tr>
        <td>Registrar o tempo em projetos concluídos</td>
        <td>Permite que os usuários registrem o tempo em um projeto que foi marcado como concluído. Se essa opção estiver desativada, os usuários não poderão registrar tempo para o trabalho que concluíram nos projetos no status [!UICONTROL Concluído].</td>
    </tr>
    <tr>
        <td>Registrar o tempo em projetos mortos</td>
        <td>Quando essa opção é ativada, os usuários podem fazer logon em projetos com um status [!UICONTROL inativo].</td>
    </tr>
   </table>

1. No **[!UICONTROL Preencher previamente as folhas de horas]** configure qualquer uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Trabalho que está dentro] &lt;number of="" weeks=""&gt; [!UICONTROL do intervalo de trabalho da folha de ponto]</td> 
      <td> <p>Define o número de semanas antes e depois do intervalo de datas da folha de ponto que contém datas de tarefas e problemas atribuídos ao usuário. A configuração padrão é 1 semana e você pode estender esse intervalo para 4 semanas. Isso significa que a folha de ponto é pré-preenchida com tarefas e problemas que têm datas entre quatro semanas antes do intervalo de datas da folha de ponto até quatro semanas após o intervalo de datas da folha de ponto, se você selecionar 4 semanas para o intervalo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tarefas e problemas que foram concluídos]</td> 
      <td>Se vários recursos normalmente forem atribuídos a uma única tarefa, recomendamos essa configuração. Isso significa que, quando um recurso registra o tempo em relação à tarefa e a marca como concluída, os outros recursos atribuídos à tarefa ainda poderão encontrar a tarefa ou o problema em sua folha de ponto, para registrar suas horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tarefas e problemas com datas planejadas no intervalo de datas da folha de ponto]</td> 
      <td> <p>Quando selecionada, a folha de ponto inclui tarefas e problemas que têm uma Data inicial planejada ou uma Data de conclusão que se enquadram no intervalo de datas da folha de ponto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tarefas com datas projetadas no intervalo de datas da folha de ponto]</td> 
      <td> <p>Quando selecionada, a folha de ponto inclui tarefas que têm uma Data de Início Projetada ou uma Data de Conclusão que se enquadram no período do projeto, mesmo se a data planejada da emissão ou tarefa estiver fora do intervalo de datas da folha de ponto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. No **[!UICONTROL Projetos, tarefas e problemas excluídos]** especifique:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ao excluir projetos]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Manter tempo registrado já adicionado às folhas de horas como horário geral]</strong>: Se esse projeto for restaurado posteriormente, o tempo permanecerá na folha de ponto.</li> 
        <li><strong>[!UICONTROL Excluir qualquer hora registrada]</strong>: Se este projeto for restaurado posteriormente, o tempo já registrado será restaurado para o projeto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ao excluir tarefas ou problemas]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Mover qualquer hora registrada para o projeto em que a tarefa ou a emissão reside]</strong>: Se essa tarefa ou problema for restaurado posteriormente, o tempo permanecerá no projeto.<br></li> 
        <li> <p><strong>[!UICONTROL Excluir qualquer hora registrada]</strong>: Se essa tarefa ou problema for restaurado posteriormente, o tempo registrado será restaurado para a tarefa ou problema.</p> <p>Para obter informações mais detalhadas sobre essas opções, consulte <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configurar efeito] em horas quando um objeto é excluído e restaurado</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

## Desbloquear folha de horas e preferências de hora para grupos

Os grupos em sua organização podem precisar de uma folha de ponto ou preferência de hora configurada de forma diferente para seus fluxos de trabalho exclusivos. Você pode desbloquear a preferência para todos os grupos em toda a organização para que eles possam configurá-la sozinhos.

Quando uma preferência é desbloqueada e um administrador de grupo a modifica, ela afeta os proprietários da folha de ponto se o grupo for seu Grupo Doméstico.

Para obter informações sobre como um administrador de grupo configura a folha de ponto e as preferências de hora para um grupo, consulte [Configurar as preferências de hora e folha de ponto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Depois de um [!DNL Workfront] O administrador desbloqueia uma preferência no nível do sistema, qualquer administrador de grupo pode configurá-la e bloqueá-la para garantir que todos no grupo e nos subgrupos abaixo estejam usando a mesma configuração. Isso é paralelo à capacidade de uma [!DNL Workfront] o administrador precisa configurar e bloquear uma preferência para todos no sistema. Para obter mais informações, consulte [Bloquear ou desbloquear uma folha de horas e uma preferência de hora do grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Para desbloquear uma preferência de projeto para que os grupos possam configurá-la:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **[!UICONTROL Folhas de Horas e Horas]**, depois clique em **[!UICONTROL Preferências]**.

1. Siga um destes procedimentos:

   * Se quiser que os administradores de grupo possam configurar uma preferência para seus grupos, desbloqueie-a ![](assets/unlock-toggle-button.png).
   * Se quiser que todos os grupos usem sua configuração como preferência, verifique se ela está bloqueada (esse é o padrão).

      >[!IMPORTANT]
      >
      >Recomendamos que você se comunique com os administradores e usuários em grupos em todo o sistema para garantir que todas as necessidades sejam contabilizadas na forma como você configura uma preferência bloqueada. Ao bloqueá-lo, sua configuração é herdada por todos os grupos no sistema. E se a preferência tiver sido desbloqueada por algum período de tempo, sua configuração substituirá aquelas que os administradores de grupo podem ter feito.

1. Clique em **[!UICONTROL Salvar]**.
