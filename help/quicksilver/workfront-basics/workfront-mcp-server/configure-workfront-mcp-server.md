---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configurar o servidor MCP do Adobe Workfront
description: Configure sua instância do Workfront e sua plataforma de IA para trabalhar com o Workfront por meio de uma conversa em idioma natural.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---


# Configurar o servidor MCP do Adobe Workfront

O servidor MCP do [!DNL Adobe Workfront] permite que você trabalhe com seus dados do Workfront por meio de conversações em linguagem natural em uma plataforma de agente de IA compatível, como Claude ou ChatGPT.

Antes de conectar uma plataforma de agente de IA ao Workfront, um administrador do Workfront deve habilitar o acesso ao servidor MCP na instância do Workfront. As etapas exatas para conectar uma plataforma de agente de IA são diferentes para cada plataforma de agente de IA compatível.

Para obter mais informações sobre o servidor Workfront MCP, consulte [Visão geral do servidor Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Plataformas de IA compatíveis

O servidor MCP do Workfront é compatível atualmente com as seguintes plataformas de agente de IA:

* [!DNL Claude]
* [!DNL ChatGPT]

## Pré-requisitos

Antes de conectar o Workfront a uma plataforma de agente de IA, é necessário:

* Ter uma conta [!DNL Adobe Workfront] ativa com permissão para acessar os dados com os quais deseja trabalhar.
* Ter acesso a uma plataforma de agente de IA como o [!DNL Claude].

### Pré-requisitos do administrador

O acesso ao servidor MCP é restringido por dois administradores separados.

* **O administrador do Workfront** controla o acesso ao servidor MCP para sua instância do Workfront. O acesso é ativado por padrão nas Preferências do sistema, portanto, nenhuma ação é necessária, a menos que o administrador tenha escolhido desativá-lo. <!-- TODO: link to the System Preferences AI preferences article once the Enable MCP toggle is documented there. -->

* Se você usar uma versão corporativa de uma plataforma de agente de IA, o administrador dessa plataforma deverá habilitar o conector [!DNL Adobe Workfront] para sua organização.


## Conectar o Workfront ao Claude

Você se conecta ao Workfront uma vez a cada conta [!DNL Claude]. A conexão é autenticada em uma instância específica do Workfront e você permanece conectado até que opte por se desconectar.

### Conectar a partir do diretório de conectores

+++ Expanda para exibir as instruções passo a passo para conectar o Workfront ao [!DNL Claude].

Para conectar o Workfront a [!DNL Claude]:

1. Abrir [!DNL Claude].

1. Navegue até a área conectores.

   <!-- NEEDS DETAIL: Exact menu path (for example, "Click Settings, then click Connectors"). -->

1. Localize **[!DNL Adobe Workfront]** na lista de conectores.

   Caso não o veja, consulte [Pré-requisitos de administração](#admin-prerequisites) neste artigo.

1. Clique em **Conectar**.

   <!-- NEEDS DETAIL: Confirm the exact button label. -->

1. Quando solicitado, faça logon na instância do Workfront.

   <!-- NEEDS DETAIL: Describe the auth flow — does it open a new browser tab, an in-app window, prompt for a Workfront domain? -->

1. Depois que a autenticação for concluída, você estará conectado.

   <!-- NEEDS DETAIL: Add a screenshot of the connected state in Claude. -->

+++

### Conectar-se com um URL

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

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Para obter uma solução de problemas diária depois de se conectar (por exemplo, resultados obsoletos ou comportamento inesperado), consulte [Usar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).


+++


<!--
+++

## Frequently asked questions about setup

+++ Expand to view frequently asked questions about setting up the Workfront MCP server.

### Can I connect to multiple Workfront instances at once?

No. Each connection ties an AI agentic platform to a single Workfront instance. To switch, disconnect and reconnect, authenticating to the new instance.

### Which administrator enables this?

Both your Workfront administrator and the administrator for your AI agentic platform. Your Workfront administrator enables MCP server access on the Workfront side. The administrator for your AI agentic platform enables Workfront access on that platform's side. For [!DNL Claude], the [!DNL Claude] Enterprise administrator enables the [!DNL Adobe Workfront] connector.

+++

-->