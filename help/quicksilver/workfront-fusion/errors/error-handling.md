---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Tratamento de erros no [!DNL Adobe Workfront Fusion]
description: Quando ocorrem erros durante a execução de um cenário, geralmente ocorre porque um serviço está indisponível devido a uma falha, um serviço responde com dados inesperados ou a validação de dados de entrada falha.
author: Becky
feature: Workfront Fusion
exl-id: a08c18a0-1797-4126-827a-1ea7e11d4bad
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Tratamento de erros no [!DNL Adobe Workfront Fusion]

Quando ocorrem erros durante a execução de um cenário, geralmente ocorre porque um serviço está indisponível devido a uma falha, um serviço responde com dados inesperados ou a validação de dados de entrada falha.

Se um módulo lançar um erro durante a execução do cenário e não houver nenhuma rota de tratamento de erros anexada ao módulo, a lógica de tratamento de erros padrão será executada, conforme descrito em [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

Ao adicionar uma rota de manipulador de erros a um módulo, você pode substituir a lógica de manipulação de erros padrão pela sua própria. [!DNL Adobe Workfront Fusion] O oferece cinco diretivas diferentes que podem ser inseridas no final das rotas do manipulador de erros.

Para obter mais informações, consulte [Diretivas para tratamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

## Rota do manipulador de erros

Para adicionar uma rota de manipulador de erros a um módulo:

1. Clique com o botão direito no módulo e selecione **[!UICONTROL Adicionar manipulador de erros]**:

   ![](assets/error-handler-route.png)

   O módulo mostra uma lista de Diretivas, bem como os aplicativos que estão sendo usados no seu cenário.

1. Se o módulo ao qual você adicionou um manipulador de erros for o último módulo em sua rota, selecione uma das diretivas.

   Ou

   Adicione um ou mais módulos à rota do manipulador de erros.

   Se você adicionar mais módulos à rota, a variável [!UICONTROL Ignorar] é aplicada por padrão e, no caso de um erro, os módulos subsequentes nessa rota serão processados.


>[!INFO]
>
>Neste exemplo, se ocorrer um erro durante a execução da variável [!UICONTROL Criar uma pasta] módulo, a variável [!UICONTROL Ignorar] A diretiva será aplicada automaticamente e o cenário será movido para o próximo módulo na rota do manipulador de erros.
>
>No entanto, se não houver erro, o cenário será movido para a tag [!UICONTROL Listar todos os arquivos em um módulo de pasta] no itinerário regular.
>
>![](assets/if-there-is-no-error-350x234.png)

Observe que uma rota de manipulador de erros é composta de círculos transparentes, enquanto uma rota regular é composta de círculos sólidos.

## Erro ao manipular diretivas

As diretivas são resumidamente explicadas a seguir. Para obter mais informações, consulte [Diretivas para tratamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

Há um total de cinco diretivas que podem ser agrupadas nas seguintes categorias com base em se a execução de um cenário deve continuar ou não.

As diretivas a seguir garantem que uma execução de cenário continue:

* **[!UICONTROL Retomar]**: permite especificar uma saída substituta para o módulo com o erro. O status de execução do cenário é marcado como sucesso
* **[!UICONTROL Ignorar]**: ignora o erro. O status de execução do cenário é marcado como sucesso
* **[!UICONTROL Interrupção]**: armazena a entrada na fila de execuções incompletas. O status de execução do cenário está marcado como aviso. Para obter mais informações, consulte [Exibir e resolver execuções incompletas no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Se uma execução de cenário precisar parar quando ocorrer um erro, use uma das seguintes diretivas:

* **[!UICONTROL Reversão]**: interrompe a execução do cenário imediatamente e marca seu status como erro
* **[!UICONTROL Confirmar]**: interrompe a execução do cenário imediatamente e marca seu status como sucesso

Para obter mais informações sobre o tratamento de erros, consulte:

* [Diretivas para tratamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)
* [Tratamento de erros avançado no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/advanced-error-handling.md)