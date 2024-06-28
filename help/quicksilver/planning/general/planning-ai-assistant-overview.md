---
title: "Visão geral do Assistente do Adobe Workfront Planning AI"
description: Você pode usar o assistente de IA para gerar, atualizar ou remover registros com base no contexto da página atual e na estrutura de registro. Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: e1e3b8b9f5497af47e14c0f54dfae8f2134b5159
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---


# Visão geral do Assistente do Adobe Workfront Planning AI

<!-- update TOC and miniTOC when making this live-->

>[!IMPORTANT]
>
>As informações neste artigo se referem ao Adobe Workfront Planning e ao Workfront AI Assistant (beta), que são novas ofertas da Adobe Workfront.
>
>Atualmente, o Workfront Planning está em uma fase de acesso antecipado, e o Assistente de IA da Workfront está em uma fase beta.
>
>O Workfront Planning e o AI Assistant (beta) estão abertos para um número limitado de clientes.
>
>Você deve ser um cliente do Workfront para usar esses recursos.
>
>Seu representante de conta informará se você fizer parte deste estágio.
>
>Para obter mais informações, consulte [Visão geral do Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Você pode usar o Assistente de IA para gerar, atualizar ou remover registros com base no contexto da página atual e na estrutura de registro.

Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.

## Considerações sobre o Assistente de IA

* O Assistente de IA está disponível para administradores do Workfront por padrão.

* O administrador do Workfront deve ativar o Assistente de IA para todos os outros usuários. Para obter mais informações, consulte [Ativar ou desativar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* O Assistente de IA funciona no contexto de cada página. As solicitações que você está enviando para o Assistente de IA devem fazer referência à funcionalidade que está disponível na página que você abriu.

* As ações executadas pelo Assistente de IA na área Planejamento se encontram no contexto das permissões do Workfront Planning e do nível de acesso do Workfront. Para obter informações, consulte os seguintes artigos:

   * [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* As alterações feitas pelo Assistente de IA em nome do usuário são rastreadas no painel Histórico do registro.

* Você pode usar comandos para desfazer suas ações. Por exemplo, você pode digitar &quot;Desfazer a última alteração&quot; para reverter a alteração.

## Funcionalidade atualmente disponível para o Assistente de IA

Atualmente, o Assistente de IA está disponível na área Planejamento do Workfront para as seguintes páginas:

* Página do Workspace
* Página de tipo de registro
* Gravar página

Você pode usar o Assistente de IA para executar as seguintes ações neste momento:

* Pesquisar registros. Você pode pesquisar pelas informações contidas em qualquer campo de registro.
* Criar registros. Uma ID com um link para o novo registro é exibida após a criação do registro. Você pode especificar os campos que deseja atualizar durante o processo de criação, como datas ou descrição.
* Crie registros com base em um documento do qual você fez upload. O Workfront é compatível com os seguintes formatos de documento para o Assistente de IA:

  .pptx, .pdf, .docx, .xlsx, .ppt, .doc, .txt e a maioria dos formatos de imagem
* Atualize os campos dos registros exibidos na tela
* Excluir registros
* Restaurar registros que você acabou de excluir

## Acessar o assistente de IA

1. Faça logon no Workfront e acesse o **Planejamento** área.

1. Clique em a **cartão do espaço de trabalho**.

1. (Opcional) Clique em uma **cartão de tipo de registro**.

1. (Opcional) Clique em uma **gravar** para abrir o registro **Detalhes** página.

1. Clique em **Ícone do Assistente de IA** no canto superior direito da tela na barra de navegação global.

   ![](assets/ai-assistant-icon-highlighted.png)

1. No espaço fornecido, comece a digitar comandos para o Assistente de IA e, em seguida, clique em Inserir quando terminar.

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   Por exemplo, você pode digitar um dos seguintes:

   * Crie uma campanha com uma data de início em 4 de julho e uma data de término em 30 de julho
   * Atualize o campo Description do registro Campanha de Verão com data a ser determinada
   * Excluir o último registro
   * Restaurar o registro

   Um indicador visual é exibido enquanto o Assistente de IA processa comandos, definindo expectativas para o tempo de resposta.

   Depois de receber uma resposta bem-sucedida, siga os links fornecidos ou observe as alterações à esquerda.
