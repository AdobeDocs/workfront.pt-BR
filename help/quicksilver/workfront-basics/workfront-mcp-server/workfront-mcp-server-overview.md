---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Visão geral do servidor Adobe Workfront MCP
description: Saiba o que o servidor MCP do Adobe Workfront faz e como ele permite trabalhar com o Workfront por meio de conversas em linguagem natural em uma plataforma de agente de IA.
author: Courtney
feature: Get Started with Workfront
source-git-commit: e7dadae62ea2f5e9772705cafdc5e067cec1ae08
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 0%

---


# Visão geral do servidor Adobe Workfront MCP

{{highlighted-preview-article-level}}


O servidor MCP [!DNL Adobe Workfront] conecta sua instância do Workfront a uma plataforma de agente de IA, como [!DNL Claude] ou [!DNL ChatGPT]. Na plataforma do agente de IA, é possível encontrar, criar, atualizar e gerenciar itens do Workfront fazendo solicitações em linguagem natural.

Por exemplo, você pode perguntar:

* *Mostre-me todos os projetos ativos para a equipe de Marketing da Marca.*
* *Atualize a tarefa &quot;Revisão de Design&quot; para que ela termine em 18 de abril.*
* *Envie um lembrete para os aprovadores do ativo &quot;Vídeo da Campanha da primavera&quot; que não responderam.*

Você não precisa saber a API do Workfront ou como os servidores MCP funcionam para usar o servidor MCP do Workfront.

>[!IMPORTANT]
>
>Atualmente, o servidor MCP do Workfront está disponível somente para clientes na região dos EUA que usam o AWS.

## O que é um servidor MCP

Um servidor MCP é um ponto de conexão que permite que uma plataforma de IA funcione com outro sistema. O servidor MCP do Workfront é o que sua plataforma de IA Agentic se conecta para que possa ler e agir em seus dados do Workfront em seu nome.

MCP significa Protocolo de Contexto de Modelo. Esse é o padrão que define como as plataformas de agentes de IA e os sistemas externos se comunicam entre si.

## Configurar a conexão

O servidor MCP do Workfront funciona com qualquer plataforma de agente de IA compatível com MCP, como [!DNL Claude] ou [!DNL ChatGPT]. Antes de poder usá-lo, o seguinte precisa acontecer:

* Um administrador do Workfront deve habilitar o acesso ao servidor MCP na instância do Workfront.
* Você (ou o administrador) deve conectar a plataforma de agente de IA à Workfront.

Para obter mais informações, consulte [Configurar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Começar a usar o servidor MCP do Workfront

Após a configuração, você pode solicitar que sua plataforma de IA Agent localize, crie, atualize e gerencie itens do Workfront em linguagem natural.

Para obter mais informações, incluindo exemplos de solicitações, itens que devem ser considerados e informações sobre dados e segurança, consulte [Usar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md).
