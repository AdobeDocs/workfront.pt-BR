---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]
description: O [!UICONTROL Execuções incompletas] A pasta armazena execuções de cenário que não foram finalizadas com êxito devido a um erro. Cada execução incompleta armazenada pode ser resolvida manual ou automaticamente.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]

O [!UICONTROL Execuções incompletas] A pasta armazena execuções de cenário que não foram finalizadas com êxito devido a um erro. Cada execução incompleta armazenada pode ser resolvida manual ou automaticamente.

>[!NOTE]
>
>Por padrão, o armazenamento de execuções incompletas é desabilitado. Para habilitá-lo, ative a variável [!UICONTROL Permitir o armazenamento de execuções incompletas] nas configurações avançadas do cenário.
>
>Para obter mais informações sobre configurações de cenário, consulte [O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Exibir execuções incompletas

Se um módulo encontrar um erro durante sua operação, uma nova execução incompleta será adicionada à pasta Incomplete executions . Cada execução incompleta contém o blueprint do cenário e todos os pacotes que podem ser mapeados no módulo com falha. A lista de execuções incompletas pode ser aberta clicando no botão [!UICONTROL Execuções incompletas] na página de detalhes do cenário:

![](assets/incomplete-executions-tab-350x102.png)

Para obter mais informações, consulte [Erros que resultam em execuções incompletas](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>O limite de tamanho atual da pasta de execuções incompletas não resolvidas por organização é de 500 MB. Se sua organização exceder esse limite, você poderá ver o seguinte erro:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Para obter mais informações, consulte [Ativar perda de dados](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) em [O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Resolver execuções incompletas

Quando uma nova execução incompleta é armazenada, é possível resolvê-la da seguinte maneira:

1. Clique no botão **[!UICONTROL Execuções incompletas]** guia .
1. Localize a execução incompleta que deseja resolver e clique em **[!UICONTROL Detalhe]**.


   Se quiser ver o log de todas as operações do módulo antes de tentar resolver a execução incompleta, poderá resolver a execução incompleta da variável [!UICONTROL Histórico] pasta:

1. Clique no botão **[!UICONTROL Histórico]** guia .
1. Localize o log de execução com falha do cenário e clique em **[!UICONTROL Detalhes]**.
1. Abra o log do módulo, onde todas as operações do módulo serão mostradas.
1. Localize a operação com falha e clique em **[!UICONTROL Resolver]**:

   ![](assets/resolve-btn-350x188.png)

## Opções relacionadas com execuções incompletas

As seguintes opções na [!UICONTROL Configurações de cenário] determinam se e como as execuções incompletas são armazenadas:

* Permitir o armazenamento de execuções incompletas
* Processamento sequencial
* Ativar perda de dados

Para obter mais informações sobre essas opções, consulte [O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Erros que resultam em execuções incompletas

Existem várias categorias de erros que resultam no armazenamento de execuções incompletas. Essas medidas podem incluir:

* Erros de validação decorrentes de dados incompletos ou errôneos, principalmente por causa de um item ausente que é esperado para processar com êxito todos os dados que passam por um módulo.
* Erros que ocorrem devido à indisponibilidade do destino final devido a uma falha de conexão temporária ou de longo prazo (por exemplo, durante a conexão com o email ou o servidor FTP remoto).

Se ocorrer um erro no primeiro módulo do cenário, a execução será interrompida imediatamente e nenhuma execução incompleta será armazenada.

Se ocorrer um erro em qualquer outro módulo e não houver uma rota de manipulador de erros conectada, uma das seguintes situações ocorrerá:

* Se o tipo de erro for `ConnectionError`, `RateLimitError`, `OutOfSpaceError` ou `ModuleTimeoutError`, um registro de execução incompleto com tentativa automática é armazenado.
* Se o tipo de erro for `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`ou `MaxResultsExceededError`, um registro de execução incompleto sem tentativa automática é armazenado.
* Se o tipo de erro for diferente do acima, a execução falhará.
