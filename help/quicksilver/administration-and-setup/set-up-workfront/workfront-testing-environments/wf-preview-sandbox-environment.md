---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: O [!DNL Adobe Workfront] Visualizar ambiente do Sandbox
description: A sandbox de visualização é um ambiente de teste que serve como réplica do ambiente ativo. É atualizado todos os fins de semana pelo Workfront. Os dados adicionados ao seu ambiente ativo na sexta-feira serão exibidos em sua sandbox de visualização na segunda-feira seguinte. Todos os pacotes de suporte têm acesso a essa sandbox.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# O [!DNL Adobe Workfront] Visualizar ambiente do Sandbox

Há dois ambientes de teste para [!DNL Workfront] que são réplicas de seus [!DNL Workfront] ambiente de produção:

* A sandbox de visualização

   A sandbox de visualização é um ambiente de teste que serve como réplica do ambiente ativo e é atualizado a cada fim de semana por [!DNL Workfront]. Os dados adicionados ao seu ambiente ativo na sexta-feira serão exibidos em sua sandbox de visualização na segunda-feira seguinte.

   Todos os pacotes de suporte têm acesso à sandbox de visualização.

* Sandbox de atualização personalizada

   A Sandbox de atualização personalizada é um ambiente de teste separado, que é atualizado manualmente por você. Há um custo adicional para obter a Caixa de proteção de atualização personalizada. Para obter mais informações sobre esse ambiente, consulte [O [!DNL Adobe Workfront] Ambiente de sandbox de atualização personalizada](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>Pacote de suporte do [!UICONTROL Standard]</strong> </p> </th> 
   <th> <p><strong>Pacotes de suporte da [!UICONTROL Plus], da [!UICONTROL Preferencial] e da [!UICONTROL Enterprise]</strong> </p> </th> 
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

A Sandbox de visualização serve como um ambiente em que os usuários em sua organização podem testar e trabalhar com dados com segurança do ambiente de produção, sem afetar o ambiente de produção.

A sandbox de visualização contém seus dados de produção reais; no entanto, ele é atualizado todos os finais de semana para que os dados possam estar até uma semana atrás do ambiente de produção. Os itens criados desde o último tempo de atualização estão no ambiente Preview Sandbox até a atualização a seguir.

Fluxos de dados de forma unidirecional, de Produção para Visualização, e não ao contrário. Uma atualização do ambiente de Visualização é sempre agendada por [!DNL Workfront] todo fim de semana. Para obter mais informações sobre o dia e a hora específicos da atualização, acesse [status.adobe.com](https://status.adobe.com/pt/).

Visualizar sandbox também permite [!DNL Workfront] para implantar novos recursos em um ambiente seguro, antes que eles estejam prontos para serem implantados em produção. Você pode testar os novos recursos e fornecer [!DNL Workfront] feedback sobre a funcionalidade ao acessar a sandbox de visualização. Por isso, o código da sandbox de visualização está sempre à frente do código de produção, embora seus dados sejam atualizados semanalmente.

O ambiente de visualização é ideal para executar treinamentos, testar novos recursos e determinar a funcionalidade de configuração.

>[!NOTE]
>
>Ao acessar a sandbox de visualização, observe o banner azul na parte superior da tela. O banner não pode ser removido enquanto você estiver trabalhando neste ambiente.
>
>O nome do ambiente que você está acessando (Visualização) e a versão de lançamento do código são exibidos no banner. Clique em **[!UICONTROL Veja as novidades]** para obter informações sobre essa versão.
>
>![](assets/preview-banner-nwe-350x161.png)

## Acessar o sandbox de visualização

Por padrão, como um [!DNL Workfront] administrador, você tem acesso ao [!UICONTROL Visualizar] Ambiente de sandbox. Se não conseguir acessar o [!UICONTROL Visualizar] Ambiente do Sandbox conforme descrito nesta seção, entre em contato com seu [!DNL Workfront] administrador ou a equipe de Suporte ao cliente.

* [Acessar o sandbox de visualização a partir do [!DNL Workfront] Interface](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [Acessar o sandbox de visualização usando um URL](#accessing-the-preview-sandbox-using-a-url)

### Acessar o sandbox de visualização a partir do [!DNL Workfront] Interface {#accessing-the-preview-sandbox-from-the-workfront-interface}

Como um [!DNL Workfront] administrador, você pode acessar a sandbox de visualização por meio da [!DNL Workfront] interface.

Para acessar a sandbox de visualização:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Sistema]** > **[!UICONTROL Preferências]**.

1. No **[!UICONTROL Testar ambientes]** seção , clique em **[!UICONTROL Visualização do Sandbox]**.

1. Faça logon com as credenciais de Visualização.

   Elas devem ser iguais às credenciais de produção, a menos que você as tenha alterado em Produção após a atualização da Pré-visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não sincronizam automaticamente.

### Acessar o sandbox de visualização usando um URL {#accessing-the-preview-sandbox-using-a-url}

* [Acessar o sandbox de visualização para contas no cluster 1, 2, 3 e 5](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [Acessar o sandbox de visualização para contas no cluster 4 (contas EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### Acessar o sandbox de visualização para contas no cluster 1, 2, 3 e 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Historicamente, você acessou a sandbox de visualização ao acessar [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

Esse URL não é mais suportado e não foi redirecionado para o novo URL do ambiente Preview Sandbox. O novo URL correto para a sandbox de visualização é: [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>Se você tinha marcadores vinculando ao URL antigo da sandbox de visualização, anote essa alteração e atualize o URL dos marcadores.

Para fazer logon na sandbox de visualização usando um URL:

1. Navegue até este URL: [[!DNL https]://companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   Se você for um cliente EMEA e sua conta estiver no Cluster 4, consulte a seção [Acessar o sandbox de visualização para contas no cluster 4 (contas EMEA)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) neste artigo.

1. Faça logon usando suas credenciais de Visualização.

   Suas credenciais de Pré-visualização devem ser iguais às credenciais de produção, a menos que você as tenha alterado em Produção após a atualização de Pré-visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não sincronizam automaticamente.

#### Acessar o sandbox de visualização para contas no cluster 4 (contas EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Para fazer logon na sandbox de visualização usando um URL:

1. Navegue até este URL: `https://companyname.preview.workfront.com/`.

   Você também pode acessar a caixa de proteção de visualização acessando [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Faça logon usando suas credenciais de Visualização.

   Suas credenciais de Pré-visualização devem ser iguais às credenciais de produção, a menos que você as tenha alterado em Produção após a atualização de Pré-visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não sincronizam automaticamente.

## Recebendo emails da sandbox de visualização

O Workfront desativa todas as comunicações por email do ambiente Preview Sandbox. Se quiser receber notificações por email do ambiente Preview Sandbox, ative essa funcionalidade nas configurações do usuário. Para obter mais informações sobre como ativar notificações por email no ambiente Preview Sandbox, consulte [Ativar a entrega de emails do ambiente Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>A entrega de relatórios e as notificações por push no aplicativo móvel ficam sempre desativadas no ambiente de sandbox de visualização. Nem você nem o [!DNL Workfront] o administrador pode ativar o delivery de relatórios ou notificações por push para o aplicativo móvel ao acessar o ambiente Preview Sandbox .
>
>Para obter mais informações sobre deliveries de relatórios para o ambiente de produção, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Acesso simples (SSO)

Se você estiver usando o SSO, trabalhe com a equipe de Suporte ao cliente para garantir que ele esteja configurado corretamente, de modo que você possa usar suas credenciais do SSO para fazer logon no [!UICONTROL Visualizar] Sandbox. Se o logon inicial falhar, entre em contato com o suporte normal ou [!DNL Workfront] para obter assistência.

Para obter mais informações sobre Logon único, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configuração do logon único na sandbox de visualização

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente às organizações que ainda não foram integradas à variável [!DNL Adobe Admin Console]. Se sua organização tiver sido integrada à [!DNL Adobe Admin Console], nenhuma ação é necessária.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à [!DNL Adobe Admin Console], consulte [Diferenças de administração baseadas em plataforma ([!UICONTROL Adobe Workfront]/[!UICONTROL Plataforma Adobe Business])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Se você quiser configurar a sandbox de visualização para funcionar com uma solução de logon único, é possível fazer isso configurando-a separadamente do ambiente de Produção. A configuração do SSO na sandbox de visualização é independente da configuração do SSO no ambiente de produção.

Quando a Caixa de proteção de visualização é atualizada (a cada fim de semana), as informações do SSO não são copiadas do ambiente de Produção para substituir a configuração da Caixa de proteção de visualização.

As etapas para configurar o logon único na sandbox de visualização são semelhantes àquelas para configurá-la no ambiente de Produção.

Para obter mais informações sobre como configurar [!DNL Workfront] com SSO, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Visualizar o desempenho e a disponibilidade do ambiente

[!DNL Workfront] Os ambientes de visualização não são destinados a testes de desempenho ou carga. Em vez disso, use esses ambientes para validar a funcionalidade do recurso com os fluxos de trabalho existentes de sua organização.

[!DNL Workfront] Os ambientes de visualização devem estar sempre disponíveis.

Qualquer interrupção para um [!DNL Workfront] O ambiente de visualização durante o horário comercial normal será uma primeira prioridade imediatamente após qualquer problema de Produção ser resolvido, caso exista.

Qualquer interrupção para um [!DNL Workfront] O ambiente de visualização nos finais de semana (sábados e domingos) será endereçado para que o ambiente esteja funcionando para o horário comercial na segunda-feira.
