---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configurar [!DNL Adobe Workfront] para [!DNL Outlook]
description: A variável [!DNL Adobe Workfront] [!DNL Outlook] permite que você execute a chave [!DNL Workfront] tarefas diretamente do Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Outlook]

<!-- Audited: 12/2023 -->

A variável [!DNL Adobe Workfront] [!DNL Outlook] permite que você execute a seguinte ação [!DNL Workfront] tarefas diretamente do Outlook:

* Atualize um projeto, tarefa ou problema existente com informações de um email. Para obter mais informações, consulte [Atualizar um objeto existente a partir de um [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Criar um [!DNL Workfront] solicitação com base em um email no [!DNL Outlook]. Para obter mais informações, consulte [Criar uma solicitação Adobe Workfront de um [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Adicione um email como uma tarefa no seu [!UICONTROL Meu trabalho] área. Para obter mais informações, consulte [Adicionar um [!DNL Outlook] enviar email como uma tarefa para sua lista de trabalho](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Responder a comentários por meio do [!DNL Workfront] suplemento para [!DNL Outlook]. Para obter informações sobre como responder a comentários do Workfront sobre [!DNL Outlook], consulte [Responder a um comentário de [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Crie tarefas e problemas do zero ou crie-os a partir de emails existentes (usando a funcionalidade arrastar e soltar). Para obter mais informações, consulte [Adicionar um [!DNL Outlook] enviar email para um projeto como uma tarefa ou um problema](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

É necessário adicionar o [!DNL Workfront] suplemento ao seu [!DNL Outlook] antes de poder usar [!DNL Workfront for Outlook].

Se não conseguir instalar o [!DNL Workfront] suplemento com o seu [!DNL Outlook] conta, entre em contato com o [!DNL Workfront] administrador assegurar que [!DNL Outlook] os suplementos estão habilitados para sua organização.

Para obter mais informações sobre como ativar o [!DNL Outlook] para sua organização, consulte [Ativar [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Requisitos de acesso

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

## Pré-requisitos

Seu [!DNL Workfront] o administrador precisa habilitar [!DNL Outlook for Office] com [!DNL Workfront] antes de usar essa integração.

## Requisitos do sistema

Os seguintes aplicativos estão disponíveis:

* **[!DNL Outlook]na Web:** A variável [!DNL Workfront] o suplemento está disponível ao usar [!DNL Outlook] de um navegador da web em um desktop ou dispositivo móvel. Essa funcionalidade também está disponível ao usar o [!DNL Outlook] Aplicativo Web.
* **[!DNL Outlook]Aplicativo de desktop:** A variável [!DNL Workfront] o suplemento está disponível ao usar o [!DNL Windows] e [!DNL Mac] versões para desktop do [!DNL Outlook] incluído com o [!DNL Office] pacote.

A variável [!DNL Workfront] suplemento para [!DNL Outlook] O é compatível com ambientes que atendem aos seguintes requisitos:

* [Requisitos do cliente](#client-requirements-client-requirements)
* [Requisitos do servidor de email](#mail-server-requirements-mail-server-requirements)

### Requisitos do cliente {#client-requirements}

O Workfront é compatível com as seguintes versões do [!DNL Outlook]:

* [!DNL Outlook 2013] ou posteriormente [!DNL Windows]
*[!DNL  Outlook 2016] ou posteriormente [!DNL Windows]
* [!DNL Outlook] em [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] em [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] na Web

Você deve estar conectado a um [!DNL Exchange Server] ou [!DNL Office 365] usando uma conexão direta.

Ao configurar o cliente, o usuário deverá selecionar um dos seguintes tipos de conta:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B;Se o cliente estiver configurado para se conectar com POP3 ou IMAP, a variável [!DNL Workfront] o suplemento não carrega.

### Requisitos do servidor de email {#mail-server-requirements}

Os requisitos do servidor de email são atendidos por padrão quando você se conecta ao [!DNL Office 365] ou [!DNL Outlook.com]. No entanto, se você estiver conectado a uma instalação local do [!DNL Exchange Server], são aplicáveis os seguintes requisitos:

* O Workfront oferece suporte a todos [!DNL Exchange On-Premise] servidores
* [!DNL Exchange Web Services] (EWS) deve ser habilitado e deve ser exposto à Internet.
* O servidor deve ter um certificado de autenticação válido para emitir tokens de identidade válidos. Novas instalações de [!DNL Exchange Server] incluir um certificado de autenticação padrão.

  <!--this used to be here but Dev asked for it to be taken out - logged issue for editing this article on 4-26-2023: For more information, see [Digital certificates and encryption in [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) and [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).-->

* Para acessar o [!DNL Workfront] suplemento do [[!DNL Office] Loja](https://store.office.com/), seus servidores de acesso para cliente devem poder se comunicar com  [https://store.office.com](https://store.office.com/).

Para obter informações mais detalhadas sobre ambientes compatíveis, consulte a [[!DNL Microsoft Office 365] home page](https://products.office.com/en-us/office-365-home).

## Instalar o suplemento

Você pode obter o suplemento Workfront para Outlook em [loja da Microsoft](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview).

### [!DNL Workfront] para [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Entrada [!DNL Outlook 365], clique no link **[!UICONTROL Procurar Suplementos]** ícone ![](assets/outlook-add-in-26x26.png)na parte superior da interface do Office 365 e clique em **[!UICONTROL Gerenciar suplementos]**.

1. No **[!UICONTROL Pesquisar suplementos]** caixa, pesquisar **[!DNL Workfront]** depois pressione [!UICONTROL Enter].

1. Clique em **[!UICONTROL Adicionar]**.

### [!DNL Workfront] para [!DNL Outlook] na Web {#workfront-for-outlook-on-the-web}

1. Abertura [!DNL Microsoft Outlook] em um navegador da Web.
1. Clique em **[!UICONTROL Procurar] suplementos** ícone ![](assets/outlook-add-in-web-version-20x20.png).

   Para localizar o ícone, consulte [Uso de suplementos no [!DNL Outlook] na Web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) na documentação do Microsoft.

1. Pesquisar por **[!DNL Workfront]** no **[!UICONTROL Pesquisar suplementos]** e pressione **[!UICONTROL Enter]**.

1. Quando ele aparecer na lista, clique em **Adicionar**.

### [!DNL Workfront for Outlook] em [!UICONTROL Windows] ou [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Clique em **[!UICONTROL Início]** > **[!UICONTROL Loja]** na fita.

1. Pesquisar por **[!DNL Workfront]** no **[!UICONTROL Pesquisar]** e pressione **[!UICONTROL Enter]**.

1. Clique no botão de alternância para ativar a **[!UICONTROL [!DNL Workfront]suplemento]**.

## Efetue logon no [!DNL Workfront] de [!DNL Outlook]

1. Entrada [!DNL Outlook], selecione uma mensagem de email e clique no link **[!DNL Workfront]** no cabeçalho do email.
1. Siga as instruções para fazer logon no [!DNL Workfront] usando a Autenticação aprimorada, o OAuth 2.0 ou o URL da SAML (Security Assertion Markup Language).

   Antes que os usuários possam fazer logon na [!DNL Workfront] add-in usando SAML, um [!DNL Workfront] o administrador precisa primeiro habilitar [!DNL Office 365] suplementos para autenticar usando uma solução SAML 2.0. Para obter mais informações, consulte a seção [Configurar [!DNL Adobe Workfront] com SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) no artigo [Configurar [!DNL Adobe Workfront] com SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Quando for solicitado que você insira o domínio de seu [!DNL Workfront] digite-a usando este formato: *yourCompany&#39;sDomain.my.workfront.com*. O domínio da sua empresa geralmente é o nome da sua empresa.
   >* A Autenticação aprimorada não estará disponível até que um [!DNL Workfront] o administrador o habilita nessa integração.

