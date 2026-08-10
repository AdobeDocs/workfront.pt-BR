---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Habilidades disponíveis para instalação direta
description: O Workfront oferece algumas habilidades que você pode instalar diretamente em seu LLM.
author: Becky
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
source-git-commit: 7fd4c07f2ea1e47e7abb7d3dd78638a6a01d0f47
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Habilidades disponíveis para instalação direta

O Adobe Workfront oferece algumas habilidades que você pode instalar diretamente em seu LLM. As habilidades orientam como essas ferramentas são usadas para tarefas específicas, com as etapas certas já incorporadas.

Você pode encontrar essas habilidades como arquivos no repositório GitHub de habilidades do Adobe. Esse repositório contém arquivos para uma variedade de produtos da Adobe. Quando você baixa esses arquivos e os copia para Claude, Claude pode então usar as habilidades descritas nos arquivos.

Por exemplo, as habilidades do Planning Solution Architect permitem que Claude responda a perguntas sobre o Workfront Planning e execute algumas ações nele.

Não é necessário chamar ou acionar essas habilidades após copiá-las para o LLM. Em vez disso, você pode interagir com o seu LLM como de costume, fazendo perguntas em linguagem natural, e o LLM usa as informações e ações descritas na habilidade que são apropriadas para a conversa.

>[!NOTE]
>
>Atualmente, essas habilidades estão disponíveis apenas para Claude.
>Para obter instruções sobre como configurar o Claude com o Adobe, consulte [Introdução](https://developer.adobe.com/adobe-for-creativity/getting-started/) na documentação do Adobe Developer.

## Instale uma habilidade do repositório GitHub da Workfront no Claude

1. Vá para o [repositório de habilidades do Adobe Workfront](https://github.com/adobe/skills/tree/main/plugins/workfront) no GitHub.
1. Baixe a pasta de habilidades que deseja usar.
1. Copie a pasta na biblioteca de habilidades do Claude.

   * Claude Desktop: `~/Library/Application Support/Claude/skills/` (macOS) ou equivalente.
   * Código Claude: `~/.claude/skills/`.

<!--

1. Go to the [Adobe Workfront skills repository](https://github.com/adobe/skills/tree/main/plugins/workfront) on GitHub.
1. Download the skill file you want to use.
1. In Claude, click **Customize**.
1. Select **Skills**.
1. Click **Create skill** -> **Upload a skill**.
1. Upload the zipped skill file to Claude, then click **Confirm** to install.

-->

## Competências disponíveis no momento

| Habilidade/Link para a pasta | Descrição da habilidade | Disponível para |
|---|---|---|
| [Arquiteto de Soluções do Planning](https://github.com/adobe/skills/tree/main/plugins/workfront/skills/wf-planning-solution-architect) | Configure um espaço de trabalho do Workfront Planning para atender às suas necessidades e responda a perguntas sobre o Workfront Planning. | Claude |
