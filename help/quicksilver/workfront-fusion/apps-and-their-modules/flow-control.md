---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Controle de fluxo no Adobe Workfront Fusion
description: Ao criar ou editar um cenário, você pode definir configurações para controlar como os dados fluem por ele.
author: Becky
feature: Workfront Fusion
exl-id: 0f315192-c15e-48e8-a5b6-827c300f0e5c
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Controle de fluxo no Adobe Workfront Fusion

Ao criar ou editar um cenário, você pode definir configurações para controlar como os dados fluem por ele.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
  <td> <p>[!UICONTROL Pro] ou superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o plano [!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Adobe Workfront], sua organização deve comprar [!DNL Adobe Workfront Fusion] e [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Repetidor

Você pode usar um módulo [!UICONTROL Repetidor] para repetir uma tarefa um determinado número de vezes. Um módulo [!UICONTROL Repetidor] gera conjuntos, um após o outro.

Por exemplo, você pode usar um módulo [!UICONTROL Repetidor] para enviar cinco emails com os assuntos &quot;Olá 1&quot;, &quot;Olá 2&quot; e assim por diante, conectando o módulo **[!UICONTROL Email] >[!UICONTROL Enviar um email]** ao módulo [!UICONTROL Repetidor].

Para usar um módulo [!UICONTROL Repetidor]:

1. Clique no ícone ![](assets/flow-control-icon.gif) do [!UICONTROL Controle de Fluxo] na parte inferior da tela e em **[!UICONTROL Repetidor]** no menu exibido.
1. Clique no pacote [!UICONTROL Repetidor] e em **[!UICONTROL Conectar-se automaticamente]** na caixa exibida.
1. Na caixa [!UICONTROL Controle de Fluxo] exibida, digite o número de repetições (pacotes de saída) desejadas na caixa **[!UICONTROL Repetições]**.

   Em nosso exemplo de email, você digitaria 5.

   ![](assets/repeater-2-350x207.png)

   O valor do item aumenta em cada repetição com este valor especificado no campo **[!UICONTROL Etapa]**, que pode ser visualizado ao selecionar **[!UICONTROL Mostrar configurações avançadas]**. Esse número é 1 por padrão.

1. Clique em **[!UICONTROL OK]** para fechar a caixa **[!UICONTROL Controle de Fluxo]**.

1. Clique no módulo de aplicativo ou serviço conectado ao módulo [!UICONTROL Repetidor].
1. Na caixa exibida, digite as informações que deseja repetir.

   No nosso exemplo de email, você digitaria Olá na caixa [!UICONTROL Assunto] e mapearia `i` do módulo do repetidor.

   ![](assets/repeater-3-350x207.png)

| Item | Descrição |
|---|---|
| [!UICONTROL Valor inicial] | Insira ou mapeie o número que você deseja que o módulo defina como `i` na primeira iteração. O valor padrão é 1. |
| [!UICONTROL Repetições] | Insira ou mapeie o número de vezes que você deseja que o módulo se repita. Esse número deve ser maior ou igual a 0 e menor ou igual a 10.000. |
| [!UICONTROL Etapa] | Este é o número pelo qual o módulo aumenta o valor de `i`. O valor padrão é 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>O número de repetições não é determinado pelo valor de `i`, pois estaria em um loop na programação. O módulo repetirá o número de vezes indicado no campo [!UICONTROL Repetições]. O valor `i` é alterado com cada iteração do módulo [!DNL repeater] e pode ser mapeado para módulos posteriores. O exemplo acima mapeia o valor de `i` na mensagem Hello, resultando em mensagens que leem &quot;Hello 1,&quot; Hello 2 e assim por diante.

## [!UICONTROL Iterador]

Um [!UICONTROL Iterador] é um tipo especial de módulo que converte uma matriz em uma série de conjuntos. Cada item de matriz será um conjunto separado na saída do módulo [!UICONTROL Iterador]. Para obter mais informações, consulte o módulo [[!UICONTROL Iterador] em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Agregador de matrizes

Um agregador de matriz é um tipo especial de módulo que permite mesclar vários pacotes em um único pacote. Para obter mais informações, consulte o módulo [[!UICONTROL Agregador] no Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Roteador]

O módulo [!UICONTROL Roteador] permite ramificar seu fluxo em várias rotas e processar os dados em cada rota de forma diferente. Depois que um módulo [!UICONTROL Roteador] receber um pacote, ele o encaminhará para cada rota conectada na ordem em que as rotas foram anexadas ao módulo [!UICONTROL Roteador]. Para obter mais informações, consulte [Módulo de roteador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
