---
product-area: workfront-integrations
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Privacidade e permissões no Workfront para Google Workspace
description: Privacidade e permissões no Workfront para Google Workspace
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Privacidade e permissões no Workfront para Google Workspace

Como a privacidade do cliente é importante, a Adobe Workfront não armazena nem coleta dados de identificação do cliente que resultem da autorização de terceiros de um aplicativo de plug-in do Google. O uso do Workfront para Google Workspace e a transferência de informações recebidas das APIs do Google para qualquer outro aplicativo seguirão a [Política de dados do usuário dos Serviços de API da Google](https://developers.google.com/terms/api-services-user-data-policy), incluindo os requisitos de uso limitado.

São necessárias as seguintes permissões para que o plug-in Workfront para Google Workspace possa fornecer seu valor máximo:

* **Exibir suas mensagens de email quando o complemento estiver em execução**: o plug-in Workfront para Google Workspace pode salvar inúmeras horas de trabalho duplicado para os usuários, convertendo emails em novas tarefas no Workfront e preenchendo automaticamente o título e a descrição da tarefa com o assunto e o corpo do email. O plug-in também permite publicar seus emails no Workfront como novos comentários. O plug-in precisa exibir suas mensagens de email quando o complemento estiver em execução para fornecer esse valor.
* **Executar como um complemento do Gmail/não confidencial**: são necessárias permissões para que o complemento Workfront for Google Workspace funcione no ambiente do Gmail. O plug-in requer um ambiente do Gmail para funcionar, portanto, ele requer a permissão `Run as a Gmail add-on / non-sensitive`.
* **Exibir os metadados da mensagem de email quando o complemento estiver em execução**: para melhorar os fluxos de trabalho, o plug-in Workfront para Google Workspace confirma se um email é uma notificação do Workfront e identifica o tipo de notificação do Workfront (nova solicitação de trabalho, solicitação de aprovação, novo comentário etc.). O plug-in requer a permissão `View your email message metadata when the add-on is running` para fornecer esse valor.
* **O plug-in precisa ser executado como um complemento do Calendário/não confidencial**: o plug-in Workfront para Google Workspace se conecta ao seu calendário para que você possa visualizar como as tarefas afetam os agendamentos. O plug-in precisa da permissão `Run as a Calendar add-on / non-sensitive` para fazer isso.
* **Permissão de conexão com um serviço externo:** Em última análise, o plug-in precisa se conectar à API do Workfront, que é o backbone do valor do plug-in. A API do Workfront é um serviço externo ao Google, portanto, o plug-in requer o `Connect to an external service permission` para funcionar.

Para obter mais informações sobre a dedicação da Adobe Workfront à privacidade do cliente, consulte o [Aviso de Privacidade da Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

Para obter mais informações, consulte [Política de Dados de Usuário dos Serviços de API da Google](https://developers.google.com/terms/api-services-user-data-policy).
