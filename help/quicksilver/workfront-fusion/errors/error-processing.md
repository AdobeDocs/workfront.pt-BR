---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Erro ao processar em  [!DNL Adobe Workfront Fusion]
description: Às vezes, um erro pode ocorrer durante a execução de um cenário. Isso geralmente acontece se um serviço estiver indisponível devido a uma falha na conexão com um serviço ou se uma validação falhar. Este artigo discute os erros comuns que você pode encontrar.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1246'
ht-degree: 1%

---

# Erro ao processar em [!DNL Adobe Workfront Fusion]

Às vezes, um erro pode ocorrer durante a execução de um cenário. Isso geralmente acontece se um serviço estiver indisponível devido a uma falha na conexão com um serviço ou se uma validação falhar. Este artigo discute os erros comuns que você pode encontrar.

[!DNL Adobe Workfront Fusion] distingue entre vários tipos de erro básicos. Ele reagirá de forma diferente dependendo do tipo de erro que ocorreu.

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
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Erro de conexão

`ConnectionError`

O erro de conexão é um dos erros mais comuns geralmente causados pela indisponibilidade do serviço de terceiros por vários motivos (sobrecarga, manutenção, interrupção e assim por diante). O tratamento padrão desse erro depende de em qual módulo ele foi encontrado:

* Se o erro ocorrer no primeiro módulo, a execução do cenário será encerrada com uma mensagem de aviso. [!DNL Workfront Fusion] então tenta executar novamente o cenário em intervalos de tempo crescentes (os quais são explicados abaixo). Se todas as tentativas falharem, [!DNL Workfront Fusion] desativará o cenário.
* Se o erro de conexão ocorrer em outro módulo que não o primeiro, as etapas subsequentes dependerão da opção [Permitir o armazenamento de execuções incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) das configurações avançadas do cenário:

   * Se essa opção estiver habilitada, a execução do cenário será movida para a pasta [!UICONTROL Execuções incompletas], onde [!DNL Workfront Fusion] tenta executar novamente o cenário em intervalos de tempo crescentes. Se todas as tentativas falharem, a execução permanecerá na pasta Incomplete executions aguardando resolução manual pelo usuário.

     Para obter mais informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Se essa opção estiver desativada, a execução do cenário terminará com um erro seguido de uma fase de reversão. [!DNL Workfront Fusion] então tenta executar novamente o cenário em intervalos de tempo crescentes. Se todas as tentativas falharem, [!DNL Workfront Fusion] desativará o cenário.

### Aumento dos intervalos de tempo

O algoritmo de aumento multiplicativo dos intervalos de tempo entre tentativas quando ocorre um erro é conhecido como retrocesso exponencial. Os intervalos de tempo crescentes são definidos da seguinte maneira:

1. 10 minutos
1. 1 hora
1. 3 horas
1. 12 horas
1. 24 horas

O principal motivo para utilizar o aumento nos intervalos de tempo em [!DNL Workfront Fusion] é para evitar que cenários executados com frequência consumam operações em tentativas repetidamente com falha.

>[!INFO]
>
>**Exemplo:**
>
>Um cenário contém o [!DNL Google Sheets] gatilho [!UICONTROL Linhas de Observação]. [!DNL Google Sheets] fica indisponível por 30 minutos devido a uma manutenção quando [!DNL Workfront Fusion] inicia o cenário, portanto, não é possível recuperar novas linhas. O cenário é interrompido e tenta novamente em 10 minutos. Como [!DNL Google Sheets] ainda está indisponível, [!DNL Workfront Fusion] ainda não pode obter informações sobre novas linhas. A próxima execução do cenário é agendada em 1 hora. [!DNL Google Sheets] está disponível novamente neste momento e o cenário foi executado com êxito.

## Erro de dados

`DataError`

Um erro de dados é gerado quando um item é mapeado incorretamente e não passa na validação executada no lado [!DNL Workfront Fusion] ou no lado do serviço de terceiros em uso.

Se esse erro ocorrer, o cenário, até o qual o módulo falhou, será movido para a pasta de execuções incompletas, onde você poderá solucionar o problema. No entanto, o cenário não pára e continua a ser executado de acordo com seu cronograma. Para interromper a execução do cenário quando Erro de dados for exibido, ative a opção Processamento sequencial no painel Configurações do cenário.

Se você não tiver habilitado a opção [!UICONTROL Permitir o armazenamento de execuções incompletas] nas configurações do cenário, a execução do cenário será encerrada com o erro e uma reversão será executada.

Para obter mais informações sobre mapeamento, consulte [Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obter informações sobre o painel de configuração de cenário, consulte [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obter informações sobre agendamentos, consulte [Agendar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Erro de dados duplicados

`DuplicateDataError`

Se [!DNL Workfront Fusion] tentar inserir o mesmo pacote duas vezes em um serviço que não permite dados duplicados, um erro de dados duplicados será gerado. Se este erro ocorrer, [!DNL Workfront Fusion] continuará da mesma forma que para o erro de dados.

## Erro de token de acesso inválido

`InvalidAccessTokenError`

Ocorre um erro de token de acesso inválido quando o [!DNL Workfront Fusion] não pode acessar sua conta registrada com um serviço de terceiros. Isso geralmente acontece quando você revoga direitos de acesso para [!DNL Workfront Fusion] na administração de um determinado serviço, mas os cenários relacionados continuam sendo executados de acordo com o agendamento.

Se esse erro ocorrer, a execução de um cenário será interrompida imediatamente. O restante do cenário que começa no módulo em que o erro ocorreu é movido para a pasta de execuções incompletas.

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Erro de limite de taxa

`RateLimitError`

Se um limite definido por um determinado serviço for excedido, um erro de limite de taxa será gerado. Se este erro ocorrer, [!DNL Workfront Fusion] continuará da mesma forma que para o Erro de Conexão.

Para obter mais informações, consulte [Erro de Conexão](#connection-error).

## Erro de dados incompletos

`IncompleteDataError`

Um erro de dados incompleto ocorre somente com acionadores. Esse erro é gerado se um acionador falha ao baixar os dados necessários de um determinado serviço.

Se um cenário terminar com `IncompleteDataError`, seu comportamento adicional dependerá da configuração de [!UICONTROL Número máximo de erros consecutivos].

Para obter mais informações, consulte [Número de erros consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) no artigo [Painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Exemplo:**
>
>Um cenário tem o [!DNL Workfront] gatilho [!UICONTROL Observar registro] definido para observar documentos. O cenário é executado enquanto você faz upload de um documento grande, como um vídeo longo. Como o [!UICONTROL Workfront Fusion] tenta baixar o vídeo enquanto ele ainda está carregando no Workfront, o cenário é encerrado com o `IncompleteDataError`.

## Erro de tempo de execução

`RuntimeError`

Se qualquer outro erro (não mencionado acima) aparecer durante a execução do cenário, ele será relatado como `RunTimeError`.

Se um cenário terminar com `RuntimeError`, seu comportamento adicional dependerá da configuração de [!UICONTROL Número máximo de erros consecutivos]. Para obter mais informações, consulte [Número de erros consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) no artigo [Painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Se um cenário inicia com um gatilho instantâneo, a configuração de [!UICONTROL Número máximo de erros consecutivos] é ignorada e o cenário é desativado imediatamente após a ocorrência do primeiro erro. Para obter mais informações, consulte [Acionadores instantâneos](../../workfront-fusion/modules/module-types.md#instant) no artigo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Erro de inconsistência

`InconsistencyError`

Se algum erro descrito acima ocorrer durante a fase de confirmação ou reversão, um cenário será encerrado com Erro de inconsistência. Para obter mais informações, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se esse erro aparecer em um cenário, a execução do cenário será imediatamente interrompida.

## Advertência

Ao executar um cenário, você pode receber um aviso informando sobre um problema. No entanto, isso não impede que o cenário seja concluído com êxito.

Por exemplo, um aviso pode aparecer quando o tamanho máximo de arquivo permitido for excedido e a opção [!UICONTROL Habilitar perda de dados] estiver desabilitada. Para obter mais informações, consulte [Habilitar perda de dados](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) no artigo [O painel de configurações do cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
