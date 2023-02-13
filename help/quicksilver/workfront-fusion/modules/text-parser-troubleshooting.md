---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Solução de problemas do analisador de texto em [!DNL Adobe Workfront Fusion]
description: Use essas informações se não for possível obter o analisador de texto para produzir qualquer saída.
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Solução de problemas do analisador de texto em [!DNL Adobe Workfront Fusion]

Use essas informações se não for possível obter um analisador de texto para produzir qualquer saída.

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

## Solução de problemas

Exemplo de cenário de caso, você gostaria de analisar o tipo de arquivo de um documento de arquivo &quot;filename.docx&quot; e a extensão do nome de arquivo sempre varia de DOCX a PDF para CSV.

A expressão que você pode optar por usar nesse caso é [!DNL \..+]

Se você usar isso na expressão regex no regex101.com, obterá uma correspondência completa.

![](assets/regex-expression-350x130.png)

Na imagem acima, a extensão de arquivo era correspondida corretamente. Caso utilize e tente implementá-lo no analisador de texto:

![](assets/text-parser-350x602.png)

você não obterá uma correspondência:

![](assets/text-parser-you-dont-get-a-match-350x365.png)

O motivo para isso é que o &quot;i&quot; mostra apenas o número de correspondências por correspondência, então neste caso, temos 2 correspondências, portanto, depois do &quot;i&quot; há um valor numérico 1 e 2. O caso de uso para isso é que, caso precise corresponder ou passar dados por um filtro, somente o segundo valor correspondente, você pode especificar qual valor é representado pelo valor numérico.

![](assets/text-parser-matches-350x355.png)

Para obter os valores de correspondência necessários para adicionar colchetes à parte que você deseja analisar (por exemplo, para extrair de &quot;filename.docx&quot; - &quot;docx&quot; somente), de acordo com a expressão regex usada para esse cenário de caso, os colchetes devem ser aplicados em \.(.+)

Isso captura o DOCX, o coloca em um grupo e deixa o &quot;.&quot; fora disso.

![](assets/text-parser-get-matches-350x592.png)

Na saída mostrada na figura abaixo, o grupo de captura corresponderá a qualquer caractere (exceto para terminadores de linha).

![](assets/text-parser-output-350x389.png)

Outra solução alternativa que também incorpora o regex está usando a função replace

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

Em seguida, substitua `abcdefghijklmno pqr stuvw xyz.docx` com sua variável de nome de arquivo real.
