---
title: Configurar notificações de lembrete
description: Configurar notificações de lembrete
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 1129f8ab93d349325bed56bc2b3ba94c2600c03f
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 1%

---

# Configurar notificações de lembrete

As notificações de lembrete enviam emails para recipients com base em critérios especificados. Como administrador do Adobe Workfront ou usuário com nível de acesso de Planejador e acesso administrativo a notificações de lembrete, você pode associar manualmente notificações de lembrete a itens de trabalho, como projetos, tarefas, problemas e folhas de horas.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Planejador ou superior, com acesso administrativo a notificações de lembrete</p> <p>Para obter informações sobre como conceder acesso administrativo a um usuário do Plano, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Personalizar o email de lembrete

Você pode personalizar a notificação de lembrete com um email personalizado que inclui um assunto e um corpo de email personalizados. O corpo do email pode conter HTML personalizado.

Ou você pode usar o email padrão incluído na notificação de lembrete. O email padrão usa o nome da notificação de lembrete como o assunto do email e o nome do objeto no corpo do email, incluindo o evento que acionou a notificação.

Se quiser personalizar o email de lembrete, crie um modelo de email e anexe-o à notificação de lembrete.

Para obter informações sobre como criar um template de email, consulte [Configurar modelos de email](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Criar uma notificação de lembrete

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **E-mail** > **Notificação** > **Notificações de lembrete**.

   ![](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Clique em **Nova Notificação de Lembrete**.

1. Na lista suspensa, clique no tipo de objeto que deseja associar à notificação de lembrete.

   Por exemplo, se você deseja anexar uma notificação de lembrete a uma folha de horas, clique em **Planilha de horas**.

1. No **Nova Notificação de Lembrete** que for exibida, especifique as informações a seguir.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome da notificação de lembrete</td> 
      <td>Especifique um nome para a notificação de lembrete.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Período de qualificação</td> 
      <td> <p>Especifique o número de horas, dias de trabalho, dias (dias do calendário), semanas ou meses antes ou depois da data no <strong>Tempo</strong> campo.</p> <p><b>Nota</b>:  
        <ul> 
         <li> <p>As notificações de lembrete começam 24 horas após a data especificada e assim que todos os critérios são atendidos.</p> </li> 
         <li> <p>Notificações de lembrete para projetos, tarefas e problemas são acionadas todas as noites à meia-noite, horário das montanhas dos EUA. Todos os objetos qualificados para uma notificação de lembrete desse dia acionam uma notificação para os usuários designados logo após esse horário.</p> </li> 
         <li> <p>Notificações de lembrete para planilhas de horas são enviadas no horário especificado com base em seu fuso horário e na Data final, Data inicial ou Data da última atualização da planilha de horas.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Intervalo</td> 
      <td> <p>Selecione o evento que aciona a notificação de lembrete a ser agendada.</p> <p>Se a notificação de lembrete for destinada a projetos, tarefas ou problemas, as opções disponíveis estarão relacionadas à Data de conclusão ou Data de início. A notificação de lembrete leva em conta a marca de data e hora nas datas de conclusão e início dos projetos, tarefas e problemas.</p>

   <p>Se a notificação de lembrete for destinada a Folhas de horas, as opções disponíveis estarão relacionadas à Data final, Data inicial ou Data da última atualização. A notificação de lembrete para Folhas de horas leva em conta o carimbo de data e hora de Término, Data de Início e Última Atualização da folha de horas. A Planilha de Horas começa à meia-noite no dia da Data de Início (12h) e termina pouco antes da meia-noite na Data de Término (23h59).</p>

   <p><b>Nota</b></p>
      <p>As notificações de lembrete de folha de horas são distribuídas apenas uma vez a cada 24 horas.</p> <p>Quando você configura várias notificações de lembrete em um período de 24 horas, o Workfront envia um email de notificação com todos os lembretes incluídos nessa notificação.</p>
      <p>Por exemplo, se você configurar três notificações de lembrete para acionar 10 horas antes, 2 horas antes e 1 hora antes de uma data de vencimento, os três lembretes serão combinados na mesma notificação se ocorrerem durante o mesmo dia.</p> <p>No entanto, se você definir uma notificação de lembrete para 26 horas antes e outra para 1 hora antes de uma data de vencimento, os usuários receberão duas notificações separadas. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Critério</td> 
      <td> <p>Selecione os critérios para qualificar a notificação de lembrete a ser agendada. Notificações de lembrete não são agendadas a menos que a seleção de critérios seja atendida.</p> <p>As opções de critérios a seguir estão disponíveis, dependendo do tipo de objeto selecionado na Etapa 4:</p> 
       <ul> 
        <li><strong>Projetos em Andamento Incompletos:</strong> (Disponível para lembretes de tarefas e problemas) A notificação de lembrete é agendada para ser enviada somente quando o status do objeto ao qual a notificação de lembrete está associada não é Concluído e o status do projeto é Atual.</li> 
        <li><strong>Todos os projetos atuais:</strong>(Disponível para lembretes de tarefas e problemas) A notificação de lembrete é agendada para ser enviada independentemente do status do objeto e somente quando o status do projeto ao qual a notificação de lembrete está associada for Atual.</li> 
        <li><strong>Projetos Incompletos:</strong> (Disponível para lembretes de projeto) A notificação de lembrete é agendada para ser enviada quando o status do projeto for qualquer item menos Concluído.</li> 
        <li><strong>Concluir projetos:</strong> (Disponível para lembretes de projeto) A notificação de lembrete é agendada para ser enviada quando o status do projeto for Concluído.</li> 
        <li><strong>Abrir Planilhas de Horas:</strong> (Disponível para lembretes de folha de horas) A notificação de lembrete é agendada para ser enviada quando o status da folha de horas for Aberto.</li> 
        <li><strong>Planilha de horas enviada:</strong> (Disponível para lembretes de folha de horas) A notificação de lembrete é agendada para ser enviada quando o status da folha de horas for Enviado.</li> 
        <li><strong>Planilha de horas em aberto ou menos de 40 horas por semana:</strong> (Disponível para lembretes de folha de horas) A notificação de lembrete é agendada para ser enviada quando o status da folha de horas for Aberto ou quando a folha de horas tiver menos de 40 horas registrada.</li> 
        <li><strong>Modelo de email:</strong> Na lista suspensa, selecione um template de email para anexar ao seu lembrete.<br>Para obter informações sobre como criar um template de email, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurar modelos de email</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recipients</td> 
      <td>Selecione os tipos de usuários que você deseja que recebam a notificação. Selecione entre vários participantes do objeto, como proprietário, aprovador ou designado.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
1. Anexe a notificação de lembrete a um item de trabalho, conforme descrito em [Anexar uma notificação de lembrete a um objeto](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Receber uma notificação de lembrete

Quando a condição for atendida no item que tem o lembrete de notificação anexado, uma notificação por email será acionada para o usuário definido na notificação de lembrete.

Para obter mais informações sobre como receber notificações de lembrete, consulte [Notificações de lembrete](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) seção em [Notificações do Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Testar entrega de notificação de lembrete

As notificações de lembrete são acionadas todas as noites à meia-noite, horário das montanhas dos EUA. Todos os objetos qualificados para uma notificação de lembrete acionam uma notificação aos usuários designados logo em seguida.

Para fazer com que as notificações de lembrete sejam acionadas manualmente, a condição para o lembrete deve ser atendida primeiro.\
Por exemplo, se um lembrete for definido para ser acionado uma hora após a Data de conclusão planejada de um projeto, esse tempo deve ter transcorrido entre o momento em que o lembrete foi definido e agora. Qualquer projeto com datas de conclusão planejadas após a ativação do lembrete não acionará uma notificação.

Para fazer com que uma notificação de lembrete seja acionada manualmente:

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Diagnóstico** no canto inferior esquerdo do Workfront.

1. Clique em **Enviar Notificações de Lembrete** e aguarde a confirmação na parte superior da tela de que eles foram enviados.

   Os usuários designados na notificação de lembrete recebem um email.
