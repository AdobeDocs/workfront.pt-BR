---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: O painel de configurações de cenário no Adobe Workfront Fusion
description: Este artigo descreve as configurações disponíveis no painel [!UICONTROL configurações de cenário] em seus [!DNL Adobe Workfront Fusion] cenários.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: b9914daa1e176d115226019d6ddf02b0953bc4d6
workflow-type: tm+mt
source-wordcount: '1206'
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
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Abrir as configurações do cenário

1. Abra o editor de cenários, conforme explicado em [O editor de cenários em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Clique no ícone de engrenagem próximo ao canto inferior esquerdo da página.

   ![](assets/scenario-settings-350x221.png)

   No painel [!UICONTROL Configurações de cenário] que é exibido, você pode definir várias configurações avançadas para o cenário.

## [!UICONTROL Permitir o armazenamento de execuções incompletas]

Esta opção determina como [!DNL Adobe Workfront Fusion] procede se ocorrer um erro durante a execução de um cenário. Com esta opção habilitada, o cenário é pausado e movido para [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Isso oferece a possibilidade de corrigir o problema e continuar a execução de onde o cenário foi interrompido. Se essa opção estiver desativada, a execução do cenário será interrompida e uma fase de reversão será iniciada.

## [!UICONTROL Processamento sequencial]

Essa opção força todas as execuções a ocorrerem em ordem e é relevante principalmente para Webhooks e Execuções incompletas.

Quando o processamento sequencial está ativado, as execuções paralelas do cenário são desativadas.

### Webhooks instantâneos

Se um acionador de webhook estiver configurado como `instant` e o &quot;Processamento sequencial&quot; estiver habilitado, todas as cargas de webhook instantâneas serão enfileiradas e processadas na ordem em que chegarem. Isso pode ser útil ao processar eventos de sistemas externos em uma ordem exata.

>[!NOTE]
>
>Haverá atrasos de processamento automático, pois cada carga será processada antes que a próxima seja iniciada.

### Execuções Incompletas

Se &quot;Execuções Incompletas&quot; também estiver ativado, se ocorrer um erro durante a execução de um cenário, ele será pausado. Uma das situações a seguir ocorre:

* Se a opção de processamento Sequencial estiver **habilitada**, o Workfront Fusion interromperá o processamento da sequência pré-existente até que todas as execuções incompletas sejam resolvidas.
* Se a opção de processamento Sequencial estiver **desabilitada**, o cenário continuará a ser executado de acordo com seu cronograma, acompanhado por tentativas repetidas de executar novamente as execuções incompletas.

Para obter mais informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

<!--

This option determines how [!DNL Workfront Fusion] proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the [!UICONTROL Sequential processing] option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the [!UICONTROL Sequential processing] option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.-->

>[!NOTE]
>
>O processamento sequencial pode causar um atraso na execução de um cenário. Se ainda houver execuções incompletas na fila quando um cenário instantâneo for acionado ou um cenário programado for definido para execução, esse cenário será executado após a conclusão de todas as execuções antes de ser concluído na fila.
>
>Se o caso de uso para seus cenários não exigir processamento sequencial, recomendamos desativar a opção de processamento sequencial.

Para obter mais informações sobre agendamento, consulte [Agendar um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Os dados são confidenciais

Depois que um cenário é executado, você pode exibir informações padrão sobre quais dados foram processados pelos módulos no cenário. Se você não quiser que essas informações sejam armazenadas, habilite a opção [!UICONTROL Os dados são confidenciais].

Para obter mais informações sobre a exibição de informações, consulte [Fluxo de execução de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Se você habilitar essa opção, poderá ser difícil resolver erros que possam ocorrer durante a execução de um cenário.

## Ativar perda de dados

Esta opção tem a ver com a habilitação da perda de dados se [!DNL Workfront Fusion] falhar ao salvar um pacote na fila de [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (por exemplo, devido à falta de espaço livre). Com essa opção ativada, os dados são perdidos para evitar interrupções na execução geral do cenário. Isso é útil para cenários em que a prioridade mais alta é a execução contínua e os dados incorretos recebidos não são tão importantes.

Além disso, ao executar um cenário, um módulo pode às vezes encontrar um arquivo maior do que o tamanho máximo permitido. Nesse caso, [!DNL Workfront Fusion] continua de acordo com a configuração da opção [!UICONTROL Habilitar perda de dados], e uma mensagem de aviso é exibida.

Para obter mais informações sobre o tamanho máximo de arquivo, consulte [Sobre o mapeamento de arquivos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Para obter mais informações sobre avisos, consulte [Processamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Confirmação automática]

As configurações de [!UICONTROL Confirmação automática] se aplicam a transações e definem a maneira de processar um cenário. Se a opção Confirmar automaticamente estiver ativada, a fase de confirmação em cada módulo será iniciada imediatamente após a conclusão da fase de operação. Com a opção Confirmar automaticamente desativada, nenhuma confirmação ocorre até que as operações sejam executadas para todos os módulos (esse é o modo padrão).

Para obter mais informações sobre transações, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Número máximo de ciclos

Definir mais ciclos pode ser útil quando você deseja impedir a interrupção da conexão com um serviço de terceiros e garantir que todos os registros sejam processados dentro de uma execução de cenário.

* Se o cenário começar com um acionador de sondagem, a configuração definirá o número máximo de ciclos permitidos durante a execução do cenário.

  Para obter mais informações sobre gatilhos de sondagem, consulte [Gatilhos de sondagem](../../workfront-fusion/modules/module-types.md#polling) em [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Se o cenário começar com um acionador instantâneo, a configuração será ignorada e todos os eventos pendentes serão processados durante uma única execução de cenário, um evento por ciclo.

  Para obter mais informações sobre acionadores instantâneos, consulte [Acionadores instantâneos](../../workfront-fusion/modules/module-types.md#instant) em [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Se o cenário não iniciar com um acionador (instantâneo/polling), o número máximo de ciclos especificado será sempre executado.

>[!INFO]
>
>**Exemplos:** [!DNL Workfront] > [!UICONTROL Observar registro] verifica novos problemas que entram, e [!DNL Workfront] >[!UICONTROL Converter objeto] converte a nova solicitação em um projeto e atribui a ela o modelo apropriado.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>Uma configuração de [!UICONTROL mais ciclos] é aplicada somente quando você agenda a execução do cenário. Ao usar o botão [!UICONTROL Executar uma vez], as configurações de ciclo são consideradas.
>
>### O número máximo de ciclos é definido como 1 (padrão)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>O [!UICONTROL número máximo de arquivos retornados] no módulo [!UICONTROL Workfront] >[!UICONTROL Watch records] está definido como `10`.
>Se 100 solicitações forem enviadas para [!DNL Workfront], e o campo [!UICONTROL Limite] estiver definido como 10, 90 arquivos serão deixados sem processamento após a execução de um cenário. Os próximos 10 arquivos são processados na próxima execução de cenário agendada.
>
>### O número máximo de ciclos é definido como 10
>
>O [!UICONTROL número máximo de arquivos retornados] no módulo [!UICONTROL Dropbox] >[!UICONTROL Observar arquivos] está definido como `10`.
>
>Se 100 arquivos forem adicionados à pasta Dropbox e a opção [!UICONTROL Número máximo de arquivos retornados] for definida como 10, 10 arquivos serão processados durante o primeiro ciclo, os próximos 10 arquivos no segundo ciclo, os próximos 10 arquivos no terceiro ciclo e assim por diante, até que todos os arquivos sejam processados.
>
>Todos os arquivos são processados em 1 execução de cenário.
>
>Você pode ver os ciclos já executados nos detalhes do Cenário:
>
>![](assets/scenario-detail-350x207.png)
>
>Para obter mais informações sobre esta página, consulte [Detalhes do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Número de erros consecutivos

Define o número máximo de tentativas consecutivas de execução antes de um cenário ser desativado (excluindo [!UICONTROL DataError], [!UICONTROL DuplicateDataError] e [!UICONTROL ConnectionError]).

Para obter mais informações sobre erros, consulte [Processamento de erros [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Se um cenário inicia com um acionador instantâneo, a configuração é ignorada e o cenário é desativado imediatamente após a ocorrência do primeiro erro.
