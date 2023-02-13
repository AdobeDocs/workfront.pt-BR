---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: O painel de configurações de cenário no Adobe Workfront Fusion
description: Este artigo descreve as configurações disponíveis no [!UICONTROL configurações de cenário] no seu painel [!DNL Adobe Workfront Fusion] cenários.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '968'
ht-degree: 0%

---

# O painel de configurações de cenário em [!DNL Adobe Workfront Fusion]

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

## Abra as configurações de cenário

1. Abra o editor de cenário, como explicado em [O editor de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Clique no ícone de engrenagem próximo ao canto inferior esquerdo da página.

   ![](assets/scenario-settings-350x221.png)

   No [!UICONTROL Configurações de cenário] painel que é exibido, é possível definir várias configurações avançadas para o cenário.

## [!UICONTROL Permitir o armazenamento de execuções incompletas]

Essa opção determina como [!DNL Adobe Workfront Fusion] prossegue se ocorrer um erro durante a execução de um cenário. Com essa opção ativada, o cenário é pausado e movido para [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Isso oferece a possibilidade de corrigir o problema e continuar a executar a partir de onde o cenário foi interrompido. Se essa opção estiver desativada, a execução do cenário será interrompida e uma fase de reversão será iniciada.

## [!UICONTROL Processamento sequencial]

Essa opção determina como [!DNL Workfront Fusion] prossegue se ocorrer um erro e a execução de um cenário for movida para a função [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Se a variável [!UICONTROL Processamento sequencial] estiver ativada, o Workfront Fusion interrompe completamente o processamento da sequência de tarefas até que todas as execuções incompletas sejam resolvidas. Se a variável [!UICONTROL Processamento sequencial] estiver desabilitada, o cenário continuará sendo executado de acordo com seu cronograma, acompanhado por tentativas repetidas de executar novamente as execuções incompletas.

Para obter mais informações sobre a programação, consulte [Programe um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Os dados são confidenciais

Depois que um cenário é executado, é possível exibir, por padrão, as informações sobre quais dados foram processados pelos módulos no cenário. Se não quiser que essas informações sejam armazenadas, ative a [!UICONTROL Os dados são confidenciais] opção.

Para obter mais informações sobre como exibir informações, consulte [Fluxo de execução do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Se você habilitar essa opção, pode ser difícil resolver erros que podem ocorrer durante a execução de um cenário.

## Ativar perda de dados

Essa opção tem a ver com a ativação de perda de dados se [!DNL Workfront Fusion] falha ao salvar um pacote na fila de [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (por exemplo, devido à falta de espaço livre). Com essa opção ativada, os dados são perdidos para evitar interrupções na execução geral do cenário. Isso é útil para cenários em que a prioridade mais alta é execução contínua e os dados incorretos recebidos não são tão importantes.

Além disso, ao executar um cenário, um módulo pode às vezes encontrar um arquivo maior do que o tamanho máximo permitido. Nesse caso, [!DNL Workfront Fusion] receitas, em conformidade com a definição da [!UICONTROL Ativar perda de dados] e uma mensagem de aviso é exibida.

Para obter mais informações sobre o tamanho máximo do arquivo, consulte [Sobre o mapeamento de arquivos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Para obter mais informações sobre avisos, consulte [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Confirmação automática]

O [!UICONTROL Confirmação automática] se aplica a transações e define como processar um cenário. Se a opção Confirmação automática estiver ativada, a fase de confirmação em cada módulo será iniciada imediatamente após concluir a fase de operação. Com a opção Confirmação automática desabilitada, nenhuma confirmação ocorre até que as operações sejam executadas para todos os módulos (esse é o modo padrão).

Para obter mais informações sobre transações, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Número máximo de ciclos

Definir mais ciclos pode ser útil quando você deseja impedir a interrupção da conexão com um serviço de terceiros e garantir que todos os registros sejam processados dentro de uma única execução de cenário.

* Se o cenário começar com um acionador de pesquisa, a configuração definirá o número máximo de ciclos permitidos durante a execução do cenário.

   Para obter mais informações sobre acionadores de pesquisa, consulte [Acionadores de pesquisa](../../workfront-fusion/modules/module-types.md#polling) em [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Se o cenário começa com um acionador instantâneo, a configuração é ignorada e todos os eventos pendentes são processados durante uma única execução de cenário, um evento por ciclo.

   Para obter mais informações sobre acionadores instantâneos, consulte [Acionadores instantâneos](../../workfront-fusion/modules/module-types.md#instant) em [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Se o cenário não começar com um acionador (instantâneo/polling), o número máximo especificado de ciclos é sempre executado.

>[!INFO]
>
>**Exemplos:**  [!DNL Workfront] > [!UICONTROL Registro de monitoramento] O busca por novos problemas que chegam e [!DNL Workfront] >[!UICONTROL Converter objeto] converte a nova solicitação em um projeto e a atribui ao modelo apropriado.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL mais ciclos] é aplicada somente quando você agenda a execução do cenário. Quando você usar a variável [!UICONTROL Executar uma vez] , configurações de ciclo são consideradas.
>
>### O número máximo de ciclos é definido como 1 (padrão)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>O [!UICONTROL Número máximo de arquivos retornados] no [!UICONTROL Dropbox] >[!UICONTROL Assistir arquivos] está configurado como `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Se forem enviadas 100 solicitações ao [!DNL Workfront]e o [!UICONTROL Limite] estiver definido como 10, então 90 arquivos não serão processados após uma execução de cenário. Os próximos 10 arquivos são processados na próxima execução de cenário agendado.
>
>### O número máximo de ciclos é definido como 10
>
>O [!UICONTROL Número máximo de arquivos retornados] no [!UICONTROL Dropbox] >[!UICONTROL Assistir arquivos] está configurado como `10`.
>
>Se 100 arquivos forem adicionados à pasta Dropbox e a [!UICONTROL Número máximo de arquivos retornados] está definida como 10, depois 10 arquivos são processados durante o primeiro ciclo, os 10 arquivos seguintes no segundo ciclo, os 10 arquivos seguintes no terceiro ciclo e assim por diante, até que todos os arquivos sejam processados.
>
>Todos os arquivos são processados em 1 execução de cenário.
>
>Você pode ver os ciclos já executados nos detalhes do Cenário:
>
>![](assets/scenario-detail-350x207.png)
>
>Para obter mais informações sobre esta página, consulte [Detalhes do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Número de erros consecutivos

Define o número máximo de tentativas de execução consecutivas antes da desativação da execução de um cenário (excluindo [!UICONTROL DataError], [!UICONTROL DuplicateDataError] e [!UICONTROL ConnectionError]).

Para obter mais informações sobre erros, consulte [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Se um cenário começar com um acionador instantâneo, a configuração será ignorada e o cenário será desativado imediatamente após o primeiro erro ter ocorrido.
