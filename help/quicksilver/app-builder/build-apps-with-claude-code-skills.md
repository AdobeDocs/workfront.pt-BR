---
title: Crie aplicativos App Builder com habilidades no Claude Code
description: Use um conjunto de habilidades do Claude Code para criar aplicativos personalizados do Adobe Workfront App Builder descrevendo o que você deseja, em vez de executar as etapas de configuração e implantação sozinho.
author: Becky
feature: Digital Content and Documents
hide: true
source-git-commit: e5a288dcac20be9176d1541d531edaf0d8c99a8c
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 5%

---


# Crie aplicativos App Builder com habilidades no Claude Code

Um conjunto de habilidades do [!DNL Claude Code] permite que o [!DNL Claude] crie aplicativos [!DNL Adobe App Builder] personalizados para [!DNL Workfront]. Isso significa que você pode criar um descrevendo o que deseja em inglês simples, sem ser um desenvolvedor ou escrever as etapas de configuração sozinho.

As extensões da interface do Workfront, viabilizadas pelo Adobe App Builder, permitem que clientes e parceiros criem experiências do usuário personalizadas. As extensões de interface do usuário permitem modificar a experiência do Workfront de sua organização para atender melhor às necessidades da organização, o que pode aprimorar a eficiência, fornecer experiências contínuas e conectadas, além de melhorar significativamente a satisfação do usuário e ajudar sua organização a realizar sua visão exclusiva.

Para obter mais informações sobre as extensões da interface do usuário do Workfront, consulte [Criar aplicativos personalizados para o Workfront com o Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Habilidades de extensibilidade da interface do usuário para Claude

Desenvolver o [!DNL Adobe App Builder] pode ser bastante técnico, o que pode criar barreiras se o usuário não estiver familiarizado com o procedimento ou as técnicas. As habilidades de Extensibilidade da Interface do Usuário simplificam esse processo usando o [!DNL Claude]. Você descreve o recurso desejado e o [!DNL Claude] faz o trabalho prático, como configurar as ferramentas, criar seu projeto no [!DNL Adobe App Builder], criar o aplicativo, implantá-lo na nuvem da Adobe e executá-lo no Workfront. Você está envolvido no processo somente quando há uma decisão ou logon que requer uma ação sua.

## Pré-requisitos

Antes de começar, verifique se você tem:

* **[!DNL Claude Code]** instalado.
* **Acesso às habilidades**.

  * Você pode encontrar as habilidades em [https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md](https://github.com/adobe/skills/blob/main/plugins/app-builder/skills/appbuilder-workfront/SKILL.md).

    Se este link não abrir para você, peça ao administrador para lhe conceder acesso.
  * Após baixar as habilidades, execute os comandos a seguir para configurá-las.

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
