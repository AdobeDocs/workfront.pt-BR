---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Tratamento de erros de jogador no Adobe Workfront Fusion
description: Em alguns casos, você pode querer interromper forçosamente a execução do cenário seguida pela fase Reverter ou Confirmar ou interromper o processamento de uma rota e, opcionalmente, armazená-la na fila de Visualização e resolver execuções incompletas no Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# Tratamento de erros de jogador em [!DNL Adobe Workfront Fusion]

Em alguns casos, talvez você queira interromper forçosamente a execução do cenário seguida por [Reversão](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) ou [Confirmar](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) ou para interromper o processamento de uma rota e, opcionalmente, armazená-la na fila de execuções incompletas.

Atualmente, as diretivas de tratamento de erros não podem ser usadas fora do escopo de um [Rota do manipulador de erros](../../workfront-fusion/errors/error-handling.md#error) e [!DNL Adobe Workfront Fusion] O não oferece um módulo que permitiria gerar (lançar) erros condicionalmente facilmente.

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obter informações sobre diretivas de tratamento de erros, consulte [Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Solução alternativa para lançamento

Para gerar um erro condicionalmente, você pode configurar um módulo para que ele falhe opcionalmente durante sua operação. Uma possibilidade é empregar a variável [!UICONTROL JSON] > [!UICONTROL Analisar JSON] módulo (consulte [Módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configurado para gerar um erro opcionalmente (BundleValidationError neste caso):

Em seguida, é possível anexar uma das diretivas de tratamento de erros à rota de tratamento de erros para:

* Forçar a execução do cenário a parar e executar a fase de reversão: [!UICONTROL Reversão]
* Forçar a execução do cenário a parar e executar a fase de confirmação: [!UICONTROL Confirmar]
* Parar o processamento de uma rota: [!UICONTROL Ignorar]
* Pare o processamento de uma rota e armazene-a na fila da pasta de execuções incompletas: [!UICONTROL Quebra]

O exemplo a seguir mostra o uso da variável [!DNL Rollback] diretiva:

![](assets/rollback-directive-350x175.png)
