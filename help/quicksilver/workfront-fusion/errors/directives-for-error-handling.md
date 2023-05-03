---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]
description: Este artigo descreve diretivas que podem ser usadas para tratamento de erros em [!DNL Adobe Workfront Fusion] cenários.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: f4e43d34068c987755559573b4ecd618ff710686
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Diretivas relativas ao tratamento de erros [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Diretivas relativas ao tratamento de erros

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Reversão</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>A execução do cenário é interrompida imediatamente e uma <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Reversão</a> é iniciada em todos os módulos em uma tentativa de revertê-los para o estado inicial. Os módulos subsequentes não são processados.</p> <p>Com alguns tipos de erro, o cenário é desativado após o número de erros consecutivos especificados nas Configurações do cenário. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Número de erros consecutivos</a>.</p> <p>O status de execução do cenário é marcado como "erro".</p> <p>Observação: Esse é o comportamento padrão se nenhuma rota do manipulador de erros estiver conectada ao módulo e a variável <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Permitir o armazenamento de execuções incompletas]</a> configuração em [!UICONTROL Configurações de cenário] não está marcada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Confirmar</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>A execução do cenário é interrompida imediatamente e uma fase de confirmação é iniciada em todos os módulos. Os módulos subsequentes não são processados.</p> <p>Todos os pacotes não processados são ignorados.</p> <p>O status de execução do cenário é marcado como "sucesso". Para obter informações sobre as fases de consolidação, consulte <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Confirmar</a> no artigo <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Execução, ciclos e fases do cenário no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Retomar</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Uma saída substituta é especificada e fornecida ao módulo que encontra um erro.</p> <p>Os módulos subsequentes são processados.</p> <p>O status de execução do cenário é marcado como "sucesso".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorar</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>O erro é ignorado e os módulos subsequentes não são processados.</p> <p>Se houver pacotes não processados, a execução do cenário continuará normalmente.</p> <p>O status de execução do cenário é marcado como "sucesso".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Quebra</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>O estado da execução do cenário é armazenado na fila de execuções incompletas, onde o erro pode ser resolvido manualmente. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Exibir e resolver execuções incompletas no Adobe Workfront Fusion</a>. </p> <p>Existem, no entanto, algumas exceções. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Permitir o armazenamento de execuções incompletas</a> no artigo <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">O painel de configurações de cenário no Adobe Workfront Fusion</a>.</p> <p>Os módulos subsequentes não são processados.</p> <p>Se houver pacotes não processados, a execução do cenário continuará normalmente.</p> <p>O status de execução do cenário é marcado como "aviso" quando a opção [!UICONTROL Concluir execução automaticamente] está desativada.</p> <p>Consulte a <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> para obter mais informações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tente novamente</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>Em alguns casos, pode ser útil executar novamente um módulo com falha por algumas vezes, quando houver uma chance de que o motivo da falha possa passar ao longo do tempo.</p> <p>Atualmente, o Workfront Fusion não oferece a diretiva Retry , embora várias soluções alternativas possam ser empregadas para imitar sua funcionalidade. Para obter mais informações, consulte <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Tente novamente o tratamento de erros no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Atualmente, as diretivas de tratamento de erros não podem ser usadas fora de uma rota de tratamento de erros.
   >
   >   Para obter mais informações, consulte [Rota do manipulador de erros](../../workfront-fusion/errors/error-handling.md#error) no artigo [Tratamento de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] No momento, o não oferece um módulo Throw que permitiria gerar (lançar) erros condicionalmente facilmente, embora uma solução alternativa possa ser empregada para simular sua funcionalidade.
   >
   >   Para obter mais informações, consulte [Solução alternativa para lançamento](../../workfront-fusion/errors/throw.md#workaround-for-throw) no artigo [Tratamento de erros de jogador no Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).


## Quebra {#break}

Quando um erro é tratado pela variável [!DNL Break] , um registro é criado na pasta Incomplete executions . Esse registro armazena o estado da execução do cenário, juntamente com dados dos módulos anteriores. O registro faz referência ao módulo em que o erro se originou e contém informações sobre quais dados foram recebidos pelo módulo como entrada. Para cada pacote de dados que causa o erro, um registro separado é criado.

Para obter mais informações, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Resolver erros resultantes da diretiva Break

Você pode resolver o erro manualmente atualizando o cenário (se necessário) e executando-o uma vez.

Você também pode configurar o cenário para processar automaticamente uma execução incompleta executando o cenário novamente. Para configurar o módulo para processar execuções incompletas:

1. No módulo Break , ative o [!UICONTROL **Concluir execução automaticamente**] opção.
1. No **Número de tentativas** , insira ou mapeie o número máximo de tentativas que você deseja que o módulo repita a execução

   Esse número deve estar entre 1 e 100.
1. No **Intervalo entre tentativas** , insira ou mapeie o número de minutos entre cada tentativa.

Com essa opção ativada, quando ocorre um erro, a execução incompleta é recuperada (após o tempo especificado na variável [!UICONTROL Intervalo entre tentativas] e executadas com os dados de entrada originais. Isso será repetido até que a execução do módulo seja concluída sem um erro ou até que o Número de tentativas especificado seja atingido.

>[!NOTE]
>
>Se a tentativa inicial de repetição falhar, o intervalo entre tentativas aumentará exponencialmente a cada outra tentativa.


Quando a opção &quot;Execução automática concluída&quot; está ativada, a execução do cenário é marcada como &quot;Sucesso&quot;, pois a repetição automática do manipulador de erros do Break está lidando com o problema automaticamente. Nesse caso, os usuários não recebem um email sobre a execução com falha.

Quando a opção &quot;Execução automática concluída&quot; está desativada, a execução é marcada como &quot;Aviso&quot;.

Há algumas exceções para execuções armazenadas em Execuções Incompletas e, com alguns tipos de erro, a repetição automática de uma execução de cenário não é possível.

Para obter mais informações, consulte [Permitir o armazenamento de execuções incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) no artigo [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obter mais informações, consulte [Tratamento avançado de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
