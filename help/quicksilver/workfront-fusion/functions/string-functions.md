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
source-git-commit: 0b286e43ed77669329fbee25618394ee5641e428
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

# Funções de string em [!DNL Adobe Workfront Fusion]

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
   <p>Atual: Não [!DNL Workfront Fusion] requisito de licença.</p> 
   <p>Ou</p> 
   <p>Herdados: Qualquer um </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produto</td>  
   <td> 
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plano: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plano: [!DNL Workfront Fusion] está incluído.</li></ul> 
   <p>Ou</p> 
   <p>Atual: sua organização deve comprar [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL comprimento (texto ou buffer)]

Retorna o tamanho da string de texto (número de caracteres) ou do buffer binário (tamanho do buffer em bytes).

>[!INFO]
>
>**Exemplo:**
>
>`length( hello )`
>
>Devoluções: 5

## [!UICONTROL inferior (texto)]

Converte todos os caracteres alfabéticos em uma cadeia de texto em minúsculas.

>[!INFO]
>
>**Exemplo:**
>
>`lower( Hello )`
>
>Retorna: olá

## [!UICONTROL colocar letra maiúscula (texto)]

Converte o primeiro caractere em uma cadeia de texto em maiúsculas.

>[!INFO]
>
>**Exemplo:**
>
>`capitalize( workfront )`
>
>Devoluções: [!DNL Workfront]

## [!UICONTROL letra inicial (texto)]

Coloca a primeira letra de cada palavra em maiúscula e coloca em minúscula todas as outras letras.

>[!INFO]
>
>**Exemplo:**
>`startcase( hello WORLD )`
>
>Devoluções: [!UICONTROL Olá, mundo]

## [!UICONTROL ascii (texto; [remover sinais diacríticos])]

Remove todos os caracteres não ascii de uma cadeia de texto.

>[!INFO]
>
>**Exemplos:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
>
>   Devoluções: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
>
>   Devoluções: [!UICONTROL escrz]



## [!UICONTROL substituir (texto;cadeia de caracteres de pesquisa; cadeia de caracteres de substituição)]

Substitui a cadeia de caracteres de pesquisa pela nova cadeia.

>[!INFO]
>
>**Exemplo:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Devoluções: [!UICONTROL Olá, mundo]

Expressões regulares (entre `/.../`) pode ser usada como sequência de pesquisa com uma combinação de sinalizadores (como `g`, `i`, `m`) anexado:

>[!INFO]
>
>**Exemplo:**
>
>![](assets/replace---1-350x31.png)
>
>Todos estes números X X X X são substituídos por X

A sequência de caracteres de substituição pode incluir os seguintes padrões de substituição especiais:

* `$&` Insere a substring correspondente.
* `$n` Onde n é um número inteiro positivo menor que 100, insere a enésima string de subcorrespondência entre parênteses. Isso é indexado com 1.

>[!INFO]
>
>**Exemplos:**
>
>![](assets/variable-value-350x63.png)
>
>Retorna: número de telefone `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>Retorna: número de telefone: `+420777111222`

>[!CAUTION]
>
>Não use grupos de captura nomeados, como `/ is (?<number>\d+)/` no argumento string de substituição. Isso resulta em um erro.

Para obter mais informações sobre expressões regulares, consulte [Analisador de texto](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL cortar (texto)]

Remove caracteres de espaço no início ou no fim do texto.

## [!UICONTROL superior (texto)]

Converte todos os caracteres alfabéticos em uma cadeia de texto em maiúsculas.

>[!INFO]
>
>**Exemplo:**
>
>`upper( Hello )`
>
>Devoluções: [!UICONTROL OLÁ]

## [!UICONTROL substring (texto; início;fim)]

Retorna uma parte de uma cadeia de texto entre a posição &quot;inicial&quot; e a posição &quot;final&quot;.

>[!INFO]
>
>**Exemplos:**
>
>* `substring( Hello ; 0 ; 3)`
>
>   Retorna: ajuda
>
>* `substring( Hello ; 1 ; 3 )`
>
>   Devoluções: el

## [!DNL indexOf (string; value; [start])]

Retorna a posição da primeira ocorrência de um valor especificado em uma string. Este método retorna &#39;-1&#39; se o valor procurado não estiver lá. O valor inicial indica onde a pesquisa deve começar na cadeia de caracteres.

>[!INFO]
>
>**Exemplos:**
>
>* `indexOf( Workfront ; o )`
>
>   Devoluções: 1
>
>* `indexOf( Workfront ; x )`
>
>   Devoluções: -1
>
>* `indexOf( Workfront ; o ; 3 )`
>
>   Devoluções: 6

## [!UICONTROL toBinary (valor)]

Converte qualquer valor em dados binários.

Você também pode especificar a codificação como um segundo argumento para aplicar conversões binárias de hexadecimal ou base64 a dados binários.

>[!INFO]
>
>**Exemplos:**
>
>* `toBinary( Workfront )`
>
>   Retorna: 57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   Retorna: 57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString (valor)]

Converte qualquer valor em uma string.

## [!UICONTROL encodeURL (texto)]

Codifica caracteres especiais em algum texto para um endereço de URL válido.

## [!UICONTROL decodeURL (texto)]

Decodifica caracteres especiais em um URL para texto.

>[!INFO]
>
>**Exemplo:**
>`decodeURL( Automate%20your%20workflow )`
>
>Devoluções: [!UICONTROL Automatizar o fluxo de trabalho]

## [!UICONTROL escapeHTML (texto)]

Escapa todas as tags HTML no texto.

>[!INFO]
>
>**Exemplo:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Devoluções: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(texto)]

Escapa todas as tags do Markdown no texto.

>[!INFO]
>
>**Exemplo:**
>
>`escapeMarkdown( # Header )`
>
>Devoluções: `&#35; Header`

## [!UICONTROL stripHTML (texto)]

Remove todas as tags HTML do texto.

>[!INFO]
>
>**Exemplo:**
>
>`stripHTML( <b>Hello</b> )`
>
>Retorna: Olá

## contains (texto; sequência de pesquisa)

Verifica se o texto contém a cadeia de caracteres de pesquisa.

>[!INFO]
>
>**Exemplos:**
>
>* `contains( Hello World ; Hello )`
>
>   Devoluções: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   Devoluções: [!UICONTROL false]

## [!UICONTROL split (texto; separador)]

Divide uma cadeia de caracteres em uma matriz de cadeias de caracteres, separando-a em subcadeias.

>[!INFO]
>
>**Exemplo:**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL md5 (texto)]

Calcula o hash md5 de uma string.

>[!INFO]
>
>**Exemplo:**
>
>`md5( Workfront )`
>
>Devoluções: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL sha1 (texto; [codificação]; [key])]

Calcula o hash sha1 de uma cadeia de caracteres. Se o argumento chave for especificado, o hash sha1 HMAC será retornado. Codificações suportadas: &quot;hex&quot; (padrão), &quot;base64&quot; ou &quot;latin1&quot;.

>[!INFO]
>
>**Exemplo:**
>
>`sha1( workfront )`
>
>Retorna: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (texto; [codificação]; [key])]

Calcula o hash sha256 de uma string. Se o argumento chave for especificado, o hash sha256 HMAC será retornado. Codificações suportadas: &quot;hex&quot; (padrão), &quot;base64&quot; ou &quot;latin1&quot;.>

>[!INFO]
>
>**Exemplo:**
>
>`sha256( workfront )`
>
>Retorna: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (texto; [codificação de saída]; [key]; [codificação de chave])]

Calcula o hash sha512 de uma string. Se o argumento de chave for especificado, o hash sha512 HMAC será retornado.

Codificações suportadas:

* &quot;[!UICONTROL hexadecimal]&quot; (padrão)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Codificações de chave suportadas:

* &quot;[!UICONTROL texto]&quot; (padrão)
* &quot;[!UICONTROL hexadecimal]&quot;
* &quot;[!UICONTROL base64]&quot; ou &quot;[!UICONTROL binário]&quot;

Ao usar &quot;[!UICONTROL binário]&quot; chave, uma chave deve ser um buffer, não uma sequência.

>[!INFO]
>
>**Exemplo:**
>
>`sha512(workfront)`
>
>Retorna: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af 35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL base64 (texto)]

Transforma texto em base64.

>[!INFO]
>
>**Exemplo:**
>
>`base64( workfront )`
>
>Retorna: d29ya2Zyb250==
