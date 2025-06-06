---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Níveis de permissões para  [!DNL Workfront]  para Outlook
description: O suplemento  [!DNL Workfront for Outlook]  requer acesso de leitura/gravação à caixa de correio. A integração  [!DNL Workfront for Outlook]  requer as permissões de nível mais alto porque tem a funcionalidade de baixar anexos de email do servidor do Outlook Exchange e carregá-los em  [!DNL Workfront], quando o usuário envia uma Solicitação de um email que contém anexos.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 704da044-21ed-4ca1-be6f-0e0aa832e069
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Níveis de permissão para [!DNL Workfront for Outlook]

>[!IMPORTANT]
>
>[O Microsoft está desabilitando o suporte para tokens herdados do Exchange online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que são usados atualmente pelo suplemento do Workfront Outlook para autenticação. Essa alteração pela Microsoft já começou a afetar os clientes e continuará a ser implementada em fases até outubro de 2025.
>
>* **Depois que o Microsoft desabilitar totalmente esses tokens, a integração do Workfront para Microsoft Outlook não funcionará mais.**
>
>Como parte dessa alteração, a Microsoft tomou a decisão de alterar a maneira como os tokens são reativados. Após **30 de junho de 2025**, os administradores não poderão mais reabilitar tokens, somente o Suporte da Microsoft poderá conceder exceções. **Em 1º de outubro de 2025, os tokens herdados serão desativados para todos os locatários. Exceções não serão concedidas.**


[!DNL Workfront for Outlook] requer o mais alto dos quatro níveis de permissões permitidos nos suplementos [!DNL Outlook].

Para obter detalhes sobre permissões em suplementos do [!DNL Outlook], consulte [Privacidade, permissões e segurança para [!DNL Outlook] suplementos](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) na documentação do [!DNL Microsoft].

O suplemento [!DNL Workfront for Outlook] requer acesso de leitura/gravação à caixa de correio (`ReadWriteMailbox`), que é o escopo de permissão mais alto.
A integração do [!DNL Workfront for Outlook] requer as permissões de nível mais alto porque tem a funcionalidade de baixar anexos de email do servidor do Exchange [!DNL Outlook] e carregá-los no [!DNL Workfront], quando o usuário envia uma Solicitação de um email que contém anexos. Para que essa funcionalidade funcione, [!DNL Workfront for Outlook] usa a função `mailbox.getCallbackTokenAsync()` da API do JavaScript de Suplemento [!DNL Office] para obter o Token e usá-lo para baixar anexos de email do servidor Exchange. A única permissão que permite o uso dessa função é `ReadWriteMailbox`. Para obter mais informações, consulte [Privacidade, permissões e segurança para suplementos do Outlook](https://docs.microsoft.com/en-us/office/dev/add-ins/outlook/privacy-and-security) na documentação do Microsoft.

O suplemento [!DNL Workfront for Outlook] também requer permissão `ReadWriteItem` (incluída em `ReadWriteMailbox`), que é usada para ler o corpo do email e ler/atualizar metadados de email:

* Ler corpo do email:

  [!DNL Workfront for Outlook] lê o corpo do email quando um usuário envia a solicitação ou envia o corpo do email como uma atualização para o objeto [!DNL Adobe Workfront].
* Ler/atualizar metadados de email:

  [!DNL Workfront for Outlook] atualiza cabeçalhos de email quando um usuário envia uma solicitação de um email. Isso é feito para armazenar informações sobre o objeto [!DNL Adobe Workfront] enviado, para que na próxima vez que o usuário abrir o suplemento para o mesmo email, as informações sobre ações anteriores com esse email sejam exibidas.

[!DNL Workfront for Outlook] acessa a Caixa de Correio de um usuário somente quando o usuário executa uma ação dentro do complemento. Ela não tem nenhuma funcionalidade em segundo plano. O Workfront para Outlook acessa a caixa de correio do usuário somente no seguinte cenário:

* O usuário tenta enviar uma solicitação, criar uma tarefa ou enviar um email como uma atualização de [!DNL Workfront for Outlook] (Abrindo o suplemento e selecionando uma ação)
   * [!DNL Workfront for Outlook] lê o corpo do email a ser preenchido no formulário dentro do suplemento.
   * [!DNL Workfront for Outlook] lê metadados de email para exibir informações sobre o suplemento sobre as ações anteriores realizadas no suplemento com o mesmo email.
* Quando um usuário envia uma solicitação, cria uma tarefa ou envia um email como uma atualização de [!DNL Workfront for Outlook] (clicando no botão [!UICONTROL enviar] no suplemento):
   * [!DNL Workfront for Outlook] lê o corpo do email para enviá-lo à Workfront como uma descrição de solicitação ou um comentário.
   * [!DNL Workfront for Outlook] atualiza os metadados de email para armazenar informações sobre as solicitações enviadas ou o objeto atualizado.
   * [!DNL Workfront for Outlook] baixa anexos de email do servidor exchange para carregar em solicitações enviadas, tarefas criadas ou objetos atualizados.
