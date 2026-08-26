---
title: Crie aplicativos App Builder com habilidades no Claude Code
description: Use um conjunto de habilidades do Claude Code para criar aplicativos personalizados do Adobe Workfront App Builder descrevendo o que você deseja, em vez de executar as etapas de configuração e implantação sozinho.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: 366cc4ffea48295b00389b5ee36f2df42b2c8a07
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 4%

---


# Crie aplicativos App Builder com habilidades no Claude Code

Um pacote de habilidades permite que o [!DNL Claude] (ou qualquer recurso de codificação de IA que suporte habilidades formatadas em Claude, como [!DNL Claude Code] ou [!DNL OpenAI Codex]) crie aplicativos [!DNL Adobe App Builder] personalizados para [!DNL Workfront]. Se você tiver acesso a uma dessas ferramentas, poderá criar uma extensão da interface do usuário descrevendo o que deseja em inglês simples, sem exigir experiência do desenvolvedor ou etapas de configuração manual.

As extensões da interface do Workfront, viabilizadas pelo Adobe App Builder, permitem que clientes e parceiros criem experiências do usuário personalizadas. As extensões de interface do usuário permitem modificar a experiência do Workfront de sua organização para atender melhor às necessidades da organização, o que pode aprimorar a eficiência, fornecer experiências contínuas e conectadas, além de melhorar significativamente a satisfação do usuário e ajudar sua organização a realizar sua visão exclusiva.

Para obter mais informações sobre as extensões da interface do usuário do Workfront, consulte [Criar aplicativos personalizados para o Workfront com o Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Habilidades de extensibilidade da interface do usuário

As habilidades de Extensibilidade da interface do usuário permitem que um recurso de codificação de IA gerencie a criação de extensões de interface do usuário no Workfront. Você descreve o recurso desejado e ele faz o trabalho prático, como configurar as ferramentas, criar seu projeto no [!DNL Adobe App Builder], criar o aplicativo, implantá-lo na nuvem da Adobe e executá-lo no Workfront. Você está envolvido no processo somente quando há uma decisão ou logon que requer uma ação sua. Este artigo usa [!DNL Claude] como exemplo, mas as instruções se aplicam a qualquer recurso de codificação de IA com suporte ao Claude Skills.

## Pré-requisitos

Antes de começar, verifique se você tem:

* **Um recurso de codificação de IA compatível com Claude Skills**, como [!DNL Claude Code].

  Para obter mais informações sobre Claude Skills, consulte [O que são habilidades?](https://support.claude.com/en/articles/12512176-what-are-skills) na documentação do Claude.

* **Acesso às habilidades**.

  * Você pode encontrar as habilidades em [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Se este link não abrir para você, peça ao administrador para lhe conceder acesso.
  * As habilidades são publicadas no marketplace de habilidades públicas da Adobe ([adobe/skills](https://github.com/adobe/skills)). Em [!DNL Claude Code], execute:

    ```
    /plugin marketplace add adobe/skills
    ```

    ```
    /plugin install app-builder@adobe-skills
    ```

* Acesso **[!DNL Adobe App Builder], com a função de Desenvolvedor**. Sua organização da Adobe precisa de uma licença do App Builder e você deve ser adicionado como um Desenvolvedor nela. É isso que permite a [!DNL Claude] abrir a Adobe Developer Console e criar seu projeto.

  Para verificar se esse pré-requisito foi atendido:

  1. Abra o [Adobe Developer Console](https://developer.adobe.com/console).
  1. Confirme se a organização mostrada no canto superior direito está correta.
  1. Clique em **Criar novo projeto** > **Criar projeto a partir do modelo**.
  1. Verifique se **App Builder** aparece na lista.

     * Se você vir **App Builder** na lista, você tem acesso.
     * Se não houver a opção **Criar projeto a partir do modelo** ou nenhuma opção **App Builder**, você ainda não terá acesso. Peça ao administrador do Workfront ou do Adobe para adicioná-lo como desenvolvedor (na página Adobe Admin Console > Usuários > Desenvolvedores) e confirmar se sua organização tem uma licença do App Builder.
* **O servidor MCP do Workfront conectou-se**, portanto, [!DNL Claude] usa a API Workfront real em vez de adivinhar os tipos de dados, campos e comandos.

  Para verificar se o servidor MCP do Workfront já está conectado, pergunte [!DNL Claude]: *&quot;Você pode ver os recursos do MCP do Workfront?&quot;*

  Para obter mais informações e instruções, consulte [Conectar o Workfront ao Claude](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#connect-workfront-to-claude)no artigo Configurar o servidor MCP do Adobe Workfront.
