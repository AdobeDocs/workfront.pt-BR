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
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 1%

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
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

## Repetidor

Você pode usar um [!UICONTROL Repetidor] módulo para repetir uma tarefa um determinado número de vezes. A [!UICONTROL Repetidor] O módulo gera pacotes, um após o outro.

Por exemplo, você pode usar um [!UICONTROL Repetidor] módulo para enviar cinco emails com os assuntos &quot;Olá 1&quot;, &quot;Olá 2&quot; e assim por diante, conectando o **[!UICONTROL E-mail] >[!UICONTROL Envie-me um email]** módulo para o [!UICONTROL Repetidor] módulo.

Para usar uma [!UICONTROL Repetidor] módulo:

1. Clique em [!UICONTROL Controle de fluxo] ícone ![](assets/flow-control-icon.gif) na parte inferior da tela e clique em **[!UICONTROL Repetidor]** no menu exibido.
1. Clique em [!UICONTROL Repetidor] e clique em **[!UICONTROL Conectar automaticamente]** na caixa exibida.
1. No [!UICONTROL Controle de fluxo] que for exibida, digite o número de repetições (pacotes enviados) desejadas na caixa **[!UICONTROL Repetições]** caixa.

   Em nosso exemplo de email, você digitaria 5.

   ![](assets/repeater-2-350x207.png)

   O valor do item aumenta em cada repetição de acordo com este valor especificado no **[!UICONTROL Etapa]** campo, que pode ser exibido ao selecionar **[!UICONTROL Mostrar configurações avançadas]**. Esse número é 1 por padrão.

1. Clique em **[!UICONTROL OK]** para fechar o **[!UICONTROL Controle de fluxo]** caixa.

1. Clique no módulo de aplicativo ou serviço conectado à [!UICONTROL Repetidor] módulo.
1. Na caixa exibida, digite as informações que deseja repetir.

   No nosso exemplo de email, você digitaria Hello no campo [!UICONTROL Assunto] , depois mapear `i` do módulo repetidor.

   ![](assets/repeater-3-350x207.png)

| Item | Descrição |
|---|---|
| [!UICONTROL Valor inicial] | Insira ou mapeie o número que você deseja que o módulo defina como `i` na primeira iteração. O valor padrão é 1. |
| [!UICONTROL Repete] | Insira ou mapeie o número de vezes que você deseja que o módulo se repita. Esse número deve ser maior ou igual a 0 e menor ou igual a 10.000. |
| [!UICONTROL Passo] | Este é o número pelo qual o módulo aumenta o valor de `i`. O valor padrão é 1. |

{style="table-layout:auto"}

>[!NOTE]
>
>O número de repetições não é determinado pelo valor de `i`, como estaria em um loop na programação. O módulo repetirá o número de vezes indicado na variável [!UICONTROL Repetições] campo. O valor `i` é alterado a cada iteração de [!DNL repeater] e podem ser mapeados para módulos posteriores. O exemplo acima mapeia o valor de `i` na mensagem Hello, resultando em mensagens que leem &quot;Hello 1&quot;, &quot;Hello 2&quot; e assim por diante.

## [!UICONTROL Iterador]

Um [!UICONTROL Iterador] é um tipo especial de módulo que converte uma matriz em uma série de pacotes. Cada item de array será um pacote separado no [!UICONTROL Iterador] saída do módulo. Para obter mais informações, consulte [[!UICONTROL Iterador] módulo no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

## Agregador de matrizes

Um agregador de matriz é um tipo especial de módulo que permite mesclar vários pacotes em um único pacote. Para obter mais informações, consulte [[!UICONTROL Agregador] módulo no Adobe Workfront Fusion](../../workfront-fusion/modules/aggregator-module.md).

## [!UICONTROL Roteador]

A variável [!UICONTROL Roteador] permite ramificar seu fluxo em várias rotas e processar os dados dentro de cada rota de forma diferente. Uma vez a [!UICONTROL Roteador] recebe um pacote, ele o encaminha para cada rota conectada na ordem em que as rotas foram anexadas ao [!UICONTROL Roteador] módulo. Para obter mais informações, consulte [Módulo de roteador em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Directives</h2>
<p>The error handling directives allow you to control how your scenario reacts to errors. For more information, see <a href="../../workfront-fusion/errors/advanced-error-handling.md" class="MCXref xref">Advanced error handling in Adobe Workfront Fusion</a> and <a href="../../workfront-fusion/errors/directives-for-error-handling.md" class="MCXref xref">Directives for error handling in Adobe Workfront Fusion</a>.</p>
</div>
-->
