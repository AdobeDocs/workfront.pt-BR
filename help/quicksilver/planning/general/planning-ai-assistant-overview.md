---
title: Visão Geral do Assistente do Adobe Workfront Planning AI
description: Você pode usar o assistente de IA para gerar, atualizar ou remover registros com base no contexto da página atual e na estrutura de registro. Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 7%

---


# Visão geral do Assistente de IA do Planejamento do Adobe Workfront

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


{{planning-important-intro}}

You can use the AI Assistant to generate, update, or remove records based on the current page context and record structure.

Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e do Planning</p>
<p>Qualquer pacote de Fluxo de Trabalho e Planejamento</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations about the AI Assistant

* The AI Assistant must be enabled for your organization before it is available for users in your company. For information, see [AI Assistant overview](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* After Workfront has enabled the AI Assistant for your organization, it is available for the main Workfront administrator. For information, see [Configure basic information for your system](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* The Workfront administrator must enable the AI Assistant for all other users. Para obter mais informações, consulte [Habilitar ou desabilitar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* O Assistente de IA funciona no contexto de cada página. As solicitações que você está enviando para o Assistente de IA devem fazer referência à funcionalidade que está disponível na página que você abriu.

* As ações executadas pelo Assistente de IA na área Planejamento se encontram no contexto das permissões do Workfront Planning e do nível de acesso do Workfront. Para obter informações, consulte os seguintes artigos:

   * [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Visão geral dos tipos de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* As alterações feitas pelo Assistente de IA em nome do usuário são rastreadas no painel Histórico do registro.

* As ações realizadas pelo Assistente de IA são permanentes e podem ser irreversíveis. Por exemplo, a exclusão de um campo não pode ser revertida. Analise todas as ações propostas pelo Assistente de IA antes de aceitá-las.

* Ao criar, atualizar ou excluir um objeto por meio do AI Assistant, o AI Assistant exibe as ações desejadas e solicita a confirmação. Você pode confirmar ou cancelar as ações.

## Funcionalidade atualmente disponível para o Assistente de IA

Atualmente, o Assistente de IA está disponível na área Planejamento do Workfront para as seguintes páginas:

* Página do Workspace
* Página de tipo de registro
* Gravar página

Você pode usar o Assistente de IA para executar as seguintes ações neste momento:

* Search for records. You can search by information contained in any record fields.
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description.
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT e a maioria dos formatos de imagem
* Atualize os campos dos registros exibidos na tela
* Excluir registros
* Restore records that you just deleted


## Localize o Assistente de IA no Workfront Planning

Você pode localizar o Assistente de IA nas seguintes áreas do Workfront Planning:

* A barra de navegação principal, no canto superior direito da tela.
* Dentro da área de detalhes de um registro, após abrir o registro na visualização ou após abrir a página do registro.

## Acessar o Assistente de IA na área Planejamento

1. Faça logon no Workfront, clique no ícone **Menu Principal** ![Menu principal Linhas](assets/lines-main-menu.png) no canto superior esquerdo e clique em **Planning**.

   A área Planejamento é aberta.

1. Clique em um **cartão de espaço de trabalho**.

1. (Optional) Click a **record type card**.

1. (Optional) Click a **record** to open the record&#39;s **Details** page.

1. Click the **AI Assistant icon** in the upper-right corner of the screen in the global navigation bar or in the upper-right corner of the record&#39;s preview or page.

   ![AI Assistant icon](assets/ai-assistant-icon-highlighted.png)

1. In the space provided, start typing commands for the AI Assistant, then click Enter when you are done.

   ![Painel do Assistente de IA com caixa de comando vazia](assets/ai-assistant-panel-with-empty-command-box.png)

   Por exemplo, você pode digitar um dos seguintes:

   * Crie uma campanha com uma data de início em 4 de julho e uma data de término em 30 de julho
   * Atualize o campo Description do registro Campanha de Verão com data a ser determinada
   * Delete the last record
   * Restaurar o registro

   Um indicador visual é exibido enquanto o Assistente de IA processa comandos, definindo expectativas para o tempo de resposta.

   Depois de receber uma resposta bem-sucedida, siga os links fornecidos ou observe as alterações à esquerda.



