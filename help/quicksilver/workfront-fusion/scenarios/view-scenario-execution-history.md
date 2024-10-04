---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exibir o histórico de um cenário no Adobe Workfront Fusion
description: Você pode exibir informações sobre todas as execuções de um cenário ou pesquisar todas as execuções do cenário por dados específicos.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 2e26c4e4b5f331ed2e609381ef442f45e90c4faa
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 0%

---

# Exibir o histórico de um cenário em [!DNL Adobe Workfront Fusion]

Você pode exibir informações sobre os eventos ou execuções de um cenário ou pesquisar todas as execuções do cenário por dados específicos.

A execução de um cenário representa uma única execução do cenário.

Um evento de cenário é uma modificação no cenário, como edição, ativação ou desativação.

>[!NOTE]
>
>O histórico de um cenário exibe todos os eventos e execuções de um cenário nos últimos 30 dias.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Exibir histórico de cenários

### Exibir o histórico de cenários na página [!UICONTROL Detalhes do Cenário]

1. Clique na guia **[!UICONTROL Cenário]** no painel esquerdo e clique no cenário.

   Ou

   Se estiver trabalhando no cenário no Editor de cenários, clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próxima ao canto superior esquerdo da janela.

1. Exiba o histórico de execução na guia **Histórico** do painel à direita.

   Os detalhes a seguir são listados para cada execução do cenário:

   * Data em que a execução foi **[!UICONTROL Iniciada]**
   * **[!UICONTROL Status]** (com êxito ou com falha)
   * Executar **[!UICONTROL Duração]**
   * Número de **[!UICONTROL Operações]**
   * Tamanho de **[!UICONTROL Transferência de Dados]**

   >[!NOTE]
   >
   >O histórico de cenários exibe um selo **Processando** ao lado dos cenários que foram executados recentemente, enquanto os detalhes da execução são gravados no armazenamento. O processamento ocorre imediatamente após a execução do cenário. e não deve durar mais do que alguns minutos. Os detalhes da execução do cenário podem não estar visíveis enquanto a execução estiver sendo processada.

1. Para exibir detalhes da execução de um cenário específico, clique nessa execução no painel direito.
1. Para exibir eventos, clique na guia **Eventos** do painel à direita.


### Exibir histórico de cenários na guia [!UICONTROL Histórico]

A guia [!UICONTROL Histórico] mostra mais detalhes do que o disponível na página [!UICONTROL Detalhes do cenário]. Você também pode filtrar e classificar as execuções na guia [!UICONTROL Histórico].

1. Clique na guia **[!UICONTROL Cenário]** no painel esquerdo e clique no cenário.

   Ou

   Se estiver trabalhando no cenário no Editor de cenários, clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próxima ao canto superior esquerdo da janela.

1. Clique na guia **[!UICONTROL Histórico]** próxima ao canto superior esquerdo da página
1. (Opcional) Para obter informações detalhadas sobre a execução de um cenário selecionado, incluindo quais pacotes foram processados, clique no botão **[!UICONTROL Detalhes]** na linha para essa execução.

   Para obter mais informações sobre o processamento de pacotes, consulte [Fluxo de execução de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* O link [!UICONTROL details] estará visível somente se a execução tiver detalhes disponíveis.
   >
   >* O histórico de cenários exibe um selo **Histórico de processamento** ao lado dos cenários que foram executados recentemente, enquanto os detalhes de execução são gravados no armazenamento. O processamento ocorre imediatamente após a execução do cenário. e não deve durar mais do que alguns minutos. Os detalhes da execução do cenário podem não estar visíveis enquanto a execução estiver sendo processada.

1. Para exibir eventos, habilite a opção **Mostrar eventos**.

## Filtrar o histórico de execução do cenário

Você pode filtrar o histórico de execução para exibir somente execuções com os valores especificados.

1. Abra o histórico de página inteira de um cenário conforme descrito em [Exibir o histórico de execução de cenários na guia [!UICONTROL Histórico]](#view-scenario-execution-history-on-the-history-tab) deste artigo.
1. Clique no ícone ![](assets/fusion-scenario-filter-icon.png) do [!UICONTROL filtro] no cabeçalho da coluna pela qual você deseja filtrar.
1. Na caixa de diálogo [!UICONTROL filtro], insira os valores pelos quais deseja filtrar.
1. Clique em **[!UICONTROL Salvar]**.

O ícone de filtro está laranja em colunas com um filtro ativo no momento.

## Classificar o histórico de execução do cenário

Você pode classificar o histórico de execução do cenário.

1. Abra o histórico de página inteira de um cenário conforme descrito em [Exibir o histórico de execução de cenários na guia [!UICONTROL Histórico]](#view-scenario-execution-history-on-the-history-tab) deste artigo.
1. Clique no ícone [!UICONTROL Classificar] no cabeçalho da coluna pela qual você deseja filtrar.
1. Opcional: Para inverter a ordem de classificação, clique novamente no ícone [!UICONTROL Classificar].

## Pesquisar todas as execuções de um cenário

1. Abra o histórico de página inteira de um cenário conforme descrito em [Exibir o histórico de execução de cenários na guia [!UICONTROL Histórico]](#view-scenario-execution-history-on-the-history-tab) deste artigo.
1. Clique em **[!UICONTROL Pesquisa de texto completo]** na parte superior da lista de execuções.

   Ou

   Digite **Ctrl+Shift+F** (Windows) ou **Cmd+Shift+F** (Mac)
A janela [!UICONTROL Pesquisar no histórico] é aberta.

1. (Opcional) Para procurar execuções que contenham texto específico, insira o texto na barra de pesquisa da janela **[!UICONTROL Pesquisar no histórico]**.

   Para procurar um texto exato, coloque o texto entre aspas duplas (&quot;exemplo&quot;).

   >[!INFO]
   >
   >**Exemplo:** Se quiser encontrar a execução que criou um projeto específico, insira a ID do projeto na barra [!UICONTROL Pesquisa de texto completo].
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Opcional) Para limitar sua pesquisa por intervalo de datas, selecione as datas de início e término da pesquisa desejada na área [!UICONTROL Por intervalo de datas].

   >[!NOTE]
   >
   >* As execuções estão disponíveis somente para os últimos 30 dias.
   >
   >* O [!DNL Workfront Fusion] armazena cargas de webhook por 30 dias. Acessar uma carga de webhook mais de 30 dias após sua criação resulta no erro &quot;[!UICONTROL Falha ao ler arquivo do armazenamento.]&quot;


1. (Opcional) Para limitar sua pesquisa por status, selecione o status desejado na lista suspensa **[!UICONTROL Por status]**.


   Os status disponíveis são:

   * [!UICONTROL Tudo]

   * [!UICONTROL Erro]

   * [!UICONTROL Aviso]

   * [!UICONTROL Êxito]

1. (Opcional) Altere a ordem de exibição dos resultados na lista suspensa **[!UICONTROL Classificar por datas]**.

1. (Opcional) Para copiar uma ID de execução de cenário, clique no ícone **[!UICONTROL Copiar ID de execução]** <img src="assets/copy-fusion-execution-id-icon.png"> na linha da execução desejada

1. (Opcional) Clique em um resultado da [!UICONTROL Pesquisa de texto completo] para examinar o pacote de saída do módulo de cenário que contém as informações.
