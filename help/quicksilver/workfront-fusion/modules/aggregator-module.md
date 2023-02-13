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
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# [!UICONTROL Agregador] módulo em [!DNL Adobe Workfront Fusion]

Um módulo agregador é um tipo de módulo projetado para unir vários pacotes de dados em um único pacote.

Para obter mais informações sobre tipos de módulos, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Agregador] módulo

Quando uma [!UICONTROL Agregador] é executado, faz o seguinte:

* Acumula todos os pacotes recebidos durante a operação de um único módulo de origem.
* Gera um único pacote com uma matriz contendo um item por cada pacote acumulado. O conteúdo dos itens da matriz depende de [!UICONTROL Agregador] e sua configuração.

A imagem a seguir mostra uma configuração típica do [!UICONTROL Agregador] módulo :

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Módulo de origem]</p> </td> 
   <td> <p>O módulo do qual a agregação de pacote será iniciada. O módulo de origem geralmente é um iterador ou um módulo de pesquisa que gera uma série de pacotes. Quando você configura o módulo de origem do agregador (e fecha a configuração do agregador), a rota entre o módulo de origem e o módulo agregador é encapsulada em uma área cinza para que você possa ver claramente o início e o fim da agregação. 
   </p> <p>Para obter mais informações sobre iteradores, consulte <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Módulo [!UICONTROL Iterator] em [!DNL Adobe Workfront Fusion]</a></p> <p>Para obter mais informações sobre módulos de pesquisa, consulte módulos de pesquisa em <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de estrutura do Target]</p> </td> 
   <td> <p>(Aplicável somente para o módulo [!UICONTROL Array aggregate].) Estrutura - alvo na qual os dados devem ser agregados. A opção padrão, [!UICONTROL Personalizado], permite escolher itens que devem ser agregados no pacote de saída do agregador de matriz A[!UICONTROL] <code>Array </code>item:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Depois de conectar mais módulos após o módulo [!UICONTROL Array aggregate] e voltar à configuração do módulo, a lista suspensa do tipo de estrutura [!UICONTROL Target] conterá todos os módulos a seguir e seus campos que sejam do tipo Array of Collections, conforme mostrado no campo [!UICONTROL Attachments] do [!DNL Slack] &gt; Módulo [!UICONTROL Criar uma mensagem]:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos agregados]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo agregador.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Agrupar por]</p> </td> 
   <td> <p>A saída do agregador pode ser dividida em vários grupos com a ajuda do campo [!UICONTROL Group by] . O campo [!UICONTROL Group by] pode conter uma fórmula que é avaliada para cada pacote de entrada do agregador. O agregador então gera um pacote por valor de fórmula distinta. Cada pacote contém dois itens:</p> 
    <ul> 
     <li><code>Key </code>contém o valor distinto.</li> 
     <li><code>Array </code>contém os dados agregados dos pacotes para os quais a fórmula foi avaliada <code>Key </code>valor.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>Parar o processamento após uma agregação vazia</p> </td> 
   <td> <p>Por padrão, o módulo [!UICONTROL Aggregator] gera o resultado da agregação mesmo no caso de nenhum pacote atingir o módulo [!UICONTROL Aggregator] (por exemplo, porque todos foram filtrados no caminho). Se a opção [!UICONTROL Parar o processamento após uma agregação vazia] estiver habilitada, o módulo [!UICONTROL Aggregator] não produzirá nenhum pacote de saída nesse caso e o fluxo será interrompido.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Pacotes gerados por módulos entre o módulo de origem e o [!UICONTROL Agregador] não são gerados pela saída do [!UICONTROL Agregador] , de modo que não sejam acessíveis pelos módulos no fluxo após a [!UICONTROL Agregador]. Se você precisar de dados de um pacote enviado por um módulo entre o módulo de origem e o [!UICONTROL Agregador] , certifique-se de incluir o item fornecido no [!UICONTROL Agregador] configuração do módulo (como no [!UICONTROL Campos agregados] na configuração do [!UICONTROL Agregador de matriz] módulo).


>[!INFO]
>
>**Exemplo:** Caso de uso: Compactar todos os anexos de email e fazer upload do ZIP para [!DNL Dropbox]
>
>O cenário abaixo mostra como:
>
>* Assista a uma caixa de entrada para receber emails: [!UICONTROL Email] >[!UICONTROL Assistir a emails] o acionador gerará um pacote com o item `Attachments[]`, que é uma matriz que contém todos os anexos do email.
>
>* Iterar os anexos do email: [!UICONTROL Email] >[!UICONTROL Iterar anexos] o iterador retira os itens do `Attachments[]` array um por um e os envia ainda mais como pacotes separados.
>
>* Agregue os pacotes fornecidos pelo [!UICONTROL Email] >[!UICONTROL Iterar anexos] módulo: [!UICONTROL Arquivar] >[!UICONTROL Criar um agregador de arquivamento] acumula todos os pacotes que recebe e gera um único pacote contendo o arquivo ZIP.
>
>* Faça upload do arquivo ZIP resultante para [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Carregar um arquivo] obtém o arquivo ZIP do [!UICONTROL Arquivar] > [!UICONTROL Criar um arquivo] e faz upload para [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>Abaixo está uma amostra da configuração do [!UICONTROL Arquivar] > [!UICONTROL Criar um arquivo] agregador:
>
>![](assets/archive-create-an-archive-350x484.png)
