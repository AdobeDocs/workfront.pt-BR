---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Gerar manipulação de erros no Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Gerar manipulação de erros em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Configurar solução alternativa de erro `throw`](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-error-handling/throw.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

Em alguns casos, você pode querer interromper forçosamente a execução do cenário seguido da fase [Reversão](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) ou [Confirmação](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) ou parar o processamento de uma rota e, opcionalmente, armazená-la na fila de execuções incompletas.

Atualmente, as diretivas de tratamento de erros não podem ser usadas fora do escopo de uma [rota do manipulador de erros](../../workfront-fusion/errors/error-handling.md#error) e [!DNL Adobe Workfront Fusion] não oferece um módulo que permitiria gerar (lançar) erros condicionalmente facilmente.

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obter informações sobre diretivas de tratamento de erros, consulte [Diretivas para tratamento de erros em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Solução alternativa para lançamento

Para emitir um erro condicionalmente, você pode configurar um módulo para que ele falhe propositalmente durante sua operação. Uma possibilidade é empregar o módulo [!UICONTROL JSON] > [!UICONTROL Parse JSON] (consulte [módulos JSON](../../workfront-fusion/apps-and-their-modules/json-modules.md)), configurado opcionalmente para emitir um erro (BundleValidationError neste caso):

Em seguida, você pode anexar uma das diretivas de tratamento de erros à rota de tratamento de erros a:

* Forçar a execução do cenário a parar e executar a fase de reversão: [!UICONTROL Reversão]
* Força a interrupção da execução do cenário e a execução da fase de confirmação: [!UICONTROL Confirmar]
* Parar o processamento de uma rota: [!UICONTROL Ignorar]
* Parar o processamento de uma rota e armazená-la na fila da pasta de execuções incompletas: [!UICONTROL Interrupção]

O exemplo a seguir mostra o uso da diretiva [!DNL Rollback]:

![](assets/rollback-directive-350x175.png)
