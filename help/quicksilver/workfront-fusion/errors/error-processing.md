---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Processamento de erros no [!DNL Adobe Workfront Fusion]
description: Às vezes, um erro pode ocorrer durante a execução de um cenário. Isso geralmente acontece se um serviço não estiver disponível devido a uma falha na conexão a um serviço ou se uma validação falhar. Este artigo discute os erros comuns que você pode encontrar.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 184033c8957e955b3011f7e0845a73029f6b7aba
workflow-type: tm+mt
source-wordcount: '1194'
ht-degree: 0%

---

# Processamento de erros no [!DNL Adobe Workfront Fusion]

Às vezes, um erro pode ocorrer durante a execução de um cenário. Isso geralmente acontece se um serviço não estiver disponível devido a uma falha na conexão a um serviço ou se uma validação falhar. Este artigo discute os erros comuns que você pode encontrar.

[!DNL Adobe Workfront Fusion] faz a distinção entre vários tipos básicos de erros. Ele reagirá de forma diferente dependendo do tipo de erro que ocorreu.

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

## Erro de conexão

`ConnectionError`

O erro de conexão é um dos erros mais comuns normalmente causados pela indisponibilidade do serviço de terceiros por vários motivos (sobrecarga, manutenção, interrupção e assim por diante). O tratamento padrão deste erro depende de qual módulo foi encontrado:

* Se o erro ocorrer no primeiro módulo, a execução do cenário será finalizada com uma mensagem de aviso. [!DNL Workfront Fusion] em seguida, tenta repetidamente executar o cenário novamente em intervalos de tempo crescentes (esses são explicados abaixo). Se todas as tentativas falharem, [!DNL Workfront Fusion] desativa o cenário.
* Se o erro de conexão ocorrer em outro módulo que não o primeiro, as etapas subsequentes dependerão do [Permitir o armazenamento de execuções incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) nas configurações avançadas do cenário:

   * Se essa opção estiver habilitada, a execução do cenário será movida para a função [!UICONTROL Execuções incompletas] pasta onde [!DNL Workfront Fusion] O tenta executar o cenário novamente em intervalos de tempo crescentes. Se todas as tentativas falharem, a execução permanecerá na pasta Incomplete executions , aguardando a resolução manual do usuário.

      Para obter mais informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Se essa opção estiver desativada, a execução do cenário terminará com um erro seguido de uma fase de reversão. [!DNL Workfront Fusion] em seguida, tenta executar o cenário novamente em intervalos de tempo crescentes. Se todas as tentativas falharem, [!DNL Workfront Fusion] desativa o cenário.

### Aumento dos intervalos de tempo

O algoritmo de intervalos de tempo de aumento multiplicativo entre tentativas quando ocorre um erro é conhecido como backoff exponencial. Os intervalos de tempo crescentes são definidos da seguinte maneira:

1. 10 minutos
1. 1 hora
1. 3 horas
1. 12 horas
1. 24 horas

A principal razão para empregar intervalos de tempo crescentes em [!DNL Workfront Fusion] O é impedir que cenários executados com frequência consumam operações em tentativas repetidamente falhadas.

>[!INFO]
>
>**Exemplo:**
>
>Um cenário contém a variável [!DNL Google Sheets] acionador [!UICONTROL Linhas de observação]. [!DNL Google Sheets] está indisponível por 30 minutos devido à manutenção quando [!DNL Workfront Fusion] inicia o cenário, portanto, não é possível recuperar novas linhas. O cenário é interrompido e tenta novamente em 10 minutos. Porque [!DNL Google Sheets] ainda não está disponível, [!DNL Workfront Fusion] O ainda não consegue obter informações sobre novas linhas. A próxima execução do cenário é agendada em 1 hora. [!DNL Google Sheets] O está disponível novamente neste momento e o cenário é executado com êxito.

## Erro de dados

`DataError`

Um erro de dados é gerado quando um item é mapeado incorretamente e não passa a validação executada no [!DNL Workfront Fusion] do lado ou do lado do serviço de terceiros que está sendo usado.

Se esse erro ocorrer, o cenário, até onde o módulo falhou, será movido para a pasta de execuções incompletas, onde você poderá solucionar o problema. No entanto, o cenário não pára e continua sendo executado de acordo com seu cronograma. Para interromper a execução do cenário quando o erro de Dados for exibido, ative a opção Processamento sequencial no painel Configurações do cenário.

Se você não tiver ativado a variável [!UICONTROL Permitir o armazenamento de execuções incompletas] nas configurações do cenário, a execução do cenário terminará com o erro e uma reversão será executada.

Para obter mais informações sobre mapeamento, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obter informações sobre o painel de configuração de cenário, consulte [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obter informações sobre programações, consulte [Programar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Erro de Dados Duplicados

`DuplicateDataError`

If [!DNL Workfront Fusion] O tenta inserir o mesmo pacote duas vezes em um serviço que não permite dados duplicados, um erro de dados duplicado é gerado. Se esse erro ocorrer, [!DNL Workfront Fusion] O continua da mesma forma que para o erro de dados.

## Erro de Token de Acesso Inválido

`InvalidAccessTokenError`

Ocorre um erro de token de acesso inválido quando [!DNL Workfront Fusion] O não pode acessar sua conta registrada com um serviço de terceiros. Isso geralmente acontece quando você revoga direitos de acesso para [!DNL Workfront Fusion] na administração de um determinado serviço, mas os cenários relacionados continuam sendo executados de acordo com o cronograma.

Se esse erro ocorrer, a execução de um cenário será interrompida imediatamente. O restante do cenário que começa no módulo em que o erro ocorreu é movido para a pasta de execuções incompletas.

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Erro de limite de taxa

`RateLimitError`

Se um limite definido por um determinado serviço for excedido, um erro de limite de taxa será gerado. Se esse erro ocorrer, [!DNL Workfront Fusion] O continua da mesma forma que para o Erro de conexão.

Para obter mais informações, consulte [Erro de conexão](#connection-error).

## Erro de dados incompletos

`IncompleteDataError`

Um erro de dados incompleto ocorre somente com acionadores. Esse erro é gerado se um acionador não conseguir baixar os dados necessários de um determinado serviço.

Se um cenário terminar com a variável `IncompleteDataError`, o seu comportamento dependerá da sua definição de [!UICONTROL Número máximo de erros consecutivos].

Para obter mais informações, consulte [Número de erros consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) no artigo [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Exemplo:**
>
>Um cenário tem a variável [!DNL Workfront] acionador [!UICONTROL Registro de monitoramento] defina como monitorar documentos. O cenário é executado enquanto você está carregando um documento grande, como um vídeo longo. Porque [!UICONTROL Workfront Fusion] O tenta baixar o vídeo enquanto ele ainda está carregando no Workfront, o cenário termina com a variável `IncompleteDataError`.

## Erro de tempo de execução

`RuntimeError`

Se qualquer outro erro (não mencionado acima) for exibido durante a execução do cenário, ele será relatado como um `RunTimeError`.

Se um cenário terminar com a variável `RuntimeError`, o seu comportamento dependerá da sua definição de [!UICONTROL Número máximo de erros consecutivos]. Para obter mais informações, consulte [Número de erros consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) no artigo [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Se um cenário começar com um acionador instantâneo, a configuração de [!UICONTROL Número máximo de erros consecutivos] é ignorado e o cenário é desativado imediatamente após a ocorrência do primeiro erro. Para obter mais informações, consulte [Acionadores instantâneos](../../workfront-fusion/modules/module-types.md#instant) no artigo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Erro de inconsistência

`InconsistencyError`

Se qualquer erro descrito acima ocorrer durante a fase de confirmação ou reversão, um cenário terminará com Erro de Inconsistência. Para obter mais informações, consulte [Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se esse erro aparecer em um cenário, a execução do cenário será interrompida imediatamente.

## Advertência

Ao executar um cenário, você pode receber um aviso informando sobre um problema. No entanto, isso não impede que o cenário seja concluído com êxito.

Por exemplo, um aviso pode aparecer quando o tamanho máximo permitido do arquivo for excedido e a variável [!UICONTROL Ativar perda de dados] está desativada. Para obter mais informações, consulte [Ativar perda de dados](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) no artigo [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
