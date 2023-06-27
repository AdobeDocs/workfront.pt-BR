---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Processamento de erros no [!DNL Adobe Workfront Fusion]
description: Às vezes, um erro pode ocorrer durante a execução de um cenário. Isso geralmente acontece se um serviço estiver indisponível devido a uma falha na conexão com um serviço ou se uma validação falhar. Este artigo discute os erros comuns que você pode encontrar.
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 0%

---

# Processamento de erros no [!DNL Adobe Workfront Fusion]

Às vezes, um erro pode ocorrer durante a execução de um cenário. Isso geralmente acontece se um serviço estiver indisponível devido a uma falha na conexão com um serviço ou se uma validação falhar. Este artigo discute os erros comuns que você pode encontrar.

[!DNL Adobe Workfront Fusion] O distingue entre vários tipos de erro básicos. Ele reagirá de forma diferente dependendo do tipo de erro que ocorreu.

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

## Erro de conexão

`ConnectionError`

O erro de conexão é um dos erros mais comuns geralmente causados pela indisponibilidade do serviço de terceiros por vários motivos (sobrecarga, manutenção, interrupção e assim por diante). O tratamento padrão desse erro depende de em qual módulo ele foi encontrado:

* Se o erro ocorrer no primeiro módulo, a execução do cenário será encerrada com uma mensagem de aviso. [!DNL Workfront Fusion] Em seguida, o tenta executar novamente o cenário em intervalos de tempo crescentes (eles são explicados abaixo). Se todas as tentativas falharem, [!DNL Workfront Fusion] desativa o cenário.
* Se o erro de conexão ocorrer em outro módulo que não o primeiro, as etapas subsequentes dependerão do [Permitir o armazenamento de execuções incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) nas configurações avançadas do cenário:

   * Se essa opção estiver habilitada, a execução do cenário será movida para a variável [!UICONTROL Execuções incompletas] pasta onde [!DNL Workfront Fusion] O tenta executar novamente o cenário em intervalos de tempo crescentes. Se todas as tentativas falharem, a execução permanecerá na pasta Incomplete executions aguardando resolução manual pelo usuário.

     Para obter mais informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).
   * Se essa opção estiver desativada, a execução do cenário terminará com um erro seguido de uma fase de reversão. [!DNL Workfront Fusion] em seguida, o tenta executar novamente o cenário em intervalos de tempo crescentes. Se todas as tentativas falharem, [!DNL Workfront Fusion] desativa o cenário.

### Aumento dos intervalos de tempo

O algoritmo de aumento multiplicativo dos intervalos de tempo entre tentativas quando ocorre um erro é conhecido como retrocesso exponencial. Os intervalos de tempo crescentes são definidos da seguinte maneira:

1. 10 minutos
1. 1 hora
1. 3 horas
1. 12 horas
1. 24 horas

A principal razão para utilizar os intervalos de tempo crescentes em [!DNL Workfront Fusion] é evitar que cenários executados com frequência consumam operações em tentativas com falha repetida.

>[!INFO]
>
>**Exemplo:**
>
>Um cenário contém o parâmetro [!DNL Google Sheets] acionador [!UICONTROL Observar linhas]. [!DNL Google Sheets] fica indisponível por 30 minutos devido a manutenção quando [!DNL Workfront Fusion] O inicia o cenário, portanto, não é possível recuperar novas linhas. O cenário é interrompido e tenta novamente em 10 minutos. Porque [!DNL Google Sheets] ainda não está disponível, [!DNL Workfront Fusion] O ainda não consegue obter informações sobre novas linhas. A próxima execução do cenário é agendada em 1 hora. [!DNL Google Sheets] O estará disponível novamente nesse momento e o cenário será executado com sucesso.

## Erro de dados

`DataError`

Um erro de dados é gerado quando um item é mapeado incorretamente e não passa na validação executada no [!DNL Workfront Fusion] ou do serviço de terceiros em uso.

Se esse erro ocorrer, o cenário, até o qual o módulo falhou, será movido para a pasta de execuções incompletas, onde você poderá solucionar o problema. No entanto, o cenário não pára e continua a ser executado de acordo com seu cronograma. Para interromper a execução do cenário quando Erro de dados for exibido, ative a opção Processamento sequencial no painel Configurações do cenário.

Se você não tiver ativado a variável [!UICONTROL Permitir o armazenamento de execuções incompletas] nas configurações do cenário, a execução do cenário é finalizada com o erro e uma reversão é executada.

Para obter mais informações sobre mapeamento, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

Para obter informações sobre o painel de configuração de cenário, consulte [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obter informações sobre programações, consulte [Programar um cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## Erro de dados duplicados

`DuplicateDataError`

Se [!DNL Workfront Fusion] O tenta inserir o mesmo pacote duas vezes em um serviço que não permite dados duplicados. Um erro de dados duplicados é gerado. Se este erro ocorrer, [!DNL Workfront Fusion] O continua da mesma forma que para o erro de dados.

## Erro de token de acesso inválido

`InvalidAccessTokenError`

Ocorre um erro de token de acesso inválido quando [!DNL Workfront Fusion] O não pode acessar sua conta registrada com um serviço de terceiros. Isso geralmente acontece quando você revoga direitos de acesso para [!DNL Workfront Fusion] na administração de um determinado serviço, mas os cenários relacionados continuam sendo executados de acordo com o agendamento.

Se esse erro ocorrer, a execução de um cenário será interrompida imediatamente. O restante do cenário que começa no módulo em que o erro ocorreu é movido para a pasta de execuções incompletas.

Para obter informações sobre execuções incompletas, consulte [Exibir e resolver execuções incompletas no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## Erro de limite de taxa

`RateLimitError`

Se um limite definido por um determinado serviço for excedido, um erro de limite de taxa será gerado. Se esse erro ocorrer, [!DNL Workfront Fusion] O continua da mesma forma que para o Erro de conexão.

Para obter mais informações, consulte [Erro de conexão](#connection-error).

## Erro de dados incompletos

`IncompleteDataError`

Um erro de dados incompleto ocorre somente com acionadores. Esse erro é gerado se um acionador falha ao baixar os dados necessários de um determinado serviço.

Se um cenário terminar com a variável `IncompleteDataError`, seu comportamento dependerá de sua configuração de [!UICONTROL Número máximo de erros consecutivos].

Para obter mais informações, consulte [Número de erros consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) no artigo [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**Exemplo:**
>
>Um cenário tem o [!DNL Workfront] acionador [!UICONTROL Assistir ao registro] defina para procurar documentos. O cenário é executado enquanto você faz upload de um documento grande, como um vídeo longo. Porque [!UICONTROL Workfront Fusion] O tenta baixar o vídeo enquanto ele ainda está carregando no Workfront, o cenário termina com `IncompleteDataError`.

## Erro de tempo de execução

`RuntimeError`

Se qualquer outro erro (não mencionado acima) for exibido durante a execução do cenário, ele será relatado como um `RunTimeError`.

Se um cenário terminar com a variável `RuntimeError`, seu comportamento dependerá de sua configuração de [!UICONTROL Número máximo de erros consecutivos]. Para obter mais informações, consulte [Número de erros consecutivos](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) no artigo [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>Se um cenário começar com um acionador instantâneo, a configuração de [!UICONTROL Número máximo de erros consecutivos] é ignorado e o cenário é desativado imediatamente após a ocorrência do primeiro erro. Para obter mais informações, consulte [Acionadores instantâneos](../../workfront-fusion/modules/module-types.md#instant) no artigo [Tipos de módulos](../../workfront-fusion/modules/module-types.md).

## Erro de inconsistência

`InconsistencyError`

Se algum erro descrito acima ocorrer durante a fase de confirmação ou reversão, um cenário será encerrado com Erro de inconsistência. Para obter mais informações, consulte [Execução de cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

Se esse erro aparecer em um cenário, a execução do cenário será imediatamente interrompida.

## Advertência

Ao executar um cenário, você pode receber um aviso informando sobre um problema. No entanto, isso não impede que o cenário seja concluído com êxito.

Por exemplo, um aviso pode ser exibido quando o tamanho máximo de arquivo permitido for excedido e a variável [!UICONTROL Ativar perda de dados] está desabilitada. Para obter mais informações, consulte [Ativar perda de dados](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) no artigo [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).
