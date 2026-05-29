---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configurar o servidor MCP do Adobe Workfront
description: Configure sua instância do Workfront e sua plataforma de IA para trabalhar com o Workfront por meio de uma conversa em idioma natural.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 7d961bca74884baa869f92a24a3f586500b824a5
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 0%

---


# Configurar o servidor MCP do Adobe Workfront

{{highlighted-preview-article-level}}

O servidor MCP do [!DNL Adobe Workfront] permite que você trabalhe com seus dados do Workfront por meio de conversas em linguagem natural em uma plataforma de agente de IA com suporte.

Antes de conectar uma plataforma de agente de IA ao Workfront, um administrador do Workfront deve habilitar o acesso ao servidor MCP na instância do Workfront. As etapas exatas para conectar uma plataforma de agente de IA são diferentes para cada plataforma de agente de IA compatível.

>[!IMPORTANT]
>
>Atualmente, o servidor MCP do Workfront está disponível somente para clientes na região dos EUA que usam o AWS.

## Plataformas de IA compatíveis

O servidor de MCP do Workfront funciona com qualquer plataforma de agente de IA compatível com o protocolo de contexto de modelo (MCP).

Este artigo aborda as etapas de conexão para:

* [!DNL Claude]
* [!DNL ChatGPT]

Se você usar uma plataforma de agente de IA compatível com MCP diferente (por exemplo, [!DNL Gemini] ou [!DNL Microsoft Copilot]), siga as etapas na documentação dessa plataforma para adicionar um servidor MCP personalizado. Quando for solicitado o URL do servidor MCP, insira: `https://mcp.workfront.adobe.com/mcp/v1/workfront`


## Pré-requisitos

Antes de conectar o Workfront a uma plataforma de agente de IA, é necessário:

* Ter uma conta [!DNL Adobe Workfront] ativa com permissão para acessar os dados com os quais deseja trabalhar
* Ter acesso a uma plataforma de agente de IA como o [!DNL Claude]
* Sua instância do Workfront deve estar ativada no Adobe Identity Management System (IMS).

### Pré-requisitos do administrador

O acesso ao servidor MCP é restringido por dois administradores separados.

* O administrador do Workfront controla o acesso ao servidor MCP para sua instância do Workfront por meio de dois alternadores nas Preferências do Sistema: **Ferramentas MCP somente leitura** (habilitadas por padrão) e **Ferramentas MCP de gravação** (desabilitadas por padrão). Se você puder encontrar itens do Workfront por meio da plataforma de agente de IA, mas não puder criá-los, atualizá-los ou excluí-los, peça ao administrador do Workfront para habilitar ações de gravação.

  Para obter mais informações, consulte [Configurar preferências do sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

* Se você usar uma versão corporativa de uma plataforma de agente de IA, o administrador dessa plataforma deverá habilitar o conector [!DNL Adobe Workfront] para sua organização ou fornecer acesso de URL personalizado para se conectar ao servidor MCP do Workfront.


## Conectar o Workfront ao Claude

Você se conecta ao Workfront uma vez a cada conta [!DNL Claude]. A conexão é autenticada em uma instância específica do Workfront e você permanece conectado até que opte por se desconectar.



### Conectar-se ao Claude Desktop a partir do diretório connectors

Em breve.

<!--

+++ Expand to view step-by-step instructions for connecting Workfront to [!DNL Claude].

To connect Workfront to [!DNL Claude]:

1. Open [!DNL Claude].

1. Navigate to the connectors area.



1. Find **[!DNL Adobe Workfront]** in the connector list.

   If you don't see it, see [Admin prerequisites](#admin-prerequisites) in this article.

1. Click **Connect**.



1. When prompted, log in to your Workfront instance.


1. After authentication completes, you're connected.



+++

-->

### Conectar-se ao Claude Desktop com um URL

+++ Expanda para exibir as instruções passo a passo para conectar o Workfront ao [!DNL Claude] com uma URL.

Para conectar o Workfront a [!DNL Claude] com uma URL:

1. Faça login em [Claude](https://claude.ai) usando suas credenciais.
1. No menu esquerdo, selecione o ícone **Personalizar**.
1. Selecione **Conectores** e o ícone **+** para adicionar um conector.
1. Selecione o botão **Criar aplicativo**.
1. Dê ao conector um nome desejado (como &quot;Workfront&quot;) e insira a URL do Servidor MCP desejada: `https://mcp.workfront.adobe.com/mcp/v1/workfront`

1. Depois que o conector é criado, uma janela de logon é exibida. Autentique usando suas credenciais da Adobe ID. Selecione a instância do Workfront desejada se você pertencer a mais de uma.

+++

### Personalizar o comportamento do Claude com habilidades

[!DNL Claude] dá suporte a conjuntos de instruções criados pelo usuário chamados habilidades. Você pode usar uma habilidade para personalizar como [!DNL Claude] se comporta com o Workfront. Por exemplo, você pode criar uma habilidade que diga a [!DNL Claude] para sempre buscar dados novos do Workfront em vez de depender de resultados anteriores.

Para saber mais sobre [!DNL Claude] habilidades, consulte a [documentação do usuário do Claude](https://code.claude.com/docs/en/skills) ou peça ajuda ao Claude com as habilidades.

## Conectar-se ao ChatGPT

1. Faça logon em [ChatGPT](https://chatgpt.com) usando suas credenciais.
1. Na parte inferior esquerda, selecione **seu nome** → **Configurações**.
1. Selecione **Aplicativos** e habilite o **Modo de desenvolvedor**.
1. Selecione o botão **Criar aplicativo**.
1. Dê um nome desejado ao aplicativo (como &quot;Workfront&quot;) e insira a URL do Servidor MCP desejada: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
1. Verifique se a Autenticação está definida como **OAuth** (definido por padrão) e marque a caixa de seleção de aceitação para continuar.
1. Depois que o aplicativo é criado, uma janela de logon é exibida. Autentique usando suas credenciais da Adobe ID. Selecione a instância do Workfront desejada se você pertencer a mais de uma.

### Personalizar o comportamento do ChatGPT com GPTs personalizados

O ChatGPT oferece suporte a assistentes criados pelo usuário chamados de GPTs personalizados. Você pode usar um GPT personalizado para personalizar como o ChatGPT se comporta com seu conector. Por exemplo, você pode criar um GPT personalizado que instrui o ChatGPT a sempre buscar dados novos do serviço conectado, em vez de depender de resultados anteriores.

Para saber mais sobre GPTs Personalizados, consulte a [documentação do usuário do ChatGPT](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts) ou peça ajuda ao ChatGPT para obter GPTs Personalizados.

## Verifique sua conexão

Para confirmar se a plataforma do agente de IA está conectada ao Workfront, peça à plataforma do agente de IA para listar as ações que o servidor MCP do Workfront disponibiliza. Por exemplo:

* *Que ações do Workfront você pode realizar?*
* *Listar as ferramentas do Workfront às quais você tem acesso.*

Você também pode ver a lista completa de ferramentas em [ferramentas de servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Ferramentas disponíveis

O servidor MCP do Workfront expõe um conjunto de ferramentas que a plataforma de agente de IA conectada chama em seu nome — por exemplo, ferramentas para pesquisar no Workfront, criar itens, atualizar campos e gerenciar aprovações. Para obter a lista de referência completa, agrupada por área do Workfront, consulte [Ferramentas de servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

## Alternar para uma instância diferente do Workfront

Cada conexão autentica a plataforma de IA em uma única instância do Workfront. Para usar uma instância diferente, desconecte e reconecte.

Para se conectar a uma instância diferente do Workfront:

1. Na plataforma do agente de IA, desconecte o servidor MCP do Workfront.
1. Reconecte o conector.
1. Autentique para a nova instância do Workfront.

>[!NOTE]
>
>Fazer logoff sozinho não alterna a instância do Workfront. Você deve desconectar e reconectar o conector.

<!--

## Connect to Gemini

>[!IMPORTANT]
>
>You must be an administrator on the Gemini platform to set up the MCP server. If you aren't an administrator, share these instructions with your administrator so they can set up the connection for you.


To set up the connection between Gemini and the Workfront MCP server, follow the instructions provided by Google for [connecting Gemini to external tools using MCP](https://docs.cloud.google.com/gemini/enterprise/docs/connectors/custom-mcp-server/set-up-custom-mcp-server). 

When prompted for the MCP Server URL, enter the following URL for your Workfront MCP server: `https://mcp.workfront.adobe.com/mcp/v1/workfront`
-->

<!--
## Connect to Microsoft Copilot

✅ 1) Copilot Studio (most common for agents / enterprise use)
This is the cleanest "paste a URL" flow.
Steps
1. Open your Copilot Studio agent
2. Go to Tools
3. Click:
    * Add a tool → New tool → Model Context Protocol
4. In the wizard, fill in:
    * Server name (anything)
    * Server description
    * ✅ Server URL (your MCP endpoint)
5. Choose auth (if needed):
    * None / API key / OAuth
6. Click Create
👉 That's it—your MCP server is now attached to the agent.
This flow is explicitly documented:
* You add MCP via Tools → Add tool → Model Context Protocol
* Then provide Server name, description, and URL ￼
￼
What happens next
* Copilot discovers tools automatically from the MCP server
* You can enable/disable tools per agent
* The agent calls them when relevant

-->

## Solução de problemas de configuração e autenticação

+++ Expanda para exibir dicas de solução de problemas para configuração e autenticação do servidor MCP do Workfront.

| Problema | Causa provável | Corrigir |
|---|---|---|
| Você não pode encontrar o conector [!DNL Adobe Workfront] em [!DNL Claude]. | O administrador do [!DNL Claude] não o habilitou. | Contate o administrador do [!DNL Claude] (não o administrador do Workfront) e peça que ele habilite o conector [!DNL Adobe Workfront]. |
| Você se conectou, mas não pode ver seus dados. | Você autenticou na instância incorreta do Workfront. | Desconecte o conector, reconecte e autentique na instância correta. |
| Falha na autenticação ou a conexão parou de funcionar. | Sua sessão de autenticação expirou ou há um erro de conexão. | Desconecte e reconecte o conector. |
| Você deseja alternar para uma instância diferente do Workfront. | Uma única conexão vincula você a uma instância. | Desconecte, reconecte e autentique na nova instância. |
| Você não pode se conectar ao Workfront ou vê uma mensagem informando que o acesso ao servidor MCP está desativado. | O administrador do Workfront desativou o acesso ao servidor MCP para sua instância. | Entre em contato com o administrador do Workfront e solicite que ele ative o acesso ao servidor MCP nas Preferências do sistema. |
| A plataforma do agente de IA pode encontrar seus itens do Workfront, mas não pode criá-los, atualizá-los ou excluí-los. | O administrador do Workfront desativou as ações de gravação do servidor MCP do Workfront. | Entre em contato com o administrador do Workfront e solicite que ele ative ações de gravação nas Preferências do sistema. |

Para obter uma solução de problemas diária depois de se conectar (por exemplo, resultados obsoletos ou comportamento inesperado), consulte [Usar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++

## Perguntas frequentes sobre configuração

+++ Expanda para exibir perguntas frequentes sobre a configuração do servidor MCP do Workfront.

### Posso me conectar a várias instâncias do Workfront de uma só vez?

Não. Cada conexão vincula uma plataforma de IA a uma única instância do Workfront. Para alternar, desconecte e reconecte, autenticando para a nova instância.

### Qual administrador habilita isto?

O administrador do Workfront e o administrador da plataforma de agente de IA. O administrador do Workfront habilita o acesso ao servidor MCP no Workfront. O administrador da sua plataforma de agente de IA habilita o acesso ao Workfront no lado dessa plataforma. Para [!DNL Claude], o administrador corporativo [!DNL Claude] habilita o conector [!DNL Adobe Workfront].

### Posso usar o servidor MCP do Workfront se minha instância do Workfront não estiver ativada no Adobe Identity Management System (IMS)?

Não. Sua instância do Workfront deve estar ativada no Adobe Identity Management System (IMS) para usar o servidor MCP do Workfront. Se não tiver certeza se sua instância está ativada no IMS, entre em contato com o administrador do Workfront.

+++
