---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1628'
ht-degree: 0%

---

# Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Mapear informações de um módulo para outro](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-data-from-one-to-another.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

O mapeamento é o processo de atribuir as saídas de um módulo, estruturadas em itens, aos campos de entrada de outro módulo.

O painel de mapeamento é exibido ao clicar em um campo no qual você deseja inserir um valor emitido de um módulo anterior em um cenário. Em um módulo, em qualquer campo disponível para mapeamento, é possível criar uma fórmula usando qualquer combinação de funções e itens mapeados do painel de mapeamento com texto estático digitado. Esses elementos podem ser aninhados um dentro do outro.

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pacotes e itens

A operação de um módulo produz zero, um ou mais pacotes como sua saída. Um pacote consiste em um ou mais itens.

Para explorar a saída de um módulo:

1. Clique em **[!UICONTROL Executar uma vez]** para executar o módulo.
1. Clique no balão acima do módulo.

   Um registro contendo todas as fases do módulo é exibido. Você pode encontrar o(s) pacote(s) emitido(s) pela fase de operação de um módulo no cabeçalho **[!UICONTROL Saída]**. Cada pacote contém seus itens e os valores de cada item.

>[!INFO]
>
>**Exemplo:** este exemplo mostra o módulo [!UICONTROL Email] > [!UICONTROL Assistir emails]. Você pode ver que ela executou 1 operação produzindo um único pacote que contém vários itens, como `Date`, `Email ID (UID)`, `size` e assim por diante.
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>As saídas dos módulos entre um [!UICONTROL Iterador] e um [!UICONTROL Agregador] não estão acessíveis além do módulo [!UICONTROL Agregador].

## Mapear um item

Depois de criar uma sequência de módulos vinculando dois ou mais deles, cada módulo pode processar valores de itens gerados pelos módulos que o precedem.

Para atribuir os itens aos campos de entrada de um módulo:

1. Clique no módulo que deve processar a saída dos módulos anteriores.
1. No painel Configurações do módulo que é exibido, clique em um campo onde você deseja usar o valor de um item emitido de um ou mais módulos anteriores.

   O painel de mapeamento é aberto.

1. Clique em um item no painel de mapeamento para inseri-lo no campo.
1. (Opcional) Para pesquisar um campo específico no painel de mapeamento, clique na barra de pesquisa do painel de mapeamento e digite o termo que deseja pesquisar. Clique no campo quando ele aparecer na lista.

   Os resultados da pesquisa contêm o termo de pesquisa e não diferenciam maiúsculas de minúsculas.

Para obter mais informações, consulte [Definir as configurações de um módulo em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## Fórmulas

Você pode mapear vários itens em um campo, combiná-los com literais (valores fixos) e empregar Operadores e Funções para criar fórmulas complexas:

![](assets/operators-and-functions.png)

Você pode encontrar as funções e os operadores no painel de mapeamento em uma de suas guias.

![](assets/functions-toolbar-350x189.png)

A primeira guia ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (exibida ao abrir o painel) exibe os itens que você pode mapear de outros módulos.

As outras guias contêm os seguintes tipos de funções:

* **Funções gerais** ![](assets/toolbar-icon-general-function.png) - Consulte [Funções gerais em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) para obter mais informações.

* **Funções matemáticas** ![](assets/toolbar-icon-math-functions.png) - Consulte [Funções matemáticas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) para obter mais informações.

* **Funções de texto e binárias** ![](assets/toolbar-icon-text&binary-functions.png) - Consulte [Funções de cadeia de caracteres em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) para obter mais informações.

* **Data e hora** ![](assets/toolbar-icon-date&time-functions.png) - Consulte as [funções de data e hora em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) e os artigos abaixo para obter mais informações.

   * [Tokens para formatação de data e hora em  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens para análise de data e hora no Adobe Workfront Fusion](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funções para trabalhar com matrizes** ![](assets/toolbar-icon-functions-for-arrays.png) - Consulte [Funções de matriz em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) para obter mais informações.

>[!TIP]
>
>Ao criar uma fórmula complexa que deseja reutilizar em outro campo, você pode clicar no campo que contém a combinação, usar Command-A ou Ctrl-A para selecioná-lo e, em seguida, copiá-lo e colá-lo no outro campo.

Para obter mais informações sobre como mapear itens usando funções, consulte [Mapear itens usando funções em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## Coleções

Alguns itens podem conter vários valores de vários tipos. Estes são itens do tipo coleção.

Você pode identificar um item do tipo [!UICONTROL coleção] pelo retângulo preto pequeno exibido à direita do rótulo do item e sua lista de subitens expandida automaticamente:

![](assets/collection.png)

>[!NOTE]
>
>Na maioria dos casos, você mapeia os subitens da coleção em vez do item que representa a coleção inteira.

Para obter mais informações sobre coleções, consulte [Tipos de dados de item no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

## Matrizes

Alguns itens podem conter vários elementos do mesmo tipo. Esses itens são do tipo matriz.

Você pode identificar um item do tipo matriz pelos colchetes no final do rótulo do item. Clique no pequeno retângulo preto à direita do rótulo do item para revelar os itens do elemento:

![](assets/array.png)

Para obter mais informações sobre matrizes, consulte [Tipos de dados do item em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### Mapear o primeiro elemento de uma matriz

Se você mapear o item `Recipient name` de uma matriz, ele será exibido no campo da seguinte maneira:

![](assets/map-array-1st-element.png)

O número entre colchetes é um índice que determina qual elemento da matriz será usado. É definido como 1 por padrão.

### Mapear o elemento n-ésimo de uma matriz

Se quiser acessar outro elemento, clique nos colchetes e edite o valor do índice:

![](assets/access-another-element.png)

### Mapear um elemento de matriz com uma determinada chave

Algumas matrizes contêm várias coleções com itens de chave e valor. Normalmente, são vários metadados, atributos e assim por diante.

O exemplo a seguir mostra a saída do aplicativo [!DNL Jira].

![](assets/output-of-jira-app-350x100.png)

Neste exemplo, obtemos um nome de arquivo de uma matriz de anexos para o anexo específico com uma ID 10108.

A saída de [!DNL Jira] tem esta aparência:

![](assets/output-from-jira-350x261.png)

O requisito típico é pesquisar um elemento por seu valor de chave determinado e obter o valor correspondente do item de valor. Isso pode ser feito com uma fórmula que emprega uma combinação das funções `map()` e `get()`.

Veja a seguir um detalhamento da fórmula:

1. O primeiro parâmetro da função `map()` é o item de matriz inteiro.
1. O segundo parâmetro é o nome bruto do item de valor. Para obter o nome bruto, passe o mouse sobre o item no painel [!UICONTROL mapeamento]:

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >Todos os parâmetros diferenciam maiúsculas de minúsculas. Mesmo que, neste exemplo específico, o rótulo do item difira de seu nome bruto apenas em maiúsculas, é necessário usar o nome bruto, que é um valor em minúsculas em contraste com o Valor do rótulo.

1. O terceiro parâmetro é o nome bruto do item-chave:

   ![](assets/3rd-parameter-350x166.png)

1. O 4º parâmetro é o valor de chave fornecido.

Como a função `map()` retorna uma matriz (já que poderia haver mais elementos com o valor de chave fornecido), é necessário aplicar a função `get()` para obter seu primeiro elemento:

* O primeiro parâmetro da função `get()` é o resultado da função `map()`.

* O 2º parâmetro é o índice do elemento - um.

Para obter mais informações sobre a função `map()`, consulte [Funções de matriz em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

Para obter mais informações sobre a função `get()`, consulte [Funções gerais em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## Conversão de elementos em uma série de pacotes

Matrizes podem ser convertidas em uma série de conjuntos usando o módulo [!UICONTROL Iterador]. Para obter mais informações, consulte o módulo [[!UICONTROL Iterador] no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## Solução de problemas

### Itens ausentes no painel de mapeamento

Para cada módulo, o painel de mapeamento exibe todos os itens de saída listados pelo autor do módulo. Em alguns casos, essa lista pode estar incompleta por vários motivos e alguns itens podem estar ausentes. O [!DNL Workfront Fusion] pode descobrir automaticamente os itens de saída ausentes quando você executa o módulo no editor de cenários. O procedimento exato difere ligeiramente dependendo do tipo do módulo:

#### Acionador instantâneo

1. Clique com o botão direito do mouse no módulo e clique em **[!UICONTROL Executar este módulo somente]** no menu exibido.

   Se não houver webhooks em fila, o módulo aguardará um novo webhook ser processado.

1. Gerar um webhook.

   Por exemplo, o módulo de webhook **[!DNL Slack]>[!UICONTROL Ouvir novos eventos]** (que observa novas mensagens de canal em um canal) envia uma mensagem para o canal.

1. Quando o módulo terminar de ser executado, clique no balão acima do módulo para explorar sua saída completa.

   O painel de mapeamento conterá todos os itens que foram descobertos na saída do módulo.

#### Acionador de sondagem

1. Clique com o botão direito do mouse no módulo e clique em **[!UICONTROL Executar este módulo somente]** no menu exibido.
1. Se não houver saída, clique em **[!UICONTROL Escolher onde começar]** e ajuste as configurações.
1. Se não houver um evento a ser processado, crie um e retorne à etapa 2.

   Por exemplo, o módulo de webhook **[!UICONTROL Gmail] >[!UICONTROL Assistir emails]** envia um email para a pasta que o módulo está assistindo.

1. Quando o módulo terminar de ser executado, clique no balão acima do módulo para explorar sua saída completa.

   O painel de mapeamento agora contém todos os itens que foram descobertos na saída do módulo.

#### Outros módulos

Você pode optar por executar:

* O cenário inteiro (ou apenas a parte que contém o módulo)

  Se o cenário iniciar com um gatilho, consulte a seção [Gatilho instantâneo](#instant-trigger) ou [Gatilho de sondagem](#polling-trigger) acima.

* Apenas o módulo único

Se você optar por executar apenas o único módulo:

1. Clique com o botão direito do mouse no módulo e clique em **[!UICONTROL Executar este módulo somente]** no menu exibido.
1. Forneça valores de exemplo para os itens de entrada, em seguida, clique em **[!UICONTROL OK]**.
1. Quando o módulo terminar de ser executado, clique no balão acima do módulo para explorar sua saída completa.

   O painel de mapeamento agora contém todos os itens que foram descobertos na saída do módulo.
