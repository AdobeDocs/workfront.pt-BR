---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: O  [!DNL Adobe Workfront] Ambiente de Sandbox de Atualização Personalizada
description: A sandbox de atualização personalizada é um ambiente em que você pode testar e trabalhar usando dados de seu ambiente de produção. Também é ideal para executar treinamentos e determinar a funcionalidade de configuração.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 7549c9699a86b6f87e5562efd7e586be282c5619
workflow-type: tm+mt
source-wordcount: '1763'
ht-degree: 0%

---

# O ambiente de sandbox de atualização personalizada do [!DNL Adobe Workfront]

A sandbox de atualização personalizada é um ambiente em que você pode testar e trabalhar usando dados de seu ambiente de produção. Também é ideal para executar treinamentos e determinar a funcionalidade de configuração.

>[!NOTE]
>
>Isso é diferente da sandbox de visualização, que também é um ambiente de teste que replica seu ambiente de produção [!DNL Workfront].
>
>* Os novos recursos são introduzidos na Sandbox de visualização antes de serem disponibilizados na produção.
>* Os novos recursos não são introduzidos na Sandbox de atualização personalizada antes de serem disponibilizados na produção.
>
>  Além disso, há um custo adicional para obter a sandbox de atualização personalizada que não é necessária para a sandbox de visualização.
>
>  Para obter mais informações sobre a Visualização da sandbox, consulte [O [!DNL Adobe Workfront] Ambiente de Visualização da Sandbox](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] plano</td> 
   <td> <p>[!UICONTROL Business] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] licença</p> </td> 
   <td> <p>[!UICONTROL Plano] </p> <p>Você deve ser um administrador [!DNL Workfront]. Para obter informações sobre administradores do [!DNL Workfront], consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pacote de suporte</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferencial] ou [!UICONTROL Enterprise]</p> <p>O pacote de suporte padrão não tem acesso à sandbox de atualização personalizada, mas tem acesso à sandbox de visualização.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Atualização da sandbox de atualização personalizada

A Sandbox de atualização personalizada contém seus dados reais de produção e não é atualizada até que você a programe para fazê-lo. Você pode programar uma atualização a qualquer momento que lhe for conveniente, com a mesma frequência de uma vez por semana.

>[!NOTE]
>
>* Você não pode programar uma atualização para o dia atual. Por exemplo, se hoje for 1º de junho, o primeiro dia em que você pode programar uma atualização será 2 de junho.
>* A atualização programada ocorre em algum momento durante a noite, com base no cluster do usuário (os clusters dos EUA são atualizados durante a noite nos EUA). O horário específico é imprevisível devido a outros clientes na fila e à quantidade de dados que são atualizados. Se a fila tiver muitos clientes grandes, a atualização pode não ser executada até mais tarde naquele dia ou no dia seguinte.
>* Sua sandbox de atualização personalizada sempre tem os mesmos recursos de produto que seu ambiente de produção. No entanto, quando você atualiza a Sandbox de atualização personalizada, ela preserva a identidade visual somente para a cor de fundo da tela de logon. Os logotipos da tela de logon e da barra de navegação são redefinidos para os padrões [!DNL Workfront], e as imagens de marca modificadas antes da atualização não são exibidas.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Acesse a sandbox de atualização personalizada a partir do ambiente de produção {#access-the-custom-refresh-sandbox-from-your-production-environment}

Como administrador do [!DNL Workfront], você pode acessar sua Sandbox de atualização personalizada no seu ambiente de produção.

>[!NOTE]
>
>Se sua conta estiver no Cluster 4 (Cluster EMEA), você não poderá acessar sua Sandbox de atualização personalizada no Ambiente de produção. Para obter mais informações sobre como acessar sua Sandbox de Atualização Personalizada quando tiver uma conta no Cluster 4, consulte [Acessar a Sandbox de Atualização Personalizada para Contas no Cluster 4 (Contas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Acessar a Sandbox de Atualização Personalizada para Contas no Cluster 4 (Contas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Para acessar sua sandbox de atualização personalizada:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Ícone do menu principal](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront] e clique no ícone **[!UICONTROL Configuração]** ![Configurações de engrenagem](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Sistema]** >**[!UICONTROL Preferências]**.

1. Na seção **[!UICONTROL Ambiente de Teste]**, clique em **[!UICONTROL Sandbox 1]** ou **[!UICONTROL Sandbox 2]**.

   Seu pacote de suporte especifica se você tem acesso a uma ou duas sandboxes de atualização personalizada.

1. Faça logon usando suas credenciais da Sandbox de atualização personalizada.

   Suas credenciais de sandbox de atualização personalizada são as mesmas de sua produção, a menos que você tenha alterado suas credenciais de produção desde a última atualização de sua sandbox de atualização personalizada. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.

   A sandbox de atualização personalizada mostra a versão, bem como a data da última atualização no banner na parte superior da tela. Todas as informações da produção estão disponíveis e prontas para uso após a conclusão de uma atualização.

## Acesse a sandbox de atualização personalizada usando um URL {#access-the-custom-refresh-sandbox-using-a-url}

Qualquer usuário pode acessar a Sandbox de atualização personalizada usando um URL.

* [Acesse a sandbox de atualização personalizada para contas nos clusters 1, 2, 3 e 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Acesse a sandbox de atualização personalizada para contas no cluster 4 (contas da EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Acesse a sandbox de atualização personalizada para contas nos clusters 1, 2, 3 e 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Dependendo do seu pacote de Suporte, você deve ter acesso a uma ou duas Sandboxes de Atualização Personalizada.

Para acessar sua sandbox de atualização personalizada usando um URL:

1. Navegue até este URL se você tiver apenas uma Sandbox de Atualização Personalizada:

   `https://companyname.sb01.workfront.com` (URL antiga:`https://cr1.attasksandbox.com/`.)

   Ou Se você tiver duas Sandboxes de Atualização Personalizada, além das URLs acima, você também poderá acessar a seguinte URL para acessar sua segunda Sandbox de Atualização Personalizada:

   `https://companyname.sb02.workfront.com` (URL antiga:`https://cr2.attasksandbox.com/`)

1. Na tela de logon, faça logon usando as credenciais da Sandbox de atualização personalizada.
1. Suas credenciais de Sandbox de atualização personalizada são as mesmas de suas credenciais de produção, a menos que você tenha alterado suas credenciais de produção desde que sua Sandbox de atualização personalizada foi atualizada pela última vez. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.

### Acesse a sandbox de atualização personalizada para contas no cluster 4 (contas da EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Se sua conta do [!DNL Workfront] estiver no Cluster 4 (cluster EMEA), você poderá acessar sua Sandbox de Atualização Personalizada apenas usando uma URL. Para descobrir em qual cluster está sua conta, entre em contato com nossa equipe de Suporte ao cliente.

Dependendo do seu pacote de Suporte, você deve ter acesso a uma ou duas Sandboxes de Atualização Personalizada.

Para acessar sua sandbox de atualização personalizada usando um URL:

1. Navegue até este URL se você tiver apenas uma Sandbox de Atualização Personalizada:

   `https://companyname.sb01.workfront.com` (URL antiga:`https://cr3.attasksandbox.com`)

   Ou

   Vá para um desses URLs se você tiver duas Sandboxes de Atualização Personalizada:

   `https://companyname.sb01.workfront.com` (URL antiga:`https://cr3.attasksandbox.com`)

   `https://companyname.sb02.workfront.com` (URL antiga:`https://cr4.attasksandbox.com`)

1. Na tela de logon, faça logon usando as credenciais da Sandbox de atualização personalizada.

   Suas credenciais de Sandbox de atualização personalizada são as mesmas de suas credenciais de produção, a menos que você tenha alterado suas credenciais de produção desde que sua Sandbox de atualização personalizada foi atualizada pela última vez. Os logons são sincronizados somente quando ocorre uma atualização. Eles não são sincronizados automaticamente.

## Agendar uma atualização da Sandbox de Atualização Personalizada

>[!IMPORTANT]
>
>A duração da atualização depende do tamanho dos dados que estão sendo atualizados. Durante o processo de atualização, é essencial que o ambiente personalizado da sandbox de atualização não esteja sendo usado de nenhuma maneira (incluindo chamadas e integrações de API), pois isso impedirá que a atualização da sandbox seja concluída com êxito. O [!DNL Workfront] desabilitará o ambiente de sandbox de atualização personalizada antes de ele começar, mas você deve encerrar todas as sessões ativas para garantir que a atualização da sandbox seja bem-sucedida.

Depois de agendar uma atualização da Sandbox de Atualização Personalizada, você pode cancelá-la clicando em [!UICONTROL Cancelar] na parte superior da página. Você também pode reagendá-lo para um momento posterior.

>[!NOTE]
>
>Não é possível programar atualizações automáticas de sandbox.

Para agendar uma atualização da Sandbox de atualização do cliente:

1. Faça logon na Sandbox de atualização personalizada.
1. Clique em **[!UICONTROL Agendar]** no banner na parte superior da tela e selecione uma data no calendário.
1. Selecione uma data para quando quiser que a atualização ocorra e clique em **[!UICONTROL Agendar Atualização]**.

## Alterne para Produção da Sandbox de Atualização Personalizada

1. Faça logon na Sandbox de atualização personalizada.

   Para obter mais informações sobre como acessar sua Sandbox de Atualização Personalizada, consulte [Acessar a Sandbox de Atualização Personalizada de seu ambiente de Produção](#access-the-custom-refresh-sandbox-from-your-production-environment) ou [Acessar a Sandbox de Atualização Personalizada usando uma URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Clique em **[!UICONTROL Ir para produção]** no banner na parte superior da tela.

   Lembre-se de que o trabalho realizado na sandbox não estará visível no ambiente [!UICONTROL produção], pois a transferência de dados é unidirecional, da produção para a sandbox de atualização personalizada, e não invertido.

## Receber emails da Sandbox de atualização personalizada

[!DNL Workfront] desabilita todas as comunicações por email do ambiente de Sandbox de Atualização Personalizada. Se você quiser receber notificações por email do ambiente Personalizar atualização da sandbox, será necessário habilitar essa funcionalidade nas configurações do usuário. Para obter mais informações sobre como ativar notificações por email no ambiente Personalizado da Sandbox de Atualização, consulte [Habilitar a entrega de emails do ambiente Visualização da Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>O delivery de relatórios e as notificações por push no aplicativo móvel estão sempre desativados para o ambiente sandbox de atualização personalizada. Nem você nem o administrador do [!DNL Workfront] podem habilitar a entrega de relatórios ou notificações por push para o aplicativo móvel quando você acessa o ambiente de sandbox de atualização personalizada.\
>Para obter mais informações sobre entregas de relatório para o ambiente de produção, consulte [Visão geral da entrega de relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Para obter mais informações sobre notificações por push no aplicativo móvel para o ambiente de produção, consulte a seção em .

## Configurar o logon único na sandbox de atualização personalizada

Se você quiser configurar sua sandbox de atualização personalizada para funcionar com uma solução de logon único, faça isso configurando-a separadamente do ambiente de produção. A configuração de SSO na sandbox de atualização personalizada é independente da sua configuração de SSO no ambiente de produção.\
Ao atualizar sua sandbox de atualização personalizada, as informações de SSO não são copiadas de seu ambiente de produção para substituir a configuração da sandbox de atualização personalizada.

As etapas para configurar o logon único na sandbox de atualização personalizada são semelhantes àquelas para configurá-lo no ambiente de Produção.\
Para obter mais informações sobre como configurar o [!DNL Workfront] com SSO, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Isso não está disponível se a instância [!DNL Workfront] da sua organização estiver habilitada com o Adobe IMS. Consulte o administrador de rede ou de TI se precisar de mais informações.

## Recálculo automático de linhas de tempo do projeto

Recalcular linhas do tempo permite que os gerentes vejam como as forças fora do projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto se refere às datas planejadas e projetadas para o projeto.

Como administrador do Workfront, você pode configurar quando o Workfront recalcula automaticamente as linhas do tempo do projeto. O Workfront pode recalcular as linhas do tempo do projeto todas as noites, quando o escopo do projeto mudar, ou ambos.

Para obter informações, consulte [Configurar recálculos de linha de tempo para projetos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

Para o ambiente Personalizar atualização da sandbox, o recálculo noturno é desativado e as linhas de tempo do projeto não são recalculadas automaticamente. Você deve recalcular manualmente a linha do tempo do projeto para o ambiente de sandbox de atualização personalizada. Para obter informações, consulte [Recalcular linhas do tempo do projeto](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Uso e disponibilidade previstos

* Os ambientes de sandbox de atualização personalizada do [!DNL Workfront] não se destinam a testes de desempenho ou carga. Em vez disso, use esses ambientes para validar a funcionalidade do recurso com os fluxos de trabalho existentes da organização.

* Os fluxos de trabalho envolvendo documentos devem se concentrar no processo e não no teste de carga. Arquivos grandes não são suportados em ambientes de sandbox.

* [!DNL Workfront] Os ambientes da Sandbox de atualização personalizada devem estar sempre disponíveis. Qualquer interrupção em um ambiente de sandbox de atualização personalizada da Workfront durante o horário comercial regular será uma prioridade imediatamente após a resolução de qualquer problema de produção, se houver. Qualquer interrupção em um ambiente Workfront Custom Refresh Sandbox nos finais de semana (sábados e domingos) será resolvida para que o ambiente funcione durante o horário comercial na segunda-feira.

* A revisão não está disponível nos ambientes de sandbox de atualização personalizada.
