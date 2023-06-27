---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mapear itens usando funções no [!DNL Adobe Workfront Fusion]
description: Ao mapear itens, você pode usar funções para criar fórmulas simples ou complexas.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Mapear itens usando funções no [!DNL Adobe Workfront Fusion]

Ao mapear itens, você pode usar funções para criar fórmulas simples ou complexas.

As funções disponíveis em [!DNL Adobe Workfront Fusion] são semelhantes a funções no Excel e em algumas linguagens de programação. Eles avaliam a lógica geral, matemática, texto, datas e matrizes. Elas permitem executar lógica condicional e transformações de valores de item, como converter um texto em maiúsculas, cortar texto, converter uma data em um formato diferente e muito mais. Para obter mais informações, consulte [Mapear informações de um módulo para outro no Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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

## Inserir funções em campos

Se você clicar em um campo, a variável [!UICONTROL mapeamento] é exibido. O painel de mapeamento contém várias guias:

![](assets/functions-toolbar-350x189.png)

A primeira guia ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (exibido ao abrir o painel) exibe os itens que você pode mapear de outros módulos.

As outras guias contêm os seguintes tipos de funções:

* **Funções gerais** ![](assets/toolbar-icon-general-function.png) - Consulte [Funções gerais no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) para obter mais informações.

* **Funções matemáticas** ![](assets/toolbar-icon-math-functions.png) - Consulte [Funções matemáticas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) para obter mais informações.

* **Funções de texto e binárias** ![](assets/toolbar-icon-text&binary-functions.png) - Consulte [Funções de string em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) para obter mais informações.

* **Data e hora** ![](assets/toolbar-icon-date&time-functions.png) - Consulte [Funções de data e hora no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) e os artigos abaixo para obter mais informações.

   * [Tokens para formatação de data e hora no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens para análise de data e hora no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funções para trabalhar com arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Consulte [Funções de matriz em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) para obter mais informações.

Para inserir uma função em um campo:

1. Clique no nome da função.

   Ou

   Arraste a função para o campo.

>[!INFO]
>
>**Exemplo:** Alguns tipos de dados impedem que os usuários insiram mais do que um determinado número de caracteres. Você pode usar a função substring para limitar um valor a um determinado número de caracteres.
>
>Neste exemplo, a função de subsequência de caracteres limita o nome do projeto a 50 caracteres.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Aninhamento de funções

É possível aninhar funções entre si.

## Uso [!DNL Google Sheets] funções

Se [!DNL Workfront Fusion] não apresenta uma função que deseja usar, mas é apresentada por [!DNL Google Sheets], você pode usá-lo seguindo estas etapas:

1. Entrada [!DNL Google Sheets], crie uma nova planilha vazia.
1. Entrada [!DNL Workfront Fusion], abra o cenário.
1. Adicione o **[!DNL Google Sheets]** >**[!UICONTROL Atualizar uma célula]** para o cenário.

   Para obter instruções sobre como adicionar um módulo, consulte [Adicionar um módulo em um cenário](../../workfront-fusion/scenarios/create-a-scenario.md#add) no artigo [Criar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Configure o módulo:

   1. Escolha a planilha recém-criada no **[!UICONTROL Planilha]** campo.
   1. Insira a fórmula que contém o [!DNL Google Sheets] função(ões) na **[!UICONTROL Valor]** campo.

      Você pode usar a saída dos módulos anteriores como de costume.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Insira o **[!UICONTROL Planilhas Google] >[!UICONTROL Obter uma célula]** para obter o resultado calculado.
1. Configure o módulo, usando a mesma ID de célula que você usou na etapa 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
