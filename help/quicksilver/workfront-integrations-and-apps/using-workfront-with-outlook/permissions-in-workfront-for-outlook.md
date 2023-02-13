---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Níveis de permissões para [!DNL Workfront] para Outlook
description: O [!DNL Workfront for Outlook] o complemento requer acesso de leitura/gravação à caixa de correio. O [!DNL Workfront for Outlook] a integração exige as permissões de mais alto nível, pois tem a funcionalidade de baixar anexos de email do servidor do Outlook Exchange e carregá-los no [!DNL Workfront], quando o usuário envia uma Solicitação de um email com anexos.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: 177bf9271dca0310653b73b9100607a82290c326
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Níveis de permissões para [!DNL Workfront for Outlook]

[!DNL Workfront for Outlook] O exige o mais alto dos quatro níveis de permissões permitidos em [!DNL Outlook] suplementos.

Para obter detalhes sobre permissões em [!DNL Outlook] suplementos, consulte [Privacidade, permissões e segurança para [!DNL Outlook] suplementos](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) no [!DNL Microsoft] documentação.

O [!DNL Workfront for Outlook] o suplemento requer acesso de leitura/gravação à caixa de correio (`ReadWriteMailbox`), que é o escopo de permissão mais alto.
O [!DNL Workfront for Outlook] a integração exige permissões de nível mais alto, pois tem a funcionalidade de baixar anexos de email do [!DNL Outlook] servidor do exchange e faça o upload para [!DNL Workfront], quando o usuário envia uma Solicitação de um email com anexos. Para que essa funcionalidade funcione, [!DNL Workfront for Outlook] usa a função `mailbox.getCallbackTokenAsync()` from [!DNL Office] API JavaScript do complemento para obter o token e usá-lo para baixar anexos de email do servidor do exchange. A única permissão que permite o uso dessa função é `ReadWriteMailbox`. Para obter mais informações, consulte [Privacidade, permissões e segurança para suplementos do Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) na documentação do Microsoft.

O [!DNL Workfront for Outlook] o suplemento também requer `ReadWriteItem` permissão (incluída em `ReadWriteMailbox`), que é usado para ler o corpo do email e ler/atualizar metadados de email:

* Ler corpo do email:

   [!DNL Workfront for Outlook] lê o corpo do email quando um usuário envia a solicitação ou envia o corpo do email como uma atualização para [!DNL Adobe Workfront] Objeto.
* Ler/atualizar metadados de email:

   [!DNL Workfront for Outlook] atualiza cabeçalhos de email quando um usuário envia uma solicitação de um email. Isso é feito para armazenar informações sobre o enviado [!DNL Adobe Workfront] para que na próxima vez que o usuário abrir o suplemento para o mesmo email, as informações sobre ações anteriores com esse email serão exibidas.

[!DNL Workfront for Outlook] O acessa a Caixa de entrada de um usuário somente quando ele executa uma ação dentro do complemento . Ele não tem nenhuma funcionalidade em segundo plano. O Workfront for Outlook acessa a caixa de entrada do usuário somente no seguinte cenário:

* O usuário tenta enviar uma solicitação, criar uma tarefa ou enviar um email como atualização de [!DNL Workfront for Outlook] (Abrir o suplemento e selecionar uma ação)
   * [!DNL Workfront for Outlook] O lê o corpo do email a ser preenchido no formulário dentro do suplemento.
   * [!DNL Workfront for Outlook] O lê metadados de email para exibir informações no suplemento sobre as ações anteriores realizadas no suplemento com o mesmo email.
* Quando um usuário envia uma solicitação, cria uma tarefa ou envia um email como atualização de [!DNL Workfront for Outlook] (clicando no botão [!UICONTROL submit] no suplemento):
   * [!DNL Workfront for Outlook] O lê o corpo do email para enviá-lo ao Workfront como uma descrição de solicitação ou um comentário.
   * [!DNL Workfront for Outlook] atualiza os metadados de email para armazenar informações sobre as solicitações enviadas ou o objeto atualizado.
   * [!DNL Workfront for Outlook] baixa anexos de email do servidor do exchange para fazer upload de solicitações enviadas, tarefas criadas ou objetos atualizados.
