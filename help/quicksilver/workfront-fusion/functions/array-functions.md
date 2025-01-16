---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções de matriz no Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 1%

---

# Funções de matriz no Adobe Workfront Fusion

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Funções de matriz](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/array-functions.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plano</td>  
   <td> <p>Qualquer</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licença</td>  
   <td> <p>Novo: [!UICONTROL Padrão]</p><p>Ou</p><p>Atual: [!UICONTROL Trabalho] ou superior</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td>  
   <td> 
   <p>Atual: nenhum requisito de licença [!DNL Workfront Fusion].</p> 
   <p>Ou</p> 
   <p>Herdados: Qualquer um </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produto</td>  
   <td> 
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] Plano [!DNL Workfront]: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>Plano [!DNL Workfront] da [!UICONTROL Ultimate] [!DNL Workfront Fusion] incluído.</li></ul> 
   <p>Ou</p> 
   <p>Atual: sua organização deve comprar o [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Funções

* [ingressar](#join-array-separator)
* [length](#length-array)
* [chaves](#keys-object)
* [fatia](#slice-array-start-end)
* [mesclar](#merge-array1-array2)
* [contém](#contains-array-value)
* [remover](#remove-array-value1-value2)
* [adicionar](#add-array-value1-value2)
* [mapa](#map-complex-array-keykey-for-filteringpossible-values-for-filtering)
* [ordem aleatória]
* [sort](#sort-array-order-key)
* [reverter](#reverse-array)
* [nivelar](#flatten-array)
* [distinct](#distinct-array-key)
* [toCollection]
* [toArray](#toarray)
* [arrayDifference](#arraydifference-array1-array2-mode)
* [desduplicar]

### [!UICONTROL junção (matriz; separador)]

Concatena todos os itens de uma matriz em uma cadeia de caracteres, usando o separador especificado entre cada item.

### [!UICONTROL comprimento (matriz)]

Retorna o número de itens em uma matriz.

### [!UICONTROL chaves (objeto)]

Retorna uma matriz das propriedades de um determinado objeto ou matriz.

### [!UICONTROL fatia (matriz; início; [fim])]

Retorna uma nova matriz contendo apenas itens selecionados.

### [!UICONTROL mesclar (matriz1; matriz2; ...)]

Mescla uma ou mais matrizes em uma matriz.

### [!UICONTROL contém (matriz; valor)]

Verifica se uma matriz contém o valor.

### [!UICONTROL remover (matriz; valor1; valor2; ...)]

Remove valores especificados nos parâmetros de uma matriz. Esta função só é eficaz em matrizes primitivas de texto ou números.

### [!UICONTROL adicionar (matriz; valor1; valor2; ...)]

Adiciona valores especificados em parâmetros a uma matriz e retorna essa matriz.

### [!UICONTROL mapa (matriz complexa; chave;[chave para filtragem];[valores possíveis para filtragem])]

Retorna uma matriz primitiva contendo valores de uma matriz complexa. Esta função permite filtrar valores. Use nomes de variáveis brutos para chaves.

>[!INFO]
>
>**Exemplos:**
>
>* `map(Emails[];email)`
>
>  Retorna uma matriz primitiva com emails
>
>* `map(Emails[];email;label;work;home)`
>
>  Retorna uma matriz primitiva com emails com rótulo igual a trabalho ou casa

Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)

### ordem aleatória

### [!UICONTROL classificar (matriz; [ordem]; [chave])]

Classifica os valores de uma matriz. Os valores válidos do parâmetro `order` são:

* `asc`

  (padrão) - ordem crescente: 1, 2, 3, ... para o tipo Número. A, B, C, a, b, c, ... para texto

* `desc`

  ordem decrescente: ..., 3, 2, 1 para o tipo Number. ..., c, b, a, C, B, A para texto.

* `asc ci`

  ordem crescente que não diferencia maiúsculas de minúsculas: A, a, B, b, C, c, ... para o tipo Text.

* `desc ci`

  ordem decrescente que não diferencia maiúsculas de minúsculas: ..., C, c, B, b, A, a para tipo de Texto.

Use o parâmetro `key` para acessar propriedades dentro de objetos complexos.

Use nomes de variáveis brutos para chaves.

Para acessar propriedades aninhadas, use a notação de pontos.

O primeiro item em uma matriz é o índice 1.

>[!INFO]
>
>**Exemplos:**
>
>* `sort(Contacts[];name)`
>
>    Classifica uma matriz de contatos pela propriedade &quot;name&quot; em ordem crescente padrão
>
>* `sort(Contacts[];desc;name)`
>
>   Classifica uma matriz de contatos pela propriedade &quot;name&quot; em ordem descendente
>
>* `sort(Contacts[];asc ci;name)`
>
>    Classifica uma matriz de contatos pela propriedade &quot;name&quot; em ordem crescente que não diferencia maiúsculas de minúsculas
>
>* `sort(Emails[];sender.name)`
>
>    Classifica uma matriz de emails pela propriedade &quot;sender.name&quot;

### [!UICONTROL inverter (matriz)]

O primeiro elemento da matriz se torna o último elemento, o segundo se torna o próximo ao último e assim por diante.

### [!UICONTROL nivelar (matriz)]

Cria uma nova matriz com todos os elementos de submatriz concatenados nela, recursivamente, até a profundidade especificada.

### [!UICONTROL distinct (matriz; [chave])]

Remove duplicatas dentro de uma matriz. Use o argumento &quot;[!UICONTROL key]&quot; para acessar propriedades dentro de objetos complexos. Para acessar propriedades aninhadas, use a notação de pontos. O primeiro item em uma matriz é o índice 1.

>[!INFO]
>
>**Exemplo:** `distinct(Contacts[];name)`
>
>Remove duplicatas dentro de uma matriz de contatos comparando a propriedade &quot;name&quot;

### toCollection

### toArray

Esta função converte uma coleção em uma matriz de pares de valores chave.

>[!INFO]
>
>**Exemplos:**
>
>Dada a coleção
>
>`{ key1: "value1", key2: "value2:}`
>
>A função
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>Retorna a matriz de pares de valores chave
>
>`[{ key1: "value1"}, { key2: "value2"}]`

### [!UICONTROL arrayDifference [array1, array2, modo]]

Retorna a diferença entre duas matrizes.

Insira um dos seguintes valores para o parâmetro `mode`.

* `classic`: retorna uma nova matriz que contém todos os elementos de `array1` que não existem em `array2`.

* `symmetric`: retorna uma matriz de elementos que não são comuns a ambas as matrizes.

  Em outras palavras, a função retorna uma matriz que contém todos os elementos de `array1` que não existem em `array2` e todos os elementos de `array2` que não existem em `array1`.

  >[!INFO]
  >
  >**Exemplos:**
  >
  >Considerando as seguintes matrizes:
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    Retorna `[1,2]`
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    Retorna `[6,7]`
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    Retorna `[1,2,6,7]`

### desduplicar

## Palavras-chave

### emptyarray
