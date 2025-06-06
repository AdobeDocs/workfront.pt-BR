---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configurar [!DNL Adobe Workfront] para [!DNL Outlook]
description: O suplemento  [!DNL Adobe Workfront] [!DNL Outlook] permite executar as tarefas principais [!DNL Workfront]  diretamente do Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>[O Microsoft está desabilitando o suporte para tokens herdados do Exchange online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que são usados atualmente pelo suplemento do Workfront Outlook para autenticação. Essa alteração pela Microsoft já começou a afetar os clientes e continuará a ser implementada em fases até outubro de 2025.
>
>* **Depois que o Microsoft desabilitar totalmente esses tokens, a integração do Workfront para Microsoft Outlook não funcionará mais.**
>
>Como parte dessa alteração, a Microsoft tomou a decisão de alterar a maneira como os tokens são reativados. Após **30 de junho de 2025**, os administradores não poderão mais reabilitar tokens, somente o Suporte da Microsoft poderá conceder exceções. **Em 1º de outubro de 2025, os tokens herdados serão desativados para todos os locatários. Exceções não serão concedidas.**


O suplemento [!DNL Adobe Workfront] [!DNL Outlook] permite executar as seguintes tarefas [!DNL Workfront] principais diretamente do Outlook:

* Atualize um projeto, tarefa ou problema existente com informações de um email. Para obter mais informações, consulte [Atualizar um objeto existente a partir de um [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Crie uma solicitação [!DNL Workfront] com base em um email no [!DNL Outlook]. Para obter mais informações, consulte [Criar uma solicitação Adobe Workfront a partir de um [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Adicione um email como uma tarefa na área [!UICONTROL Meu Trabalho]. Para obter mais informações, consulte [Adicionar um [!DNL Outlook] email como uma tarefa à sua lista de trabalho](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Responder comentários por meio do suplemento [!DNL Workfront] para [!DNL Outlook]. Para obter informações sobre como responder a comentários do Workfront para [!DNL Outlook], consulte [Responder a um comentário de [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Crie tarefas e problemas do zero ou crie-os a partir de emails existentes (usando a funcionalidade arrastar e soltar). Para obter mais informações, consulte [Adicionar um [!DNL Outlook] email a um projeto como uma tarefa ou um problema](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Você deve adicionar o suplemento [!DNL Workfront] à sua conta [!DNL Outlook] antes de poder usar [!DNL Workfront for Outlook].

Se você não conseguir instalar o suplemento [!DNL Workfront] com sua conta [!DNL Outlook], contate o administrador do [!DNL Workfront] para garantir que os suplementos do [!DNL Outlook] estejam habilitados para sua organização.

Para obter informações sobre como habilitar a integração do [!DNL Outlook] para sua organização, consulte [Habilitar [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> 
   <p>Novo plano: [!UICONTROL Padrão]</p> 
   <p>Plano atual:[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

O administrador do [!DNL Workfront] deve habilitar [!DNL Outlook for Office] com [!DNL Workfront] antes que você possa usar essa integração.

## Requisitos do sistema

Os seguintes aplicativos estão disponíveis:

* **[!DNL Outlook]na Web:** O suplemento [!DNL Workfront] está disponível ao usar [!DNL Outlook] de um navegador da Web em um computador ou dispositivo móvel. Essa funcionalidade também está disponível ao usar o Aplicativo Web [!DNL Outlook].
* Aplicativo de Área de Trabalho **[!DNL Outlook]:** O suplemento [!DNL Workfront] está disponível ao usar as versões de área de trabalho [!DNL Windows] e [!DNL Mac] de [!DNL Outlook] incluídas no pacote [!DNL Office].

O suplemento [!DNL Workfront] para [!DNL Outlook] tem suporte em ambientes que atendem aos seguintes requisitos:

* [Requisitos do cliente](#client-requirements-client-requirements)
* [Requisitos do servidor de email](#mail-server-requirements-mail-server-requirements)

### Requisitos do cliente {#client-requirements}

O Workfront oferece suporte às seguintes versões do [!DNL Outlook]:

* [!DNL Outlook 2013] ou posterior em [!DNL Windows]
* [!DNL Outlook 2016] ou posterior em [!DNL Windows]
* [!DNL Outlook] em [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] em [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] na Web

Você deve estar conectado a um [!DNL Exchange Server] ou [!DNL Office 365] usando uma conexão direta.

Ao configurar o cliente, o usuário deverá selecionar um dos seguintes tipos de conta:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com] Se o cliente estiver configurado para se conectar com POP3 ou IMAP, o suplemento [!DNL Workfront] não será carregado.

### Requisitos do servidor de email {#mail-server-requirements}

Os requisitos do servidor de email são atendidos por padrão quando você se conecta ao [!DNL Office 365] ou ao [!DNL Outlook.com]. No entanto, se você estiver conectado a uma instalação local do [!DNL Exchange Server], os seguintes requisitos se aplicam:

* A Workfront oferece suporte a todos os [!DNL Exchange On-Premise] servidores
* [!DNL Exchange Web Services] (EWS) deve ser habilitado e deve ser exposto à Internet.
* O servidor deve ter um certificado de autenticação válido para emitir tokens de identidade válidos. As novas instalações do [!DNL Exchange Server] incluem um certificado de autenticação padrão.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Para acessar o suplemento [!DNL Workfront] da [[!DNL Office] Loja](https://store.office.com/), os servidores de acesso para cliente devem ser capazes de se comunicar com [https://store.office.com](https://store.office.com/).

Para obter informações mais detalhadas sobre os ambientes compatíveis, consulte a [[!DNL Microsoft Office 365] home page](https://products.office.com/en-us/office-365-home).

## Instalar o suplemento

Você pode obter o suplemento Workfront para Outlook na [Microsoft store](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] para [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Em [!DNL Outlook 365], clique no ícone **[!UICONTROL Procurar Suplementos]** ![Procurar Suplementos](assets/outlook-add-in-26x26.png)na parte superior da interface do Office 365 e clique em **[!UICONTROL Gerenciar suplementos]**.

1. Na caixa **[!UICONTROL Pesquisar suplementos]**, procure **[!DNL Workfront]** e pressione [!UICONTROL Enter].

1. Clique em **[!UICONTROL Adicionar]**.

### [!DNL Workfront] para [!DNL Outlook] na Web {#workfront-for-outlook-on-the-web}

1. Abra [!DNL Microsoft Outlook] em um navegador da Web.
1. Clique no ícone **[!UICONTROL Procurar] suplementos** ![Procurar suplementos](assets/outlook-add-in-web-version-20x20.png).

   Para localizar o ícone, consulte [Uso de suplementos [!DNL Outlook] na Web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) na documentação do Microsoft.

1. Pesquise por **[!DNL Workfront]** no campo **[!UICONTROL Pesquisar suplementos]** e pressione **[!UICONTROL Enter]**.

1. Quando ele aparecer na lista, clique em **Adicionar**.

### [!DNL Workfront for Outlook] no [!UICONTROL Windows] ou [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Clique em **[!UICONTROL Página Inicial]** > **[!UICONTROL Loja]** na faixa de opções.

1. Pesquise por **[!DNL Workfront]** no campo **[!UICONTROL Pesquisa]** e pressione **[!UICONTROL Enter]**.

1. Clique no botão de alternância para habilitar o suplemento **[!UICONTROL [!DNL Workfront]]**.

## Fazer logon em [!DNL Workfront] a partir de [!DNL Outlook]

1. Em [!DNL Outlook], selecione uma mensagem de email e clique no ícone **[!DNL Workfront]** no cabeçalho do email.
1. Na página de logon, clique em **Fazer logon no Workfront**.
1. Siga as instruções para fazer logon em [!DNL Workfront] usando OAuth 2.0. <!--Enhanced Authentication or your Security Assertion Markup Language (SAML) URL.-->

   <!--Before users can log in to the [!DNL Workfront] add-in using SAML, a [!DNL Workfront] administrator must first enable [!DNL Office 365] add-ins to authenticate using a SAML 2.0 solution. For more information, see the section [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) in the article [Configure [!DNL Adobe Workfront] with SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).-->

   >[!NOTE]
   >
   >* Se for solicitado que você insira o domínio da sua conta do [!DNL Workfront], digite-o usando este formato: *yourCompany&#39;sDomain.my.workfront.com*. O domínio da sua empresa geralmente é o nome da sua empresa.

<!--ADDITIONAL BULLET REMOVED FROM NOTE BOX: Enhanced Authentication is not available until a Workfront administrator enables it for this integration.-->
