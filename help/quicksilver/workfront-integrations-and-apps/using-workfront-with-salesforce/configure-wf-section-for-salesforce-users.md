---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configure o [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários
description: Depois de instalar [!DNL Adobe Workfront] para o Salesforce as a [!DNL Workfront] administrador, você pode disponibilizá-lo para seus usuários, adicionando-o em uma nova seção aos layouts das páginas Oportunidade e Conta no Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# Configure o [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários

A [!UICONTROL Pro] [!DNL Workfront] O plano é necessário para usar esse recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [[!DNL Workfront] Planos.](https://www.workfront.com/plans)

Depois de instalar [!DNL Adobe Workfront] para [!DNL Salesforce] como [!DNL Workfront] administrador, você pode disponibilizá-lo aos usuários, adicionando-o em uma nova seção a eles [!UICONTROL Oportunidade] e [!UICONTROL Conta]
layouts de página em [!UICONTROL Salesforce].

Para obter informações sobre a instalação [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Para usuários que têm [!DNL Workfront] disponível em ambas as [!DNL Classic] e [!DNL Lightning Experience] , você deve adicionar o [!DNL WorkfrontOpportunities] e [!DNL WorkfrontAccounts] [!UICONTROL Força Visual] páginas para a [!UICONTROL Oportunidade] e [!UICONTROL Contas] layouts de página, respectivamente.

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
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

* Você deve ter um [!DNL Salesforce] com acesso a uma conta de administrador do sistema.
* Você deve ter um [!DNL Workfront] com acesso a uma conta de administrador do sistema.

## Configure o [!DNL Workfront] na seção [!DNL Salesforce Classic] estrutura

1. Faça logon em [!DNL Salesforce] como administrador do Workfront.
1. Clique em **[!UICONTROL Configuração].**
1. No **[!UICONTROL Criar]** seção, expandir **[!UICONTROL Personalizar].**

1. Expandir **[!UICONTROL Oportunidades]**, depois clique em **[!UICONTROL Layouts de página]** para adicionar o [!DNL Workfront] para uma Oportunidade.

   Ou

   Expandir **[!UICONTROL Contas]**, depois clique em **[!UICONTROL Layouts de página]** para adicionar o [!DNL Workfront] para uma conta .

1. Clique em **[!UICONTROL Editar]** em um layout existente.

   Ou

   Clique em **[!UICONTROL Novo]** para adicionar um novo layout.

1. (Opcional) Arraste o **[!UICONTROL Seção]** para o layout e solte-o na posição desejada.\

1. (Opcional) Especifique um nome para a nova seção.

   Recomendamos que você nomeie esta seção **[!DNL Workfront]**.

1. (Opcional) Especifique os **[!UICONTROL Layout]** e **[!UICONTROL Ordem das teclas de tabulação]** para a nova seção.

   Recomendamos que você selecione **[!UICONTROL 1-Coluna]** layout para o [!DNL Workfront] seção.

1. Clique em **[!UICONTROL OK]**.
1. No **[!UICONTROL Layout]** , clique em **[!UICONTROL Páginas da força de visita].**

1. Arraste e solte a **[!UICONTROL OportunidadesDaFrente DeTrabalhos]** para a nova seção na **[!UICONTROL Oportunidades]** Layout.

   Ou

   Arraste e solte a **[!UICONTROL WorkfrontAccounts]** para a nova seção na  **[!UICONTROL Conta]** Layout.\

1. Clique no botão **[!UICONTROL Propriedades]** ícone no canto superior direito do componente recém-adicionado.\

1. Para obter uma exibição ideal, especifique as seguintes propriedades para a variável [!DNL Workfront Visualforce] página:

   * **[!UICONTROL Largura (em pixels ou %)]**: 100%
   * **[!UICONTROL Altura (em pixels)]**: 600
   * Selecionar **[!UICONTROL Mostrar barras de rolagem]**.

1. Clique em **[!UICONTROL OK]**.
1. Clique em **[!UICONTROL Salvar]** para salvar o layout.

   Todos os usuários que têm esse layout atribuído a eles agora podem ver a variável [!DNL Workfront] seção sobre os [!UICONTROL Oportunidades] ou [!UICONTROL Contas] objetos.

   Os usuários veem um [!DNL Workfront] tela de logon na [!DNL Workfront] seção. Se não tiverem uma [!DNL Workfront] , eles podem recolher a seção, mas não removê-la de seu layout.

## Configure o [!DNL Workfront] na seção [!DNL Salesforce Lightning Experience] estrutura

Você pode adicionar o [!DNL Workfront] para o layout de um [!DNL Salesforce] [!UICONTROL Oportunidade] ou Conta no [!DNL Salesforce Lightning Experience] ou acessando a [!UICONTROL Configuração] ou de uma Conta ou [!UICONTROL Oportunidade] objeto.

* [Configure o [!DNL Workfront] na seção [!UICONTROL Configuração] nível](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configure o [!DNL Workfront] Seção no nível Oportunidade ou Conta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configure o [!DNL Workfront] na seção [!UICONTROL Configuração] nível {#configure-the-workfront-section-at-the-setup-level}

1. Faça logon [!DNL Salesforce] como administrador do sistema.
1. Clique no botão **[!UICONTROL Configuração]** ícone e, em seguida, clique em **[!UICONTROL Configuração]**.

1. Expandir **[!UICONTROL Objeto e campos]**, depois clique em **[!UICONTROL Gerenciador de objetos]**.

1. Clique em **[!UICONTROL Oportunidade]** para personalizar o layout de uma Oportunidade.

   Ou

   Clique em **[!UICONTROL Conta]** para personalizar o layout de uma conta.

1. Clique em **[!UICONTROL Layouts de página]**.
1. Clique no nome de um layout de página existente para editá-lo.

   Ou

   Clique em **[!UICONTROL Novo]** para criar um novo layout de página.

1. Continue com [Configure o [!DNL Workfront] Seção no nível Oportunidade ou Conta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) abaixo.

### Configure o [!DNL Workfront] Seção no nível Oportunidade ou Conta {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Faça logon em [!DNL Salesforce] como administrador do sistema.
1. Ir para um **[!UICONTROL Oportunidade]** ou **[!UICONTROL Conta]**.

1. Clique no botão **[!UICONTROL Configuração]** ícone e, em seguida, clique em **[!UICONTROL Editar página]**.\

1. Expanda o **[!UICONTROL Personalizado gerenciado]** seção.
1. Arraste e solte a **[!DNL Workfront]** no seu [!UICONTROL Oportunidade] ou página Conta.

   Recomendamos o uso da largura total da página para o [!DNL Workfront] em vez de uma das colunas do layout.

1. Clique em **[!UICONTROL Salvar]**.

   Todos os usuários que têm esse layout atribuído a eles agora podem ver a variável [!DNL Workfront] seção sobre os [!UICONTROL Oportunidades] ou [!UICONTROL Contas] objetos.

   >[!NOTE]
   >
   >Os usuários veem um [!DNL Workfront] tela de logon na [!DNL Workfront] seção. Se não tiverem uma [!DNL Workfront] , eles podem recolher a seção, mas não removê-la de seu layout. Os usuários podem fazer logon usando o método de autenticação habilitado: Autenticação aprimorada ou o URL de SAML (Security Assertion Markup Language).

