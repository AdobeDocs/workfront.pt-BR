---
product-area: workfront-integrations
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Privacidade e permissões no Workfront para G Suite
description: Privacidade e permissões no Workfront para G Suite
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 0862af846ca77c33132ec631cf1e3eae253d3cd8
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Privacidade e permissões no Workfront para G Suite

Como a privacidade do cliente é importante, a Adobe Workfront não armazena nem coleta dados de identificação do cliente que resultem da autorização de terceiros de um aplicativo de plug-in do Google.

Precisamos das seguintes permissões para que o plug-in Workfront for G Suite possa fornecer seu valor máximo:

* **Exibir suas mensagens de email quando o complemento estiver em execução**: O plug-in Workfront for G Suite pode salvar inúmeras horas de trabalho duplicado para usuários, convertendo emails em novas tarefas no Workfront e preenchendo automaticamente o título e a descrição da tarefa com o assunto e o corpo do email. O plug-in também permite publicar seus emails no Workfront como novos comentários. O plug-in precisa exibir suas mensagens de email quando o complemento estiver em execução para fornecer esse valor.
* **Executar como um complemento Gmail / não sensível**: As permissões são necessárias para que o complemento Workfront for G Suite funcione no ambiente Gmail. O plug-in requer um ambiente Gmail para funcionar, portanto, requer o `Run as a Gmail add-on / non-sensitive` permissão.
* **Exibir os metadados da mensagem de email quando o complemento estiver em execução**: Para melhorar os fluxos de trabalho, o plug-in do Workfront for G Suite confirma se um email é uma notificação do Workfront e identifica o tipo de notificação do Workfront (nova solicitação de trabalho, solicitação de aprovação, novo comentário etc.). O plug-in exige que o `View your email message metadata when the add-on is running` permissão para fornecer esse valor.
* **O plug-in precisa ser executado como um complemento de calendário/não sensível**: O plug-in Workfront for G Suite se conecta ao seu calendário, para que você possa visualizar como as tarefas afetam os agendamentos. O plug-in precisa da função `Run as a Calendar add-on / non-sensitive` permissão para fazer isso.
* **Conexão com uma permissão de serviço externo:** Em última análise, o plug-in precisa se conectar à API do Workfront, que é a espinha dorsal do valor do plug-in. A API do Workfront é um serviço externo ao Google, portanto, o plug-in requer o `Connect to an external service permission` para fazer o plug-in funcionar.

Para obter mais informações sobre a dedicação da Adobe Workfront à privacidade do cliente, consulte [Aviso de privacidade da Workfront](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

