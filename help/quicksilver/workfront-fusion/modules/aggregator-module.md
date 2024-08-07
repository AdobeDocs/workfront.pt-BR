---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Módulo agregador no Adobe Workfront Fusion
description: Um módulo agregador é um tipo de módulo projetado para unir vários pacotes de dados em um único pacote.
author: Becky
feature: Workfront Fusion
exl-id: cdc32842-8717-4e05-ab19-2661ee14c12c
source-git-commit: 948fe5fc249e0dcb04655f015c8e46493159c3ed
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 0%

---

# Módulo [!UICONTROL Aggregator] em [!DNL Adobe Workfront Fusion]

Um módulo agregador é um tipo de módulo projetado para unir vários pacotes de dados em um único pacote.

Para obter mais informações sobre tipos de módulo, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Visão geral do módulo [!UICONTROL Agregador]

Quando um módulo [!UICONTROL Aggregator] é executado, ele faz o seguinte:

* Acumula todos os pacotes que recebe durante a operação de um único módulo de origem.
* Gera um único pacote com uma matriz contendo um item para cada pacote acumulado. O conteúdo dos itens da matriz depende do módulo [!UICONTROL Aggregator] específico e de sua configuração.

A imagem a seguir mostra uma configuração típica do módulo [!UICONTROL Agregador]:

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Módulo Source]</p> </td> 
   <td> <p>O módulo onde a agregação do pacote começa. O módulo de origem geralmente é um iterador ou um módulo de pesquisa que gera uma série de pacotes.</p><p>Quando você configura o módulo de origem do agregador (e fecha a configuração do agregador), a rota entre o módulo de origem e o módulo do agregador é colocada em uma área cinza para que você possa ver claramente o início e o fim da agregação. 
   </p> <p>Para obter mais informações sobre iteradores, consulte o módulo <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!UICONTROL Iterator] em [!DNL Adobe Workfront Fusion]</a></p> <p>Para obter mais informações sobre módulos de pesquisa, consulte módulos de pesquisa em <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de estrutura de destino]</p> </td> 
   <td> <p>(Aplicável somente ao módulo [!UICONTROL Array aggregator].) A estrutura de público-alvo onde os dados são agregados. A opção padrão, [!UICONTROL Personalizado], permite que você escolha itens que devem ser agregados no <code>Array </code>item do pacote de saída do [!UICONTROL Array aggregator]:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Depois de conectar mais módulos após o módulo [!UICONTROL Array aggregator] e voltar à configuração do módulo, o menu suspenso do tipo de estrutura [!UICONTROL Target] conterá todos os módulos a seguir e seus campos que são do tipo "Matriz de Coleções", conforme mostrado no campo [!UICONTROL Attachments] do módulo [!DNL Slack] &gt;[!UICONTROL Criar uma Mensagem]:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos Agregados]</td> 
   <td>Os campos que você deseja incluir na saída do módulo agregador.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Agrupar por]</p> </td> 
   <td> <p>A saída do agregador pode ser dividida em vários grupos com a ajuda do campo [!UICONTROL Agrupar por]. O campo [!UICONTROL Agrupar por] pode conter uma fórmula que é avaliada para cada pacote de entrada do agregador. O agregador então gera um pacote por valor de cada fórmula distinta. Cada pacote contém dois itens:</p> 
    <ul> 
     <li><code>Key </code>contém o valor distinto.</li> 
     <li><code>Array </code>contém os dados agregados dos pacotes para os quais a fórmula avaliou para o valor <code>Key </code>.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Parar o processamento após uma agregação vazia</p> </td> 
   <td> <p>Por padrão, o módulo [!UICONTROL Aggregator] gera o resultado da agregação mesmo que nenhum pacote tenha atingido o módulo [!UICONTROL Aggregator] (por exemplo, porque todos foram filtrados no caminho). Se a opção [!UICONTROL Parar processamento após uma agregação vazia] estiver habilitada, o módulo [!UICONTROL Aggregator] não produzirá nenhum conjunto de saída nesse caso, e o fluxo será interrompido.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Os pacotes gerados pelos módulos entre o módulo de origem e o módulo [!UICONTROL Agregador] não são gerados pelo módulo [!UICONTROL Agregador], portanto, não são acessíveis pelos módulos no fluxo após o [!UICONTROL Agregador]. Se você precisar de dados de um pacote emitido por um módulo entre o módulo de origem e o módulo [!UICONTROL Agregador], inclua o item fornecido na configuração do módulo [!UICONTROL Agregador] (como no campo [!UICONTROL Campos agregados] da configuração do módulo [!UICONTROL Agregador de matrizes]).


## Exemplo de cenário de como os agregadores funcionam

Este exemplo de cenário mostra como compactar todos os anexos de email e fazer upload do ZIP para [!DNL Dropbox].

![](assets/dropbox-archive-350x87.png)

O cenário abaixo mostra como:

* O primeiro módulo observa uma caixa de entrada de emails: o gatilho [!UICONTROL Email] >[!UICONTROL Observar emails] gerará um pacote com o item `Attachments[]`, que é uma matriz que contém todos os anexos de email.

* O segundo modelo repete os anexos do email: [!UICONTROL Email] >[!UICONTROL Iterar anexos] O iterador pega os itens da matriz `Attachments[]` um por um e os envia como pacotes separados.

* O terceiro módulo agrega os pacotes gerados pelo módulo [!UICONTROL Email] >[!UICONTROL Iterar anexos]: [!UICONTROL Arquivo morto] >[!UICONTROL Criar um agregador de arquivo morto] acumula todos os pacotes que recebe e gera um único pacote contendo o arquivo ZIP.

* O último módulo carrega o arquivo ZIP resultante para [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Carregar um arquivo] obtém o arquivo ZIP do módulo [!UICONTROL Arquivar] > [!UICONTROL Criar um arquivo] e o carrega para [!DNL Dropbox].



Abaixo está uma configuração de exemplo do agregador [!UICONTROL Arquivo] > [!UICONTROL Criar um arquivo]:

![](assets/archive-create-an-archive-350x484.png)
