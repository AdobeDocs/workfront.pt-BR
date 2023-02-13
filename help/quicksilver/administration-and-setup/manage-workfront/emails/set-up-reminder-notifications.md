---
title: Configurar notificações de lembrete
description: Configurar notificações de lembrete
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6c0fa8af-cd89-4941-a6f6-aa4e84a7dc67
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 1%

---

# Configurar notificações de lembrete

As notificações de lembrete enviam emails para recipients com base em critérios especificados. Como administrador do Adobe Workfront ou usuário com nível de acesso do Planejador e acesso administrativo a notificações de lembrete, você pode associar manualmente notificações de lembrete aos itens de trabalho, como projetos, tarefas, problemas e folhas de horas.

<!--
DRAFTED IN FLARE:
An example of how this can be used would be helpful here and/or in the section </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications" class="MCXref xref">Reminder notifications</a>
 in </span>
<a href="../../../workfront-basics/using-notifications/wf-notifications.md" class="MCXref xref">Adobe Workfront notifications</a>

-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Planejador ou superior, com acesso administrativo às notificações de lembrete</p> <p>Para obter informações sobre como conceder acesso administrativo a um Usuário do Plano, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Personalizar o email de lembrete

Você pode personalizar a notificação do lembrete com um email personalizado que inclui um assunto e um corpo de email personalizados. O corpo do email pode conter HTML personalizado.

Ou você pode usar o email padrão incluído com a notificação do lembrete. O email padrão usa o nome da notificação de lembrete como o assunto do email e o nome do objeto no corpo do email, incluindo o evento que acionou a notificação.

Se quiser personalizar o email de lembrete, é necessário criar um modelo de email e anexá-lo à notificação de lembrete.

Para obter informações sobre como criar um modelo de email, consulte [Configurar modelos de email](../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md).

## Criar uma notificação de lembrete

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Email** > **Notificações**.

1. Clique no botão **Notificações de Lembrete** e, em seguida, clique em **Notificação de novo lembrete**.

1. Na lista suspensa, clique no tipo de objeto que deseja associar à notificação de lembrete.

   Por exemplo, se você quiser anexar uma notificação de lembrete a uma folha de ponto, clique em **Folha de Horas**.

1. No **Notificação de novo lembrete** especifique as seguintes informações.

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
      <td> <p>Especifique o número de horas, dias de trabalho, dias (dias de calendário), semanas ou meses antes ou depois da data no <strong>Tempo</strong> campo.</p> <p><b>Nota</b>:  
        <ul> 
         <li> <p>As notificações de lembrete começam 24 horas após a data especificada e depois que todos os critérios são atendidos.</p> </li> 
         <li> <p>Lembre-se das notificações de projetos, tarefas e problemas que são acionados todas as noites à meia-noite, Hora das Montanhas dos EUA. Todos os objetos que se qualificam para uma notificação de lembrete a partir desse dia acionam uma notificação para os usuários designados logo após esse período.</p> </li> 
         <li> <p>As notificações de lembrete das folhas de ponto são enviadas no horário especificado com base no fuso horário e na Data final, Data inicial ou Data da última atualização da folha de ponto.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Intervalo</td> 
      <td> <p>Selecione o evento que aciona a notificação de lembrete a ser agendada.</p> <p>Se a notificação de lembrete for destinada a projetos, tarefas ou problemas, as opções disponíveis estarão relacionadas à Data de conclusão ou Data inicial. A notificação de lembrete leva em conta o carimbo de data e hora de conclusão e de início de projetos, tarefas e problemas.</p> <p>Se a notificação de lembrete for destinada às Folhas de horas, as opções disponíveis estarão relacionadas à Data final, Data inicial ou Data da última atualização. A notificação de lembrete para Folhas de Horas leva em consideração o carimbo de data e hora do Fim da Folha de Horas, Início e Data da Última Atualização. A Folha de Horas começa à meia-noite no dia da Data de Início (12:00 AM) e termina logo antes da meia-noite na Data de Término (11:59 PM).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Critério</td> 
      <td> <p>Selecione os critérios para qualificar a notificação de lembrete a ser agendada. As notificações de lembrete não são programadas, a menos que a seleção do critério seja atendida.</p> <p>As opções de critérios a seguir estão disponíveis, dependendo do tipo de objeto selecionado na Etapa 4:</p> 
       <ul> 
        <li><strong>Incompleto em projetos atuais:</strong> (Disponível para lembretes de tarefas e de problemas) A notificação de lembrete é agendada para ser enviada somente quando o status do objeto ao qual a notificação de lembrete está associada não estiver Concluído e o status do projeto for Atual.</li> 
        <li><strong>Todos nos Projetos atuais:</strong>(Disponível para lembretes de tarefas e de problemas) A notificação de lembrete é agendada para ser enviada independentemente do status do objeto e somente quando o status do projeto ao qual a notificação de lembrete está associada é Current.</li> 
        <li><strong>Projetos incompletos:</strong> (Disponível para lembretes de projeto) A notificação de lembrete é agendada para ser enviada quando o status do projeto não for Concluído.</li> 
        <li><strong>Projetos completos:</strong> (Disponível para lembretes de projeto) A notificação de lembrete é agendada para ser enviada quando o status do projeto for Concluído.</li> 
        <li><strong>Abrir Folhas de Horas:</strong> (Disponível para lembretes de folha de ponto) A notificação de lembrete é agendada para ser enviada quando o status da folha de ponto é Aberta.</li> 
        <li><strong>Folhas de Horas Enviadas:</strong> (Disponível para lembretes de folha de ponto) A notificação de lembrete é agendada para ser enviada quando o status da folha de ponto é Enviado.</li> 
        <li><strong>Abrir Folha de Horas ou Menos de 40 Horas por Semana:</strong> (Disponível para lembretes de folha de ponto) A notificação de lembrete é agendada para ser enviada quando o status da folha de ponto é Aberta ou quando a folha de ponto tem menos de 40 horas registradas.</li> 
        <li><strong>Modelo de email:</strong> No menu suspenso , selecione um template de email para anexar ao seu lembrete.<br>Para obter informações sobre como criar um template de email, consulte <a href="../../../administration-and-setup/manage-workfront/emails/configure-email-templates.md" class="MCXref xref">Configurar modelos de email</a>.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Recipients</td> 
      <td>Selecione os tipos de usuários que deseja receber a notificação. Selecione dentre vários participantes do objeto, como proprietário, aprovador ou destinatário.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.
1. Anexe a notificação do lembrete a um item de trabalho, conforme descrito em [Anexar uma notificação de lembrete a um objeto](../../../workfront-basics/using-notifications/attach-reminder-notification-object.md).

## Receber uma notificação de lembrete

Quando a condição é atendida no item que tem a notificação de lembrete anexada, uma notificação por email é acionada ao usuário definido na notificação do lembrete.

Para obter mais informações sobre o recebimento de notificações de lembrete, consulte o [Notificações de lembrete](../../../workfront-basics/using-notifications/wf-notifications.md#reminder-notifications) seção em [Notificações do Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Teste o delivery de notificação do lembrete

As notificações de lembrete são acionadas todas as noites à meia-noite, Mountain Time. Todos os objetos que se qualificam para uma notificação de lembrete acionam uma notificação para os usuários designados logo depois disso.

Para fazer com que as notificações de lembrete sejam acionadas manualmente, a condição do lembrete deve ser cumprida primeiro.\
Por exemplo, se um lembrete for definido para disparar uma hora após a Data de conclusão planejada de um projeto, esse tempo deve ter passado entre quando o lembrete foi definido e agora. Qualquer projeto que tenha programado datas de conclusão antes de o lembrete ser ativado não acionará uma notificação.

Para fazer com que uma notificação de lembrete seja acionada manualmente:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Diagnóstico** no canto inferior esquerdo do Workfront.

1. Clique em **Enviar notificações de lembrete** e aguarde a confirmação na parte superior da tela de que eles foram enviados.

   Os usuários designados na notificação do lembrete recebem um email.
