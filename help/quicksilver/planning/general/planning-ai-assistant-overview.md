---
title: Visão Geral do Assistente do Adobe Workfront Planning AI
description: Você pode usar o assistente de IA para gerar, atualizar ou remover registros com base no contexto da página atual e na estrutura de registro. Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---


# Visão geral do Assistente do Adobe Workfront Planning AI

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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


## Localize o Assistente de IA no Workfront Planning

Você pode localizar o Assistente de IA nas seguintes áreas do Workfront Planning:

* A barra de navegação principal, no canto superior direito da tela.
* <span class="preview">Dentro da área de detalhes de um registro, após abrir o registro na visualização ou após abrir a página do registro.</span>

## Acessar o Assistente de IA na área Planejamento

1. Faça logon no Workfront e clique no ícone ![](assets/dots-main-menu.png) do **Menu principal**, no canto superior direito da tela, ou no ícone ![](assets/lines-main-menu.png) do **Menu principal**, no canto superior esquerdo, se disponível.

. Clique em **Planning**. A área Planejamento é aberta.

1. Clique em um **cartão de espaço de trabalho**.

1. (Opcional) Clique em um **cartão de tipo de registro**.

1. (Opcional) Clique em um **registro** para abrir a página **Detalhes** do registro.

1. Clique no **ícone do Assistente de IA**, no canto superior direito da tela da barra de navegação global <span class="preview"> ou no canto superior direito da visualização ou página do registro.</span>

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



