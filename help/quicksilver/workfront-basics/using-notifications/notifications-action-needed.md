---
content-type: reference
navigation-topic: notifications
title: "Notificações: ação necessária"
description: As notificações a seguir informam se é necessário realizar alguma ação em um item de trabalho. Para obter informações sobre como configurar as notificações recebidas, consulte Modificar suas próprias notificações por email.
author: Lisa
feature: Get Started with Workfront
exl-id: dd383bd4-da30-45ea-889e-e6b49416974b
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '2442'
ht-degree: 0%

---

# Notificações: [!UICONTROL Ação necessária]

As notificações a seguir informam se é necessário realizar alguma ação em um item de trabalho. Para obter informações sobre como configurar as notificações recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Consulte também [Notificações de eventos](../../workfront-basics/using-notifications/event-notifications.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th> <p>Campos incluídos </p> <p> *Somente campos de resumo diários</p> </th> 
   <th>Status padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recebo uma nova solicitação de trabalho</strong> </p> <p>O destinatário do item de trabalho recebe uma notificação por email, a menos que o usuário que faz a solicitação também seja o destinatário. </p> <p>Uma notificação não será enviada se o status da tarefa for [!UICONTROL Concluído] ou se o status do problema for [!UICONTROL Fechado].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Nova Solicitação de Trabalho]: &lt;Nome da Solicitação&gt;</em></p> <p>O assunto da notificação de resumo diário é: <em>[!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome da tarefa</p> <p>[!UICONTROL Data de Término Planejada]</p> <p>Pais</p> <p>Atribuído por</p> <p>Atribuído a</p> <p>[!UICONTROL Status]</p> <p>[!UICONTROL Descrição]</p> <p>Botão [!UICONTROL View]<br>Opção para adicionar ao resumo diário</p> <br> </td> 
   <td><strong>Instantâneo e</strong> <strong>Diário</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Preciso aprovar um documento</strong> </p> <p>O aprovador de um documento recebe uma notificação quando está listado como o aprovador.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome do usuário que enviou a aprovação&gt; [!UICONTROL solicitou a aprovação de um documento em [!DNL Adobe Workfront].]</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Nome do usuário que enviou a aprovação<br>Nome do Documento<br>Número de Referência do Documento<br>Data e Hora da Aprovação Solicitada<br>Detalhes do Documento (formato, tamanho, número da versão)<br><strong>[!UICONTROL Tomar Decisão de Aprovação]</strong> botão<br>*Número total de aprovações de documentos pendentes<br>*Link para <strong>[!UICONTROL Aprovações de Documentos</strong>*<strong>Ver Todas as Aprovações]</strong> botão<br>*Data do resumo diário<br></td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Preciso aprovar um projeto</strong> </p> <p>No caso de aprovações de funções de trabalho, os usuários que recebem uma notificação por email para esse evento dependerão se a configuração '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]' está habilitada (conforme descrito em <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>). </p> <p><strong>Se esta opção estiver habilitada</strong>, uma notificação por email será enviada a todos os usuários do sistema com a função de trabalho associada à aprovação. </p> <p><strong>Se esta opção estiver desabilitada</strong>, somente membros da equipe do projeto com a função de trabalho associada ao processo de aprovação receberão uma notificação por email.</p> <p>Se a aprovação estiver associada a um usuário, ele receberá a notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Projeto Pendente de Aprovação]: &lt;Nome do Projeto&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que enviou a aprovação<br>Status de Aprovação Pendente<br>Data e Hora da Aprovação Solicitada<br>Prioridade do Projeto<br>Etapa de Aprovação Pendente de Aprovação<br>Número de decisões aguardando aprovação<br>Nome dos Aprovadores (somente usuários)<br>[!UICONTROL Data de Conclusão Planejada do Projeto] <br><strong>[!UICONTROL Tomar Decisão de Aprovação]</strong> botão<br>*Número total de aprovações de projeto pendentes <br>*Link para <strong>&rbrace;[!UICONTROL Aprovações de Projeto]</strong><br>*<strong>[!UICONTROL Ver Todas as Aprovações]</strong> botão<br>*Data do resumo diário</p> </td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Preciso aprovar uma tarefa</strong> </p> <p>No caso de aprovações de funções de trabalho, os usuários que recebem uma notificação por email para esse evento dependerão se a configuração '[!UICONTROL Approver not required to be on the project team (for approval processes that include a role)]' está habilitada (conforme descrito em <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">Definir configurações de aprovação global</a>). </p> <p><strong>Se esta opção estiver habilitada</strong>, uma notificação por email será enviada a todos os usuários do sistema com a função de trabalho associada à aprovação. </p> <p><strong>Se esta opção estiver desabilitada</strong>, somente membros da equipe do projeto com a função de trabalho associada ao processo de aprovação receberão uma notificação por email.</p> <p>Se a aprovação estiver associada a um usuário, ele receberá a notificação. </p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Tarefa Pendente de Aprovação]: &lt;Nome da Tarefa&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> <p>Nome da Tarefa<br>Nome do Projeto<br>Nome do usuário que enviou a aprovação<br>Status de Aprovação Pendente<br>Data e Hora da Aprovação Solicitada<br>Prioridade da Tarefa<br>Nome do Estágio de Aprovação<br>Nomes dos Aprovadores<br>[!UICONTROL Data de Conclusão Planejada da Tarefa]<br><strong>[!UICONTROL Tomar Decisão de Aprovação]</strong> botão<br>*Número total de aprovações de tarefas pendentes<br>*Link para<strong>[!UICONTROL Aprovações de Tarefas *Ver Todas as Aprovações]</strong> botão<strong></strong>*Data do resumo diário<br></p> </td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Preciso aprovar uma planilha de horas</strong> </p> <p>O Aprovador de Planilha de Horas recebe uma notificação por e-mail quando uma planilha de horas que ele precisa aprovar é enviada, a menos que o usuário que enviou a planilha de horas também seja o Aprovador de Planilha de Horas.</p> <p>Uma notificação só será enviada se o status da folha de horas for [!UICONTROL Enviado].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Planilha de Horas Enviada]: &lt;Proprietário da Planilha de Horas&gt;, &lt;Data de Início da Planilha de Horas&gt; - &lt;Data de Término da Planilha de Horas&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do usuário que enviou a folha de horas para aprovação<br>Data e Hora de envio da folha de horas<br>Status da folha de horas<br>Datas de Início e Término da Folha de Horas<br>Número de horas registradas na folha de horas<br>Número de horas extras registradas na folha de horas<br><strong>[!UICONTROL Revisão]</strong> e <strong>[!UICONTROL Aprovar]</strong> botões<br>*O número total de aprovações pendentes na folha de horas<br>*Link para <strong> 1&rbrace;[!UICONTROL Aprovações de Planilha de Horas]</strong><br><strong>[!UICONTROL *Ver Todas as Aprovações]</strong> botão<br>*Data do resumo diário </td> 
   <td><strong>Instantâneo e</strong> <strong>Diário</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Preciso aprovar um problema</strong> </p> <p>No caso de aprovações de funções de trabalho, os usuários que recebem uma notificação por email para esse evento dependerão se a configuração '[!UICONTROL Aprovador não precisa estar na equipe do projeto (para processos de aprovação que incluem uma função)]' está habilitada (conforme descrito em <a href="../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref">[!UICONTROL Configurar aprovação global] configurações</a>). </p> <p><strong>Se esta opção estiver habilitada</strong>, uma notificação por email será enviada a todos os usuários do sistema com a função de trabalho associada à aprovação. </p> <p><strong>Se esta opção estiver desabilitada</strong>, somente membros da equipe do projeto com a função de trabalho associada ao processo de aprovação receberão uma notificação por email.</p> <p>Se a aprovação estiver associada a um usuário, ele receberá a notificação. </p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Problema Pendente de Aprovação]: &lt;Nome do Problema&gt;</em></p> <p> O assunto da notificação de resumo diário é: <em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt; </em></p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que enviou o problema para aprovação<br>Status de Aprovação Pendente<br>Data e Hora da Aprovação Solicitada<br>Prioridade do Problema<br>Estágio de Aprovação<br>Nomes dos Aprovadores<br>[!UICONTROL Data de Conclusão Planejada do Problema]<br>[!UICONTROL Contato Principal]<br><strong>[!UICONTROL Tomar Decisão de Aprovação]</strong> botão<br>*O número total de aprovações de problemas pendentes<br> Link para <strong>[!UICONTROL Aprovações de Problemas]</strong><br><strong>[!UICONTROL *Ver Todas as Aprovações]</strong> botão<br>*Data do resumo diário </td> 
   <td><strong>Instantâneo e</strong> <strong>Diário</strong></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Preciso revisar um projeto, cuja aprovação foi delegada</strong> </p> <p>Uma aprovação de projeto foi delegada a você e você precisa revisá-la.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Aprovação de Projeto Delegada - Favor Revisar] &lt;Nome do Projeto&gt;</em></p> <p><em>O assunto da notificação de resumo diário é: [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em> </p> </td> 
   <td> Nome do Projeto<br>Nome do Portfolio<br>Número de Referência do Projeto<br>Nome do usuário que solicitou a aprovação<br>Nome do usuário em cujo nome você está aprovando o Projeto<br>Status de Aprovação Pendente<br>Data e Hora da Aprovação Solicitada<br>Prioridade do Projeto<br>Etapa de Aprovação<br>Nomes dos Aprovadores<br>[!UICONTROL Data de Conclusão Planejada do Projeto]<br><strong>[!UICONTROL Tomar Decisão de Aprovação]</strong> botão<br>*Número total de aprovações de projetos pendentes<br>*Link para 14&rbrace;[!UICONTROL Aprovações de Projetos *Ver Todas as Aprovações]</strong> botão <br>*Data do resumo diário<strong> </td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Preciso revisar uma tarefa, cuja aprovação foi delegada</strong> </p> <p>Uma aprovação de tarefa foi delegada a você e você precisa revisá-la.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Aprovação de Tarefa Delegada - Favor Revisar &#x200B;]&lt;Nome da Tarefa&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Nome do usuário que solicitou a aprovação<br>Nome do usuário em cujo nome você está aprovando a Tarefa<br>Status de Aprovação Pendente<br>Data e Hora da Aprovação Solicitada<br>Prioridade da Tarefa<br>Estágio da Aprovação<br>Nomes de Aprovadores<br>[!UICONTROL Data de Conclusão Planejada da Tarefa]<br><strong>[!UICONTROL Tomar Decisão de Aprovação]</strong> botão <br>*Número total de aprovações de tarefas pendentes<br>*Link para <strong>4&rbrace;[!UICONTROL Aprovações de Tarefas *Ver Todas as Aprovações]</strong> botão<br>*Data do resumo diário </td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Preciso revisar um problema, cuja aprovação foi delegada a mim</strong> </p> <p>Uma aprovação de problema foi delegada a você e você precisa revisá-la.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Aprovação de Problema Delegada - Favor Revisar] &lt;Nome do Problema&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome do Problema<br>Nome do Projeto<br>Número de Referência do Problema<br>Nome do usuário que solicitou a aprovação<br>Nome do usuário em cujo nome você está aprovando o Problema<br>Status de Aprovação Pendente<br>Data e Hora da Aprovação Solicitada<br>Prioridade do Problema<br>Estágio de Aprovação<br>Nomes dos Aprovadores<br>Data de Conclusão Planejada do Problema<br>Contato Principal<br><strong>[!UICONTROL Tomar Decisão de Aprovação]</strong> botão<br>*Número total de aprovações de problemas pendentes<br> Link para <strong>[!UICONTROL Aprovações de Problemas]</strong><br><strong>[!UICONTROL *Ver Todas as Aprovações]</strong> botão<br>*Data do resumo diário<br></td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estou atribuído a um problema</strong> </p> <p>O destinatário do problema recebe uma notificação por email. O destinatário do problema não receberá um email se o status do problema for ou igual a [!UICONTROL Fechado].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Nova Solicitação de Trabalho]: &lt;Nome da Questão&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome do Problema<br>Nome do Projeto<br>[!UICONTROL Número de Referência do Problema]<br>Seu Nome<br>Data de Conclusão do Problema ([!UICONTROL Data de Conclusão Planejada])<br>Nome do usuário que atribuiu o problema a você<br><strong>[!UICONTROL Trabalhar Nele]</strong> botão<br>*Número total de atribuições<br>*Número total de tarefas e problemas atribuídos a você<br>*Link para <strong>[!UICONTROL Solicitações de Trabalho]</strong><br>*Data do resumo diário<br></p> </td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estou definido como o destinatário primário de uma tarefa</strong> </p> <p>O Destinatário da tarefa receberá uma notificação por e-mail se for o principal destinatário da tarefa, a menos que o destinatário seja o usuário que fez a atribuição.</p> <p>Uma notificação será enviada se o status do projeto for [!UICONTROL Atual] e a tarefa não estiver marcada como [!UICONTROL Concluído].</p> <p>Os usuários com uma licença de [!UICONTROL Review] ou [!UICONTROL Requestor] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Nova Solicitação de Trabalho]: &lt;Nome da Tarefa&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> Nome da Tarefa<br>Nome do Projeto<br>Número de Referência da Tarefa<br>Seu Nome<br>Data de Conclusão da Tarefa ([!UICONTROL Data de Conclusão Planejada])<br>Nome do usuário que atribuiu a tarefa a você<br><strong>[!UICONTROL Trabalhar Nela]</strong> botão<br>*Número total de tarefas e problemas atribuídos a você<br>*Link para <strong>[!UICONTROL Solicitações de Trabalho]</strong>*Data do resumo diário </td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Minha equipe recebe uma nova solicitação de trabalho</strong> </p> <p>Os membros da equipe recebem uma notificação por e-mail quando a equipe recebe uma nova solicitação de trabalho. (O usuário que enviou a solicitação não recebe uma notificação se for membro da equipe.)</p> <p>Uma notificação só será enviada se o status do projeto for [!UICONTROL Atual] e o status da Solicitação de Trabalho for [!UICONTROL Novo].</p> <p>Os usuários com uma licença de [!UICONTROL Review] não recebem uma notificação.</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Nova Solicitação de Trabalho]: &lt;Nome da Solicitação&gt;</em></p> <p>O assunto da notificação de resumo diário é: <em>[!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p> Nome do Problema<br>Nome do Projeto (Nome da Fila de Solicitações)<br>Número de Referência do Problema<br>Nome da Equipe<br>Data de Conclusão do Problema (Data de Conclusão Planejada)<br>Nome do usuário que enviou a Solicitação<br><strong>[!UICONTROL Trabalhar Nela]</strong> botão<br>*Número total de solicitações atribuídas à sua equipe</p> <p>*Nome da solicitação de trabalho</p> <p>[!UICONTROL *Data de Término Planejada]</p> <p>*Nome do usuário que enviou a solicitação<br>*Link para <strong>[!UICONTROL Solicitações de Equipe]</strong><br>*Data do resumo diário </p> <p><span class="preview">*Atribuições de equipe</span> </p> </td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Minha Planilha de Horas foi reaberta</strong> </p> <p>O Proprietário da folha de horas recebe uma notificação por email quando a folha de horas é reaberta, a menos que o usuário que a reabriu também seja o proprietário da folha de horas.</p> <p>Uma notificação por email será enviada somente se o status da folha de horas for [!UICONTROL Abrir].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Planilha de Horas Reaberta]: &lt;Data de Início da Planilha de Horas&gt; - &lt;Data de Término da Planilha de Horas&gt;</em></p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </td> 
   <td> Nome do usuário que reabriu a Planilha de Horas<br>Data e Hora em que a Planilha de Horas foi reaberta<br>Status da Planilha de Horas ([!UICONTROL Reaberto])<br>Número Total de Horas registradas na Planilha de Horas<br>Número de Horas Extras registradas na Planilha de Horas<br><strong>[!UICONTROL Review]</strong> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Minha planilha de horas foi rejeitada</strong> </p> <p>O Proprietário da folha de horas recebe uma notificação por email quando a folha de horas é rejeitada, a menos que o usuário que a rejeitou também seja o proprietário.</p> <p>Uma notificação por email será enviada somente se o status da folha de horas for [!UICONTROL Rejeitado].</p> <p>O assunto do email de notificação instantânea é: <em>[!UICONTROL Planilha de Horas Rejeitada]:&lt;Data de Início da Planilha de Horas&gt; - &lt;Data de Término da Planilha de Horas&gt;</em></p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </td> 
   <td> Nome do usuário que rejeitou a Folha de Horas<br>Status da Folha de Horas ([!UICONTROL Rejeitado])<br>Data e Hora em que a Folha de Horas foi rejeitada<br><strong>[!UICONTROL Revisão]</strong> botão </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém está solicitando acesso a mim</strong> </p> <p>Pedindo para eu fazer algo, então ligue-o.</p> <p>A pessoa que cria o projeto tem acesso a ele.</p> <p>É isso que faz com que o usuário receba a notificação quando alguém solicita acesso.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome do usuário que solicitou o acesso&gt; [!UICONTROL precisa acessar] &lt;Nome do Objeto&gt;</em></p> <p>O assunto da notificação de resumo diário é:<em> [!UICONTROL Resumo da Ação Necessária] &lt;Data do resumo diário&gt;</em></p> </td> 
   <td> <p>Nome do Objeto<br>Nome do Objeto Pai<br>Número de Referência do Objeto<br>Nome do usuário que solicitou o acesso<br>Tipo de acesso que o usuário está solicitando<br><strong>[!UICONTROL Conceder] &lt;Nome do acesso solicitado&gt; Acesso</strong> e <strong>[!UICONTROL Conceder acesso diferente]</strong> botões<br>*Número total de aprovações de solicitações de acesso pendentes<br>*Link para <strong>[!UICONTROL Solicitação de Acesso]</strong> Aprovações<br>*Data do resumo diário</p> </td> 
   <td><strong>Instantâneo e Diário</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Alguém solicitou que eu carregue um documento</strong> </p> <p>O Solicitante de documentos recebe uma notificação por email quando um usuário recebe uma solicitação para carregar um documento.</p> <p>O assunto do email de notificação instantânea é: <em>&lt;Nome do usuário que solicita o documento&gt; [!UICONTROL precisa de um documento seu em [!DNL Workfront].]</em></p> <p> <p>Observação: não é possível configurar essa notificação para um email de resumo diário.</p> </p> </td> 
   <td> Nome do usuário que solicita o documento<br>Nome do objeto no qual o documento deve ser carregado<br><strong>[!UICONTROL Anexar aqui]</strong> link </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
