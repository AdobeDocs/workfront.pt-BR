---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções gerais no Adobe Workfront Fusion
description: As seguintes funções gerais estão disponíveis no painel Mapeamento do Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 4cca9738ad9537247234faa0b1c441163d4e315f
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Funções gerais em [!DNL Adobe Workfront Fusion]

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
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL obter (objeto ou matriz; caminho)]

Retorna o caminho do valor de um objeto ou matriz. Para acessar objetos aninhados, use a notação de pontos. O primeiro item em uma matriz é o índice 1.

>[!INFO]
>
>**Exemplos:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if (expressão; valor1; valor2)]

Retorna `value1` se a expressão for avaliada como verdadeira; caso contrário, retorna `value2`.

Para criar uma instrução if que retorne um valor somente se duas ou mais expressões forem avaliadas como true, use a palavra-chave `and`.

Para combinar instruções `if`, use os operadores `and` e `or`.

![e operador](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**Exemplos:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    Retorna A
>
>* `if( 1 = 2 ; A ; B )`
>
>   Devoluções B
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    Devoluções B
>   

## [!UICONTROL ifempty (value1; value2)]

Retorna `value1` se este valor não estiver vazio; caso contrário, retorna `value2`.

>[!INFO]
>
>**Exemplos:**
>
>* `ifempty(` `A` `;` `B` )
>
>   Retorna A
>
>* `ifempty(` `unknown` `;` `B` )
>
>   Devoluções B
>
>* `ifempty(` `""` `;` `B` )
>
>   Devoluções B

## [!UICONTROL opção (expressão; valor1; resultado1; [valor2; resultado2; ...]; [outra])]

Avalia um valor (chamado de expressão) em relação a uma lista de valores; retorna o resultado correspondente ao primeiro valor correspondente. Para incluir um valor `else`, adicione-o depois da expressão ou valor final.

>[!INFO]
>
>**Exemplos:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Devoluções 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   Devoluções 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>   Devoluções 4
>   
>   Nesta função, 4 é o valor a ser retornado se nenhuma expressão se aplicar (o valor `else`).

## [!UICONTROL omit(object; key1; [key2; ...])]

Omite as chaves fornecidas do objeto e retorna o restante.

>[!INFO]
>
>**Exemplo:**
>
>`omit(` Usuário `;` senha `)`
>
>Retorna uma coleção das informações do usuário, excluindo a senha.

## [!UICONTROL pick(object; key1; [key2; ...])]

Seleciona somente as chaves fornecidas do objeto.

>[!INFO]
>
>**Exemplo:**
>
>`pick(` Usuário `;` senha `;` email `)`
>
>Retorna uma coleção somente da senha e do endereço de email do usuário.
