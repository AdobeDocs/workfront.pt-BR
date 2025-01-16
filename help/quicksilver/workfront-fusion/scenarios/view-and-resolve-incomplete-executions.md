---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 5%

---

# Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Exibir e resolver execuções incompletas](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-and-resolve-incomplete-executions.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

A pasta [!UICONTROL Execuções incompletas] armazena execuções de cenário que não foram finalizadas com êxito devido a um erro. Cada execução incompleta armazenada pode ser resolvida manual ou automaticamente.

>[!NOTE]
>
>Por padrão, o armazenamento de execuções incompletas é desativado. Para habilitá-lo, habilite a opção [!UICONTROL Permitir o armazenamento de execuções incompletas] nas configurações avançadas de cenário.
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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
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

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Exibir execuções incompletas

Se um módulo encontrar um erro durante sua operação, uma nova execução incompleta será adicionada à pasta Incomplete executions. Cada execução incompleta contém o blueprint do cenário e todos os pacotes que podem ser mapeados no módulo com falha. É possível abrir a lista de execuções incompletas clicando na guia [!UICONTROL Execuções Incompletas] na página de detalhes do cenário.

<!--

![](assets/incomplete-executions-tab-350x102.png)

-->

Para obter mais informações, consulte [Erros resultantes em execuções incompletas](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>O limite de tamanho atual da pasta de execuções incompletas não resolvidas por organização é de 500 MB. Se sua organização exceder esse limite, você poderá ver o seguinte erro:
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>Para obter mais informações, consulte [Habilitar perda de dados](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) em [O painel de configurações do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Resolver execuções incompletas

Quando uma nova execução incompleta é armazenada, você pode resolvê-la da seguinte maneira:

1. Clique na guia **[!UICONTROL Execuções incompletas]**.
1. Localize a execução incompleta que você deseja resolver e clique em **[!UICONTROL Detalhe]**.


   Se quiser ver o log de todas as operações do módulo antes de tentar resolver a execução incompleta, você poderá resolver a execução incompleta na pasta [!UICONTROL Histórico]:

1. Clique na guia **[!UICONTROL Histórico]**.
1. Localize o log de execução com falha do cenário e clique em **[!UICONTROL Detalhes]**.
1. Abra o registro do módulo em que todas as operações do módulo são exibidas.
1. Localize a operação com falha e clique em **[!UICONTROL Resolver]**:

   ![](assets/resolve-btn-350x188.png)

## Opções relacionadas a execuções incompletas

As seguintes opções no painel [!UICONTROL Configurações de cenário] determinam se e como as execuções incompletas são armazenadas:

* Permitir o armazenamento de execuções incompletas
* Processamento sequencial
* Ativar perda de dados

Para obter mais informações sobre essas opções, consulte [O painel de configurações do cenário [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Erros que resultam em execuções incompletas

Há várias categorias de erros que resultam no armazenamento de execuções incompletas. Estas podem incluir:

* Erros de validação decorrentes de dados incompletos ou errôneos, principalmente por causa de um item ausente esperado para processar com êxito todos os dados que passam por um módulo.
* Erros que ocorrem devido à indisponibilidade do destino final devido a uma falha temporária ou de longa duração na conexão (por exemplo, durante a conexão com o servidor de email ou FTP remoto).

Se ocorrer um erro no primeiro módulo do cenário, a execução será interrompida imediatamente e nenhuma execução incompleta será armazenada.

Se ocorrer um erro em qualquer outro módulo e não houver nenhuma rota de manipulador de erros anexada, uma das seguintes situações ocorrerá:

* Se o tipo de erro for `ConnectionError`, `RateLimitError`, `OutOfSpaceError` ou `ModuleTimeoutError`, um registro de execução incompleto com repetição automática será armazenado.
* Se o tipo de erro for `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError` ou `MaxResultsExceededError`, um registro de execução incompleto sem repetição automática será armazenado.
* Se o tipo de erro for diferente dos mencionados acima, a execução falhará.
