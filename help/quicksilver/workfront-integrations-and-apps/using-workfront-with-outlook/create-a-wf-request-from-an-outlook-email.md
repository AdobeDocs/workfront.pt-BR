---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Criar uma solicitação [!DNL Adobe Workfront] de um email do Outlook
description: Você pode criar uma solicitação  [!DNL Adobe Workfront]  de um email no Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Criar uma solicitação [!DNL Adobe Workfront] de um email do [!UICONTROL Outlook]

>[!IMPORTANT]
>
>[O Microsoft está desabilitando o suporte para tokens herdados do Exchange online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que são usados atualmente pelo suplemento do Workfront Outlook para autenticação. Essa alteração pela Microsoft já começou a afetar os clientes e continuará a ser implementada em fases até outubro de 2025.
>
>* **Depois que o Microsoft desabilitar totalmente esses tokens, a integração do Workfront para Microsoft Outlook não funcionará mais.**
>
>Como parte dessa alteração, a Microsoft tomou a decisão de alterar a maneira como os tokens são reativados. Após **30 de junho de 2025**, os administradores não poderão mais reabilitar tokens, somente o Suporte da Microsoft poderá conceder exceções. **Em 1º de outubro de 2025, os tokens herdados serão desativados para todos os locatários. Exceções não serão concedidas.**


Você pode criar uma solicitação [!DNL Adobe Workfront] de um email no Outlook.

Ao criar uma solicitação [!DNL Workfront] com base em um email, o conteúdo do email (incluindo o assunto e o corpo) é incluído na solicitação por padrão.

>[!NOTE]
>
>Não é possível criar uma solicitação [!DNL Workfront] de uma caixa de correio [!UICONTROL Outlook] compartilhada.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

O administrador do [!DNL Workfront] deve habilitar [!DNL Outlook for Office] com [!DNL Workfront] antes que você possa usar essa integração.

## Criar uma solicitação de um email do [!DNL Outlook]

Para criar uma Solicitação [!DNL Workfront] de [!DNL Outlook]:

1. Selecione o email que contém as informações que você deseja incluir em uma solicitação [!DNL Workfront].
1. Clique no ícone **[!DNL Workfront]** no canto superior direito da mensagem de email para exibir o suplemento do Workfront.\
   Talvez seja necessário clicar na seta para baixo na parte superior direita do email para acessar o ícone [!DNL Workfront].

1. Clique no ícone **[!UICONTROL Menu]** ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png) para exibir a lista de opções [!DNL Workfront] disponíveis.

1. Clique em **[!UICONTROL Enviar solicitação]**.
1. No campo **[!UICONTROL Selecionar um Tipo de Solicitação]**, selecione a fila de solicitações na qual deseja enviar a solicitação.

1. Especifique as seguintes informações:\
   Dependendo de como a fila de solicitações foi configurada, os campos disponíveis podem variar. Para obter uma lista completa e uma descrição de possíveis campos, consulte o artigo [Criar e enviar [!DNL Adobe Workfront] solicitações](../../manage-work/requests/create-requests/create-submit-requests.md).

   * **[!UICONTROL Assunto]:** Especifique um assunto para a solicitação. Por padrão, o assunto do email é usado.
   * **[!UICONTROL Descrição]:** Especifique uma descrição para a solicitação. Por padrão, o corpo do email é usado.
   * **[!UICONTROL Documentos]:** Anexe quaisquer documentos que você deseja incluir na solicitação. Você pode anexar documentos arrastando e soltando-os ou clicando em **[!UICONTROL Selecionar arquivo]** e navegando até o documento e selecionando-o.\

     Por padrão, todos os documentos anexados ao email são incluídos na solicitação.

1. Clique em **[!UICONTROL Enviar solicitação]**.\
   A solicitação foi enviada para [!DNL Workfront], na fila de solicitações especificada.

1. (Opcional) Volte para [!DNL Outlook] e selecione o email original.\
   Na parte superior do painel de suplementos do [!DNL Workfront], observe a confirmação com um link de que o email foi adicionado ao Workfront como uma solicitação. O link inclui a data em que foi convertido.\
