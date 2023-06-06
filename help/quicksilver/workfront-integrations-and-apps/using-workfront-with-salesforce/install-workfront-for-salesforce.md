---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Instalar [!DNL Adobe Workfront] para [!DNL Salesforce]
description: Para instalar o aplicativo antes que ele fique disponível no [!DNL Salesforce] AppExchange, consulte Instalação [!DNL Workfront] para Salesforce antes que ele se torne disponível no AppExchange Marketplace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: 0c49ab99653f390d592bba39bcb92145b8bedd0c
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 1%

---

# Instalar [!DNL Adobe Workfront for Salesforce]

Para instalar o aplicativo antes que ele fique disponível no [!DNL Salesforce AppExchange], consulte [Instalando [!DNL Workfront for Salesforce] antes de se tornar disponível no [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

Como um [!DNL Salesforce] e [!DNL Adobe Workfront] administrador, você pode instalar [!DNL Workfront for Salesforce] para permitir que seus [!DNL Salesforce] usuários a enviar [!DNL Workfront] e criar projetos automaticamente sem sair do Salesforce.

Para obter uma compreensão geral sobre o que você pode esperar ao instalar o [!DNL Workfront for Salesforce], consulte [[!DNL Adobe Workfront for Salesforce] visão geral](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Pré-requisitos para instalação e uso [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Instalando [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade descrita neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano]</p> </td> 
  </tr>  </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Pré-requisitos para instalação e uso [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Você deve ter um [!DNL Salesforce] com acesso a uma conta de administrador do sistema para instalar o aplicativo.
* Você deve ter um [!DNL Workfront] com acesso a uma conta de administrador do sistema para configurar a integração.
* [!UICONTROL Salesforce] os usuários devem ter uma [!DNL Workfront] conta para poder

   * Criar [!DNL Workfront] solicitações de [!DNL Salesforce] ou
   * Exibir [!DNL Workfront] solicitações ou projetos no Salesforce.

## Instalando [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

Você deve ser um [!DNL Salesforce] e uma [!DNL Workfront] administrador do sistema instalar e configurar [!DNL Workfront for Salesforce].

As subseções a seguir descrevem como instalar o [!DNL Workfront] para seu [!DNL Salesforce] Ambiente de produção. Você pode seguir as mesmas etapas para instalar o [!DNL Workfront] para seu [!DNL Salesforce] Ambiente de sandbox.

* [Instalando [!DNL Workfront for Salesforce] antes de se tornar disponível no [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Instalando [!DNL Workfront for Salesforce] no [!DNL Salesforce Classic] Estrutura](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Instalando [!DNL Workfront for Salesforce] no [!DNL Salesforce Lightning Experience] Estrutura](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Instalando [!DNL Workfront for Salesforce] antes de se tornar disponível no [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] estará disponível no [!DNL Salesforce AppExchange] em breve.

Para instalar o aplicativo antes que ele esteja disponível:

1. No ambiente de Produção, acesse

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

   No ambiente de sandbox, acesse

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r](https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002SE0r)

1. Verifique a **[!UICONTROL Sim, conceder acesso a esses sites de terceiros]** caixa.

   Uma tela de carregamento é exibida e a instalação pode demorar um pouco.

1. Clique em **[!UICONTROL Concluído]** quando a instalação for concluída.

1. Navegue até **[!UICONTROL Configuração>Controles de Segurança>Configurações do Site Remoto]**.
1. (Condicional) Se você não vir a sua [!DNL Workfront] URL listado no **[!UICONTROL Todos os locais remotos]** clique em **[!UICONTROL Novo local remoto]**.

1. Especifique a **[!UICONTROL Nome do local remoto]**.

   Por exemplo, *[!DNL Workfront]*.

1. Especifique a **[!UICONTROL URL do local remoto]**.

   Por exemplo, *yourDomain.my.workfront.com*.

1. Clique em **[!UICONTROL Salvar]**.

   A variável [!DNL Workfront] O aplicativo agora está instalado em seu [!DNL Salesforce] instância e o **[!UICONTROL OportunidadesWorkfront]** e **[!UICONTROL Contas do Workfront]** [!UICONTROL Visualforce] As páginas foram criadas em seu ambiente.

   [!DNL Salesforce] os usuários podem usar o aplicativo depois que você adiciona o [!DNL Workfront] para a sua [!UICONTROL Oportunidade] ou [!UICONTROL Conta] layouts de página.\
   Para obter informações sobre como configurar a seção Workfront para usuários, consulte [Configurar a seção Adobe Workfront para usuários do Salesforce](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalando [!DNL Workfront] para [!DNL Salesforce] no [!DNL Salesforce Classic] Estrutura

1. Efetue logon no [!DNL Salesforce] como administrador do sistema.
1. Ir para **Configuração.**
1. No **Build** clique em **AppExchange Marketplace**.

1. No **Pesquisar aplicativos de AppExchange** caixa, digite **Workfront**.

1. Clique no aplicativo ao encontrá-lo e clique em **Obtenha agora**.
1. Clique em **[!UICONTROL Instalar na produção]** para instalar o [!DNL Workfront] aplicativo no seu [!DNL Salesforce] Ambiente de produção. (recomendado)
1. Selecione o **[!UICONTROL Li e concordo com os termos e condições]** depois de ler e concordar com os termos e condições.
1. Clique em **[!UICONTROL Confirmar e instalar]**.
1. Selecionar **[!UICONTROL Instalar para todos os usuários]** (recomendado) e clique em **[!UICONTROL Instalar]**.

1. (Condicional) Se for solicitado se você deseja aprovar o acesso de terceiros, selecione **[!UICONTROL Sim, conceder acesso a esses sites de terceiros]** e, em seguida, clique em **[!UICONTROL Continuar]**.

1. Clique em **[!UICONTROL Concluído]** quando a instalação for concluída.

   A variável [!DNL Workfront] o aplicativo está listado em **[!UICONTROL Pacotes instalados]**.


1. Navegue até **[!UICONTROL Configuração>Controles de Segurança>Configurações do Site Remoto]**.
1. (Condicional) Se você não vir a sua [!DNL Workfront] URL listado no **[!UICONTROL Todos os locais remotos]** clique em **[!UICONTROL Novo local remoto]**.\

1. Especifique a **[!UICONTROL Nome do local remoto]**.\
   Por exemplo, *[!DNL Workfront]*.

1. Especifique a **[!UICONTROL URL do local remoto]**.\
   Por exemplo, *yourDomain.my.workfront.com*.

1. Clique em **[!UICONTROL Salvar]**.\
   A variável [!DNL Workfront] O aplicativo agora está instalado em seu [!DNL Salesforce] instância e o **[!UICONTROL OportunidadesWorkfront]** e **[!UICONTROL Contas do Workfront]** [!UICONTROL Visualforce] As páginas foram criadas em seu ambiente.\
   [!DNL Salesforce] os usuários ainda não podem usar o aplicativo até que você adicione o [!DNL Workfront] para a sua [!UICONTROL Oportunidade] ou [!UICONTROL Conta] layouts de página.\
   Para obter informações sobre a configuração do [!DNL Workfront] para usuários, consulte [Configure o [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Instalando [!DNL Workfront for Salesforce] no [!DNL Salesforce Lightning Experience] Estrutura

1. Efetue logon no [!DNL Salesforce] como administrador do sistema.
1. Clique em **[!UICONTROL Configuração] ícone** e, em seguida, clique em **[!UICONTROL Configuração]**.

1. No **[!UICONTROL FERRAMENTAS DA PLATAFORMA]** seção, expandir **[!UICONTROL Aplicativos].**

1. Clique em **[!DNL AppExchange Marketplace]**.
1. No **[!UICONTROL Pesquisar [!DNL AppExchange] Aplicativos]** caixa, digite **[!DNL Workfront]**.

1. Clique no aplicativo ao encontrá-lo e clique em **[!UICONTROL Obtenha agora]**.
1. Clique em **[!UICONTROL Abrir tela de login]**.\
   Você deve entrar com seu [!DNL Workfront] conta de administrador para [!DNL Salesforce].

1. Clique em **[!UICONTROL Permitir]**.
1. No **[!UICONTROL Instalar nesta Organização]** clique em **[!UICONTROL Instalar aqui]** para instalar [!DNL Workfront] no seu [!DNL Salesforce] Ambiente de produção. (recomendado)

1. Selecione o **[!UICONTROL Li e concordo com os termos e condições]** depois de ler e concordar com os termos e condições.
1. Clique em **[!UICONTROL Confirmar e instalar]**.
1. Selecionar **[!UICONTROL Instalar para todos os usuários]** (recomendado) e clique em **[!UICONTROL Instalar]**.

1. (Condicional) Se for solicitado se você deseja aprovar o acesso de terceiros, selecione **[!UICONTROL Sim, conceder acesso a esses sites de terceiros]** e, em seguida, clique em **[!UICONTROL Continuar]**.

1. Clique em **[!UICONTROL Concluído]** quando a instalação for concluída.

   A variável [!DNL Workfront] o aplicativo está listado em **[!UICONTROL Pacotes instalados]**.

1. Navegue até **[!UICONTROL Configuração].**
1. No **[!UICONTROL CONFIGURAÇÕES]** seção, expandir&#x200B;**[!UICONTROL Segurança].**

1. Clique em **[!UICONTROL Configurações do site remoto]**.
1. (Condicional) Se você não vir a sua [!DNL Workfront] URL listado no **[!UICONTROL Todos os locais remotos]** clique em **[!UICONTROL Novo local remoto]**.

1. Especifique a **[!UICONTROL Nome do local remoto]**.

   Por exemplo, *[!DNL Workfront]*.

1. Especifique a **[!UICONTROL URL do local remoto]**.

   Por exemplo, *yourDomain.my.workfront.com*.

1. Clique em **[!UICONTROL Salvar]**.

   A variável [!DNL Workfront] O aplicativo agora está instalado em seu [!DNL Salesforce] instância e o **[!DNL Workfront]** O componente agora é adicionado ao seu ambiente.

   [!UICONTROL Salesforce] os usuários podem usar o [!DNL Workfront] depois de adicionar o [!DNL Workfront] para a sua [!UICONTROL Oportunidade] ou [!UICONTROL Conta] layouts de página.\
   Para obter informações sobre a configuração do [!DNL Workfront] para usuários, consulte [Configure o [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
