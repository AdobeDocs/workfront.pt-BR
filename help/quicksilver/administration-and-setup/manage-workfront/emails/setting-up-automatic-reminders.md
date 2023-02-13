---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Configurar lembretes automáticos
description: Configurar lembretes automáticos
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# Configurar lembretes automáticos

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador do Adobe Workfront, você pode configurar lembretes automáticos para acionar notificações por email quando todas as tarefas ou problemas forem devidos, atrasados ou próximos da data de conclusão planejada. Após definir essas configurações, os usuários não poderão desativar lembretes automáticos.

Para notificações tardias, o email é enviado noturna até que a tarefa ou o problema seja concluído.

Um lembrete automático pode ser enviado para um ou mais dos seguintes:

* Os usuários atribuídos a uma tarefa ou problema
* O gerente imediato do usuário
* O gerente do gerente imediato

>[!NOTE]
>
>Não é possível alterar o conteúdo ou a linha de assunto do email acionada por um lembrete automático.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Administrador do sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar lembretes automáticos

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Email** >**Lembretes Automáticos**.

1. No **Enviar uma notificação atrasada para** selecione qualquer uma das seguintes opções:

   <table>
    <tr>
        <td>O usuário "Atribuído a"</td>
        <td>Selecione esta opção se desejar que o usuário atribuído a uma tarefa ou emissão receba uma notificação tardia sobre o atraso do item de trabalho.</td>
        <td></td>
    </tr>
    <tr>
        <td>O gerente do usuário</td>
        <td>Selecione essa opção se desejar que o gerente do usuário receba uma notificação tardia sobre o atraso do item de trabalho do relatório direto.</td>
        <td></td>
    </tr>
    <tr>
        <td>O gerente do gerente</td>
        <td>Selecione essa opção se desejar que o gerente imediato receba uma notificação tardia sobre um item de trabalho de um dos usuários do relatório direto atrasados.</td>
        <td></td>
    </tr>
    <tr>
        <td>O usuário "Atribuído a"</td>
        <td>(No <b>Enviar lembrete de prazo para</b> área.) Selecione esta opção se desejar que o usuário atribuído a uma tarefa ou problema receba uma notificação sobre seu item de trabalho se aproximando da data de vencimento.</td>
        <td></td>
    </tr>
</table>

1. Selecione a hora para enviar o lembrete automático selecionando a quantidade de tempo antes ou depois da data de vencimento do item de trabalho.

   A hora é calculada a partir da Data de Conclusão Planejada da tarefa ou emissão.

   Especifique o número de minutos, horas, dias, semanas ou meses para adicionar tempo à Data de conclusão planejada das tarefas ou problemas. Selecionar **Minutos Aprovados**, **Horas Decorridas**, **Dias Aproveitados** ou **Semanas Decorrido** para adicionar tempo que inclua todos os fins de semana, feriados e horas que não estejam funcionando, conforme indicado em sua programação.

   Por exemplo, se uma tarefa for atribuída na sexta-feira e tiver uma duração de 3 dias decorridos, a data de conclusão da tarefa será definida para Segunda-feira (supondo que sábado e domingo seja um fim de semana). Se a tarefa tiver uma duração de 3 dias (não decorrido), a data de conclusão da tarefa será definida para quarta-feira.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Clique em **Salvar**.

## Receber lembretes automáticos

Se você for a entidade designada em uma notificação de lembrete automático, receberá um email quando o prazo especificado for atingido. Para notificações tardias, o email é enviado noturna até que a tarefa ou o problema seja concluído.

Tarefas com determinados tipos de dependência podem ser entregues após a data de início especificada, mesmo que estejam vencidas. Por exemplo, se uma tarefa tiver um antecessor com uma dependência de Finish-Start (fs), ela não será incluída no email, mesmo que tenha passado a data de início especificada, pois não é possível iniciar a tarefa até que o antecessor esteja concluído.

Para obter mais informações sobre como receber emails de Lembretes Automáticos, consulte o [Lembretes automáticos](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) seção em [Notificações do Adobe Workfront](../../../workfront-basics/using-notifications/wf-notifications.md).

## Enviar lembretes automáticos

Os lembretes automáticos são enviados assim que a hora selecionada pelo administrador do Workfront é atendida.

Se quiser acionar o envio manual dos emails de lembrete automático, é possível fazer isso usando o Diagnostics. Para obter mais informações sobre como acessar e usar Diagnósticos no Workfront, consulte [Use o Diagnostics para acionar processos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
