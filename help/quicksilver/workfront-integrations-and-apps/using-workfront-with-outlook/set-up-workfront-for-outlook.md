---
product-area: workfront-integrations
navigation-topic: workfront-for-outlook
title: Configurar [!DNL Adobe Workfront] para [!DNL Outlook]
description: O Adobe Workfront Fusion oferece uma integração com o Outlook. Este artigo descreve como você pode começar a usar essa integração em seus próprios fluxos de trabalho.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 57f0560b-68c2-4654-863e-bd728e76da29
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Outlook]

O [!DNL Adobe Workfront] [!DNL Outlook] o add-in permite fazer a seguinte chave [!DNL Workfront] tarefas diretamente do Outlook:

* Atualize um projeto, tarefa ou problema existente com informações de um email. Para obter mais informações, consulte [Atualizar um objeto existente de um [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/update-an-existing-object-from-an-outlook-email.md).
* Crie um [!DNL Workfront] com base em um email no [!DNL Outlook]. Para obter mais informações, consulte [Criar uma solicitação do Adobe Workfront a partir de um [!DNL Outlook] email](../../workfront-integrations-and-apps/using-workfront-with-outlook/create-a-wf-request-from-an-outlook-email.md).
* Adicionar um email como tarefa em seu [!UICONTROL Meu trabalho] área. Para obter mais informações, consulte [Adicione um [!DNL Outlook] enviar email como uma tarefa para sua lista de trabalho](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-as-task-to-your-work-list.md).
* Responder aos comentários por meio da [!DNL Workfront] suplemento para [!DNL Outlook]. Para obter informações sobre como responder a comentários do Workfront para [!DNL Outlook], consulte [Responder a um comentário de [!DNL Outlook]](../../workfront-integrations-and-apps/using-workfront-with-outlook/reply-to-a-comment-from-outlook.md).
* Crie tarefas e problemas do zero ou crie-os a partir de emails existentes (usando a funcionalidade de arrastar e soltar). Para obter mais informações, consulte [Adicione um [!DNL Outlook] enviar um email para um projeto como uma tarefa ou um problema](../../workfront-integrations-and-apps/using-workfront-with-outlook/add-outlook-email-to-project-as-task-or-issue.md).

Você deve adicionar o [!DNL Workfront] suplemento ao seu [!DNL Outlook] antes de usar [!DNL Workfront for Outlook].

Se não conseguir instalar o [!DNL Workfront] com seu [!DNL Outlook] entre em contato com sua [!DNL Workfront] para garantir que [!DNL Outlook] os suplementos são ativados para a organização.

Para obter informações sobre como ativar a variável [!DNL Outlook] integração para sua organização, consulte [Habilitar [!DNL Adobe Workfront for Outlook]](../../administration-and-setup/configure-integrations/enable-workfront-for-outlook.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Seu [!DNL Workfront] o administrador deve habilitar [!DNL Outlook for Office] com [!DNL Workfront] antes de poder usar essa integração.

## Requisitos do sistema

Os seguintes aplicativos estão disponíveis:

* **[!DNL Outlook]na Web:** O [!DNL Workfront] o suplemento está disponível ao usar [!DNL Outlook] em um navegador da Web em um desktop ou dispositivo móvel. Essa funcionalidade também está disponível ao usar a variável [!DNL Outlook] Aplicativo da Web.
* **[!DNL Outlook]Aplicativo de desktop:** O [!DNL Workfront] o suplemento está disponível ao usar o [!DNL Windows] e [!DNL Mac] versões para desktop de [!DNL Outlook] incluído na [!DNL Office] pacote.

O [!DNL Workfront] suplemento para [!DNL Outlook] O é compatível com ambientes que atendem aos seguintes requisitos:

* [Requisitos do cliente](#client-requirements-client-requirements)
* [Requisitos do servidor de correio](#mail-server-requirements-mail-server-requirements)

### Requisitos do cliente {#client-requirements}

Oferecemos suporte para as seguintes versões de [!DNL Outlook]:

* [!DNL Outlook 2013] ou mais tarde [!DNL Windows]
*[!DNL  Outlook 2016] ou mais tarde [!DNL Windows]
* [!DNL Outlook] on [!DNL Mac] ([!DNL Microsoft 365])
* [!DNL Outlook] on [!DNL Windows] ([!DNL Microsoft 365])
* [!DNL Outlook] na Web

Você deve estar conectado a um [!DNL Exchange Server] ou [!DNL Office 365] usando uma conexão direta.

Ao configurar o cliente, o usuário deve selecionar um dos seguintes tipos de conta:

* [!DNL Exchange]
* [!DNL Office 365]
* [!DNL Outlook.com]&#x200B;**&#x200B;**&#x200B; Se o cliente estiver configurado para se conectar com POP3 ou IMAP, a variável [!DNL Workfront] o suplemento não é carregado.

### Requisitos do servidor de correio {#mail-server-requirements}

Os requisitos do servidor de email são atendidos por padrão ao se conectar ao [!DNL Office 365] ou [!DNL Outlook.com]. No entanto, se estiver conectado a uma instalação local do [!DNL Exchange Server], aplicam-se os seguintes requisitos:

* Apoiamos [!DNL Exchange 2016 On-Premise]
* [!DNL Exchange Web Services] (EWS) deve ser ativado e exposto à Internet.
* O servidor deve ter um certificado de autenticação válido para que o servidor emita tokens de identidade válidos. Novas instalações de [!DNL Exchange Server] incluir um certificado de autenticação padrão.

   Para obter mais informações, consulte [Certificados digitais e criptografia em [!DNL Exchange 2016]](https://technet.microsoft.com/en-us/library/dd351044(v=exchg.160).aspx) e [Set-AuthConfig](https://technet.microsoft.com/en-us/library/jj215766(v=exchg.160).aspx).

* Para acessar o [!DNL Workfront] suplemento do [[!DNL Office] Loja](https://store.office.com/), seus servidores de acesso ao cliente devem ser capazes de se comunicar com o  [https://store.office.com](https://store.office.com/).

Para obter informações mais detalhadas sobre os ambientes compatíveis, consulte o [[!DNL Microsoft Office 365] página inicial](https://products.office.com/en-us/office-365-home).

## Instalar o suplemento

Para obter mais informações sobre como configurar a variável [!DNL Workfront] suplemento para [!DNL Outlook], consulte [[!DNL Workfront] - Gestão do Trabalho Colaborativo.](https://appsource.microsoft.com/en-us/product/office/WA104380943?tab=Overview)

* [[!DNL Workfront] por [!DNL Outlook 365]](#workfront-for-outlook-365-workfront-for-outlook-365)
* [[!DNL Workfront] para [!DNL Outlook] na Web](#workfront-for-outlook-on-the-web-workfront-for-outlook-on-the-web)
* [[!DNL Workfront] para [!DNL Outlook] on [!DNL Windows] ou [!DNL Mac]](#workfront-for-outlook-on-windows-or-mac-workfront-for-outlook-on-windows-or-mac)

### [!DNL Workfront] por [!DNL Outlook 365] {#workfront-for-outlook-365}

1. Em [!DNL Outlook 365], clique no botão **[!UICONTROL Procurar Suplementos]** ícone ![](assets/outlook-add-in-26x26.png)na parte superior da interface do Office 365, em seguida, clique em **[!UICONTROL Gerenciar suplementos]**.

1. No **[!UICONTROL Pesquisar suplementos]** , pesquisar por **[!DNL Workfront]** pressione [!UICONTROL Enter].

1. Clique em **[!UICONTROL Adicionar]**.

### [!DNL Workfront] para [!DNL Outlook] na Web {#workfront-for-outlook-on-the-web}

1. Abrir [!DNL Microsoft Outlook] em um navegador da Web.
1. Clique no botão **[!UICONTROL Procurar] suplementos** ícone ![](assets/outlook-add-in-web-version-20x20.png).

   Para localizar o ícone, consulte [Uso de suplementos em [!DNL Outlook] na Web](https://support.microsoft.com/en-us/office/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce#bkmk_addaddinsicon) na documentação do Microsoft.

1. Procurar por **[!DNL Workfront]** no **[!UICONTROL Pesquisar suplementos]** e pressione **[!UICONTROL Enter]**.

   ![workfront_for_outlook_on_the_web.png](assets/workfront-for-outlook-on-the-web-350x116.png)

1. Quando aparecer na lista, clique em **Adicionar**.

### [!DNL Workfront for Outlook] on [!UICONTROL Windows] ou [!DNL Mac] {#workfront-for-outlook-on-windows-or-mac}

1. Clique em **[!UICONTROL Início]** > **[!UICONTROL Loja]** na fita.

1. Procurar por **[!DNL Workfront]** no **[!UICONTROL Pesquisar]** e pressione **[!UICONTROL Enter]**.

   ![o365_addin_search.png](assets/o365-addin-search-350x158.png)

1. Clique no botão para ativar a variável **[!UICONTROL [!DNL Workfront]suplemento]**.

## Faça logon em [!DNL Workfront] from [!DNL Outlook]

1. Em [!DNL Outlook], selecione uma mensagem de email e clique no botão **[!DNL Workfront]** no cabeçalho do email.
1. Siga as instruções para fazer logon no [!DNL Workfront] usando Autenticação aprimorada, OAuth 2.0 ou o URL de SAML (Security Assertion Markup Language).

   Antes que os usuários possam fazer logon na [!DNL Workfront] suplemento utilizando SAML, um [!DNL Workfront] o administrador deve primeiro habilitar [!DNL Office 365] suplementos para autenticar usando uma solução SAML 2.0. Para obter mais informações, consulte a seção [Configurar [!DNL Adobe Workfront] com SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md#enable-saml-with-office-365) no artigo [Configurar [!DNL Adobe Workfront] com SAML 2.0](../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2.md).

   >[!NOTE]
   >
   >* Quando for solicitado a inserir o domínio de [!DNL Workfront] digite-a usando este formato: *sua empresa&#39;sDomain.my.workfront.com*. O domínio de sua empresa geralmente é o nome de sua empresa.
   >* A Autenticação aprimorada não está disponível até que um [!DNL Workfront] O administrador o habilita para essa integração.


