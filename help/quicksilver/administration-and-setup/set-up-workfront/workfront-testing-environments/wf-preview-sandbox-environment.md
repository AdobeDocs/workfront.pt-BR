---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: A variável [!DNL Adobe Workfront] Visualizar ambiente de sandbox
description: A sandbox de visualização é um ambiente de teste que serve como uma réplica do seu ambiente ativo. Ele é atualizado todos os finais de semana pelo Workfront. Os dados adicionados ao seu ambiente ativo na sexta-feira aparecem em sua sandbox de visualização na segunda-feira seguinte. Todos os pacotes de suporte têm acesso a esta sandbox.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 616bca509b87fbd746132c2eeb5130e0b7789c47
workflow-type: tm+mt
source-wordcount: '1282'
ht-degree: 0%

---

# A variável [!DNL Adobe Workfront] Visualizar ambiente de sandbox

Existem dois ambientes de teste para [!DNL Workfront] que são réplicas do seu [!DNL Workfront] ambiente de produção:

* A sandbox de visualização

   A sandbox de visualização é um ambiente de teste que serve como uma réplica do seu ambiente ativo e é atualizado todos os finais de semana pela [!DNL Workfront]. Os dados adicionados ao seu ambiente ativo na sexta-feira aparecem em sua sandbox de visualização na segunda-feira seguinte.

   Todos os pacotes de suporte têm acesso à sandbox de visualização.

* A sandbox de atualização personalizada

   A sandbox de atualização personalizada é um ambiente de teste separado que é atualizado manualmente por você. Há um custo adicional para obter a sandbox de atualização personalizada. Para obter mais informações sobre esse ambiente, consulte [A variável [!DNL Adobe Workfront] Ambiente de sandbox de atualização personalizada](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Pacote de Suporte do [!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>Pacotes de Suporte do [!UICONTROL Plus], [!UICONTROL Preferencial] e [!UICONTROL Enterprise]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Visualizar sandbox</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Sandbox de atualização personalizada</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Visualizar sandbox

A sandbox de visualização serve como um ambiente em que os usuários em sua organização podem testar e trabalhar com dados do ambiente de produção com segurança, sem afetar o ambiente de produção.

A Sandbox de visualização contém seus dados reais de produção; no entanto, é atualizada todos os finais de semana para que os dados possam estar até uma semana atrás do ambiente de produção. Os itens criados desde a última atualização estão no ambiente Visualização da sandbox até a atualização seguinte.

Os dados fluem de forma unidirecional, da Produção para a Pré-visualização, e não invertida. Uma atualização do ambiente de Visualização é sempre agendada por [!DNL Workfront] cada fim de semana.

A pré-visualização de sandbox também permite [!DNL Workfront] para implantar novos recursos em um ambiente seguro, antes que eles estejam prontos para serem implantados na produção. Você pode testar os novos recursos e fornecer [!DNL Workfront] feedback sobre a funcionalidade acessando a sandbox de visualização. Por esse motivo, o código da sandbox de visualização está sempre à frente do código de produção, embora os dados sejam atualizados semanalmente.

O ambiente de visualização é ideal para executar treinamentos, testar novos recursos e determinar a funcionalidade de configuração.

>[!NOTE]
>
>Ao acessar a Visualização da sandbox, observe o banner azul na parte superior da tela. O banner não pode ser removido enquanto você estiver trabalhando neste ambiente.
>
>O nome do ambiente que você está acessando (Pré-visualização) e a versão de lançamento do código são exibidos no banner. Clique em **[!UICONTROL Veja as novidades]** para obter informações sobre essa versão.
>
>![](assets/preview-banner-nwe-350x161.png)

## Acesso à sandbox de visualização

Por padrão, como um [!DNL Workfront] administrador, você tem acesso ao [!UICONTROL Visualizar] Ambiente de sandbox. Se não conseguir acessar o [!UICONTROL Visualizar] Ambiente de sandbox conforme descrito nesta seção, entre em contato com o [!DNL Workfront] administrador ou nossa equipe de Suporte ao cliente.

* [Acessar a sandbox de visualização no [!DNL Workfront] Interface](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [Acesso à sandbox de visualização usando um URL](#accessing-the-preview-sandbox-using-a-url)

### Acessar a sandbox de visualização no [!DNL Workfront] Interface {#accessing-the-preview-sandbox-from-the-workfront-interface}

Como um [!DNL Workfront] administrador, você poderá acessar a Visualização da sandbox usando a [!DNL Workfront] interface.

Para acessar a sandbox de visualização:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront]e, em seguida, clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Sistema]** > **[!UICONTROL Preferências]**.

1. No **[!UICONTROL Ambientes de teste]** clique em **[!UICONTROL Visualização da sandbox]**.

1. Faça logon com as credenciais de Visualização.

   Elas devem ser iguais às suas credenciais de produção, a menos que você as tenha alterado na Produção após a atualização da Visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.

### Acesso à sandbox de visualização usando um URL {#accessing-the-preview-sandbox-using-a-url}

* [Acesso à sandbox de visualização para contas no cluster 1, 2, 3 e 5](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [Acesso à sandbox de visualização para contas no cluster 4 (contas EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### Acesso à sandbox de visualização para contas no cluster 1, 2, 3 e 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Historicamente, você acessou a opção Visualizar sandbox acessando [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

Este URL não é mais suportado e não foi redirecionado para o nosso novo URL para o ambiente Visualização da sandbox. O novo URL correto para a sandbox de visualização é: [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>Se você tiver marcadores vinculados ao URL antigo da sandbox de visualização, anote essa alteração e atualize o URL em seus marcadores.

Para fazer logon na sandbox de visualização usando um URL:

1. Navegue até este URL: [[!DNL https]://companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   Se você for um cliente EMEA e sua conta estiver no Cluster 4, consulte a seção [Acesso à sandbox de visualização para contas no cluster 4 (contas EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) neste artigo.

1. Faça logon usando as credenciais de Visualização.

   Suas credenciais de Visualização devem ser as mesmas que suas credenciais de produção, a menos que você as tenha alterado na Produção após a atualização da Visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.

#### Acesso à sandbox de visualização para contas no cluster 4 (contas EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Para fazer logon na sandbox de visualização usando um URL:

1. Navegue até este URL: `https://companyname.preview.workfront.com/`.

   Você também pode acessar a opção Visualizar sandbox acessando [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Faça logon usando as credenciais de Visualização.

   Suas credenciais de Visualização devem ser as mesmas que suas credenciais de produção, a menos que você as tenha alterado na Produção após a atualização da Visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.

## Recebimento de emails da sandbox de visualização

O Workfront desativa todas as comunicações por email do ambiente Visualizar sandbox. Se você quiser receber notificações por email do ambiente Visualizar sandbox, será necessário habilitar essa funcionalidade nas configurações do usuário. Para obter mais informações sobre como ativar notificações por email no ambiente Visualização da sandbox, consulte [Ativar a entrega de emails do ambiente Visualização da sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>O delivery de relatórios e as notificações por push no aplicativo móvel estão sempre desativados para o ambiente Visualização da sandbox. Nem você nem o [!DNL Workfront] O administrador pode habilitar a entrega de relatórios ou notificações por push para o aplicativo móvel quando você acessar o ambiente Visualizar sandbox.
>
>Para obter mais informações sobre deliveries de relatórios para o ambiente de produção, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Acesso simples (SSO)

Se você estiver usando o SSO, trabalhe com nossa equipe de Suporte ao cliente para garantir que ele esteja configurado corretamente para que você possa usar suas credenciais de SSO para fazer logon na [!UICONTROL Visualizar] Sandbox. Se seu login inicial falhar, entre em contato com seu contato de suporte regular ou [!DNL Workfront] administrador para obter assistência.

Para obter mais informações sobre o Logon único, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configuração do logon único na sandbox de visualização

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas na [!DNL Adobe Admin Console]. Se sua organização foi integrada à [!DNL Adobe Admin Console], nenhuma ação é necessária.
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à [!DNL Adobe Admin Console], consulte [Diferenças de administração baseadas em plataforma ([!UICONTROL Adobe Workfront]/[!UICONTROL Plataforma comercial Adobe])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Se você quiser configurar sua sandbox de visualização para funcionar com uma solução de logon único, faça isso configurando-a separadamente do ambiente de produção. A configuração de SSO na sandbox de visualização é independente da sua configuração de SSO no ambiente de produção.

Quando a sandbox de visualização é atualizada (todos os finais de semana), as informações de SSO não são copiadas do ambiente de produção para substituir a configuração da sandbox de visualização.

As etapas para configurar o logon único na Sandbox de visualização são semelhantes àquelas para configurá-lo no ambiente de Produção.

Para obter mais informações sobre a configuração [!DNL Workfront] com SSO, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Pré-visualizar o desempenho e a disponibilidade do ambiente

[!DNL Workfront] Os ambientes de visualização não se destinam a testes de desempenho ou carga. Em vez disso, use esses ambientes para validar a funcionalidade do recurso com os fluxos de trabalho existentes da organização.

[!DNL Workfront] Os ambientes de visualização devem estar sempre disponíveis.

Qualquer interrupção em um [!DNL Workfront] O ambiente de visualização durante o horário comercial regular será a primeira prioridade imediatamente após a resolução de qualquer problema de produção, se houver.

Qualquer interrupção em um [!DNL Workfront] O ambiente de visualização nos finais de semana (sábados e domingos) será tratado para que o ambiente esteja em execução durante o horário comercial na segunda-feira.
