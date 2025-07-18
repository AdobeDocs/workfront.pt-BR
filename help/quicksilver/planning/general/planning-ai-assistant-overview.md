---
title: Visão Geral do Assistente do Adobe Workfront Planning AI
description: Você pode usar o assistente de IA para gerar, atualizar ou remover registros com base no contexto da página atual e na estrutura de registro. Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: a36968bdae5756f0f8283da04a2afca83b4dd94a
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---


# Visão geral do Assistente do Adobe Workfront Planning AI

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

Você pode usar o Assistente de IA para gerar, atualizar ou remover registros com base no contexto da página atual e na estrutura de registro.

Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.

## Considerações sobre o Assistente de IA

* O Assistente de IA deve estar ativado para sua organização antes de estar disponível para usuários em sua empresa. Para obter informações, consulte [Visão geral do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Depois que a Workfront ativar o Assistente de IA para sua organização, ele estará disponível para o administrador principal do Workfront. Para obter informações, consulte [Configurar informações básicas do sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* O administrador do Workfront deve ativar o Assistente de IA para todos os outros usuários. Para obter mais informações, consulte [Habilitar ou desabilitar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* O Assistente de IA funciona no contexto de cada página. As solicitações que você está enviando para o Assistente de IA devem fazer referência à funcionalidade que está disponível na página que você abriu.

* As ações executadas pelo Assistente de IA na área Planejamento se encontram no contexto das permissões do Workfront Planning e do nível de acesso do Workfront. Para obter informações, consulte os seguintes artigos:

   * [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* As alterações feitas pelo Assistente de IA em nome do usuário são rastreadas no painel Histórico do registro.

* Você pode usar comandos para desfazer suas ações. Por exemplo, você pode digitar &quot;Desfazer a última alteração&quot; para reverter a alteração.

* Ao criar, atualizar ou excluir um objeto por meio do AI Assistant, o AI Assistant exibe as ações desejadas e solicita a confirmação. Você pode confirmar ou cancelar as ações.

## Funcionalidade atualmente disponível para o Assistente de IA

Atualmente, o Assistente de IA está disponível na área Planejamento do Workfront para as seguintes páginas:

* Página do Workspace
* Página de tipo de registro
* Gravar página

Você pode usar o Assistente de IA para executar as seguintes ações neste momento:

* Pesquisar registros. Você pode pesquisar pelas informações contidas em qualquer campo de registro.
* Criar registros. Uma ID com um link para o novo registro é exibida após a criação do registro. Você pode especificar os campos que deseja atualizar durante o processo de criação, como datas ou descrição.
* Crie registros com base em um documento do qual você fez upload. O Workfront é compatível com os seguintes formatos de documento para o Assistente de IA:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT e a maioria dos formatos de imagem
* Atualize os campos dos registros exibidos na tela
* Excluir registros
* Restaurar registros que você acabou de excluir


## Localize o Assistente de IA no Workfront Planning

Você pode localizar o Assistente de IA nas seguintes áreas do Workfront Planning:

* A barra de navegação principal, no canto superior direito da tela.
* Dentro da área de detalhes de um registro, após abrir o registro na visualização ou após abrir a página do registro.

## Acessar o Assistente de IA na área Planejamento

1. Faça logon no Workfront e clique no ícone **Menu Principal**, ![Menu principal Pontos](assets/dots-main-menu.png), no canto superior direito da tela, ou no ícone **Menu Principal**, ![Menu principal Linhas](assets/lines-main-menu.png), no canto superior esquerdo, se disponível.

. Clique em **Planning**. A área Planejamento é aberta.

1. Clique em um **cartão de espaço de trabalho**.

1. (Opcional) Clique em um **cartão de tipo de registro**.

1. (Opcional) Clique em um **registro** para abrir a página **Detalhes** do registro.

1. Clique no **ícone do Assistente de IA**, no canto superior direito da tela da barra de navegação global ou no canto superior direito da visualização ou página do registro.

   ![Ícone do Assistente de IA](assets/ai-assistant-icon-highlighted.png)

1. No espaço fornecido, comece a digitar comandos para o Assistente de IA e, em seguida, clique em Inserir quando terminar.

   ![Painel do Assistente de IA com caixa de comando vazia](assets/ai-assistant-panel-with-empty-command-box.png)

   Por exemplo, você pode digitar um dos seguintes:

   * Crie uma campanha com uma data de início em 4 de julho e uma data de término em 30 de julho
   * Atualize o campo Description do registro Campanha de Verão com data a ser determinada
   * Excluir o último registro
   * Restaurar o registro

   Um indicador visual é exibido enquanto o Assistente de IA processa comandos, definindo expectativas para o tempo de resposta.

   Depois de receber uma resposta bem-sucedida, siga os links fornecidos ou observe as alterações à esquerda.



