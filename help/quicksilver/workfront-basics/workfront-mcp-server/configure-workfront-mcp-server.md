---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Configurar o servidor MCP do Adobe Workfront
description: Configure sua instância do Workfront e seu assistente de IA para que você possa trabalhar com o Workfront por meio de uma conversa em idioma natural.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 4%

---


# Configurar o servidor MCP do Adobe Workfront

O servidor MCP [!DNL Adobe Workfront] permite que você trabalhe com seus dados do Workfront por meio de uma conversa em linguagem natural em um assistente de IA compatível, como Claude ou ChatGPT.

Antes de conectar um assistente de IA ao Workfront, um administrador do Workfront deve habilitar o acesso ao servidor MCP na instância do Workfront. As etapas exatas para conectar um assistente de IA são diferentes para cada assistente de IA compatível.

Para obter mais informações sobre o servidor Workfront MCP, consulte [Visão geral do servidor Adobe Workfront MCP](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Assistentes de IA compatíveis

O servidor MCP do Workfront atualmente suporta os seguintes assistentes de IA:

* [!DNL Claude]

<!-- NEEDS DETAIL: Update this list as Adobe adds support for additional AI assistants (for example, [!DNL Gemini], or [!DNL Microsoft Copilot]). -->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront package requirement (Select, Prime, Ultimate, Any?) --></p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p><!-- NEEDS DETAIL: Confirm Workfront license requirement (Standard, Work, etc.) --></p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de conectar o Workfront a um assistente de IA, é necessário:

* Ter uma conta [!DNL Adobe Workfront] ativa com permissão para acessar os dados com os quais deseja trabalhar.
* Ter acesso a um assistente de IA como o [!DNL Claude].

  <!-- NEEDS DETAIL: Confirm which Claude tiers are supported. Claude Enterprise is confirmed; Claude Pro and Claude Team support is unconfirmed. -->

### Pré-requisitos do administrador

O acesso ao servidor MCP é restringido por dois administradores separados. Ambos devem habilitar o acesso para que você possa se conectar.

* **O administrador do Workfront** deve habilitar o acesso ao servidor MCP na instância do Workfront.

* Se você usar uma versão corporativa de um assistente de IA, o administrador do assistente de IA deverá habilitar o conector [!DNL Adobe Workfront] para sua organização.


## Conectar o Workfront ao Claude

Você se conecta ao Workfront uma vez a cada conta [!DNL Claude]. A conexão é autenticada em uma instância específica do Workfront e você permanece conectado até que opte por se desconectar.


>[!IMPORTANT]
>
>Se você usa o [!DNL Claude] Enterprise, **o [!DNL Claude] administrador Enterprise** deve habilitar o conector [!DNL Adobe Workfront] para sua organização. Até que o façam, o conector [!DNL Adobe Workfront] não aparecerá quando você procurar por ele em [!DNL Claude]. Contate primeiro o administrador do [!DNL Claude].


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

### Verifique sua conexão

Para confirmar se [!DNL Claude] está conectado ao Workfront, peça a [!DNL Claude] para listar as ações que o servidor MCP do Workfront disponibiliza. Por exemplo:

* *Que ações do Workfront você pode realizar?*
* *Listar as ferramentas do Workfront às quais você tem acesso.*

[!DNL Claude] retorna a lista de ações disponíveis.

<!-- NEEDS DETAIL: Add a screenshot of the tool-list response. -->

### Alternar para uma instância diferente do Workfront

Cada conexão autentica [!DNL Claude] em uma única instância do Workfront. Para usar uma instância diferente, desconecte e reconecte.

Para se conectar a uma instância diferente do Workfront:

1. Em [!DNL Claude], desconecte o conector [!DNL Adobe Workfront].
1. Reconecte o conector.
1. Autentique para a nova instância do Workfront.

>[!NOTE]
>
>Fazer logout de [!DNL Claude] sozinho não alterna a instância do Workfront. Você deve desconectar e reconectar o conector.

## Personalizar o comportamento do Claude com habilidades

<!-- NEEDS DETAIL: Confirm whether Adobe is shipping any pre-built Claude skills alongside the MCP server. If yes, list them and link to download or installation guidance. If no, decide whether to mention skills as a user-driven workaround at all, or remove this section. -->

[!DNL Claude] dá suporte a conjuntos de instruções criados pelo usuário chamados habilidades. Você pode usar uma habilidade para personalizar como [!DNL Claude] se comporta com o Workfront. Por exemplo, você pode criar uma habilidade que diga a [!DNL Claude] para sempre buscar dados novos do Workfront em vez de depender de resultados anteriores.

## Solução de problemas de configuração e autenticação

| Problema | Causa provável | Corrigir |
|---|---|---|
| Você não pode encontrar o conector [!DNL Adobe Workfront] em [!DNL Claude]. | O administrador do [!DNL Claude] não o habilitou. | Contate o administrador do [!DNL Claude] (não o administrador do Workfront) e peça que ele habilite o conector [!DNL Adobe Workfront]. |
| Você se conectou, mas não pode ver seus dados. | Você autenticou na instância incorreta do Workfront. | Desconecte o conector, reconecte e autentique na instância correta. |
| Falha na autenticação ou a conexão parou de funcionar. | Sua sessão de autenticação expirou ou há um erro de conexão. | Desconecte e reconecte o conector. |
| Você deseja alternar para uma instância diferente do Workfront. | Uma única conexão vincula você a uma instância. | Desconecte, reconecte e autentique na nova instância. |

<!-- NEEDS DETAIL: Add additional setup/authentication troubleshooting scenarios discovered during hands-on testing. -->

Para obter uma solução de problemas diária depois de se conectar (por exemplo, resultados obsoletos ou comportamento inesperado), consulte [Usar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).

## Perguntas frequentes sobre configuração

### Posso me conectar a várias instâncias do Workfront de uma só vez?

Não. Cada conexão vincula um assistente de IA a uma única instância do Workfront. Para alternar, desconecte e reconecte, autenticando para a nova instância.

### Isso funciona com Claude Pro ou Claude Team, ou apenas com Claude Enterprise?

<!-- NEEDS DETAIL: Confirm Claude tier support and answer this directly. -->

### Qual administrador habilita isto?

O administrador do Workfront e o administrador do assistente de IA. O administrador do Workfront habilita o acesso ao servidor MCP no Workfront. O administrador do assistente de IA habilita o acesso ao Workfront no lado do assistente de IA. Para [!DNL Claude], o administrador corporativo [!DNL Claude] habilita o conector [!DNL Adobe Workfront].
