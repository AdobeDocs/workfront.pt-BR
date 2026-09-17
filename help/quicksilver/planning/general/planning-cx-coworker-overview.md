---
title: Visão Geral do Adobe Workfront Planning CX Coworker
description: Você pode usar o CX Coworker no Workfront Planning para executar ações semelhantes a registros e outros objetos no Planning que normalmente seriam executados na interface. Os comandos do usuário e a execução desses comandos pela IA trabalham juntos para garantir que as alterações feitas pela IA sejam refletidas com precisão no ambiente.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: d5f36e0c8dbd9749503de25b75e70bf18b1d187b
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 5%
---

# Visão geral do Adobe Workfront Planning CX Coworker


<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Após o lançamento para Pré-visualização, os mesmos recursos também estarão disponíveis mensalmente no ambiente de Produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

O CX Coworker é uma interface conversacional em que você descreve uma meta em linguagem simples e, em seguida, planeja, executa e valida o trabalho em todos os sistemas Adobe e conectados antes de trazê-lo de volta para sua aprovação.

O CX Coworker preserva tudo o que o AI Assistant faz hoje e, ao mesmo tempo, adiciona recursos completos mais avançados em uma nova experiência de tela cheia e no painel direito do Workfront.

Ela opera nos controles de acesso de nível de produto existentes em sua organização, de modo que os usuários só podem realizar ações para as quais já têm permissão no Workfront, com acesso somente leitura por padrão e acesso de gravação controlado por administradores do Workfront.

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
<p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p>
Ou
<p>Qualquer pacote do Planning quando adquirido como um produto independente</p>
   </td> </tr>
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td>  
   <p>O administrador deve fazer o seguinte para permitir o acesso ao CX Coworker no Planning:</p>
   <ul>
   <li><p>Adicione um Workflow e um tipo de licença do Planning ao seu nível de acesso quando você tiver um Workflow e um pacote do Planning</p></li>
   <li><p>Desmarque Desativar o painel CX Coworker na configuração do Workfront no seu nível de acesso. Ela é selecionada por padrão.</p></li></ul>
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Configurações do sistema</p></td> 
   <td>   <p>O administrador do Workfront deve selecionar as ferramentas MCP somente leitura e somente gravação na área Preferências do sistema da Configuração. As ferramentas de MCP somente leitura são selecionadas por padrão.</p> 
    </td> 
  </tr> 
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerações para a CX Coworker

* A CX Coworker deve estar ativada para sua organização antes de estar disponível para os usuários em sua empresa.

  Para obter informações, consulte [visão geral do CX Coworker](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

* Depois que a Workfront ativar o agente para sua organização, ele estará disponível para o administrador principal do Workfront. Para obter informações, consulte [Configurar informações básicas do sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* O administrador do Workfront deve ativar o Assistente de IA para todos os outros usuários. Para obter mais informações, consulte [Habilitar ou desabilitar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* O Assistente de IA funciona no contexto de cada página. As solicitações que você está enviando para o Assistente de IA devem fazer referência à funcionalidade que está disponível na página que você abriu.

* As ações executadas pelo Assistente de IA na área Planejamento se encontram no contexto das permissões do Workfront Planning e do nível de acesso do Workfront. Para obter informações, consulte os seguintes artigos:

  * [Visão geral das permissões de compartilhamento no Planejamento do Adobe Workfront](/help/quicksilver/planning/access/sharing-permissions-overview.md)
  * [Visão geral dos tipos de licença ao usar o Planejamento do Adobe Workfront](/help/quicksilver/planning/access/license-type-overview.md)

* As alterações feitas pelo Assistente de IA em nome do usuário são rastreadas no painel Histórico do registro.

* As ações realizadas pelo Assistente de IA são permanentes e podem ser irreversíveis. Por exemplo, a exclusão de um campo não pode ser revertida. Analise todas as ações propostas pelo Assistente de IA antes de aceitá-las.

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

1. Faça logon no Workfront, clique no ícone **Menu Principal** ![Menu principal Linhas](assets/lines-main-menu.png) no canto superior esquerdo e clique em **Planning**.

   A área Planejamento é aberta.

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



