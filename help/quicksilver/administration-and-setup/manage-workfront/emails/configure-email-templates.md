---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: Configurar modelos de email
description: Como administrador do Adobe Workfront, você pode configurar modelos de email para suportar notificações de lembrete.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 1%

---

# Configurar modelos de email

Como administrador do Adobe Workfront, você pode configurar modelos de email para suportar notificações de lembrete.

Os modelos de email contêm a mensagem enviada aos usuários quando uma notificação de lembrete é iniciada.\
Sem um template de email, a notificação do lembrete será entregue como conteúdo vazio no corpo do email.

Os modelos de email podem ser associados a notificações de lembrete para problemas, tarefas, projetos e folhas de horas. Ao criar modelos de email, o administrador do Workfront pode fornecer conteúdo para o email e uma linha de assunto.

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

## Criar um novo modelo de email {#create-a-new-email-template}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel à esquerda, clique em **Email** > **Notificações**.

1. Clique no botão **Modelos de email** e, em seguida, clique em **Novo modelo de email**.

1. No **Novo modelo de email** na caixa exibida, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Modelo de email</td> 
      <td>Título do modelo de email (obrigatório).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Descrição do modelo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto</td> 
      <td>Especifique o tipo de objeto ao qual você deseja associar o modelo (obrigatório, por padrão, ele será definido como "Ocorrência").</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assunto </td> 
      <td>Assunto exibido quando a mensagem de email é enviada (obrigatório).</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> <p>Conteúdo exibido quando a mensagem de email é enviada.</p> <p>Você pode usar a formatação HTML para o conteúdo do email, conforme descrito em <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Adicionar a formatação de HTML a um modelo de email</a> neste artigo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

## Adicionar a formatação de HTML a um modelo de email {#add-html-formatting-to-an-email-template}

Você pode adicionar tags HTML a modelos de email para produzir notificações personalizadas.\
Comece a criar o template de email conforme descrito em [Criar um novo modelo de email](#create-a-new-email-template).

A formatação de HTML pode enriquecer seus modelos de email, conforme mostrado nas seções a seguir.

* [Vincular a objetos Workfront](#link-to-workfront-objects)
* [Vincular a campos personalizados com HTML](#link-to-custom-fields-with-html)
* [Exemplos de email do HTML](#html-email-examples)

### Vincular a objetos Workfront {#link-to-workfront-objects}

Você pode incluir links para campos do Workfront usando a variável `$$` curinga para informar ao gerador de email para procurar valores do banco de dados associado a um objeto específico.

Por exemplo, o corpo do email para uma notificação alertando o destinatário da tarefa que a tarefa está prestes a iniciar pode seguir esta estrutura:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b><strong>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td></tr>
</table>
</html>
```

Para obter o valor &quot;curinga&quot; para um objeto, siga um destes procedimentos:

<!-- Refer to the API Explorer and select the names of your objects from the Fields tab of any object. For more information about the API Explorer, see [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

* Use o valor &quot;campo de valor&quot; localizado dentro de uma exibição em modo de texto de um relatório. Para obter mais informações sobre valores do modo de texto, consulte [Visão geral do modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   O valor &quot;cabeçalho&quot; pode ser o nome do objeto, conforme você quer que ele apareça no corpo do email.

### Vincular a campos personalizados com HTML {#link-to-custom-fields-with-html}

Você pode incluir links para usuários e campos personalizados usando o **$$** curinga para informar ao gerador de email para procurar valores do banco de dados associado ao objeto. Eles devem estar presentes em ambos os lados da referência de atributo do banco de dados.

Por exemplo, adicionar o seguinte texto como HTML adicionaria o nome do usuário atribuído à notificação de lembrete associada a uma tarefa:

`assignedTo:firstName`

Para adicionar campos personalizados usando a mesma formatação, você pode adicionar o seguinte na notificação por email:

`DE:Custom Field As It Appears in Workfront`

Por exemplo, esse é um modelo de email que inclui uma referência a um campo personalizado chamado Data da entrega e assume-se que o campo Data da entrega pertence a uma tarefa.

Substituir `<your domain>` com o domínio Workfront de sua empresa, sem os colchetes:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which has a Delivery Date of $$DE:Task:Delivery Date$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
<tr>
<td><b>Description:</b></td>
<td>$$description$$</td>
<tr>
<td><b>Estimated Effort:</b></td>
<td>$$work$$ hours</td>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
<td><b>Delivery Date:</b></td>
<td>$$DE:Task:Delivery Date$$</td>
</tr>
</table>
</html>
```

>[!NOTE]
>
>Se o campo pertencer a um projeto, substitua a tarefa pelo projeto:
>
>`DE:Project:Delivery Date`

### Exemplos de email do HTML {#html-email-examples}

* [Notificação de lembrete de projeto atrasado (exemplo)](#late-project-reminder-notification-example)
* [Tarefa ou problema Sobre o lembrete de início (exemplo)](#task-or-issue-about-to-start-reminder-example)

#### Notificação de lembrete de projeto atrasado (exemplo) {#late-project-reminder-notification-example}

Para editar um modelo de email para um lembrete de projeto tardio, considere essas informações para os campos Assunto e Conteúdo .

Substituir `<your domain>` com o domínio Workfront de sua empresa, sem os colchetes.

**Assunto:**

Um Projeto Que Você Gerencia Ficou Atrasado

**Conteúdo:**

```html
<html>
<p>The <b><a href="https://<your domain>.my.workfront.com/project/view?ID=$$ID$$">$$name$$</a></b> project you are assigned as the owner of just became late.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
</tr>
</table>
<p>Please review the task plan and bring it up to date to reflect the progress made so far. If it is necessary to update the plan to bring it reflect reality going forward, be sure to speak to $$sponsor:name$$ for approval before make these changes to the work breakdown structure.</p>
</html>
```

Isso produz um email semelhante ao seguinte:

![](assets/screen-shot-2016-09-16-at-3.52.54-pm-350x103.png)

#### Tarefa ou problema Sobre o início do lembrete {#task-or-issue-about-to-start-reminder-example}

Você também pode criar uma notificação de lembrete para uma tarefa ou problema futuro.

O código a seguir pode ser incluído em um template de email a ser usado para tarefas e emitir notificações de lembrete que são enviadas qualquer número de dias antes da data de início planejada da tarefa ou problema.

Substituir `<your domain>` com o domínio Workfront de sua empresa, sem os colchetes.

Para usar isso em um email de Problema, altere o `/task/view.` no link para o item de trabalho para `/issue/view`.

**Assunto:**

`$$name$$ to start on $$plannedStartDate$$`

**Conteúdo:**

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><ahref=https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<tablewidth=350"style=font-size:12px;">
<tr>
<td><b>Task Name:</b></td>
<td>$$name$$</td>
</tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<td><b>Created on:</b></td>
<td>$$entryDate$$</td>
</tr>
<tr>
<td><b>Project Manager:</b></td>
<td>$$project:owner:name$$</td>
<tr>
<td><b>Priority:</b></td>
<td>$$priority$$</td>
</tr>
<tr>
<td><b>Who is assigned to:</b></td>
<td>$$assignedTo:name$$</td>
</tr>
<tr>
<td><b>When it's due:</b></td>
<td>$$estCompletionDate$$</td>
</tr>
</table>
</html>
```

![email_template_delivered.png](assets/email-template-delivered.png)

Depois que um modelo de email é criado, os usuários podem associá-lo às notificações de lembrete, conforme descrito em [Configurar notificações de lembrete](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
