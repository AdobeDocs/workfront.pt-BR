---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções de string no Adobe Workfront Fusion
description: As seguintes funções de string estão disponíveis no painel de mapeamento do Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 3%

---

# Funções de string em [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ascii (texto; [remover diacríticos])]

Remove todos os caracteres não ascii de uma string de texto.

>[!INFO]
>
>**Exemplos:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
   >
   >   Retorna: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
   >
   >   Retorna: [!UICONTROL escrz]


## [!UICONTROL base64 (texto)]

Transforma o texto em base64.

>[!INFO]
>
>**Exemplo:**
>
>`base64( workfront )`
>
>Retorna: d29ya2Zyb250==

## [!UICONTROL capitalizar (texto)]

Converte o primeiro caractere em uma string de texto em maiúsculas.

>[!INFO]
>
>**Exemplo:**
>
>`capitalize( workfront )`
>
>Retorna: [!DNL Workfront]

## contém (texto; sequência de pesquisa)

Verifica se o texto contém a string de pesquisa.

>[!INFO]
>
>**Exemplos:**
>
>* `contains( Hello World ; Hello )`
   >
   >   Retorna: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
   >
   >   Retorna: [!UICONTROL false]


## [!UICONTROL decodeURL (texto)]

Decodifica caracteres especiais em um URL para texto.

>[!INFO]
>
>**Exemplo:**
>`decodeURL( Automate%20your%20workflow )`
>
>Retorna: [!UICONTROL Automatizar seu fluxo de trabalho]

## [!UICONTROL encodeURL (texto)]

Codifica caracteres especiais em algum texto em um endereço de URL válido.

## [!UICONTROL escapeHTML (texto)]

Escapa todas as tags HTML no texto.

>[!INFO]
>
>**Exemplo:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Retorna: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

Escapa todas as tags do Markdown no texto.

>[!INFO]
>
>**Exemplo:**
>
>`escapeMarkdown( # Header )`
>
>Retorna: `&#35; Header`

## [!DNL indexOf (string; value; [start])]

Retorna a posição da primeira ocorrência de um valor especificado em uma string. Este método retornará &#39;-1&#39; se o valor pesquisado não estiver presente. O valor inicial indica onde a pesquisa deve começar na string.

>[!INFO]
>
>**Exemplos:**
>
>* `indexOf( Workfront ; o )`
   >
   >   Retorna: 1
>
>* `indexOf( Workfront ; x )`
   >
   >   Retorna: -1
>
>* `indexOf( Workfront ; o ; 3 )`
   >
   >   Retorna: 6


## [!UICONTROL length (texto ou buffer)]

Retorna o comprimento da string de texto (número de caracteres) ou do buffer binário (tamanho do buffer em bytes).

>[!INFO]
>
>**Exemplo:**
>
>`length( hello )`
>
>Retorna: 5

## [!UICONTROL lower (texto)]

Converte todos os caracteres alfabéticos em uma sequência de texto em minúsculas.

>[!INFO]
>
>**Exemplo:**
>
>`lower( Hello )`
>
>Retorna: hello

## [!UICONTROL md5 (texto)]

Calcula o hash md5 de uma string.

>[!INFO]
>
>**Exemplo:**
>
>`md5( Workfront )`
>
>Retorna: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL substituir (texto; pesquisar string; string de substituição)]

Substitui a string de pesquisa pela nova string.

>[!INFO]
>
>**Exemplo:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Retorna: [!UICONTROL Hi World]

Expressões regulares (delimitadas por `/.../`) pode ser usada como string de pesquisa com uma combinação de sinalizadores (como `g`, `i`, `m`) anexado:

>[!INFO]
>
>**Exemplo:**
>
>![](assets/replace---1-350x31.png)
>
>Todos estes números X X X X são substituídos por X

A sequência de caracteres de substituição pode incluir os seguintes padrões especiais de substituição:

* `$&` Insere a substring correspondente.
* `$n` Onde n é um inteiro positivo menor que 100, insere a enésima cadeia de subcorrespondência entre parênteses. Isso é indexado em 1.

>[!INFO]
>
>**Exemplos:**
>
>![](assets/variable-value-350x63.png)
>
>Retorna: Número de telefone `+420777111222`
>>![](assets/variable-value---2-350x55.png)
>Retorna: Número de telefone: `+420777111222`

>[!CAUTION]
Não use grupos de captura nomeados como `/ is (?<number>\d+)/` no argumento da string de substituição. Isso resulta em um erro.

Para obter mais informações sobre expressões regulares, consulte [Analisador de texto](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1 (texto; [codificação]; [key])]

Calcula o hash sha1 de uma string. Se o argumento principal for especificado, sha1 HMAC hash será retornado. Codificações suportadas: &quot;hex&quot; (padrão), &quot;base64&quot; ou &quot;latin1&quot;.

>[!INFO]
**Exemplo:**
`sha1( workfront )`
Retorna: b2b30b8ae1f9e5b40fbb0696eabdbfd8d0c087f

## [!UICONTROL sha256 (texto; [codificação]; [key])]

Calcula o hash sha256 de uma string. Se o argumento principal for especificado, o hash HMAC sha256 será retornado. Codificações suportadas: &quot;hex&quot; (padrão), &quot;base64&quot; ou &quot;latin1&quot;.>

>[!INFO]
**Exemplo:**
`sha256( workfront )`
Retorna: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (texto; [codificação de saída]; [key]; [codificação de chave])]

Calcula o hash sha512 de uma string. Se o argumento principal for especificado, o hash HMAC sha512 será retornado.

Codificações suportadas:

* &quot;[!UICONTROL hexadecimal]&quot; (padrão)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Codificações de chave suportadas:

* &quot;[!UICONTROL texto]&quot; (padrão)
* &quot;[!UICONTROL hexadecimal]&quot;
* &quot;[!UICONTROL base64]&quot; ou &quot;[!UICONTROL binário]&quot;

Ao usar &quot;[!UICONTROL binário]&quot; codificação de chave, uma chave deve ser um buffer, não uma string.

>[!INFO]
**Exemplo:**
`sha512(workfront)`
Retorna: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd19b 85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL Split (texto; separador)]

Divida uma string em uma matriz de strings, separando a string em subsequências.

>[!INFO]
**Exemplo:**
`split( John, George, Paul ; , )`

## [!UICONTROL inicial (texto)]

Coloca a primeira letra de cada palavra em maiúsculas e minúsculas em todas as outras letras.

>[!INFO]
**Exemplo:**
`startcase( hello WORLD )`
Retorna: [!UICONTROL Hello World]

## [!UICONTROL stripHTML (texto)]

Remove todas as tags de HTML do texto.

>[!INFO]
**Exemplo:**
`stripHTML( <b>Hello</b> )`
Retorna: Hello

## [!UICONTROL substring (texto; start;end)]

Retorna uma parte de uma string de texto entre a posição &quot;inicial&quot; e &quot;final&quot;.

>[!INFO]
**Exemplos:**
* `substring( Hello ; 0 ; 3)`

   Retorna: Hel
* `substring( Hello ; 1 ; 3 )`

   Retorna: el


## [!UICONTROL toBinary (valor)]

Converte qualquer valor em dados binários.

Também é possível especificar a codificação como um segundo argumento para aplicar conversões binárias de hex ou base64 a dados binários.

>[!INFO]
**Exemplos:**
* `toBinary( Workfront )`

   Retorna: 57 6f 72 6b 66 72 6f 6e 74
* `toBinary( V29ya2Zyb250 ; base64 )`

   Retorna: 57 6f 72 6b 66 72 6f 6e 74


## [!UICONTROL toString (valor)]

Converte qualquer valor em uma string.

## [!UICONTROL trim (texto)]

Remove caracteres de espaço no início ou no fim do texto.

## [!UICONTROL upper (texto)]

Converte todos os caracteres alfabéticos em uma sequência de texto em maiúsculas.

>[!INFO]
**Exemplo:**
`upper( Hello )`
Retorna: [!UICONTROL HELLO]
