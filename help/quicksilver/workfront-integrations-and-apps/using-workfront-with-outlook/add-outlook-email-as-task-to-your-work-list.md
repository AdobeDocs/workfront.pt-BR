---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Adicionar um email do Outlook como uma tarefa à sua lista de trabalho
description: Você pode converter [!DNL Outlook] emails em [!DNL Adobe Workfront] tarefas. Depois que um email é convertido, a tarefa é disponibilizada na Lista de trabalho na área Página inicial.
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# Adicionar um email do [!DNL Outlook] como uma tarefa à sua lista de trabalho

>[!IMPORTANT]
>
>[O Microsoft está desabilitando o suporte para tokens herdados do Exchange online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que são usados atualmente pelo suplemento do Workfront Outlook para autenticação. Essa alteração pela Microsoft já começou a afetar os clientes e continuará a ser implementada em fases até outubro de 2025.
>
>* **Depois que o Microsoft desabilitar totalmente esses tokens, a integração do Workfront para Microsoft Outlook não funcionará mais.**
>
>Como parte dessa alteração, a Microsoft tomou a decisão de alterar a maneira como os tokens são reativados. Após **30 de junho de 2025**, os administradores não poderão mais reabilitar tokens, somente o Suporte da Microsoft poderá conceder exceções. **Em 1º de outubro de 2025, os tokens herdados serão desativados para todos os locatários. Exceções não serão concedidas.**


Você pode converter [!DNL Outlook] emails em [!DNL Adobe Workfront] tarefas. Depois que um email é convertido, a tarefa fica disponível na sua Lista de [!UICONTROL Trabalho] na área [!UICONTROL Página inicial].

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

## Adicionar um email do [!DNL Outlook] como uma tarefa à sua lista de trabalho

1. Selecione o email em [!DNL Outlook] que você deseja converter em uma tarefa.
1. Clique no ícone **[!DNL Workfront]** no canto superior direito do email para exibir o suplemento [!DNL Workfront].\
   Talvez seja necessário clicar na seta para baixo na parte superior direita do email para acessar o ícone [!DNL Workfront].

1. Clique no ícone **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) para exibir a lista de opções [!DNL Workfront] disponíveis.\


1. Clique em **[!UICONTROL Adicionar ao Trabalho]**.\

1. Desmarque o campo **[!UICONTROL Adicionar ao projeto]**.
1. (Opcional) É possível atualizar as seguintes informações do email antes de salvá-lo como uma tarefa:

   * **[!UICONTROL Nome da tarefa]:** por padrão, o nome da tarefa é igual ao Assunto do email. Você pode modificar o nome da tarefa conforme desejado.
   * **[!UICONTROL Descrição]:** Por padrão, a descrição é igual ao Corpo do email. Você pode modificar a descrição conforme desejado.
   * **[!UICONTROL Anexos]:** Todos os anexos de email são salvos na área [!UICONTROL Documentos] da tarefa. É possível excluir quaisquer anexos antes de salvar o email como uma tarefa.

1. Clique em **[!UICONTROL Adicionar]**.\
   A tarefa foi adicionada à [!UICONTROL Lista de Trabalho] na sua Área inicial sem data de confirmação.

1. (Opcional) Clique em **[!UICONTROL Exibir no Workfront]** para exibir a tarefa no aplicativo [!DNL Workfront] em uma nova guia.

1. (Opcional) Volte para [!DNL Outlook] e selecione o email original.\
   Na parte superior do painel de suplementos do [!DNL Workfront], observe a confirmação com um link de que o email foi adicionado ao Workfront como uma tarefa. O link inclui a data em que foi convertido.\
