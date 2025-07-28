---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Instalar [!DNL Adobe Workfront] por [!DNL Jira]
description: Você pode usar o [!DNL Adobe Workfront] for [!DNL Jira] para integrar seus [!DNL Jira] e [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# Instalar [!DNL Adobe Workfront for Jira]

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Jira não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Jira.
>
>Oito modelos de Automação e Integração do Workfront prontos para uso para Jira estarão disponíveis até agosto para ajudar a replicar fluxos de trabalho comuns e acelerar a implementação. Os modelos são totalmente personalizáveis para atender às necessidades específicas dos negócios e podem ser estendidos à medida que os requisitos evoluem.
> 
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Jira, consulte [módulos do Software Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

Você pode usar o [!DNL Adobe Workfront for Jira] para integrar seus sistemas [!DNL Jira] e [!DNL Workfront].

Após instalar o complemento, você pode definir fluxos de trabalho que criem [!DNL Jira] problemas automaticamente quando [!DNL Workfront] itens de trabalho forem criados. Os itens em ambos os aplicativos ficam vinculados e algumas de suas informações podem ser atualizadas automaticamente em ambos os sistemas.

Todos os usuários em [!DNL Workfront] e [!DNL Jira] podem se beneficiar dessa integração. Eles só precisam de uma licença para o sistema em que trabalham mais, e não para ambos os sistemas.

Este complemento está disponível para as versões [!UICONTROL Server] e [!UICONTROL OnDemand] (ou [!UICONTROL Cloud]) do Software [!DNL Jira]. Este complemento não está disponível para a versão [!DNL Data Center] do Software [!DNL Jira].

Para obter uma lista de [!DNL Jira] versões que [!DNL Workfront for Jira] suporta atualmente, consulte [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) no Atlassian Marketplace.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> 
   <p>Novo: Qualquer um</p>
   <p>Atual: [!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Visão geral das licenças do Adobe [!DNL Workfront]</td> 
   <td> 
   <p>Novo: Padrão</p>
   <p>Atual: [!UICONTROL Plano]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] acesso</td> 
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no [!DNL Jira] e no [!DNL Workfront] para se dedicar a essa integração, em vez de usar as existentes que podem estar anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td><p>Você deve ser um administrador [!DNL Workfront].</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Instalar o [!DNL Workfront] para [!DNL Jira]

A instalação do [!DNL Workfront] for [!DNL Jira] OnDemand é idêntica à instalação dele em uma instância do Servidor [!DNL Jira].

Você deve ser um administrador [!DNL Jira] para instalar o complemento [!DNL Workfront].

Se você não for um administrador do [!DNL Jira], poderá procurar o complemento [!DNL Workfront] e solicitar que ele seja instalado. Sua solicitação é enviada ao administrador do [!DNL Jira] para aprovação e instalação.

Para obter mais informações sobre como solicitar a instalação de um complemento no aplicativo [!DNL Jira], consulte [Gerenciando solicitações de usuários para complementos.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Para instalar [!DNL Workfront for Jira]:

1. Faça logon em [!DNL Jira] como administrador [!DNL Jira].
1. Localize o complemento **[!DNL Workfront for Jira]** em [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Clique em **[!UICONTROL Obter agora]** para instalá-lo.

   Após a conclusão da instalação, faça logon no [!DNL Workfront] a partir do [!DNL Jira] e configure sua integração.

   Para obter mais informações, consulte [Configurar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considerações para uma instalação do [!DNL Jira Server]

>[!NOTE]
>
>Estes requisitos não se aplicam à versão [!UICONTROL OnDemand] ([!UICONTROL Cloud]) do Software [!DNL Jira].

Embora a instalação do complemento [!DNL Workfront] nos dois ambientes [!DNL Jira] seja semelhante, você deve considerar o seguinte ao trabalhar com uma instalação [!DNL Jira Server]:

* Ao configurar o complemento no [!DNL Jira], o endereço especificado no campo **[!DNL JIRA Base URL]** pode não ser a mesma URL que você usa para acessar [!DNL Jira] em seu servidor privado. O **[!DNL JIRA Base URL]** deve ser um endereço acessível publicamente conectado ao seu servidor privado usando NAT ou protocolos de proxy reverso, para que o [!DNL Workfront] possa acessá-lo e fazer solicitações ao seu servidor.

* Você deve usar a criptografia SSL para proteger a comunicação entre [!DNL Jira] e [!DNL Workfront]. Ao habilitar o SSL, você deve ter uma pilha completa de certificados SSL de uma autoridade de certificação. Não oferecemos suporte a certificados autoassinados.
* Você deve garantir que o domínio [!DNL jira.workfront.com] possa ser acessado de seus servidores corporativos. Ele serve como um ambiente middleware entre [!DNL Workfront] e [!DNL Jira] e é necessário para que o complemento funcione.

  Incluir na lista de permissões Você também deve adicionar os seguintes endereços IP estáticos ao arquivo no firewall para conexões de entrada e saída.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Para obter mais informações sobre como configurar o firewall para funcionalidade ideal com o [!DNL Workfront], consulte [Configurando o Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
