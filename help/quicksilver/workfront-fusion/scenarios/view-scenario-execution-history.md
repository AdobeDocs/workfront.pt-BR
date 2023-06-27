---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exibir o histórico de execução de um cenário no Adobe Workfront Fusion
description: Você pode exibir informações sobre todas as execuções de um cenário ou pesquisar todas as execuções do cenário por dados específicos.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 1%

---

# Exibir o histórico de execução de um cenário em [!DNL Adobe Workfront Fusion]

Você pode exibir informações sobre todas as execuções de um cenário ou pesquisar todas as execuções do cenário por dados específicos.

O histórico de execução de um cenário exibe todas as execuções de um cenário nos últimos 30 dias.

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Exibir todas as execuções de um cenário

### Exibir o histórico de execução do cenário no [!UICONTROL Detalhes do cenário] página

1. Clique em **[!UICONTROL Cenário]** no painel esquerdo e clique no cenário.

   Ou

   Se estiver trabalhando no cenário no Editor de cenários, clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próximo ao canto superior esquerdo da janela.

1. Veja as informações na lista à direita.

   ![](assets/open-history-tab-350x202.png)

   C

   Você também pode clicar em para visualizar uma página inteira dessas informações. A exibição de página inteira permite filtrar o histórico para exibir execuções específicas.

   Os detalhes a seguir são listados para cada execução do cenário:

   * Data em que foi executada **[!UICONTROL Iniciado]**
   * **[!UICONTROL Status]** (êxito ou falha)
   * Executar **[!UICONTROL Duração]**
   * Número de **[!UICONTROL Operações]**
   * Tamanho de **[!UICONTROL Transferência de dados]**
   * Vincular a **[!UICONTROL Detalhes]**

### Exibir o histórico de execução do cenário no [!UICONTROL Histórico] guia

A variável [!UICONTROL Histórico] A guia mostra mais detalhes do que o disponível na [!UICONTROL Detalhes do cenário] página. Também é possível filtrar e classificar as execuções no [!UICONTROL Histórico] guia.

1. Clique em **[!UICONTROL Cenário]** no painel esquerdo e clique no cenário.

   Ou

   Se estiver trabalhando no cenário no Editor de cenários, clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próximo ao canto superior esquerdo da janela.

1. Clique em **[!UICONTROL Histórico]** próximo ao canto superior esquerdo da página
1. (Opcional) Para obter informações detalhadas sobre uma execução de cenário selecionada, incluindo quais pacotes foram processados, clique no link **[!UICONTROL Detalhes]** link.

   Para obter mais informações sobre pacotes de processamento, consulte [Fluxo de execução de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >A variável [!UICONTROL detalhes] O link estará visível somente se a execução tiver detalhes disponíveis.

## Filtrar o histórico de execução do cenário

Você pode filtrar o histórico de execução para exibir somente execuções com os valores especificados.

1. Abra o histórico de página inteira para um cenário conforme descrito em [Exibir o histórico de execução do cenário no [!UICONTROL Histórico] guia](#view-scenario-execution-history-on-the-history-tab) neste artigo.
1. Clique em [!UICONTROL filtro] ícone ![](assets/fusion-scenario-filter-icon.png) no cabeçalho da coluna pela qual você deseja filtrar.
1. No [!UICONTROL filtro] digite os valores pelos quais deseja filtrar.
1. Clique em **[!UICONTROL Salvar]**.

O ícone de filtro está laranja em colunas com um filtro ativo no momento.

## Classificar o histórico de execução do cenário

Você pode classificar o histórico de execução do cenário.

1. Abra o histórico de página inteira para um cenário conforme descrito em [Exibir o histórico de execução do cenário no [!UICONTROL Histórico] guia](#view-scenario-execution-history-on-the-history-tab) neste artigo.
1. Clique em [!UICONTROL Ordenar] ícone no cabeçalho da coluna pela qual você deseja filtrar.
1. Opcional: Para inverter a ordem de classificação, clique no [!UICONTROL Ordenar] ícone novamente.

## Pesquisar todas as execuções de um cenário

1. Clique em **[!UICONTROL Cenário]** ícone ![](assets/scenarios-icon.png) no painel esquerdo, clique no cenário.

   Ou

   Se estiver trabalhando no cenário no Editor de cenários, clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próximo ao canto superior esquerdo da janela.

1. Clique em **[!UICONTROL Histórico]** próximo ao canto superior esquerdo da tela.
1. Clique em **[!UICONTROL Pesquisa de texto completo]** no topo da lista de execuções.

   Ou

   Tipo **Ctrl+Shift+F** (Windows) ou **Cmd+Shift+F** (Mac) A [!UICONTROL Pesquisar no histórico] é aberta.

1. (Opcional) Para pesquisar execuções que contenham texto específico, insira o texto na barra de pesquisa do **[!UICONTROL Pesquisar no histórico]** janela.

   Para procurar um texto exato, coloque o texto entre aspas duplas (&quot;exemplo&quot;).

   >[!INFO]
   >
   >**Exemplo:** Se quiser encontrar a execução que criou um projeto específico, insira a ID do projeto na variável [!UICONTROL Pesquisa de texto completo] barra.
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Opcional) Para limitar sua pesquisa por intervalo de datas, selecione as datas de início e término da pesquisa desejada na [!UICONTROL Por intervalo de datas] área.

   >[!NOTE]
   >
   >* As execuções estão disponíveis somente para os últimos 30 dias.
   >
   >* [!DNL Workfront Fusion] O armazena cargas do webhook por 30 dias. Acessar uma carga de webhook mais de 30 dias após sua criação resulta no erro &quot;[!UICONTROL Falha ao ler o arquivo do armazenamento.]&quot;


1. (Opcional) Para limitar sua pesquisa por status, selecione o status desejado na **[!UICONTROL Por status]** lista suspensa.


   Os status disponíveis são:

   * [!UICONTROL Todos]

   * [!UICONTROL Erro]

   * [!UICONTROL Advertência]

   * [!UICONTROL Êxito]

1. (Opcional) Altere a ordem de exibição dos resultados no **[!UICONTROL Classificar por datas]** lista suspensa.

1. (Opcional) Para copiar uma ID de execução de cenário, clique no link **[!UICONTROL Copiar ID de execução]** ícone <img src="assets/copy-fusion-execution-id-icon.png"> na linha da execução desejada

1. (Opcional) Clique em um resultado da variável [!UICONTROL Pesquisa de texto completo] para examinar o pacote de saída do módulo de cenário que contém as informações.
