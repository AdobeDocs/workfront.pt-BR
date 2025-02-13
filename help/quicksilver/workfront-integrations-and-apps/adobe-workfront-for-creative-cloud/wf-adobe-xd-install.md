---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Instalar e abrir o Adobe Workfront para XD
description: Você pode instalar o plug-in do Adobe Workfront para XD no Adobe Marketplace.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: a5c4479833243bb5817196a3af8acaa063a16747
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 1%

---

# Instalar e abrir o [!DNL Adobe Workfront for XD]

Você pode instalar o plug-in [!DNL Adobe Workfront for XD] do Adobe Marketplace. O plug-in é compatível com os seguintes idiomas:

* Inglês
* Francês
* Alemão
* Italiano
* Espanhol
* Português
* Japonês
* Chinês simplificado
* Chinês tradicional
* Coreano

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Produto</td> 
   <td><p>Você deve ter uma licença [!DNL Adobe Creative Cloud] além de uma licença [!DNL Workfront].</p><p>Para obter mais informações, consulte <a href="https://helpx.adobe.com/support/programs/cc-support-policy.html#cce" class="MCXref xref" xrefformat="{para}">Política de Suporte da Creative Cloud</a>.</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

+++

## Pré-requisitos

* Você deve instalar o aplicativo [!DNL Adobe XD] antes de instalar o plug-in do Workfront.

## Instalar o plug-in [!DNL Adobe Workfront for XD] para sua organização

Se você for um administrador [!DNL Adobe Admin Console], poderá incluir o plug-in em [!DNL Creative Cloud] pacotes de implantação. Para obter mais informações, consulte [Incluindo plug-ins em seu pacote](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html).

[Veja um tutorial em vídeo aqui](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}.

Os administradores do [!DNL Adobe Admin Console] também podem criar pacotes somente de plug-in para distribuição aos usuários. Para obter mais informações, consulte [Criar [!UICONTROL [!DNL Adobe Workfront] para [!DNL Creative Cloud]] pacotes para seus usuários no [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## Instalar o plug-in [!DNL Adobe Workfront for XD] individualmente

Você pode instalar o plug-in [!DNL Adobe Workfront for XD] por conta própria a partir do [!DNL Adobe Exchange].

1. Vá para a [página de instalação do Adobe Workfront para XD](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&amp;workflow=share) no Adobe Exchange.
1. Na caixa de diálogo exibida, clique em **Abrir [!DNL Adobe Creative Cloud] aplicativo de desktop**.
1. Depois que o gerenciador de plug-in [!DNL Adobe XD] for aberto, clique em **[!UICONTROL Instalar]**.
1. Leia as informações na caixa de diálogo e clique em **[!UICONTROL OK]**.
1. Prossiga para a seção a seguir para obter informações sobre como abrir o plug-in.

## Abrir o plug-in [!DNL Adobe Workfront for XD]

1. Abrir [!DNL Adobe XD].

1. Crie um novo arquivo ou abra um existente.

1. No canto inferior esquerdo, clique no ícone **Plug-ins**.

![Janela de plug-in do XD](assets/xd-plugin-window-350x620.png)

1. No **[!UICONTROL Painel de Plug-ins]**, localize o **[!UICONTROL Adobe Workfront para XD]**.

1. Prossiga para a seção a seguir para obter informações sobre como fazer logon no plug-in.

## Fazer logon em [!DNL Adobe Workfront for XD]

1. Verifique se o painel Plug-in está aberto e clique em **[!DNL Adobe Workfront for XD]**.
1. Insira seu domínio e clique em **[!UICONTROL Fazer logon]**. Uma página do navegador é aberta.

   >[!TIP]
   >
   >* Para localizar seu domínio, abra um navegador, navegue até a instância do [!DNL Workfront] e copie a primeira parte da URL:\
   >![Localizar domínio](assets/domain-350x50.png)
   >
   > * Se sua instância do Workfront estiver integrada ao Experience Cloud, peça ao administrador para fornecer o domínio do Workfront encontrado em Produto > Workfront no Admin Console.

1. No navegador, insira suas credenciais do [!DNL Workfront] e clique em **[!DNL Log in]**. Se sua empresa usa um logon único (SSO), você será direcionado à página do seu provedor de SSO para fazer logon.

   >[!NOTE]
   >
   >Talvez você não seja solicitado a inserir suas credenciais do [!DNL Workfront] se tiver feito logon recentemente.

   Siga as instruções para fazer logon no [!DNL Workfront].

   >[!NOTE]
   >
   >* O [!DNL Workfront] se conecta ao [!DNL Adobe Creative Cloud] usando o OAuth 2.0, um padrão seguro usado pela maioria das integrações baseadas na Web para a autenticação e autorização de usuários.
   >* Quando for solicitado que você insira o [domínio ou host] da sua conta do [!DNL Workfront], digite-o usando este formato: *yourCompany&#39;sDomain.my.workfront.com*. O domínio da sua empresa geralmente é o nome da sua empresa.

1. Clique em **[!UICONTROL Permitir Acesso]** para concluir o logon e voltar para [!DNL Adobe XD] para ver seu trabalho.

### Solução de problemas de erros de logon

**O erro &quot;Algo deu errado&quot; é exibido ao tentar fazer logon**


Você não pode usar uma URL que comece com `experience.adobe.com` para fazer logon no plug-in.

![erro de logon](assets/plugin-log-in-error.png) ![domínio](assets/incorrect-domain.png)


Para corrigir esse problema,

1. Desinstale e reinstale o plug-in do Adobe Workfront para XD para limpar o domínio e o erro.

1. Insira seu domínio do Workfront. O domínio deve ser `company-name.my.workfront.com` e não `experience.adobe.com`.

Para encontrar seu domínio do Workfront se você estiver na Experiência unificada da Adobe, acesse
