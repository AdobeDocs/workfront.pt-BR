---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções de string no Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Funções de cadeia de caracteres em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Funções de cadeia de caracteres](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/string-functions.html)
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

## [!UICONTROL colocar em maiúsculas (texto)]

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
>Retorna: [!UICONTROL Olá, Mundo]

## [!UICONTROL ascii (texto; [remover diacríticos])]

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
>   Retorna: [!UICONTROL escrz]



## [!UICONTROL substituir (texto;cadeia de caracteres de pesquisa; cadeia de caracteres de substituição)]

Substitui a cadeia de caracteres de pesquisa pela nova cadeia.

>[!INFO]
>
>**Exemplo:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Retorna: [!UICONTROL Olá, Mundo]

Expressões regulares (entre `/.../`) podem ser usadas como cadeia de caracteres de pesquisa com uma combinação de sinalizadores (como `g`, `i`, `m`) adicionados:

>[!INFO]
>
>**Exemplo:**
>
>![](assets/replace---1-350x31.png)
>
>Todos estes números X X X X são substituídos por X

A sequência de caracteres de substituição pode incluir os seguintes padrões de substituição especiais:

* `$&` Insere a subcadeia de caracteres correspondente.
* `$n` Onde n é um inteiro positivo menor que 100, insere a enésima cadeia de caracteres de subcorrespondência entre parênteses. Isso é indexado com 1.

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
>Retorna: Telefone: `+420777111222`

>[!CAUTION]
>
>Não use grupos de captura nomeados, como `/ is (?<number>\d+)/`, no argumento de cadeia de caracteres de substituição. Isso resulta em um erro.

Para obter mais informações sobre expressões regulares, consulte [Analisador de texto](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL cortar (texto)]

Remove caracteres de espaço no início ou no fim do texto.

## [!UICONTROL parte superior (texto)]

Converte todos os caracteres alfabéticos em uma cadeia de texto em maiúsculas.

>[!INFO]
>
>**Exemplo:**
>
>`upper( Hello )`
>
>Retorna: [!UICONTROL OLÁ]

## [!UICONTROL subcadeia de caracteres (texto; início;fim)]

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
>Retorna: [!UICONTROL Automatize seu fluxo de trabalho]

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
>   Retorna: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   Retorna: [!UICONTROL false]

## [!UICONTROL divisão (texto; separador)]

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

## [!UICONTROL sha1 (texto; [codificação]; [chave])]

Calcula o hash sha1 de uma cadeia de caracteres. Se o argumento chave for especificado, o hash sha1 HMAC será retornado. Codificações suportadas: &quot;hex&quot; (padrão), &quot;base64&quot; ou &quot;latin1&quot;.

>[!INFO]
>
>**Exemplo:**
>
>`sha1( workfront )`
>
>Retorna: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (text; [codificação]; [chave])]

Calcula o hash sha256 de uma string. Se o argumento chave for especificado, o hash sha256 HMAC será retornado. Codificações suportadas: &quot;hex&quot; (padrão), &quot;base64&quot; ou &quot;latin1&quot;.>

>[!INFO]
>
>**Exemplo:**
>
>`sha256( workfront )`
>
>Retorna: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (text; [codificação de saída]; [chave]; [codificação de chave])]

Calcula o hash sha512 de uma string. Se o argumento de chave for especificado, o hash sha512 HMAC será retornado.

Codificações suportadas:

* &quot;[!UICONTROL hex]&quot; (padrão)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Codificações de chave suportadas:

* &quot;[!UICONTROL texto]&quot; (padrão)
* &quot;[!UICONTROL hexadecimal]&quot;
* &quot;[!UICONTROL base64]&quot; ou &quot;[!UICONTROL binary]&quot;

Ao usar a codificação de chave &quot;[!UICONTROL binary]&quot;, uma chave deve ser um buffer, não uma cadeia de caracteres.

>[!INFO]
>
>**Exemplo:**
>
>`sha512(workfront)`
>
>Devoluções: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af3

## [!UICONTROL base64 (texto)]

Transforma texto em base64.

>[!INFO]
>
>**Exemplo:**
>
>`base64( workfront )`
>
>Retorna: d29ya2Zyb250==
