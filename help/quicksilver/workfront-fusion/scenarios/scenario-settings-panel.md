---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: O painel de configurações de cenário no Adobe Workfront Fusion
description: Este artigo descreve as configurações disponíveis na [!UICONTROL configurações de cenário] no seu [!DNL Adobe Workfront Fusion] cenários.
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 0%

---

# O painel de configurações do cenário no [!DNL Adobe Workfront Fusion]

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

## Abrir as configurações do cenário

1. Abra o editor de cenários, conforme explicado em [O editor de cenários no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md).
1. Clique no ícone de engrenagem próximo ao canto inferior esquerdo da página.

   ![](assets/scenario-settings-350x221.png)

   No [!UICONTROL Configurações de cenário] que é exibido, é possível definir várias configurações avançadas para o cenário.

## [!UICONTROL Permitir o armazenamento de execuções incompletas]

Essa opção determina como [!DNL Adobe Workfront Fusion] continua se ocorrer um erro durante a execução de um cenário. Com essa opção ativada, o cenário é pausado e movido para [Exibir e resolver execuções incompletas no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Isso oferece a possibilidade de corrigir o problema e continuar a execução de onde o cenário foi interrompido. Se essa opção estiver desativada, a execução do cenário será interrompida e uma fase de reversão será iniciada.

## [!UICONTROL Processamento sequencial]

Essa opção determina como [!DNL Workfront Fusion] continua se ocorrer um erro e a execução de um cenário for movida para a variável [Exibir e resolver execuções incompletas no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). Se a variável [!UICONTROL Processamento sequencial] estiver ativada, o Workfront Fusion interromperá o processamento completo da sequência de tarefas até que todas as execuções incompletas sejam resolvidas. Se a variável [!UICONTROL Processamento sequencial] estiver desativada, o cenário continuará a ser executado de acordo com seu agendamento, acompanhado por tentativas repetidas de executar novamente as execuções incompletas.

Para obter mais informações sobre programação, consulte [Agendar um cenário no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Os dados são confidenciais

Depois que um cenário é executado, você pode exibir informações padrão sobre quais dados foram processados pelos módulos no cenário. Se não quiser que essas informações sejam armazenadas, habilite a opção [!UICONTROL Os dados são confidenciais] opção.

Para obter mais informações sobre a exibição de informações, consulte [Fluxo de execução de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

>[!IMPORTANT]
>
>Se você habilitar essa opção, poderá ser difícil resolver erros que possam ocorrer durante a execução de um cenário.

## Ativar perda de dados

Essa opção tem a ver com ativar a perda de dados se [!DNL Workfront Fusion] falha ao salvar um pacote na fila de [Exibir e resolver execuções incompletas no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) (por exemplo, devido à falta de espaço livre). Com essa opção ativada, os dados são perdidos para evitar interrupções na execução geral do cenário. Isso é útil para cenários em que a prioridade mais alta é a execução contínua e os dados incorretos recebidos não são tão importantes.

Além disso, ao executar um cenário, um módulo pode às vezes encontrar um arquivo maior do que o tamanho máximo permitido. Nesse caso, [!DNL Workfront Fusion] procede em conformidade com a fixação do montante [!UICONTROL Ativar perda de dados] e uma mensagem de aviso será exibida.

Para obter mais informações sobre o tamanho máximo do arquivo, consulte [Sobre o mapeamento de arquivos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

Para obter mais informações sobre avisos, consulte [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

## [!UICONTROL Confirmar automaticamente]

A variável [!UICONTROL Confirmar automaticamente] se aplica a transações e define a maneira de processar um cenário. Se a opção Confirmar automaticamente estiver ativada, a fase de confirmação em cada módulo será iniciada imediatamente após a conclusão da fase de operação. Com a opção Confirmar automaticamente desativada, nenhuma confirmação ocorre até que as operações sejam executadas para todos os módulos (esse é o modo padrão).

Para obter mais informações sobre transações, consulte [Execução de cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Número máximo de ciclos

Definir mais ciclos pode ser útil quando você deseja impedir a interrupção da conexão com um serviço de terceiros e garantir que todos os registros sejam processados dentro de uma execução de cenário.

* Se o cenário começar com um acionador de sondagem, a configuração definirá o número máximo de ciclos permitidos durante a execução do cenário.

  Para obter mais informações sobre acionadores de pesquisa, consulte [Acionadores de sondagem](../../workfront-fusion/modules/module-types.md#polling) in [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Se o cenário começar com um acionador instantâneo, a configuração será ignorada e todos os eventos pendentes serão processados durante uma única execução de cenário, um evento por ciclo.

  Para obter mais informações sobre acionadores instantâneos, consulte [Acionadores instantâneos](../../workfront-fusion/modules/module-types.md#instant) in [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

* Se o cenário não iniciar com um acionador (instantâneo/polling), o número máximo de ciclos especificado será sempre executado.

>[!INFO]
>
>**Exemplos:**  [!DNL Workfront] > [!UICONTROL Assistir ao registro] observa novos problemas que aparecem e [!DNL Workfront] >[!UICONTROL Converter objeto] converte a nova solicitação em um projeto e a atribui ao modelo apropriado.
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>A [!UICONTROL mais ciclos] A configuração é aplicada somente quando você agenda a execução do cenário. Quando você usa o [!UICONTROL Executar uma vez] são consideradas as configurações de ciclo.
>
>### O número máximo de ciclos é definido como 1 (padrão)
>
>![](assets/max-number-cycles-1-350x201.png)
>
>A variável [!UICONTROL Número máximo de arquivos retornados] no [!UICONTROL Dropbox] >[!UICONTROL Observar arquivos] o módulo está definido como `10`.
>
>![](assets/max-number-cycles-10-350x175.png)
>
>Se 100 solicitações forem enviadas para o [!DNL Workfront], e o [!UICONTROL Limite] for definido como 10 e, em seguida, 90 arquivos serão deixados sem processamento após a execução de um cenário. Os próximos 10 arquivos são processados na próxima execução de cenário agendada.
>
>### O número máximo de ciclos é definido como 10
>
>A variável [!UICONTROL Número máximo de arquivos retornados] no [!UICONTROL Dropbox] >[!UICONTROL Observar arquivos] o módulo está definido como `10`.
>
>Se 100 arquivos forem adicionados à pasta Dropbox e a variável [!UICONTROL Número máximo de arquivos retornados] for definida como 10, então 10 arquivos serão processados durante o primeiro ciclo, os próximos 10 arquivos no segundo ciclo, os próximos 10 arquivos no terceiro ciclo e assim por diante, até que todos os arquivos sejam processados.
>
>Todos os arquivos são processados em 1 execução de cenário.
>
>Você pode ver os ciclos já executados nos detalhes do Cenário:
>
>![](assets/scenario-detail-350x207.png)
>
>Para obter mais informações sobre essa página, consulte [Detalhes do cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md).

## Número de erros consecutivos

Define o número máximo de tentativas consecutivas de execução antes da desativação da execução de um cenário (excluindo [!UICONTROL DataError], [!UICONTROL DuplicateDataError] e [!UICONTROL ConnectionError]).

Para obter mais informações sobre erros, consulte [Processamento de erros no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md).

>[!NOTE]
>
>Se um cenário inicia com um acionador instantâneo, a configuração é ignorada e o cenário é desativado imediatamente após a ocorrência do primeiro erro.
