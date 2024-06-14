---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Instalar [!DNL Adobe Workfront] para [!DNL Jira]
description: Você pode usar [!DNL Adobe Workfront] para [!DNL Jira] para integrar o [!DNL Jira] e [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Instalar [!DNL Adobe Workfront for Jira]

Você pode usar [!DNL Adobe Workfront for Jira] para integrar o [!DNL Jira] e [!DNL Workfront] sistemas.

Após instalar o complemento, é possível definir workflows que criam [!DNL Jira] problemas automaticamente quando [!DNL Workfront] itens de trabalho são criados. Os itens em ambos os aplicativos ficam vinculados e algumas de suas informações podem ser atualizadas automaticamente em ambos os sistemas.

Todos os usuários em [!DNL Workfront] e [!DNL Jira] podem se beneficiar dessa integração. Eles só precisam de uma licença para o sistema em que trabalham mais, e não para ambos os sistemas.

Esse complemento está disponível para o [!UICONTROL Servidor] e [!UICONTROL OnDemand] (ou [!UICONTROL Nuvem]) versões de [!DNL Jira] Software. Este complemento não está disponível para o [!DNL Data Center] versão de [!DNL Jira] Software.

Para obter uma lista de [!DNL Jira] versões que [!DNL Workfront for Jira] atualmente compatíveis, consulte [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) no Mercado Atlassiano.

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
   <td role="rowheader">Adobe [!DNL Workfront] visão geral das licenças</td> 
   <td> 
   <p>Novo: Padrão</p>
   <p>Atual: [!UICONTROL Plano]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] acesso</td> 
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no [!DNL Jira] e [!DNL Workfront] para se dedicar a essa integração, em vez de usar as existentes que podem ser anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td><p>Você deve ser um [!DNL Workfront] administrador.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Instalar [!DNL Workfront] para [!DNL Jira]

Instalando [!DNL Workfront] para [!DNL Jira] O OnDemand é idêntico à instalação em um [!DNL Jira] Instância do servidor.

Você deve ser um [!DNL Jira] administrador para instalar o [!DNL Workfront] complementar.

Se você não for um [!DNL Jira] administrador, você pode procurar a [!DNL Workfront] e solicite que ele seja instalado. Sua solicitação é enviada para o [!DNL Jira] administrador para aprovação e instalação.

Para obter mais informações sobre como solicitar que um complemento seja instalado no [!DNL Jira] aplicativo, consulte [Gerenciar solicitações de usuário para complementos.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Para instalar [!DNL Workfront for Jira]:

1. Efetue logon no [!DNL Jira] as a [!DNL Jira] administrador.
1. Localize o **[!DNL Workfront for Jira]** complemento no [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Clique em **[!UICONTROL Obtenha agora]** para instalá-lo.

   Depois que a instalação for concluída, faça logon no [!DNL Workfront] de [!DNL Jira] e configurar sua integração.

   Para obter mais informações, consulte [Configurar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considerações para uma [!DNL Jira Server] instalação

>[!NOTE]
>
>Estes requisitos não se aplicam à [!UICONTROL OnDemand] ([!UICONTROL Nuvem]) versão de [!DNL Jira] Software.

Embora a instalação do [!DNL Workfront] complemento nos dois [!DNL Jira] é semelhante, você deve considerar o seguinte ao trabalhar com um [!DNL Jira Server] instalação:

* Ao configurar o complemento no [!DNL Jira], o endereço especificado no **[!DNL JIRA Base URL]** O campo pode não ser o mesmo URL que você usa para acessar [!DNL Jira] no servidor privado. A variável **[!DNL JIRA Base URL]** deve ser um endereço acessível publicamente conectado ao seu servidor privado usando NAT ou protocolos de proxy reverso, portanto [!DNL Workfront] O pode acessá-lo para fazer solicitações ao seu servidor.

* Você deve usar a criptografia SSL para proteger a comunicação entre [!DNL Jira] e [!DNL Workfront]. Ao habilitar o SSL, você deve ter uma pilha completa de certificados SSL de uma autoridade de certificação. Não oferecemos suporte a certificados autoassinados.
* Você deve garantir que a variável [!DNL jira.workfront.com] o domínio pode ser acessado pelos servidores corporativos. Ele serve como um ambiente middleware entre [!DNL Workfront] e [!DNL Jira] e é necessário para que o complemento funcione.

  Incluir na lista de permissões Você também deve adicionar os seguintes endereços IP estáticos ao arquivo no firewall para conexões de entrada e saída.

  `35.162.128.73`

  `34.213.36.118`

  `35.160.0.242`

  `3.209.27.146`

  `18.205.251.4`

  Para obter mais informações sobre como configurar seu firewall para funcionalidade ideal com o [!DNL Workfront], consulte [Configuração do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
