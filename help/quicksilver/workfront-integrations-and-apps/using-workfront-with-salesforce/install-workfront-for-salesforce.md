---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Instalar [!DNL Adobe Workfront] por [!DNL Salesforce]
description: Para instalar o aplicativo antes que ele se torne disponível no [!DNL Salesforce] AppExchange, consulte Instalação [!DNL Workfront] do Salesforce antes que ele se torne disponível no AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 1%

---

# Instalar [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Salesforce não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Salesforce.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Salesforce, consulte [módulos do Salesforce](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Como administrador do [!DNL Salesforce] e do [!DNL Adobe Workfront], você pode instalar o [!DNL Workfront for Salesforce] para permitir que seus usuários do [!DNL Salesforce] enviem solicitações do [!DNL Workfront] e criem projetos automaticamente sem sair da Salesforce.

Para obter uma compreensão geral sobre o que você pode esperar ao instalar o [!DNL Workfront for Salesforce], consulte [[!DNL Adobe Workfront for Salesforce] visão geral](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Pré-requisitos para Instalação e Utilização do  [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Instalando [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para usar a funcionalidade descrita neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p><p>Ou</p><p>Atual: [!UICONTROL Plano]</p> </td> 
  </tr>  </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos para Instalar e Usar o [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Você deve ter uma instância [!DNL Salesforce] com acesso a uma conta de administrador do sistema para instalar o aplicativo.
* Você deve ter uma instância [!DNL Workfront] com acesso a uma conta de administrador do sistema para configurar a integração.
* Os usuários do [!UICONTROL Salesforce] devem ter uma conta [!DNL Workfront] para poder:

   * Criar [!DNL Workfront] solicitações de [!DNL Salesforce]
   * Exibir [!DNL Workfront] solicitações ou projetos no Salesforce

## Instalando [!DNL Workfront for Salesforce]  {#installing-workfront-for-salesforce}

Você precisa ser um [!DNL Salesforce] e um administrador do sistema [!DNL Workfront] para instalar e configurar o [!DNL Workfront for Salesforce].

As subseções a seguir descrevem como instalar o [!DNL Workfront] para seu ambiente de Produção [!DNL Salesforce]. Você pode seguir as mesmas etapas para instalar o [!DNL Workfront] para seu ambiente de sandbox do [!DNL Salesforce].

* [Instalando [!DNL Workfront for Salesforce] antes que ele se torne disponível no [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Instalando [!DNL Workfront for Salesforce] na [!DNL Salesforce Classic] Estrutura](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Instalando [!DNL Workfront for Salesforce] na [!DNL Salesforce Lightning Experience] Estrutura](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Instalando o [!DNL Workfront for Salesforce] antes que ele se torne disponível no [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] estará disponível em [!DNL Salesforce AppExchange] em breve.

Para instalar o aplicativo antes que ele esteja disponível:

1. No ambiente de Produção, acesse

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   No ambiente de sandbox, acesse

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >Você deve estar conectado ao Salesforce para acessar essas páginas.

1. Marque a caixa **[!UICONTROL Sim, conceder acesso a esses sites de terceiros]**.

   Uma tela de carregamento é exibida. A instalação pode levar algum tempo.

1. Clique em **[!UICONTROL Concluído]** quando a instalação for concluída.

1. Navegue até **[!UICONTROL Configuração]** > **[!UICONTROL Segurança] Controles** > **[!UICONTROL Configurações de Site Remoto]**.
1. (Condicional) Selecione Workfront na lista.

   Ou

   Se você não vir a URL [!DNL Workfront] listada na lista **[!UICONTROL Todos os Sites Remotos]**, clique em **[!UICONTROL Novo Site Remoto]**.

1. (Condicional) Ao adicionar o site, especifique o **[!UICONTROL Nome do Site Remoto]**.

   Por exemplo, *[!DNL Workfront]*.

1. (Condicional) Se estiver adicionando o site, especifique a **[!UICONTROL URL do Site Remoto]**.

   Por exemplo, *yourDomain.my.workfront.com*.

1. Clique em **[!UICONTROL Salvar]**.

   O aplicativo [!DNL Workfront] agora está instalado em sua instância [!DNL Salesforce] e as **[!UICONTROL WorkfrontOpportunity]** e **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] Páginas foram criadas em seu ambiente.

   [!DNL Salesforce] usuários podem usar o aplicativo depois que você adiciona a seção [!DNL Workfront] aos layouts de página de [!UICONTROL Oportunidade] ou [!UICONTROL Conta].\
   Para obter informações sobre como configurar a seção Workfront para usuários, consulte [Configurar a seção Adobe Workfront para usuários do Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalando o [!DNL Workfront] para [!DNL Salesforce] na Estrutura [!DNL Salesforce Classic]

1. Faça logon em [!DNL Salesforce] como administrador do sistema.
1. Ir para **Instalação.**
1. Na seção **Build**, clique em **AppExchange Marketplace**.

1. Na caixa **Pesquisar Aplicativos AppExchange**, digite **Workfront**.

1. Clique no aplicativo Workfront ao encontrá-lo e clique em **Obter agora**.
1. Clique em **[!UICONTROL Instalar em Produção]** para instalar o aplicativo [!DNL Workfront] no ambiente de Produção [!DNL Salesforce]. (recomendado)
1. Depois de ler e concordar com os termos e condições, habilite o campo **[!UICONTROL Eu li e concordo com os termos e condições]**.
1. Clique em **[!UICONTROL Confirmar e instalar]**.
1. Selecione **[!UICONTROL Instalar para todos os usuários]** (recomendado) e clique em **[!UICONTROL Instalar]**.

1. (Condicional) Se você for solicitado a aprovar o acesso de terceiros, selecione **[!UICONTROL Sim, conceda acesso a esses sites]** e clique em **[!UICONTROL Continuar]**.

1. Clique em **[!UICONTROL Concluído]** quando a instalação for concluída.

   O aplicativo [!DNL Workfront] está listado em **[!UICONTROL Pacotes Instalados]**.


1. Navegue até **[!UICONTROL Configuração>Controles de Segurança>Configurações do Site Remoto]**.
1. (Condicional) Se você não vir a URL [!DNL Workfront] listada na lista **[!UICONTROL Todos os Sites Remotos]**, clique em **[!UICONTROL Novo Site Remoto]**.

1. (Condicional) Ao adicionar o site, especifique o **[!UICONTROL Nome do Site Remoto]**.
Por exemplo, *[!DNL Workfront]*.

1. (Condicional) Se estiver adicionando o site, especifique a **[!UICONTROL URL do Site Remoto]**.
Por exemplo, *yourDomain.my.workfront.com*.

1. Clique em **[!UICONTROL Salvar]**.\
   O aplicativo [!DNL Workfront] agora está instalado em sua instância [!DNL Salesforce]. As **[!UICONTROL Oportunidades do Workfront]** e **[!UICONTROL Contas do Workfront]** [!UICONTROL Visualforce] páginas foram criadas em seu ambiente.\
   [!DNL Salesforce] usuários ainda não podem usar o aplicativo até que você adicione a seção [!DNL Workfront] aos seus layouts de página [!UICONTROL Oportunidade] ou [!UICONTROL Conta].\
   Para obter informações sobre como configurar a seção [!DNL Workfront] para usuários, consulte [Configurar a [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalando [!DNL Workfront for Salesforce] na Estrutura [!DNL Salesforce Lightning Experience]

1. Faça logon em [!DNL Salesforce] como administrador do sistema.
1. Clique no ícone **[!UICONTROL Instalação]** e em **[!UICONTROL Instalação]**.

1. Na seção **[!UICONTROL FERRAMENTAS DA PLATAFORMA]**, expanda **[!UICONTROL Aplicativos].**

1. Clique em **[!DNL AppExchange Marketplace]**.
1. Na caixa **[!UICONTROL Pesquisar [!DNL AppExchange] Aplicativos]**, digite **[!DNL Workfront]**.

1. Clique no aplicativo Workfront ao encontrá-lo e clique em **Obter agora**.
1. Clique em **[!UICONTROL Abrir tela de logon]**.\
   Você deve entrar com sua conta de administrador do [!DNL Workfront] para [!DNL Salesforce].

1. Clique em **[!UICONTROL Permitir]**.
1. Na caixa **[!UICONTROL Instalar nesta Organização]**, clique em **[!UICONTROL Instalar Aqui]** para instalar o [!DNL Workfront] no ambiente de Produção [!DNL Salesforce]. (recomendado)

1. Depois de ler e concordar com os termos e condições, habilite o campo **[!UICONTROL Eu li e concordo com os termos e condições]**.
1. Clique em **[!UICONTROL Confirmar e instalar]**.
1. Selecione **[!UICONTROL Instalar para todos os usuários]** (recomendado) e clique em **[!UICONTROL Instalar]**.

1. (Condicional) Se você for solicitado a aprovar o acesso de terceiros, selecione **[!UICONTROL Sim, conceda acesso a esses sites]** e clique em **[!UICONTROL Continuar]**.

1. Clique em **[!UICONTROL Concluído]** quando a instalação for concluída.

   O aplicativo [!DNL Workfront] está listado em **[!UICONTROL Pacotes Instalados]**.

1. Navegue até **[!UICONTROL Configuração].**
1. Na seção **[!UICONTROL CONFIGURAÇÕES]**, expanda **[!UICONTROL Segurança].**

1. Clique em **[!UICONTROL Configurações do Site Remoto]**.
1. (Condicional) Se você não vir a URL [!DNL Workfront] listada na lista **[!UICONTROL Todos os Sites Remotos]**, clique em **[!UICONTROL Novo Site Remoto]**.

1. (Condicional) Ao adicionar o site, especifique o **[!UICONTROL Nome do Site Remoto]**.
Por exemplo, *[!DNL Workfront]*.

1. (Condicional) Se estiver adicionando o site, especifique a **[!UICONTROL URL do Site Remoto]**.
Por exemplo, *yourDomain.my.workfront.com*.

1. Clique em **[!UICONTROL Salvar]**.

   O aplicativo [!DNL Workfront] agora está instalado em sua instância [!DNL Salesforce], e o componente **[!DNL Workfront]** agora é adicionado ao seu ambiente.

   Os usuários do [!UICONTROL Salesforce] podem usar o aplicativo [!DNL Workfront] depois que você adicionar a seção [!DNL Workfront] aos layouts de página de [!UICONTROL Oportunidade] ou [!UICONTROL Conta].\
   Para obter informações sobre como configurar a seção [!DNL Workfront] para usuários, consulte [Configurar a [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Configurar permissões para a integração do Workfront para Salesforce

### Permissões para `workfront_business`

1. Navegue até **Configuração** > **Segurança** > **URLs Confiáveis**.
1. Selecione `workfront_business` na lista.
1. Clique em **Editar**.
1. Nas Diretivas CSP, verifique as seguintes opções:

   * connect-src (scripts)
   * font-src (fontes)
   * frame-src (conteúdo de iframe)
   * img-src (imagens)
   * media-src (áudio e vídeo)
   * style-src (folhas de estilos)

1. Clique em **Salvar**.


### Permissões para workfront_session

1. Navegue até **Configuração** > **Segurança** > **URLs Confiáveis**.
1. Selecione `workfront_session` na lista.
1. Clique em **Editar**.
1. Nas Diretivas CSP, verifique as seguintes opções:

   * connect-src (scripts)
   * font-src (fontes)
   * frame-src (conteúdo de iframe)
   * img-src (imagens)
   * media-src (áudio e vídeo)
   * style-src (folhas de estilos)

1. Clique em **Salvar**.

