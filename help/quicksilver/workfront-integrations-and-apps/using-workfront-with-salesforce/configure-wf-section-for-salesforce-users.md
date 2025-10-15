---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Configurar a seção  [!DNL Adobe Workfront]  para  [!DNL Salesforce]  usuários
description: Depois de instalar o [!DNL Adobe Workfront] for Salesforce como administrador [!DNL Workfront] você pode disponibilizá-lo para os usuários adicionando-o em uma nova seção aos layouts das páginas Oportunidade e Conta no Salesforce.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 1%

---

# Configurar a seção [!DNL Adobe Workfront] para [!DNL Salesforce] usuários

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Salesforce não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Salesforce.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Salesforce, consulte [módulos do Salesforce](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

É necessário um Plano [!UICONTROL Pro] [!DNL Workfront] para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [[!DNL Workfront] Planos.](https://business.adobe.com/br/products/workfront/pricing.html)

Depois de instalar o [!DNL Adobe Workfront] for [!DNL Salesforce] como administrador do [!DNL Workfront], você poderá disponibilizá-lo para os seus usuários adicionando-o em uma nova seção às suas [!UICONTROL Oportunidades] e [!UICONTROL Conta]
layouts de página no [!UICONTROL Salesforce].

Para obter informações sobre como instalar o [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Para que os usuários tenham [!DNL Workfront] disponível nas estruturas [!DNL Classic] e [!DNL Lightning Experience], você deve adicionar as páginas [!DNL WorkfrontOpportunities] e [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] aos layouts de página [!UICONTROL Oportunidade] e [!UICONTROL Contas], respectivamente.

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
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

* Você deve ter uma instância [!DNL Salesforce] com acesso a uma conta de administrador do sistema.
* Você deve ter uma instância [!DNL Workfront] com acesso a uma conta de administrador do sistema.

## Configurar a seção [!DNL Workfront] na estrutura [!DNL Salesforce Classic]

1. Faça logon em [!DNL Salesforce] como administrador do Workfront.
1. Clique em **[!UICONTROL Instalação].**
1. Na seção **[!UICONTROL Build]**, expanda **[!UICONTROL Personalizar].**

1. Expanda **[!UICONTROL Oportunidades]** e clique em **[!UICONTROL Layouts de Página]** para adicionar a seção [!DNL Workfront] a uma Oportunidade.

   Ou

   Expanda **[!UICONTROL Contas]** e clique em **[!UICONTROL Layouts de Página]** para adicionar a seção [!DNL Workfront] a uma Conta
.

1. Clique em **[!UICONTROL Editar]** em um layout existente.

   Ou

   Clique em **[!UICONTROL Novo]** para adicionar um novo layout.

1. (Opcional) Arraste o componente **[!UICONTROL Seção]** para o layout e solte-o na posição desejada.\

1. (Opcional) Especifique um nome para a nova seção.

   Recomendamos que você nomeie esta seção **[!DNL Workfront]**.

1. (Opcional) Especifique o **[!UICONTROL Layout]** e a **[!UICONTROL Ordem das teclas de tabulação]** desejados para a nova seção.

   Recomendamos que você selecione o layout **[!UICONTROL 1-Coluna]** para a seção [!DNL Workfront].

1. Clique em **[!UICONTROL OK]**.
1. Na área **[!UICONTROL Layout]**, clique em **[!UICONTROL Páginas do Visualforce].**

1. Arraste e solte o componente **[!UICONTROL WorkfrontOpportunity]** para a nova seção no layout **[!UICONTROL Oportunidades]**.

   Ou

   Arraste e solte o componente **[!UICONTROL WorkfrontAccounts]** para a nova seção no layout **[!UICONTROL Conta]**.\

1. Clique no ícone **[!UICONTROL Propriedades]** na parte superior direita do componente recém-adicionado.\

1. Para obter uma exibição ideal, especifique as seguintes propriedades para a página [!DNL Workfront Visualforce]:

   * **[!UICONTROL Largura (em pixels ou %)]**: 100%
   * **[!UICONTROL Altura (em pixels)]**: 600
   * Selecione **[!UICONTROL Mostrar barras de rolagem]**.

1. Clique em **[!UICONTROL OK]**.
1. Clique em **[!UICONTROL Salvar]** para salvar seu layout.

   Todos os usuários aos quais este layout foi atribuído podem ver a seção [!DNL Workfront] em seus objetos [!UICONTROL Oportunidades] ou [!UICONTROL Contas].

   Os usuários verão uma tela de logon do [!DNL Workfront] na seção [!DNL Workfront]. Se eles não tiverem uma conta [!DNL Workfront], poderão recolher a seção, mas não removê-la do layout.

## Configurar a seção [!DNL Workfront] na estrutura [!DNL Salesforce Lightning Experience]

Você pode adicionar a seção [!DNL Workfront] ao layout de uma [!DNL Salesforce] [!UICONTROL Oportunidade] ou Conta
na estrutura [!DNL Salesforce Lightning Experience], acessando a área [!UICONTROL Configuração] ou de uma Conta
ou objeto [!UICONTROL Opportunity].

* [Configurar a seção  [!DNL Workfront]  no nível [!UICONTROL Instalação]](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Configurar a Seção  [!DNL Workfront]  no nível da Oportunidade ou da Conta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Configurar a seção [!DNL Workfront] no nível [!UICONTROL Instalação] {#configure-the-workfront-section-at-the-setup-level}

1. Entre em [!DNL Salesforce] como administrador do sistema.
1. Clique no ícone **[!UICONTROL Instalação]** e em **[!UICONTROL Instalação]**.

1. Expanda **[!UICONTROL Objeto e Campos]** e clique em **[!UICONTROL Gerenciador de Objetos]**.

1. Clique em **[!UICONTROL Oportunidade]** para personalizar o layout de uma oportunidade.

   Ou

   Clique em **[!UICONTROL Conta]** para personalizar o layout de uma Conta.

1. Clique em **[!UICONTROL Layouts de página]**.
1. Clique no nome de um layout de página existente para editá-lo.

   Ou

   Clique em **[!UICONTROL Novo]** para criar um novo layout de página.

1. Continue com [Configurar a [!DNL Workfront] Seção no nível de Oportunidade ou Conta](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) abaixo.

### Configurar a Seção [!DNL Workfront] no nível da Oportunidade ou da Conta {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Faça logon em [!DNL Salesforce] como administrador do sistema.
1. Vá para uma **[!UICONTROL Oportunidade]** ou uma **[!UICONTROL Conta]**.

1. Clique no ícone **[!UICONTROL Configuração]** e em **[!UICONTROL Editar página]**.\

1. Expanda a seção **[!UICONTROL Gerenciado de forma personalizada]**.
1. Arraste e solte o componente **[!DNL Workfront]** na sua [!UICONTROL Oportunidade] ou conta
página.

   Recomendamos o uso da largura total da página para a seção [!DNL Workfront] em vez de uma das colunas do layout.

1. Clique em **[!UICONTROL Salvar]**.

   Todos os usuários aos quais este layout foi atribuído podem ver a seção [!DNL Workfront] em seus objetos [!UICONTROL Oportunidades] ou [!UICONTROL Contas].

   >[!NOTE]
   >
   >Os usuários verão uma tela de logon do [!DNL Workfront] na seção [!DNL Workfront]. Se eles não tiverem uma conta [!DNL Workfront], poderão recolher a seção, mas não removê-la do layout. Os usuários podem fazer logon usando o método de autenticação que você ativou: Autenticação aprimorada ou o URL do SAML (Security Assertion Markup Language).

