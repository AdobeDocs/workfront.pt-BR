---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: O [!DNL Adobe Workfront] Ambiente de sandbox de atualização personalizada
description: A Sandbox de atualização personalizada é um ambiente em que você pode testar e trabalhar usando dados do ambiente de produção. Também é ideal para executar treinamentos e determinar a funcionalidade de configuração.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---

# O [!DNL Adobe Workfront] Ambiente de sandbox de atualização personalizada

A Sandbox de atualização personalizada é um ambiente em que você pode testar e trabalhar usando dados do ambiente de produção. Também é ideal para executar treinamentos e determinar a funcionalidade de configuração.

>[!NOTE]
>
>Isso é diferente da sandbox de visualização, que também é um ambiente de teste que replica o [!DNL Workfront] ambiente de produção.
>
>* Novos recursos são introduzidos na sandbox de visualização antes de serem disponibilizados na produção.
>* Os novos recursos não são introduzidos na sandbox de atualização personalizada antes de serem disponibilizados em produção.
>
>  Além disso, há um custo adicional para obter a Sandbox de atualização personalizada que não é necessária para a Sandbox de visualização.
>
>  Para obter mais informações sobre a sandbox de visualização, consulte [O [!DNL Adobe Workfront] Visualizar ambiente do Sandbox](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Requisitos de acesso

Você deve ter o seguinte:

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
   <td> <p>[!UICONTROL Plan] </p> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pacote de suporte</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferencial] ou [!UICONTROL Enterprise]</p> <p>O pacote de suporte padrão não tem acesso à Caixa de proteção de atualização personalizada, mas tem acesso à Caixa de proteção de visualização.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizar a sandbox de atualização personalizada

A Sandbox de Atualização Personalizada contém seus dados de produção reais e não é atualizada até que você a programe para isso. Você pode programar uma atualização sempre que for conveniente para você, com a mesma frequência que uma vez por semana.

>[!NOTE]
>
>* Não é possível agendar uma atualização para o dia atual. Por exemplo, se hoje for 1º de junho, o primeiro dia em que você puder agendar uma atualização será 2 de junho.
>* Sua sandbox de atualização personalizada sempre tem os mesmos recursos de produto que seu ambiente de produção. No entanto, ao atualizar a sandbox de atualização personalizada, ela preserva a marca somente para a cor de fundo da tela de logon. Os logotipos da tela de logon e da barra de navegação são redefinidos para [!DNL Workfront] padrões e as imagens de marca que você modificou antes da atualização não são exibidas.
>




<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Acessar o sandbox de atualização personalizada do seu ambiente de produção {#access-the-custom-refresh-sandbox-from-your-production-environment}

Como um [!DNL Workfront] administrador, você pode acessar a Caixa de proteção de atualização personalizada no ambiente de produção.

>[!NOTE]
>
>Se sua conta estiver no Cluster 4 (Cluster da EMEA), você não poderá acessar o Sandbox de atualização personalizada no Ambiente de produção. Para obter mais informações sobre como você pode acessar sua Sandbox de atualização personalizada quando tiver uma conta no Cluster 4, consulte [Acessar o Sandbox de Atualização Personalizada para Contas no Cluster 4 (Contas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Acessar o Sandbox de Atualização Personalizada para Contas no Cluster 4 (Contas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

Para acessar sua sandbox de atualização personalizada:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Sistema]** >**[!UICONTROL Preferências]**.

1. No **[!UICONTROL Ambiente de teste]** seção , clique em **[!UICONTROL Sandbox 1]** ou **[!UICONTROL Sandbox 2]**.

   Seu pacote de suporte especifica se você tem acesso a uma ou duas sandboxes de atualização personalizadas.

1. Faça logon usando as credenciais da Sandbox de atualização personalizada.

   Suas credenciais de sandbox de atualização personalizada são iguais às credenciais de produção, a menos que você tenha alterado suas credenciais de produção desde a última vez que atualizou sua sandbox de atualização personalizada. Os logons são sincronizados somente quando ocorre uma atualização. Eles não sincronizam automaticamente.

   A Caixa de proteção de atualização personalizada mostra a versão e a última data de atualização no banner na parte superior da tela. Todas as informações da produção estão disponíveis e prontas para funcionar após a conclusão de uma atualização.

## Acessar o sandbox de atualização personalizada usando um URL {#access-the-custom-refresh-sandbox-using-a-url}

Qualquer usuário pode acessar a Caixa de proteção de atualização personalizada usando um URL.

* [Acessar o Sandbox de Atualização Personalizada para contas nos Clusters 1, 2, 3 e 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Acessar o Sandbox de Atualização Personalizada para Contas no Cluster 4 (Contas EMEA)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Acessar o Sandbox de Atualização Personalizada para contas nos Clusters 1, 2, 3 e 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Dependendo do seu pacote de suporte, você deve ter acesso a uma ou duas sandboxes de atualização personalizadas.

Para acessar sua sandbox de atualização personalizada usando um URL:

1. Navegue até esse URL se você tiver apenas uma Sandbox de atualização personalizada:

   https://companyname.sb01.workfront.com (URL antigo):https://cr1.attasksandbox.com/.)

   Ou Se você tiver duas sandboxes de atualização personalizadas, além dos URLs acima, também poderá acessar o seguinte URL para acessar a segunda sandbox de atualização personalizada:

   https://companyname.sb02.workfront.com (URL antigo):https://cr2.attasksandbox.com/)

1. Na tela de logon, faça logon usando as credenciais da Sandbox de atualização personalizada.
1. Suas credenciais de sandbox de atualização personalizada são iguais às credenciais de produção, a menos que você tenha alterado suas credenciais de produção desde que a sandbox de atualização personalizada foi atualizada pela última vez. Os logons são sincronizados somente quando ocorre uma atualização. Eles não sincronizam automaticamente.

### Acessar o Sandbox de Atualização Personalizada para Contas no Cluster 4 (Contas EMEA) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Se o seu [!DNL Workfront] Se a conta estiver no Cluster 4 (cluster EMEA), você pode acessar a Caixa de proteção de atualização personalizada somente usando um URL. Para descobrir em qual cluster sua conta está, entre em contato com a equipe de Suporte ao cliente.

Dependendo do seu pacote de suporte, você deve ter acesso a uma ou duas sandboxes de atualização personalizadas.

Para acessar sua sandbox de atualização personalizada usando um URL:

1. Navegue até esse URL se você tiver apenas uma Sandbox de atualização personalizada:

   https://companyname.sb01.workfront.com (URL antigo):https://cr3.attasksandbox.com)

   Ou

   Vá para qualquer um desses URLs se tiver duas sandboxes de atualização personalizadas:

   https://companyname.sb01.workfront.com (URL antigo):https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (URL antigo):https://cr4.attasksandbox.com)

1. Na tela de logon, faça logon usando as credenciais da Sandbox de atualização personalizada.

   Suas credenciais de sandbox de atualização personalizada são iguais às credenciais de produção, a menos que você tenha alterado suas credenciais de produção desde que a sandbox de atualização personalizada foi atualizada pela última vez. Os logons são sincronizados somente quando ocorre uma atualização. Eles não sincronizam automaticamente.

## Programar uma atualização da sua sandbox de atualização personalizada

>[!IMPORTANT]
>
>A duração da atualização depende do tamanho dos dados que estão sendo atualizados. Durante o processo de atualização, é importante que o ambiente de sandbox de atualização personalizada não esteja sendo usado de nenhuma maneira (incluindo chamadas de API e integrações), pois isso impedirá que a atualização da sandbox seja concluída com êxito. [!DNL Workfront] O desativará o ambiente de sandbox de atualização personalizada antes de ele começar, mas você deve encerrar todas as sessões ativas para garantir que a atualização da sandbox seja bem-sucedida.

Depois de programar uma atualização da Caixa de proteção de atualização personalizada, você pode cancelá-la clicando em [!UICONTROL Cancelar] na parte superior da página. Você também pode reagendá-lo para um momento posterior.

>[!NOTE]
>
>Não é possível agendar atualizações automáticas de sandbox.

Para agendar uma atualização da sandbox de atualização do cliente:

1. Faça logon no Sandbox de atualização personalizada.
1. Clique em **[!UICONTROL Agendar]** no banner na parte superior da tela e selecione uma data no calendário.
1. Selecione uma data para quando deseja que a atualização ocorra e clique em **[!UICONTROL Agendar atualização]**.

## Alternar para produção da sandbox de atualização personalizada

1. Faça logon no Sandbox de atualização personalizada.

   Para obter mais informações sobre como acessar sua sandbox de atualização personalizada, consulte [Acessar o sandbox de atualização personalizada do seu ambiente de produção](#access-the-custom-refresh-sandbox-from-your-production-environment) ou [Acessar o sandbox de atualização personalizada usando um URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Clique em **[!UICONTROL Ir para produção]** no banner na parte superior da tela.

   Lembre-se de que o trabalho feito na sandbox não estará visível no [!UICONTROL produção] , já que a transferência de dados é unidirecional, da produção ao seu Sandbox de atualização personalizada e não inversa.

## Receber emails da sandbox de atualização personalizada

[!DNL Workfront] desativa todas as comunicações por email do ambiente Sandbox de atualização personalizada. Se quiser receber notificações por email do ambiente Caixa de proteção de atualização personalizada, ative essa funcionalidade nas configurações do usuário. Para obter mais informações sobre como ativar notificações por email no ambiente de Caixa de proteção de atualização personalizada, consulte [Ativar a entrega de emails do ambiente Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>A entrega de relatórios e as notificações por push no aplicativo móvel são sempre desativadas no ambiente Sandbox de atualização personalizada. Nem você nem o [!DNL Workfront] o administrador pode habilitar a entrega de relatórios ou notificações por push para o aplicativo móvel ao acessar o ambiente Caixa de proteção de atualização personalizada.\
>Para obter mais informações sobre deliveries de relatórios para o ambiente de produção, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Para obter mais informações sobre notificações por push no aplicativo móvel para o ambiente de produção, consulte a seção em .

## Configurar logon único na sandbox de atualização personalizada

Se você quiser configurar a Caixa de proteção de atualização personalizada para funcionar com uma solução de logon único, poderá fazer isso configurando-a separadamente do ambiente de Produção. A configuração do SSO na Sandbox de atualização personalizada é independente da configuração do SSO no ambiente de Produção.\
Quando você atualiza a Sandbox de atualização personalizada, as informações do SSO não são copiadas do ambiente de Produção para substituir a configuração da Sandbox de atualização personalizada.

As etapas para configurar o logon único na Sandbox de atualização personalizada são semelhantes àquelas para configurá-la no ambiente de Produção.\
Para obter mais informações sobre como configurar [!DNL Workfront] com SSO, consulte [Visão geral do logon único no Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Isso não está disponível se o [!DNL Workfront] está habilitada com o Adobe IMS. Consulte seu administrador de rede ou de TI se precisar de mais informações.

## Utilização e disponibilidade previstas

[!DNL Workfront] Os ambientes de sandbox de atualização personalizada não se destinam a testes de desempenho ou carga. Em vez disso, use esses ambientes para validar a funcionalidade do recurso com os fluxos de trabalho existentes de sua organização.

[!DNL Workfront] Os ambientes de sandbox de atualização personalizada devem estar sempre disponíveis. Qualquer interrupção em um ambiente de sandbox de atualização personalizada do Workfront durante o horário comercial regular será uma primeira prioridade imediatamente após qualquer problema de produção ser resolvido, se houver. Qualquer interrupção em um ambiente Workfront Custom Refresh Sandbox nos finais de semana (sábados e domingos) será solucionada para que o ambiente esteja em execução no horário comercial da segunda-feira.
