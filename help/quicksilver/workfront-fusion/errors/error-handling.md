---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Tratamento de erros em [!DNL Adobe Workfront Fusion]
description: Quando ocorrem erros durante a execução de um cenário, geralmente ocorre porque um serviço não está disponível devido a uma falha, um serviço responde com dados inesperados ou a validação de dados de entrada falha.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: e936bbd2837e4aec67d4136b8efcccb6f8454a89
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# Tratamento de erros em [!DNL Adobe Workfront Fusion]

Quando ocorrem erros durante a execução de um cenário, geralmente ocorre porque um serviço não está disponível devido a uma falha, um serviço responde com dados inesperados ou a validação de dados de entrada falha.

Se um módulo gerar um erro durante a execução do cenário e não houver uma rota de tratamento de erros anexada ao módulo, a lógica de tratamento de erros padrão será executada, conforme descrito em [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Ao adicionar uma rota do manipulador de erros a um módulo, você pode substituir a lógica padrão de tratamento de erros pela sua. [!DNL Adobe Workfront Fusion] O oferece cinco diretivas diferentes que podem ser inseridas no final de suas rotas do manipulador de erros.

Para obter mais informações, consulte [Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Rota do manipulador de erros

Para adicionar uma rota do manipulador de erros a um módulo:

1. Clique com o botão direito do mouse no módulo e selecione **[!UICONTROL Adicionar manipulador de erros]**:

   ![](assets/error-handler-route.png)

   O módulo mostra uma lista de Diretivas, bem como os aplicativos que estão sendo usados em seu cenário.

1. Se o módulo ao qual você adicionou um manipulador de erros for o último módulo em sua rota, selecione uma das diretivas.

   Ou

   Adicione um ou mais módulos à rota do manipulador de erros.

   Se você adicionar mais módulos à rota, a variável [!UICONTROL Ignorar] for aplicada por padrão e, em caso de erro, os módulos subsequentes nessa rota serão processados.


>[!INFO]
>
>Neste exemplo, se ocorrer um erro ao executar o [!UICONTROL Criar uma pasta] , o [!UICONTROL Ignorar] a diretiva será aplicada automaticamente e o cenário será movido para o próximo módulo na rota do manipulador de erros.
>
>No entanto, se não houver erro, o cenário será movido para a variável [!UICONTROL Listar todos os arquivos em um módulo de pasta] na rota regular.
>
>![](assets/if-there-is-no-error-350x234.png)

Observe que uma rota do manipulador de erros é composta por círculos transparentes, enquanto uma rota regular é composta de círculos sólidos.

## Diretivas de tratamento de erros

As diretivas são brevemente explicadas a seguir. Para obter mais informações, consulte [Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Há um total de cinco diretivas que podem ser agrupadas nas seguintes categorias com base em se uma execução de cenário deve continuar ou não.

As diretivas a seguir garantem que a execução de um cenário continue:

* **[!UICONTROL Retomar]**: Permite especificar uma saída substituta para o módulo com o erro. O status de execução do cenário é marcado como bem-sucedido
* **[!UICONTROL Ignorar]**: ignora o erro. O status de execução do cenário é marcado como bem-sucedido
* **[!UICONTROL Quebra]**: Armazena a entrada na fila de execuções incompletas. O status de execução do cenário é marcado como aviso. Para obter mais informações, consulte [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Se uma execução de cenário deve parar quando ocorrer um erro, use uma das seguintes diretivas:

* **[!UICONTROL Reversão]**: Interrompe a execução do cenário imediatamente e marca seu status como erro
* **[!UICONTROL Confirmar]**: Interrompe a execução do cenário imediatamente e marca seu status como sucesso

Para obter mais informações sobre tratamento de erros, consulte:

* [Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Tratamento de erros avançado em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)