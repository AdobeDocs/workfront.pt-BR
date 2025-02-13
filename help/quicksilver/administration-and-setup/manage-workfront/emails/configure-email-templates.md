---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: Configurar modelos de e-mail
description: Como administrador do Adobe Workfront, você pode configurar modelos de email para aceitar notificações de lembrete.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 3%

---


# Configurar modelos de email

<!--Audited: 10/2024-->


Como administrador do Adobe Workfront, você pode configurar modelos de email para aceitar notificações de lembrete.

Modelos de email contêm a mensagem enviada aos usuários quando uma notificação de lembrete é iniciada.\
Sem um template de email, a notificação de lembrete será entregue como conteúdo vazio no corpo do email.

Os modelos de email podem ser associados a notificações de lembrete para problemas, tarefas, projetos e folhas de horas. Ao criar modelos de email, o administrador do Workfront pode fornecer conteúdo para o email e uma linha de assunto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
   Ou
   <p>Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuração do nível de acesso</td> 
   <td> <p>Administrador do sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um modelo de email {#create-an-email-template}

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Email** > **Notificações**> **Modelos de email**.

   ![Guia Modelos de email](assets/email-templates-tab-under-setup-email-notifications-area.png)

1. Clique em **Novo Modelo de email**.

1. Na caixa **Novo Modelo de email**, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Adicione um título para o modelo de email. Este campo é obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto</td> 
      <td>Especifique o tipo de objeto ao qual deseja associar o modelo. Escolha entre os seguintes objetos:
      <ul>
      <li>Projeto</li>
      <li>Tarefa</li>
      <li>Problema</li>
      <li>Planilha de horas</li> </ul>

   Este campo é obrigatório e está definido como Projeto, por padrão.</td>
   </tr>
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Adicione mais informações sobre o modelo de email, sua finalidade e público-alvo.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Assunto </td> 
      <td>Adicione o texto que é exibido na linha Assunto do email, quando a mensagem de email gerada pelo template é enviada. Este campo é obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Corpo </td> 
      <td> <p>Adicione o texto para o conteúdo da mensagem de email.</p> <p>Você pode usar a formatação HTML para o conteúdo de email, conforme descrito na seção <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Adicionar formatação HTML a um modelo de email</a> deste artigo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

## Adicionar formatação de HTML a um modelo de email {#add-html-formatting-to-an-email-template}

Você pode adicionar tags HTML a modelos de email para produzir notificações personalizadas.\
Comece a criar o modelo de email conforme descrito em [Criar um novo modelo de email](#create-a-new-email-template).

A formatação de HTML pode enriquecer seus modelos de email, conforme mostrado nas seções a seguir.

* [Vincular a objetos do Workfront](#link-to-workfront-objects)
* [Vincular a campos personalizados com HTML](#link-to-custom-fields-with-html)
* [exemplos de email do HTML](#html-email-examples)

### Vincular a objetos do Workfront {#link-to-workfront-objects}

Você pode incluir links para campos do Workfront usando o curinga `$$` para instruir o gerador de email a procurar valores no banco de dados associado a um objeto específico.

Por exemplo, o corpo do email de uma notificação alertando o destinatário da tarefa que a tarefa está prestes a iniciar pode seguir esta estrutura:

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

Para obter o valor &quot;curinga&quot; de um objeto, siga um destes procedimentos:

* Consulte o API Explorer e selecione os nomes dos objetos na guia Fields de qualquer objeto. Para obter mais informações sobre o API Explorer, consulte [API Explorer](/help/quicksilver/wf-api/general/api-explorer.md).

* Use o valor `valuefield` encontrado em um modo de exibição de texto de um relatório. Para obter mais informações sobre valores de modo de texto, consulte [Visão geral do Modo de Texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

O valor `heading` pode ser o nome do objeto, conforme você quer que ele apareça no corpo do email.

### Vincular a campos personalizados com HTML {#link-to-custom-fields-with-html}

Você pode incluir links para usuários e campos personalizados usando o curinga `$$` para instruir o gerador de email a procurar valores no banco de dados associado ao objeto. Eles devem estar presentes em ambos os lados da referência de atributo do banco de dados.

Por exemplo, adicionar o texto a seguir como HTML adicionaria o nome do usuário atribuído à notificação de lembrete associada a uma tarefa:

`assignedTo:firstName`

Para adicionar campos personalizados usando a mesma formatação, você pode adicionar o seguinte na notificação por email:

`DE:Custom Field As It Appears in Workfront`

Por exemplo, este é um template de email que inclui uma referência a um campo personalizado chamado Data de entrega e está presumindo que o campo Data de entrega pertence a uma tarefa.

Substitua `<your domain>` pelo domínio Workfront da sua empresa, sem os colchetes:

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
>Se o campo pertencer a um projeto, substituir tarefa por projeto:
>
>`DE:Project:Delivery Date`

### exemplos de email do HTML {#html-email-examples}

* [Notificação de lembrete de Projeto Atrasado (exemplo)](#late-project-reminder-notification-example)
* [Lembrete sobre Tarefa ou Problema Prestes a Iniciar (exemplo)](#task-or-issue-about-to-start-reminder-example)

#### Notificação de lembrete de Projeto atrasado (exemplo) {#late-project-reminder-notification-example}

Para editar um modelo de email para um lembrete de projeto atrasado, considere essas informações para os campos Assunto e Conteúdo.

Substitua `<your domain>` pelo domínio Workfront da sua empresa, sem os colchetes.

**Assunto:**

Um Projeto Que Você Gerencia Se Atrasou

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

Isso produzirá um email semelhante ao seguinte:

![Email de atraso do projeto](assets/project-became-late-email.png)

#### Lembrete de Tarefa ou Problema Prestes a Iniciar {#task-or-issue-about-to-start-reminder-example}

Você também pode criar uma notificação de lembrete para uma tarefa ou problema futuro.

O código a seguir pode ser incluído em um modelo de email a ser usado para notificações de lembrete de tarefas e problemas que são enviadas qualquer número de dias antes da data planejada de início da tarefa ou problema.

Substitua `<your domain>` pelo domínio Workfront da sua empresa, sem os colchetes.

Para usar isso para um email de Problema, altere o valor `/task/view.` no link para o item de trabalho `/issue/view`.

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

![modelo_de_email_entregue.png](assets/email-template-delivered.png)

Depois que um modelo de email é criado, os usuários podem associá-lo a notificações de lembrete, conforme descrito em [Configurar notificações de lembrete](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
