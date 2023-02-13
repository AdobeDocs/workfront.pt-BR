---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visualizar o histórico de execução de um cenário no Adobe Workfront Fusion
description: Você pode exibir informações sobre todas as execuções de um cenário ou pesquisar todas as execuções do cenário para obter dados específicos.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# Visualize o histórico de execução de um cenário em [!DNL Adobe Workfront Fusion]

Você pode exibir informações sobre todas as execuções de um cenário ou pesquisar todas as execuções do cenário para obter dados específicos.

O histórico de execução de um cenário exibe todas as execuções de um cenário dos últimos 30 dias.

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
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Exibir todas as execuções de um cenário

### Exibir o histórico de execução do cenário no [!UICONTROL Detalhe do cenário] página

1. Clique no botão **[!UICONTROL Cenário]** no painel esquerdo e, em seguida, clique no cenário.

   Ou

   Se você estiver trabalhando no cenário no Editor de cenário, clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próximo ao canto superior esquerdo da janela.

1. Exiba as informações na lista à direita.

   ![](assets/open-history-tab-350x202.png)

   C

   Você também pode clicar em para ver uma exibição de página completa dessas informações. A exibição de página inteira permite filtrar o histórico para exibir execuções específicas.

   Os detalhes a seguir são listados para cada execução do cenário:

   * Data em que a execução foi **[!UICONTROL Iniciado]**
   * **[!UICONTROL Status]** (sucesso ou falha)
   * Executar **[!UICONTROL Duração]**
   * Número de **[!UICONTROL Operações]**
   * Tamanho da **[!UICONTROL Transferência de dados]**
   * Link para **[!UICONTROL Detalhes]**

### Exibir o histórico de execução do cenário no [!UICONTROL Histórico] guia

O [!UICONTROL Histórico] mostra mais detalhes do que o disponível na guia [!UICONTROL Detalhes do cenário] página. Você também pode filtrar e classificar as execuções no [!UICONTROL Histórico] guia .

1. Clique no botão **[!UICONTROL Cenário]** no painel esquerdo e, em seguida, clique no cenário.

   Ou

   Se você estiver trabalhando no cenário no Editor de cenário, clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próximo ao canto superior esquerdo da janela.

1. Clique no botão **[!UICONTROL Histórico]** próximo ao canto superior esquerdo da página
1. (Opcional) Para obter informações detalhadas sobre uma execução de cenário selecionada, incluindo quais pacotes foram processados, clique no link **[!UICONTROL Detalhes]** link .

   Para obter mais informações sobre pacotes de processamento, consulte [Fluxo de execução do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >O [!UICONTROL detalhes] link fica visível somente se a execução tiver detalhes disponíveis.

## Filtrar o histórico de execução do cenário

Você pode filtrar o histórico de execução para exibir somente as execuções com os valores especificados.

1. Abra o histórico de páginas completo para um cenário, como descrito em [Exibir o histórico de execução do cenário no [!UICONTROL Histórico] guia](#view-scenario-execution-history-on-the-history-tab) neste artigo.
1. Clique no botão [!UICONTROL filter] ícone ![](assets/fusion-scenario-filter-icon.png) no cabeçalho da coluna que deseja filtrar.
1. No [!UICONTROL filter] digite os valores que deseja filtrar.
1. Clique em **[!UICONTROL Salvar]**.

O ícone de filtro é laranja em colunas com um filtro ativo no momento.

## Classifique o histórico de execução do cenário

Você pode classificar o histórico de execução do cenário.

1. Abra o histórico de páginas completo para um cenário, como descrito em [Exibir o histórico de execução do cenário no [!UICONTROL Histórico] guia](#view-scenario-execution-history-on-the-history-tab) neste artigo.
1. Clique no botão [!UICONTROL Classificar] no cabeçalho da coluna que deseja filtrar.
1. Opcional: Para inverter a ordem da classificação, clique no botão [!UICONTROL Classificar] ícone novamente.

## Pesquisar todas as execuções de um cenário

1. Clique no botão **[!UICONTROL Cenário]** ícone ![](assets/scenarios-icon.png) no painel esquerdo, em seguida, clique no cenário .

   Ou

   Se você estiver trabalhando no cenário no Editor de cenário, clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próximo ao canto superior esquerdo da janela.

1. Clique no botão **[!UICONTROL Histórico]** próximo ao canto superior esquerdo da tela.
1. Clique em **[!UICONTROL Pesquisa de texto completo]** na parte superior da lista de execuções.

   Ou

   Tipo **Ctrl+Shift+F** (Windows) ou **Cmd+Shift+F** (Mac) A variável [!UICONTROL Pesquisar no histórico] será aberta.

1. (Opcional) Para pesquisar execuções que contenham texto específico, insira o texto na barra de pesquisa do **[!UICONTROL Pesquisar no histórico]** janela.

   Para procurar texto exato, coloque o texto entre aspas duplas (&quot;exemplo&quot;).

   >[!INFO]
   >
   >**Exemplo:** Se quiser encontrar a execução que criou um projeto específico, insira a ID do projeto no [!UICONTROL Pesquisa de texto completo] bar.
   >
   >&quot;625ef2ef006036bd1794b6e52d737c5&quot;

1. (Opcional) Para limitar sua pesquisa por intervalo de datas, selecione as datas de início e término da pesquisa desejada na [!UICONTROL Por intervalo de datas] área.

   >[!NOTE]
   >
   >* As execuções só estão disponíveis nos 30 dias anteriores.
   >
   >* [!DNL Workfront Fusion] armazena cargas do webhook por 30 dias. Acessar uma carga do webhook mais de 30 dias após sua criação resulta no erro &quot;[!UICONTROL Falha ao ler arquivo do armazenamento.]&quot;



1. (Opcional) Para limitar sua pesquisa por status, selecione o status desejado na variável **[!UICONTROL Por status]** lista suspensa.


   Os status disponíveis são:

   * [!UICONTROL Todas]

   * [!UICONTROL Erro]

   * [!UICONTROL Advertência]

   * [!UICONTROL Êxito]

1. (Opcional) Altere a ordem em que os resultados são exibidos na variável **[!UICONTROL Classificar por datas]** lista suspensa.

1. (Opcional) Para copiar uma ID de execução de cenário, clique no botão **[!UICONTROL Copiar ID de execução]** ícone <img src="assets/copy-fusion-execution-id-icon.png"> na linha da execução desejada

1. (Opcional) Clique em um resultado da variável [!UICONTROL Pesquisa de texto completo] para examinar o pacote de saída do módulo de cenário que contém as informações.
