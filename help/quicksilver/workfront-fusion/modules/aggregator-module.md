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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# [!UICONTROL Agregador] módulo no [!DNL Adobe Workfront Fusion]

Um módulo agregador é um tipo de módulo projetado para unir vários pacotes de dados em um único pacote.

Para obter mais informações sobre tipos de módulo, consulte [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
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

## [!UICONTROL Agregador] módulo

Quando um [!UICONTROL Agregador] for executado, o módulo fará o seguinte:

* Acumula todos os pacotes que recebe durante a operação de um único módulo de origem.
* Gera um único pacote com uma matriz contendo um item para cada pacote acumulado. O conteúdo dos itens da matriz depende de propriedades [!UICONTROL Agregador] e sua configuração.

A imagem a seguir mostra uma configuração típica do [!UICONTROL Agregador] módulo:

![](assets/array-aggregator-350x190.png)

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Módulo de Origem]</p> </td> 
   <td> <p>O módulo a partir do qual a agregação do pacote será iniciada. O módulo de origem geralmente é um iterador ou um módulo de pesquisa que gera uma série de pacotes. Quando você configura o módulo de origem do agregador (e fecha a configuração do agregador), a rota entre o módulo de origem e o módulo do agregador é colocada em uma área cinza para que você possa ver claramente o início e o fim da agregação. 
   </p> <p>Para obter mais informações sobre iteradores, consulte <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Módulo [!UICONTROL Iterador] em [!DNL Adobe Workfront Fusion]</a></p> <p>Para obter mais informações sobre módulos de pesquisa, consulte módulos de pesquisa em <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Tipo de estrutura de destino]</p> </td> 
   <td> <p>(Aplicável somente ao módulo [!UICONTROL Array aggregator].) A estrutura-alvo na qual os dados devem ser agregados. A opção padrão, [!UICONTROL Personalizado], permite que você escolha itens que devem ser agregados no conjunto de saída do A[!UICONTROL agregador de matriz] <code>Array </code>item:</p> <p> <img src="assets/output-bundle's-array-item-350x213.png" style="width: 350;height: 213;"> </p> <p>Depois de conectar mais módulos após o módulo [!UICONTROL Array aggregator] e voltar à configuração do módulo, a lista suspensa de tipo de estrutura [!UICONTROL Target] conterá todos os módulos a seguir e seus campos que são do tipo Matriz de Coleções, conforme mostrado no campo [!UICONTROL Attachments] do [!DNL Slack] Módulo &gt;[!UICONTROL Criar uma Mensagem]:</p> <p> <img src="assets/array-aggregator-slack-350x253.png" style="width: 350;height: 253;"> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos Agregados]</td> 
   <td>Selecione os campos que deseja incluir na saída do módulo agregador.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Agrupar por]</p> </td> 
   <td> <p>A saída do agregador pode ser dividida em vários grupos com a ajuda do campo [!UICONTROL Agrupar por]. O campo [!UICONTROL Agrupar por] pode conter uma fórmula que é avaliada para cada pacote de entrada do agregador. O agregador então gera um pacote por valor de cada fórmula distinta. Cada pacote contém dois itens:</p> 
    <ul> 
     <li><code>Key </code>contém o valor distinto.</li> 
     <li><code>Array </code>contém os dados agregados dos pacotes para os quais a fórmula avaliou para o <code>Key </code>valor.</li> 
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
>Pacotes gerados por módulos entre o módulo de origem e o [!UICONTROL Agregador] Os módulos do não são gerados pelo [!UICONTROL Agregador] módulo, de modo que não sejam acessíveis pelos módulos no fluxo após o [!UICONTROL Agregador]. Se você precisar de dados de um pacote emitido por um módulo entre o módulo de origem e o [!UICONTROL Agregador] módulo, certifique-se de incluir o item fornecido na variável [!UICONTROL Agregador] configuração do módulo (como na variável [!UICONTROL Campos agregados] na configuração do [!UICONTROL Agregador de matrizes] módulo).


>[!INFO]
>
>**Exemplo:** Caso de uso: compactar todos os anexos de email e fazer upload do ZIP para [!DNL Dropbox]
>
>O cenário abaixo mostra como:
>
>* Verifique se há emails de entrada em uma caixa de correio: [!UICONTROL E-mail] >[!UICONTROL Assistir a emails] o acionador gerará um pacote com o item `Attachments[]`, que é uma matriz que contém todos os anexos do email.
>
>* Repita os anexos do email: [!UICONTROL E-mail] >[!UICONTROL Iterar anexos] o iterador pega os itens do `Attachments[]` um por um e os envia como pacotes separados.
>
>* Agregar os pacotes gerados pelo [!UICONTROL E-mail] >[!UICONTROL Iterar anexos] módulo: [!UICONTROL Arquivar] >[!UICONTROL Criar um agregador de arquivo] O acumula todos os pacotes que recebe e gera um único pacote contendo o arquivo ZIP.
>
>* Faça upload do arquivo ZIP resultante para [!DNL Dropbox]: [!DNL Dropbox] > [!UICONTROL Carregar um arquivo] obtém o arquivo ZIP do [!UICONTROL Arquivar] > [!UICONTROL Criar um arquivo] e faz upload para [!DNL Dropbox].
>
>![](assets/dropbox-archive-350x87.png)
>
>Abaixo está uma amostra da configuração de [!UICONTROL Arquivar] > [!UICONTROL Criar um arquivo] agregador:
>
>![](assets/archive-create-an-archive-350x484.png)
