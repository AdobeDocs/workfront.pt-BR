---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-microsoft-teams
title: Instalar o  [!DNL Adobe Workfront] for Microsoft Teams
description: O aplicativo [!DNL Adobe Workfront for Microsoft Teams] permite executar ações básicas no [!DNL Workfront] sem sair dos [!DNL Microsoft Teams] canais de chat.
author: Becky
feature: Workfront Integrations and Apps
exl-id: a8d4e48c-1ccc-4e6e-a0a0-9b68748590c0
source-git-commit: 41d898e82bc5b06498966ba938b68ed10e742d3b
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Instalar [!DNL Adobe Workfront] para equipes da Microsoft

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>A partir de 1º de julho de 2025, a Microsoft removerá o suporte das equipes clássicas desktop aplicativo. Como resultado, a integração da Workfront com as Equipes da Microsoft não será suportada depois que as equipes clássicas desktop aplicativo não estiver mais disponível.


O aplicativo [!DNL Adobe Workfront for Microsoft Teams] permite executar ações básicas no [!DNL Workfront] sem sair dos canais de chat do [!DNL Microsoft Teams].

>[!NOTE]
>
>[!DNL Microsoft Teams] não dá mais suporte a [!DNL Internet Explorer]. Para usar o [!DNL Adobe Workfront for Microsoft Teams integration], você deve usar um navegador da Web diferente do [!DNL Internet Explorer].


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: Padrão</p>
    <p>Atual: [!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve ser um equipe proprietário [!DNL Microsoft Teams] para instalar[!DNL Workfront].[!DNL Microsoft Teams]

## Instalar [!DNL Workfront for Microsoft Teams]

Como equipe proprietário, [!DNL Microsoft Teams]você pode instalar o [!DNL Workfront for Microsoft Teams] aplicativo para cada uma de suas equipes, seja na Loja ou a [!DNL Microsoft] partir de um arquivo fornecido por [!DNL Workfront].

### Instalar [!DNL Workfront for Microsoft Teams] do Repositório [!DNL Microsoft]

1. Faça logon em [!DNL Microsoft Teams] como proprietário de equipe.
1. Selecione a equipe para a qual você deseja instalar o aplicativo [!DNL Workfront for Microsoft Teams].
1. Clique **[!UICONTROL em Armazenar]** na barra lateral navegação.

1. **[!UICONTROL Na caixa Search,]** digite *[!DNL Workfront]*.

1. Clique na **[!DNL Workfront]** cartão e seguir as instruções na assistente.
1. (Recomendado) Selecione uma equipe no **[!UICONTROL menu suspenso Adicionar a um equipe]** e ative a opção **[!UICONTROL Sim]** para adicionar o aplicativo a um equipe.

   ![ms_team_add_to_a_team_option.png](assets/ms-teams-add-to-a-team-option-350x122.png)

1. Para o canal, selecione **[!UICONTROL Geral]** para usar o aplicativo nesse canal para a equipe selecionada e clique em **[!UICONTROL Configurar]** para os recursos desejados.

1. Quando a instalação for concluída, uma notificação de que a instalação foi bem-sucedida aparecerá no canal [!UICONTROL Geral] da equipe selecionada. Todos os membros da equipe podem ver essa notificação.
1. (Opcional) Fixe seu aplicativo [!DNL Workfront] para facilitar o acesso:

   1. Clique no ícone **[!UICONTROL Mais]** sob o campo de mensagem no canal [!UICONTROL Geral].

   1. Passe o mouse sobre o aplicativo [!DNL Workfront] na lista e clique no ícone **[!UICONTROL Mais]** à direita.

   1. Clique em **[!UICONTROL Fixar]**.

      Isso adiciona um ícone [!DNL Workfront] sob o campo de chat. Você pode acessar rapidamente a área [!UICONTROL Pesquisa] daqui.

      Para obter informações sobre a pesquisa de [!DNL Workfront] itens, consulte [Pesquisar e compartilhar [!DNL Adobe Workfront] itens em [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

1. Clique em **[!UICONTROL Fazer logon em[!DNL Workfront]]** para acessar [!DNL Workfront from Microsoft Teams].

   Para obter informações sobre fazendo logon no [!DNL Workfront]site, consulte o [Login no Workfront na seção Microsoft Teams](#log-in-to-workfront-from-microsoft-teams) neste artigo.

### Instalar a [!DNL Workfront for Microsoft Teams] partir de um arquivo privado

Se sua organização restringir o acesso ao download de aplicativos na [!DNL Microsoft] Loja, você deve entrar em contato com nossa Equipe de suporte e solicitação um arquivo privado do [!DNL Workfront for Microsoft Teams] aplicativo para instalar o aplicativo.

Para obter informações sobre como entrar em contato com a Equipe de Suporte, consulte [Entrar em contato com o Suporte ao Cliente](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

Para instalar [!DNL Workfront for Microsoft Teams] de um arquivo particular:

1. Salve o arquivo particular que você recebeu de [!DNL Workfront] em seu computador.
1. Faça logon [!DNL Microsoft Teams] como um [!DNL Microsoft] equipe proprietário.
1. Clique no **[!UICONTROL ícone Mais]** para a equipe para a qual deseja instalar [!DNL Workfront for Microsoft Teams].

1. Clique **[!UICONTROL em Gerenciar equipe]**.
1. Selecione os **[!UICONTROL guia aplicativos]** e clique **[!UICONTROL em Fazer upload de um aplicativo]** personalizado no canto inferior direito da tela.

1. Procure o arquivo privado salvo em seu computador e seguir as etapas de instalação para instalar [!DNL Workfront for Microsoft Teams].
1. Quando a instalação for concluída, aparecerá uma notificação de que a instalação foi bem-sucedida no canal General (Geral) da equipe selecionada. Todos os membros da equipe podem ver essa notificação.
1. (Opcional) Clique no ícone **[!UICONTROL Mais]** (três pontos) no campo **[!UICONTROL Digite suas perguntas aqui]**.

1. (Opcional) Passe o mouse sobre o aplicativo [!DNL Workfront] na lista e clique no ícone **[!UICONTROL Mais]** à direita.

1. (Opcional) Clique em **[!UICONTROL Pin]**.

   Isso adiciona um ícone [!DNL Workfront] no campo [!UICONTROL Digite suas perguntas aqui]. Você pode acessar rapidamente a área de [!UICONTROL Search] aqui.\
   Para obter informações sobre a pesquisa de itens da Workfront, consulte [Search e compartilhe [!DNL Adobe Workfront] itens. [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md)

## Fazer logon nas [!DNL Workfront] [!DNL Microsoft] equipes

Como equipe [!DNL Microsoft Teams] proprietário, você deve instalar o aplicativo para sua [!DNL Workfront for Microsoft Teams] equipe antes que você ou qualquer pessoa na equipe possa fazer logon [!DNL Workfront from Microsoft Teams].

Ao fazer logon [!DNL Workfront] a partir de [!DNL Microsoft Teams]então, você pode receber [!DNL Workfront] notificações no [!DNL Workfront] bot canal ou executar determinadas ações no [!DNL Workfront] [!DNL Microsoft Teams].

Para obter informações sobre como instalar o aplicativo [!DNL Workfront], consulte a seção [Instalar [!DNL Workfront for Microsoft Teams]](#install-workfront-for-microsoft-teams) neste artigo.

Para obter informações sobre como acessar [!DNL Workfront] de [!DNL Microsoft Teams] para executar determinadas ações, consulte [Acesso [!DNL Adobe Workfront] de [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/access-workfront-from-ms-teams.md).

Para fazer login em [!DNL Workfront] a partir de [!DNL Microsoft Teams]:

1. Vá para o canal **[!UICONTROL Geral]** da equipe em que o aplicativo [!DNL Workfront for Microsoft Teams] foi instalado e clique em **[!UICONTROL Fazer logon no Workfront]**.

   O [!DNL Workfront] canal de bate-papo bot é adicionado aos seus [!DNL Microsoft Teams] canais de bate-papo.

1. Vá para o [!DNL Workfront] bot bate-papo canal [!DNL Microsoft Teams] e digite *[!UICONTROL logon no]* **[!UICONTROL campo Digite suas perguntas aqui]** .

   Ou

   Clique em **[!UICONTROL Fazer logon]**.

   Uma nova guia do navegador é aberta.

1. Siga as instruções para fazer logon no [!DNL Workfront] usando a Autenticação Aprimorada, o OAuth 2.0 ou a URL da Linguagem de Marcação de Asserção de Segurança (SAML).

   >[!NOTE]
   >
   >* Quando for solicitado que você insira o domínio da sua conta do [!DNL Workfront], digite-o usando este formato: *yourCompany&#39;sDomain.my.workfront.com*. O domínio da sua empresa geralmente é o nome da sua empresa.
   >* A Autenticação Aprimorada não estará disponível até que um administrador do [!DNL Workfront] a habilite para esta integração.


1. Feche a guia do navegador usada para fazer logon e retornar para [!DNL Microsoft Teams].

   Uma notificação é exibida no canal de chat do bot [!DNL Workfront] para confirmar que você fez logon no [!DNL Workfront] com êxito.
