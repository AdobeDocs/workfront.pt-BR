---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Instalar [!DNL Adobe Workfront] para [!DNL Jira]
description: Você pode usar [!DNL Adobe Workfront] para [!DNL Jira] para integrar [!DNL Jira] e [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: f6e0feb1-349f-459f-9f93-c7492cb15f11
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Instalar [!DNL Adobe Workfront for Jira]

Você pode usar [!DNL Adobe Workfront for Jira] para integrar [!DNL Jira] e [!DNL Workfront] sistemas.

Depois de instalar o complemento, você pode definir workflows que criam [!DNL Jira] emite automaticamente quando [!DNL Workfront] itens de trabalho são criados. Os itens em ambos os aplicativos são vinculados, e algumas de suas informações podem ser atualizadas automaticamente em ambos os sistemas.

Todos os usuários em [!DNL Workfront] e [!DNL Jira] pode se beneficiar dessa integração. Eles só precisam de uma licença para o sistema em que trabalham mais, e não para ambos os sistemas.

Este complemento está disponível para a [!UICONTROL Servidor] e [!UICONTROL OnDemand] ou [!UICONTROL Cloud]) versões de [!DNL Jira] Software. Este complemento não está disponível para a variável [!DNL Data Center] versão de [!DNL Jira] Software.

Para uma lista de [!DNL Jira] versões que [!DNL Workfront for Jira] atualmente compatível, consulte [[!DNL [!DNL Workfront for Jira]]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) no Atlassian Marketplace.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plano</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] visão geral das licenças</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] acesso</td> 
   <td> <p>Acesso do administrador do sistema</p> <p>Importante: Recomendamos que você crie contas de administrador de sistema separadas em [!DNL Jira] e [!DNL Workfront] dedicar-se a essa integração, em vez de usar as existentes que podem ser vinculadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Instalar [!DNL Workfront] para [!DNL Jira]

Instalar [!DNL Workfront] para [!DNL Jira] O OnDemand é idêntico à instalação em um [!DNL Jira] Instância do servidor.

Você deve ser um [!DNL Jira] administrador para instalar o [!DNL Workfront] complemento.

Se você não for um [!DNL Jira] administrador, você pode procurar pelo [!DNL Workfront] e solicitar que seja instalado. Sua solicitação é enviada para o [!DNL Jira] administrador para aprovação e instalação.

Para obter mais informações sobre como solicitar que um complemento seja instalado em seu [!DNL Jira] aplicativo, consulte [Gerenciando solicitações de usuários para complementos.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Para instalar [!DNL Workfront for Jira]:

1. Faça logon em [!DNL Jira] como [!DNL Jira] administrador.
1. Encontre a **[!DNL Workfront for Jira]** no complemento [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview).

1. Clique em **[!UICONTROL Obtenha agora]** para instalá-lo.

   Depois que a instalação for concluída, você poderá fazer logon no [!DNL Workfront] from [!DNL Jira] e configure a integração.
   [!DNL ]
Para obter mais informações, consulte [Configurar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Considerações para um [!DNL Jira Server] instalação

>[!NOTE]
>
>Estes requisitos não se aplicam à [!UICONTROL OnDemand] ([!UICONTROL Cloud]) versão de [!DNL Jira] Software.

Embora a instalação do [!DNL Workfront] complemento nos dois [!DNL Jira] for semelhante, você deve considerar o seguinte ao trabalhar com um [!DNL Jira Server] instalação:

* Ao configurar o complemento em [!DNL Jira], o endereço especificado no **[!DNL JIRA Base URL]** pode não ser o mesmo URL que você usa para acessar [!DNL Jira] no seu servidor privado. O **[!DNL JIRA Base URL]** deve ser um endereço acessível publicamente conectado ao servidor privado usando protocolos NAT ou proxy reverso, portanto [!DNL Workfront] O pode acessá-lo para fazer solicitações ao servidor.

* Você deve usar a criptografia SSL para proteger a comunicação entre [!DNL Jira] e [!DNL Workfront]. Ao habilitar o SSL, você deve ter uma pilha completa de certificados SSL de uma autoridade de certificação. Não oferecemos suporte a certificados autoassinados.
* Você deve garantir que a variável [!DNL jira.workfront.com] O domínio é acessível a partir dos servidores corporativos. Ele serve como um ambiente middleware entre [!DNL Workfront] e [!DNL Jira] e é necessário para que o complemento funcione.

   Você também deve adicionar os seguintes endereços IP estáticos à lista de permissões do firewall para conexões de saída e de entrada.

   `35.162.128.73`

   `34.213.36.118`

   `35.160.0.242`

   `3.209.27.146`

   `18.205.251.4`

   Para obter mais informações sobre como configurar seu firewall para obter a funcionalidade ideal com o [!DNL Workfront], consulte [Configurar o firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
