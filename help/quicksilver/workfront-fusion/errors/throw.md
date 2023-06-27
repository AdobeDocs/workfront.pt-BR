---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gerar manipulação de erros no Adobe Workfront Fusion
description: Em alguns casos, você pode querer interromper de forma forçada a execução do cenário seguida pela fase Reverter ou Confirmar, ou interromper o processamento de uma rota e, opcionalmente, armazená-la na fila de Exibir e resolver execuções incompletas no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Acionar tratamento de erros no [!DNL Adobe Workfront Fusion]

Em alguns casos, convém interromper à força a execução do cenário seguida de [Reversão](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) ou [Confirmar](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) fase ou para interromper o processamento de uma rota e, opcionalmente, armazená-la na fila de execuções incompletas.

Atualmente, as diretivas de tratamento de erros não podem ser usadas fora do escopo de um [Rota do manipulador de erros](../../workfront-fusion/errors/error-handling.md#error) e [!DNL Adobe Workfront Fusion] O não oferece um módulo que permitiria gerar facilmente erros condicionalmente (throw).

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obter informações sobre diretivas de tratamento de erros, consulte [Diretivas para tratamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Solução alternativa para lançamento

Para emitir um erro condicionalmente, você pode configurar um módulo para que ele falhe propositalmente durante sua operação. Uma possibilidade é empregar o [!UICONTROL JSON] > [!UICONTROL Analisar JSON] módulo (consulte [Módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configurado para emitir um erro opcionalmente (BundleValidationError neste caso):

Em seguida, você pode anexar uma das diretivas de tratamento de erros à rota de tratamento de erros a:

* Force a execução do cenário para parar e executar a fase de reversão: [!UICONTROL Reversão]
* Force a interrupção da execução do cenário e execute a fase de confirmação: [!UICONTROL Confirmar]
* Interromper o processamento de um roteiro: [!UICONTROL Ignorar]
* Parar o processamento de uma rota e armazená-la na fila da pasta de execuções incompletas: [!UICONTROL Interrupção]

O exemplo a seguir mostra o uso de [!DNL Rollback] diretiva:

![](assets/rollback-directive-350x175.png)
