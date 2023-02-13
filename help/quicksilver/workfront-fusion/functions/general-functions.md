---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Funções gerais no Adobe Workfront Fusion
description: As seguintes funções gerais estão disponíveis no painel de mapeamento do Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 2%

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

## [!UICONTROL get (objeto ou matriz; path)]

Retorna o caminho do valor de um objeto ou matriz. Para acessar objetos aninhados, use a notação de pontos. O primeiro item em uma matriz é o índice 1.

>[!INFO]
>
>**Exemplos:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`


## [!UICONTROL if (expressão; valor1; value2)]

Retorna o `value1` se a expressão for avaliada como true; caso contrário, retornará a variável `value2`.

>[!INFO]
>
>**Exemplos:**
>
>* `if( 1 = 1 ; A ; B )`
   >
   >    Retorna A
>
>* `if( = 2 ; A ; B )`
   >
   >   Retorna B


## [!UICONTROL ifempty (valor1; value2)]

Retorna o `value1` se este valor não estiver vazio; caso contrário, retornará a variável `value2`.

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
   >   Retorna B
>
>* `ifempty(` `""` `;` `B` )
   >
   >   Retorna B


## [!UICONTROL switch (expressão; valor1; resultado1; [valor2; Resultado2; ...]; [else])]

Avalia um valor (chamado de expressão) em relação a uma lista de valores; retorna o resultado correspondente ao primeiro valor correspondente.

>[!INFO]
>
>**Exemplos:**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
   >
   >   Retorna 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
   >
   >   Retorna 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>  Retorna 4

## [!UICONTROL omit(object; chave1; [chave2; ...])]

Omite as teclas fornecidas do objeto e retorna o restante.

>[!INFO]
>
>**Exemplo:**
>
>`omit(` Usuário `;` senha `)`
>
>Retorna uma coleção das informações do usuário, excluindo a senha.

## [!UICONTROL select(object; chave1; [chave2; ...])]

Seleciona apenas as teclas fornecidas a partir do objeto.

>[!INFO]
>
>**Exemplo:**
>
>`pick(` Usuário `;` senha `;` email `)`
>
>Retorna uma coleção somente da senha e do endereço de email do usuário.
