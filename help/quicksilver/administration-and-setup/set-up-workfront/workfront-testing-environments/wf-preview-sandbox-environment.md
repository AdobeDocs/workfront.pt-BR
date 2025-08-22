---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: O  [!DNL Adobe Workfront] Ambiente de pré-visualização da sandbox
description: A sandbox de visualização é um ambiente de teste que serve como uma réplica do seu ambiente ativo. Ele é atualizado todos os finais de semana pelo Workfront. Os dados adicionados ao seu ambiente ativo na sexta-feira aparecem em sua sandbox de visualização na segunda-feira seguinte. Todos os pacotes de suporte têm acesso a esta sandbox.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: d2dd148c8b7a08f4ea9a13e325a33f753eea2d7d
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# O Ambiente de Sandbox de Visualização [!DNL Adobe Workfront]

<!-- Audited: 12/2023 -->

Há dois ambientes de teste para [!DNL Workfront] que são réplicas do seu ambiente de produção [!DNL Workfront]:

* A sandbox de visualização

  A sandbox de visualização é um ambiente de teste que serve como uma réplica do seu ambiente ativo e é atualizado todos os finais de semana por [!DNL Workfront]. Os dados adicionados ao seu ambiente ativo na sexta-feira aparecem em sua sandbox de visualização na segunda-feira seguinte.

  Todos os pacotes de suporte têm acesso à sandbox de visualização.

* A sandbox de atualização personalizada

  A sandbox de atualização personalizada é um ambiente de teste separado que é atualizado manualmente por você. Há um custo adicional para obter a sandbox de atualização personalizada. Para obter mais informações sobre este ambiente, consulte [O [!DNL Adobe Workfront] ambiente de Sandbox de Atualização Personalizada](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Padrão] Pacote de Suporte</strong> </p> </th> 
   <th> <p>Pacotes de Suporte <strong>[!UICONTROL Plus], [!UICONTROL Preferencial] e [!UICONTROL Empresa]</strong> </p> </th> 
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

Os dados fluem de forma unidirecional, da Produção para a Pré-visualização, e não invertida. Uma atualização do ambiente de Visualização é sempre agendada por [!DNL Workfront] a cada fim de semana.

A Pré-visualização de Sandbox também permite que o [!DNL Workfront] implante novos recursos em um ambiente seguro, antes que eles estejam prontos para serem implantados em produção. Você pode testar os novos recursos e fornecer feedback de [!DNL Workfront] sobre suas funcionalidades acessando a Sandbox de Visualização. Por esse motivo, o código da sandbox de visualização está sempre à frente do código de produção, embora os dados sejam atualizados semanalmente.

O ambiente de visualização é ideal para executar treinamentos, testar novos recursos e determinar a funcionalidade de configuração.

>[!NOTE]
>
>Ao acessar a Visualização da sandbox, observe o banner azul na parte superior da tela. O banner não pode ser removido enquanto você estiver trabalhando neste ambiente.
>
>O nome do ambiente que você está acessando (Pré-visualização) e a versão de lançamento do código são exibidos no banner. Clique em **[!UICONTROL Ver novidades]** para obter informações sobre essa versão.
>
>![Banner de visualização](assets/preview-banner-nwe-350x161.png)

## Acesso à sandbox de visualização

Por padrão, como administrador [!DNL Workfront], você tem acesso ao ambiente de sandbox [!UICONTROL Preview]. Se você não conseguir acessar o ambiente de Sandbox [!UICONTROL Pré-visualização] conforme descrito nesta seção, entre em contato com o administrador do [!DNL Workfront] ou com a nossa equipe de Suporte ao Cliente.


### Acessando a Sandbox de Visualização da Interface [!DNL Workfront] {#accessing-the-preview-sandbox-from-the-workfront-interface}

Como administrador [!DNL Workfront], você pode acessar a Sandbox de Visualização pela interface [!DNL Workfront].

Para acessar a sandbox de visualização:

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Sistema]** > **[!UICONTROL Preferências]**.

1. Na seção **[!UICONTROL Ambientes de Teste]**, clique em **[!UICONTROL Visualização de Sandbox]**.

1. Faça logon com as credenciais de Visualização.

   Elas devem ser iguais às suas credenciais de produção, a menos que você as tenha alterado na Produção após a atualização da Visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.

### Acesso à sandbox de visualização usando um URL {#accessing-the-preview-sandbox-using-a-url}

Você pode acessar a sandbox de visualização usando um URL.

#### Acesso à sandbox de visualização para contas no cluster 1, 2, 3 e 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

A URL para a Sandbox de Visualização é: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Se você tiver marcadores vinculados ao URL antigo da sandbox de visualização, anote essa alteração e atualize o URL em seus marcadores.

Para fazer logon na sandbox de visualização usando um URL:

1. Navegue até esta URL: `https://companyname.preview.workfront.com/`.

   Se você for um cliente EMEA e sua conta estiver no Cluster 4, consulte a seção Acesso à sandbox de visualização para contas no Cluster 4 (contas EMEA) abaixo.

1. Faça logon usando as credenciais de Visualização.

   >[!TIP]
   >
   >Suas credenciais de Visualização devem ser as mesmas que suas credenciais de produção, a menos que você as tenha alterado na Produção após a atualização da Visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.


#### Acesso à sandbox de visualização para contas no cluster 4 (contas EMEA) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

Para fazer logon na sandbox de visualização usando um URL:

1. Navegue até esta URL: `https://companyname.preview.workfront.com/`.

   Você também pode acessar a Área Restrita de Visualização acessando [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Faça logon usando as credenciais de Visualização.

   Suas credenciais de Visualização devem ser as mesmas que suas credenciais de produção, a menos que você as tenha alterado na Produção após a atualização da Visualização. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.

## Recebimento de emails da sandbox de visualização

O Workfront desativa todas as comunicações por email do ambiente Visualizar sandbox. Se você quiser receber notificações por email do ambiente Visualizar sandbox, será necessário habilitar essa funcionalidade nas configurações do usuário. Para obter mais informações sobre como ativar notificações por email no ambiente Visualização da sandbox, consulte [Habilitar a entrega de emails do ambiente Visualização da sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>O delivery de relatórios e as notificações por push no aplicativo móvel estão sempre desativados para o ambiente Visualização da sandbox. Nem você nem o administrador do [!DNL Workfront] podem habilitar a entrega de relatórios ou notificações por push para o aplicativo móvel quando você acessa o ambiente Visualizar Sandbox.
>
>Para obter mais informações sobre entregas de relatórios para o ambiente de produção, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Acesso simples (SSO)

Se você estiver usando o SSO, trabalhe com nossa equipe de Suporte ao Cliente para garantir que ele esteja configurado corretamente e que você possa usar suas credenciais de SSO para fazer logon na Sandbox [!UICONTROL Pré-visualização]. Se seu login inicial falhar, contate seu contato de suporte regular ou o administrador do [!DNL Workfront] para obter assistência.

Para obter mais informações sobre Logon Único, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Configuração do logon único na sandbox de visualização

>[!IMPORTANT]
>
>O procedimento descrito nesta seção foi removido porque se aplicou apenas a organizações que ainda não foram integradas ao Adobe Admin Console.
>
>Todas as organizações da Workfront foram integradas à Adobe Admin Console.

<!--DELETE THIS SECTION MARCH 2026-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the [!DNL Adobe Admin Console]. If your organization has been onboarded to the [!DNL Adobe Admin Console], no action is necessary.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the [!DNL Adobe Admin Console], see [Platform-based administration differences ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


If you want to configure your Preview Sandbox to work with a Single Sign-On solution, you can do so by configuring it separately from your Production environment. The SSO configuration in the Preview Sandbox is independent from your SSO configuration in the Production environment.

When your Preview Sandbox refreshes (every weekend), the SSO information is not copied from your Production environment to overwrite the Preview Sandbox configuration.

The steps for configuring single sign-on in the Preview Sandbox are similar to those for configuring it in the Production environment.

For more information about configuring [!DNL Workfront] with SSO, see [Overview of single sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).-->

## Recálculo automático de linhas de tempo do projeto

Recalcular linhas do tempo permite que os gerentes vejam como as forças fora do projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto se refere às datas planejadas e projetadas para o projeto.

Como administrador do Workfront, você pode configurar quando o Workfront recalcula automaticamente as linhas do tempo do projeto. O Workfront pode recalcular as linhas do tempo do projeto todas as noites, quando o escopo do projeto mudar, ou ambos.

Para obter informações, consulte [Configurar recálculos de linha de tempo para projetos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para o ambiente de Pré-visualização, o recálculo noturno é desativado e as linhas de tempo do projeto não são recalculadas automaticamente. Você deve recalcular manualmente a linha do tempo do projeto para o ambiente de Pré-visualização. Para obter informações, consulte [Recalcular linhas do tempo do projeto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Pré-visualizar o desempenho e a disponibilidade do ambiente

* Os ambientes de visualização do [!DNL Workfront] não se destinam a testes de desempenho ou carga. Em vez disso, use esses ambientes para validar a funcionalidade do recurso com os fluxos de trabalho existentes da organização.

* Os fluxos de trabalho envolvendo documentos devem se concentrar no processo e não no teste de carga. Arquivos grandes não são suportados em ambientes de sandbox.

* [!DNL Workfront] Os ambientes de visualização devem estar sempre disponíveis.

* Qualquer interrupção em um ambiente de Visualização do [!DNL Workfront] durante o horário comercial regular será uma prioridade imediatamente após a resolução de quaisquer problemas de Produção, se houver.

* Qualquer interrupção em um ambiente de Visualização do [!DNL Workfront] nos finais de semana (sábados e domingos) será resolvida para que o ambiente funcione durante o horário comercial na segunda-feira.
