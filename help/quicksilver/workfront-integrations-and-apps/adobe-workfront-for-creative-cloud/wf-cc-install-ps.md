---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Instalar e abrir [!DNL Adobe Workfront for Photoshop]
description: Você pode instalar o plug-in do Adobe Workfront para Photoshop no Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: f5e9f121-a711-4b75-8564-54f29c5cfa48
source-git-commit: 61e5b763ec527aeb846e975e06842dc2c4c69918
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 2%

---

# Instalar e abrir o [!DNL Adobe Workfront for Photoshop]

Você pode instalar o plug-in [!DNL Adobe Workfront for Photoshop] do [!DNL Adobe Marketplace]. O plug-in é compatível com os seguintes idiomas:

* Inglês
* Francês
* Alemão
* Italiano
* espanhol
* Português
* japonês
* Chinês simplificado
* Chinês tradicional
* coreano

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td><p>Você deve ter uma licença [!DNL Adobe Creative Cloud] além de uma licença [!DNL Workfront].</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

* Você deve instalar o aplicativo [!DNL Adobe Photoshop] antes de instalar o plug-in [!DNL Workfront].

## Instalar o plug-in [!DNL Adobe Workfront for Photoshop] para sua organização

Se você for um administrador [!DNL Adobe Admin Console], poderá incluir o plug-in em [!DNL Creative Cloud] pacotes de implantação. Para obter mais informações, consulte [Incluindo plug-ins em seu pacote](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[Veja um tutorial em vídeo aqui](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

Os administradores do [!DNL Adobe Admin Console] também podem criar pacotes somente de plug-in para distribuição aos usuários. Para obter mais informações, consulte [Criar [!UICONTROL [!DNL Adobe Workfront] para [!DNL Creative Cloud]] pacotes para seus usuários no [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Instalar o plug-in [!DNL Adobe Workfront for Photoshop] individualmente

Você pode instalar o plug-in [!DNL Adobe Workfront for Photoshop] por conta própria a partir do [!DNL Adobe Exchange].

1. Vá para a [página de instalação do Adobe Workfront para Photoshop](https://adobe.com/go/cc_plugins_discover_plugin?pluginId=37722a55&workflow=share) no Adobe Exchange.
1. Na caixa de diálogo exibida, clique em **Abrir [!DNL Adobe Creative Cloud] aplicativo de desktop**.
1. Depois que o gerenciador de plug-in [!DNL Adobe Photoshop] for aberto, clique em **[!UICONTROL Instalar]**.
1. Leia as informações na caixa de diálogo, clique em **[!UICONTROL OK]** e siga as instruções na tela para concluir a instalação.

1. Prossiga para a seção a seguir para obter informações sobre como abrir o plug-in.

## Abrir o plug-in [!DNL Adobe Workfront for Photoshop]

1. Abrir [!DNL Photoshop].

1. Crie um novo arquivo ou abra um existente.

1. No menu superior, clique em **[!UICONTROL Plug-ins]** > **[!UICONTROL Painel Plug-ins]**.

   ![Painel de plug-ins](assets/plugins-panel-ps.png)

1. No **[!UICONTROL Painel Plug-ins]**, escolha a guia **[!UICONTROL Plug-ins]** e localize o **[!UICONTROL Workfront for Adobe Photoshop]**.

   >[!TIP]
   >
   >   Se você não vir o plug-in depois de abri-lo no [!UICONTROL Painel Plug-ins], ele pode estar atrás do aplicativo Photoshop. Tente minimizar o Photoshop para encontrar o plug-in.

1. Prossiga para a seção a seguir para obter informações sobre como fazer logon no plug-in.

## Fazer logon em [!DNL Adobe Workfront for Photoshop]

1. No menu **[!UICONTROL Plug-ins]**, na parte superior da tela, selecione **[!UICONTROL Painel de Plug-ins]**.
1. Selecione **[!DNL Adobe Workfront for Photoshop]**.
1. Insira seu domínio e clique em **[!UICONTROL Fazer logon]**. Uma página do navegador é aberta. Talvez seja necessário conceder permissão à Photoshop para abrir o navegador.

   >[!TIP]
   >
   >* Para localizar seu domínio, abra um navegador, navegue até a instância do [!DNL Workfront] e copie a primeira parte da URL:\
   >![Localizar domínio](assets/domain-350x50.png)
   >
   >* Se sua instância do Workfront estiver integrada ao Experience Cloud e o domínio começar com `experience.adobe.com`, peça ao administrador para fornecer o domínio do Workfront encontrado em Produto > Workfront no Admin Console.

1. No navegador, insira suas credenciais do [!DNL Adobe] e clique em **[!UICONTROL Fazer logon]**. Se sua empresa usa um logon único (SSO), você será direcionado à página do seu provedor de SSO para fazer logon.

   >[!NOTE]
   >
   >Talvez você não seja solicitado a inserir suas credenciais do [!DNL Workfront] se tiver feito logon recentemente.

1. Siga as instruções para fazer logon no [!DNL Workfront].

   >[!NOTE]
   >
   >* O [!DNL Workfront] se conecta ao [!DNL Adobe Creative Cloud] usando o OAuth 2.0, um padrão seguro usado pela maioria das integrações baseadas na Web para a autenticação e autorização de usuários.


1. Clique em **[!UICONTROL Permitir Acesso]** para concluir o logon.
1. Retorne ao [!UICONTROL Adobe Photoshop] para ver seu trabalho.

### Solução de problemas de erros de logon

**O erro &quot;Algo deu errado&quot; é exibido ao tentar fazer logon**


Você não pode usar uma URL que comece com `experience.adobe.com` para fazer logon no plug-in.

![erro de logon](assets/plugin-log-in-error.png) ![domínio](assets/incorrect-domain.png)


Para corrigir esse problema,

1. Exclua a pasta que armazena o domínio do plug-in.

   >[!TIP]
   >
   >Em uma Mac, vá para Localizador, pressione **Command+Shift+.** para exibir pastas ocultas, navegue até **/Users//Library/Application Support** e exclua a pasta **Workfront**.


1. Volte para o plug-in e insira o domínio do Workfront. O domínio deve ser `company-name.my.workfront.com` e não `experience.adobe.com`.

   Para [encontrar seu domínio do Workfront](/help/quicksilver/wf-api/tips-tricks-and-troubleshooting/locate-domain-for-api.md), se você estiver na Experiência unificada da Adobe, vá para Configuração, Informações do cliente.
