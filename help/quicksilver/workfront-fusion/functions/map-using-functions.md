---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mapear itens usando funções no [!DNL Adobe Workfront Fusion]
description: Ao mapear itens, você pode usar funções para criar fórmulas simples ou complexas.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Mapear itens usando funções no [!DNL Adobe Workfront Fusion]

Ao mapear itens, você pode usar funções para criar fórmulas simples ou complexas.

As funções disponíveis em [!DNL Adobe Workfront Fusion] são semelhantes às funções no Excel e em algumas linguagens de programação. Eles avaliam a lógica geral, a matemática, o texto, as datas e os arrays. Elas permitem executar a lógica condicional e transformações de valores de item, como converter um texto em maiúsculas, aparar texto, converter uma data em um formato diferente e muito mais. Para obter mais informações, consulte [Mapear informações de um módulo para outro no Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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

## Inserir funções em campos

Se você clicar em um campo, a variável [!UICONTROL mapeamento] será exibido. O painel de mapeamento contém várias guias:

![](assets/functions-toolbar-350x189.png)

A primeira guia ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (mostrado ao abrir o painel) exibe os itens que você pode mapear de outros módulos.

As outras guias contêm os seguintes tipos de funções:

* **Funções gerais** ![](assets/toolbar-icon-general-function.png) - Consulte [Funções gerais em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) para obter mais informações.

* **Funções matemáticas** ![](assets/toolbar-icon-math-functions.png) - Consulte [Funções matemáticas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) para obter mais informações.

* **Funções binárias e de texto** ![](assets/toolbar-icon-text&binary-functions.png) - Consulte [Funções de string em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) para obter mais informações.

* **Data e hora** ![](assets/toolbar-icon-date&time-functions.png) - Consulte [Funções de data e hora em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) e os artigos abaixo para obter mais informações.

   * [Tokens para formatação de data e hora em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens para análise de data e hora em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funções para trabalhar com arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Consulte [Funções de matriz em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) para obter mais informações.

Para inserir uma função em um campo:

1. Clique no nome da função.

   Ou

   Arraste a função para o campo .

>[!INFO]
>
>**Exemplo:** Alguns tipos de dados impedem que os usuários insiram mais de um determinado número de caracteres. Você pode usar a função de substring para limitar um valor a um determinado número de caracteres.
>
>Neste exemplo, a função de substring limita o nome do projeto a 50 caracteres.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Funções de aninhamento

Você pode aninhar funções entre si.

## Use [!DNL Google Sheets] funções

If [!DNL Workfront Fusion] não apresenta uma função que você deseja usar, mas ela é apresentada por [!DNL Google Sheets], você pode usá-lo seguindo estas etapas:

1. Em [!DNL Google Sheets], crie uma nova planilha vazia.
1. Em [!DNL Workfront Fusion], abra o cenário.
1. Adicione o **[!DNL Google Sheets]** >**[!UICONTROL Atualizar uma célula]** para o cenário.

   Para obter instruções sobre como adicionar um módulo, consulte [Adicionar um módulo em um cenário](../../workfront-fusion/scenarios/create-a-scenario.md#add) no artigo [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configure o módulo :

   1. Escolha a planilha recém-criada na **[!UICONTROL Planilha]** campo.
   1. Insira sua fórmula contendo o [!DNL Google Sheets] função(ões) na **[!UICONTROL Valor]** campo.

      Você pode usar a saída dos módulos anteriores como de costume.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Insira o **[!UICONTROL Google Sheets] >[!UICONTROL Obter uma célula]** para obter o resultado calculado.
1. Configure o módulo, usando a mesma ID de célula usada na etapa 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
