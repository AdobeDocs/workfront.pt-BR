---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Configurar lembretes automáticos
description: Você pode configurar lembretes automáticos para acionar notificações por email quando todas as tarefas ou problemas estiverem vencidos, atrasados ou próximos à data planejada de conclusão.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sxv8RUKwTr-SABLfOrmTa0J9ToM62-1tF5rFEnu41UI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f283a5f64062e5878373527de46b0d993b545ba7
workflow-type: tm+mt
source-wordcount: 836
ht-degree: 6%

---

# Configurar lembretes automáticos

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador do Adobe Workfront, você pode configurar lembretes automáticos para acionar notificações por email quando todas as tarefas, problemas ou outros itens de trabalho atribuídos estiverem vencidos, atrasados ou próximos à data de conclusão planejada.

Após definir essas configurações, os usuários não poderão desativar lembretes automáticos. Os lembretes automáticos serão enviados independentemente das configurações de notificação de um usuário na área Minhas configurações.

Para notificações de atraso, o email é enviado à noite até que a tarefa ou o problema seja concluído. Isso significa que o usuário receberá uma notificação todos os dias enquanto a tarefa ou problema não for concluído.

Um lembrete automático pode ser enviado para um ou mais dos seguintes itens:

* Os usuários atribuídos a uma tarefa ou problema
* O gerente imediato do usuário
* O gerente do gerente imediato

>[!NOTE]
>
>Não é possível alterar o conteúdo ou a linha de assunto do email acionado por um lembrete automático.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <td>
   <p>Padrão</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Administrador do sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Detalhes da funcionalidade de lembrete automática

### Distinção de outros tipos de lembretes

Os lembretes automáticos são o recurso de lembrete no nível da configuração para tarefas e problemas do Workfront e são separados do recurso de Notificações de lembrete no nível do objeto. Para obter informações sobre a diferença entre lembretes automáticos e notificações de lembrete, consulte [Lembretes automáticos vs. notificações de lembrete](/help/quicksilver/administration-and-setup/tips-tricks-and-troubleshooting/auto-reminders-vs-reminder-notifications.md).

As decisões de prova e prova também não são tratadas por lembretes automáticos e seguem um processo de lembrete separado. Para obter detalhes sobre provas e lembretes de decisão de prova, consulte os artigos em [Notificações e lembretes de prova](/help/quicksilver/workfront-proof/wp-emailsntfctns/wp-emails-and-notifications.md).

## Considerações ao usar lembretes automáticos

Considere o seguinte ao usar lembretes automáticos:

* Os emails vencidos são enviados como um email de resumo por destinatário por dia, não como emails separados por item.
* Ativar lembretes automáticos pode fazer com que problemas ou tarefas que já estão vencidas apareçam no próximo email de resumo vencido, independentemente de quanto tempo o item está vencido.
* Os lembretes se aplicam somente a projetos com status Atual/Ativo.
* &quot;Dias&quot; na configuração automática de lembrete refere-se aos dias úteis com reconhecimento de agendamento, não aos dias decorridos ou à hora do calendário.



## Configurar lembretes automáticos

{{step-1-to-setup}}

1. Clique em **Email** > **Lembretes automáticos**.

1. Na área **Enviar uma notificação de atraso para**, selecione uma das seguintes opções:

   <table>
    <tr>
        <td>O usuário "Atribuído a"</td>
        <td>Selecione essa opção se desejar que o usuário atribuído a uma tarefa ou problema receba uma notificação de atraso sobre o atraso do item de trabalho.</td>
        <td></td>
    </tr>
    <tr>
        <td>O gerente do usuário</td>
        <td>Selecione essa opção se desejar que o gerente do usuário receba uma notificação atrasada sobre o atraso do item de trabalho do subordinado direto.</td>
        <td></td>
    </tr>
    <tr>
        <td>O gerente do gerente</td>
        <td>Selecione essa opção se desejar que o gerente imediato receba uma notificação de atraso sobre um item de trabalho de um dos usuários do subordinado direto atrasados.</td>
        <td></td>
    </tr>
    <tr>
        <td>O usuário "Atribuído a"</td>
        <td>(Na área <b>Enviar lembrete de prazo final para</b>.) Selecione esta opção se quiser que o usuário atribuído a uma tarefa ou um problema receba uma notificação sobre seu item de trabalho perto da data de vencimento.</td>
        <td></td>
    </tr>
   </table>

1. Selecione o tempo para o lembrete automático a ser enviado, selecionando o tempo antes ou depois da data de vencimento do item de trabalho.

   A hora é calculada a partir da Data de conclusão planejada da tarefa ou problema.

   Especifique o número de minutos, horas, dias, semanas ou meses para adicionar tempo à Data de conclusão planejada das tarefas ou problemas. Selecione **Minutos Decorridos**, **Horas Decorridas**, **Dias Decorridos** ou **Semanas Decorridas** para adicionar horas que incluam finais de semana, feriados e horas fora do horário comercial conforme indicado em sua agenda.

   Por exemplo, se uma tarefa for atribuída na sexta-feira e tiver uma duração de 3 dias decorridos, a data de conclusão da tarefa será definida para segunda-feira (supondo que sábado e domingo seja um fim de semana). Se a tarefa tiver uma duração de 3 dias (não decorridos), a data de conclusão da tarefa será definida para quarta-feira.

   ![Incrementos de tempo](assets/time-increments-for-automatic-reminder.png)

1. Clique em **Salvar**.

## Receber lembretes automáticos

Se você for a entidade designada em uma notificação de Lembrete automático, você receberá um email quando o prazo especificado for atingido. Para notificações de atraso, o email é enviado à noite até que a tarefa ou o problema seja concluído.

As tarefas com determinados tipos de dependência podem ser entregues após a data de início especificada, mesmo que estejam vencidas. Por exemplo, se uma tarefa tiver uma predecessora com uma dependência Finish-Start (fs), ela não será incluída no email, mesmo que tenha passado da data de início especificada, porque você não pode iniciar a tarefa até que a predecessora seja concluída.

Para obter mais informações sobre como receber emails de Lembretes automáticos, consulte a seção [Lembretes automáticos](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) em [Notificações do Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Enviar lembretes automáticos

Os lembretes automáticos são enviados assim que a hora selecionada pelo administrador do Workfront é atingida.

Se quiser acionar o envio manual dos emails de lembrete automáticos, use o Diagnóstico. Para obter mais informações sobre como acessar e usar o Diagnóstico no Workfront, consulte [Usar Diagnóstico para acionar processos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
