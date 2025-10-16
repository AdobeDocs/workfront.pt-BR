---
title: Configurar Notificações de Lembrete
description: As notificações de lembrete geram emails enviados aos usuários com base em critérios especificados. Notificações de lembrete lembram os usuários de uma ação que eles precisam tomar para uma tarefa, problema, projeto ou planilha de horas.
author: Alina, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 2%

---

# Configurar notificações de lembrete

<!-- Audited: 1/2024 -->

Como administrador do Workfront, você pode criar notificações de lembrete para usuários e associá-las a objetos aos quais você deseja que os usuários prestem atenção especial.

As notificações de lembrete geram emails enviados aos usuários com base em critérios especificados. Notificações de lembrete lembram os usuários de uma ação que eles precisam tomar para uma tarefa, problema, projeto ou planilha de horas.

Depois de criar as notificações de lembrete, os usuários podem associá-las manualmente a itens de trabalho, como projetos, tarefas, problemas e planilhas de horas. Para obter informações, consulte [Anexar uma notificação de lembrete a um objeto](/help/quicksilver/workfront-basics/using-notifications/attach-reminder-notification-object.md).

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard </p>
<p>Plano</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Planejador ou superior, com acesso administrativo a notificações de lembrete</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar o email de lembrete

Você pode personalizar o assunto, o corpo e a HTML no email de notificação de lembrete.

Ou você pode usar o email padrão incluído na notificação de lembrete. O email padrão usa o nome da notificação de lembrete como o assunto do email e o nome do objeto no corpo do email, incluindo o evento que acionou a notificação.

Se quiser personalizar o email de lembrete, crie um modelo de email e anexe-o à notificação de lembrete.

Para obter informações sobre como criar um modelo de email, consulte [Configurar modelos de email](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Criar uma notificação de lembrete

{{step-1-to-setup}}

1. Clique em **Email** > **Notificações** > **Notificações de Lembrete**.

   ![Guia de notificações de lembrete](assets/remider-notifications-tab-in-setup-email-notifications-area.png)

1. Clique em **Nova Notificação de Lembrete**.

1. Na lista suspensa, clique no tipo de objeto que deseja associar à notificação de lembrete.

   Por exemplo, se você deseja anexar uma notificação de lembrete a uma folha de horas, clique em **Folha de horas**.

1. Na caixa **Nova Notificação de Lembrete** exibida, especifique as informações a seguir.

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
      <td> <p>Especifique o número de horas, dias úteis, dias (dias do calendário), semanas ou meses antes ou depois da data no campo <strong>Horário</strong>.</p> <p><b>NOTA</b>:  
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
      <td role="rowheader">Critérios</td> 
      <td> <p>Selecione os critérios para qualificar a notificação de lembrete a ser agendada. Notificações de lembrete não são agendadas a menos que a seleção de critérios seja atendida.</p> <p>As opções de critérios a seguir estão disponíveis, dependendo do tipo de objeto selecionado na Etapa 4:</p> 
       <ul> 
        <li><strong>Incompleto nos Projetos Atuais:</strong> <i>(Disponível para lembretes de tarefas e problemas)</i> A notificação de lembrete está agendada para ser enviada somente quando o status do objeto ao qual a notificação de lembrete está associada não é Concluído e o status do projeto é Atual.</li> 
        <li><strong>Todos nos Projetos Atuais:</strong> <i>(Disponível para lembretes de tarefas e problemas)</i> A notificação de lembrete está agendada para ser enviada independentemente do status do objeto e somente quando o status do projeto ao qual a notificação de lembrete está associada for Atual.</li> 
        <li><strong>Projetos Incompletos:</strong> <i>(Disponível para lembretes de projeto)</i> A notificação de lembrete está agendada para ser enviada quando o status do projeto for qualquer coisa menos Concluído.</li> 
        <li><strong>Todos os Projetos:</strong> <i>(Disponível para lembretes de projeto)</i> A notificação de lembrete está agendada para ser enviada independentemente do status do projeto.</li> 
        <li><strong>Abrir Planilha de Horas:</strong> <i>(Disponível para lembretes de planilha de horas)</i> A notificação de lembrete está agendada para ser enviada quando o status da planilha de horas for Aberto.</li> 
        <li><strong>Folhas de Horas Enviadas:</strong> <i>(Disponível para lembretes de folha de horas)</i> A notificação de lembrete está agendada para ser enviada quando o status da folha de horas for Enviado.</li> 
        <li><strong>Abrir Planilha de Horas ou Menos de 40 Horas por Semana:</strong> <i>(Disponível para lembretes de planilha de horas)</i> A notificação de lembrete está agendada para ser enviada quando o status da planilha de horas for Aberto ou quando a planilha de horas tiver menos de 40 horas registrada.</li> 
        <li><strong>Modelo de email:</strong> No menu suspenso, selecione um modelo de email para anexar ao seu lembrete.<br>Para obter informações sobre como criar um modelo de email, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurar modelos de email</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recipients</td> 
      <td><p>Dependendo do objeto ao qual se destina a notificação de lembrete, selecione um dos seguintes tipos de usuários que você deseja receber a notificação:</p>
      <ul>
      <li>Atribuído para</li>
      <li>Cadastrado por</li>
      <li>Equipe do projeto (todos os usuários na equipe do projeto recebem o lembrete)</li>
      <li>Tarefas dependentes atribuídas (os usuários atribuídos a tarefas dependentes recebem o lembrete)</li>
      <li>Proprietário do projeto</li>
      <li>Atribuído a (os usuários atribuídos a uma tarefa ou um problema recebem o lembrete)</li>
      <li>Proprietário da planilha de horas</li>
      <li>Aprovador de planilha de horas</li>
      <li>Gerenciador do proprietário da planilha de horas</li></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
1. Anexe a notificação de lembrete a um item de trabalho, conforme descrito em [Anexar uma notificação de lembrete a um objeto](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Receber uma notificação de lembrete

Quando a condição for atendida no item que tem o lembrete de notificação anexado, uma notificação por email será acionada para o usuário definido na notificação de lembrete.

Para obter mais informações sobre como receber notificações de lembrete, consulte a seção [Notificações de lembrete](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) em [Notificações do Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Testar entrega de notificação de lembrete

As notificações de lembrete são acionadas todas as noites à meia-noite, horário das montanhas dos EUA. Todos os objetos qualificados para uma notificação de lembrete acionam uma notificação aos usuários designados logo em seguida.

Para fazer com que as notificações de lembrete sejam acionadas manualmente, a condição para o lembrete deve ser atendida primeiro.\
Por exemplo, se um lembrete for definido para ser acionado uma hora após a Data de conclusão planejada de um projeto, esse tempo deve ter transcorrido entre o momento em que o lembrete foi definido e agora. Qualquer projeto com datas de conclusão planejadas após a ativação do lembrete não acionará uma notificação.

Para fazer com que uma notificação de lembrete seja acionada manualmente:

{{step-1-to-setup}}

1. Clique em **Sistema** > **Diagnósticos** no canto inferior esquerdo do Workfront.

1. Clique em **Enviar Notificações de Lembrete** e aguarde a confirmação na parte superior da tela de que elas foram enviadas.

   Os usuários designados na notificação de lembrete recebem um email.

![Teste de notificação de lembrete](assets/reminder-test.png)
